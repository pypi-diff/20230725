# Comparing `tmp/molecule-6.0.0a0.tar.gz` & `tmp/molecule-6.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-6.0.0a0.tar", last modified: Wed Jul 12 12:47:21 2023, max compression
+gzip compressed data, was "molecule-6.0.0a1.tar", last modified: Tue Jul 25 14:58:37 2023, max compression
```

## Comparing `molecule-6.0.0a0.tar` & `molecule-6.0.0a1.tar`

### file list

```diff
@@ -1,390 +1,416 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.450082 molecule-6.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.config/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/molecule/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/molecule.spec
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.config/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/patchback.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/redirects.yml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.npmrc
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.418081 molecule-6.0.0a0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 12:47:04.000000 molecule-6.0.0a0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-12 12:47:04.000000 molecule-6.0.0a0/DCO_1_1.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-12 12:47:04.000000 molecule-6.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 12:47:04.000000 molecule-6.0.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-12 12:47:21.450082 molecule-6.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-12 12:47:04.000000 molecule-6.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-12 12:47:04.000000 molecule-6.0.0a0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 12:47:04.000000 molecule-6.0.0a0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-12 12:47:04.000000 molecule-6.0.0a0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.406081 molecule-6.0.0a0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/_static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   143898 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/_static/images/logo_big.png
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/ci.md
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/google04e29a42ae6e6cbc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/next.md
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/podman.md
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/redirects.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-12 12:47:04.000000 molecule-6.0.0a0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 12:47:04.000000 molecule-6.0.0a0/linkcheckerrc
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-12 12:47:04.000000 molecule-6.0.0a0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.406081 molecule-6.0.0a0/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/molecule/podman/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/molecule/podman/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-12 12:47:04.000000 molecule-6.0.0a0/molecule/podman/tasks/create-fail.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-12 12:47:04.000000 molecule-6.0.0a0/playbooks/snap-pre-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-07-12 12:47:04.000000 molecule-6.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 12:47:04.000000 molecule-6.0.0a0/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:47:21.450082 molecule-6.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.422081 molecule-6.0.0a0/snap/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 12:47:04.000000 molecule-6.0.0a0/snap/snapcraft.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.406081 molecule-6.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.426082 molecule-6.0.0a0/src/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/command/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/idempotence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/command/init/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/init/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/init/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/init/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/side_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/command/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/driver.json
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/init-scenario.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/molecule.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/data/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/data/templates/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/templates/scenario/converge.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/templates/scenario/create.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/templates/scenario/destroy.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/data/templates/scenario/molecule.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/dependency/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.430081 molecule-6.0.0a0/src/molecule/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/driver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/driver/delegated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.434081 molecule-6.0.0a0/src/molecule/model/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/model/schema_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/platforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.434081 molecule-6.0.0a0/src/molecule/provisioner/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33606 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/provisioner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.434081 molecule-6.0.0a0/src/molecule/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.434081 molecule-6.0.0a0/src/molecule/test/a_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/command/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/init/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_idempotence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_side_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/command/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/dependency/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/driver/test_delegated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/lint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/lint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_dependency_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_driver_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_platforms_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_provisioner_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_scenario_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_verifier_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_scenarios_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.438082 molecule-6.0.0a0/src/molecule/test/a_unit/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/a_unit/verifier/test_ansible.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/b_functional/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/b_functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/b_functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/b_functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/b_functional/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/invalid_role_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/invalid_role_template/bad_format/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/invalid_role_template/bad_format/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/invalid_role_template/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/playbooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/roles/molecule/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/roles/get_rich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/invalid/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/valid/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.410081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.442082 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/hosts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/molecule/raises/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/idempotence/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.414081 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.446082 molecule-6.0.0a0/src/molecule/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/verifier/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-12 12:47:04.000000 molecule-6.0.0a0/src/molecule/verifier/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.426082 molecule-6.0.0a0/src/molecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 12:47:21.000000 molecule-6.0.0a0/src/molecule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:47:21.450082 molecule-6.0.0a0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/get-version.sh
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/opts.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/smoketest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/test-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tools/update-version.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-12 12:47:04.000000 molecule-6.0.0a0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.854848 molecule-6.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.766845 molecule-6.0.0a1/.config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.766845 molecule-6.0.0a1/.config/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/molecule/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/molecule.spec
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.770846 molecule-6.0.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.770846 molecule-6.0.0a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/patchback.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.774845 molecule-6.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.774845 molecule-6.0.0a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-25 14:58:16.000000 molecule-6.0.0a1/DCO_1_1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-25 14:58:16.000000 molecule-6.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 14:58:16.000000 molecule-6.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 14:58:37.854848 molecule-6.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-25 14:58:16.000000 molecule-6.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-25 14:58:16.000000 molecule-6.0.0a1/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-25 14:58:16.000000 molecule-6.0.0a1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-25 14:58:16.000000 molecule-6.0.0a1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.702844 molecule-6.0.0a1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/_static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   143898 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/_static/images/logo_big.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/ci.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/google04e29a42ae6e6cbc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/next.md
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/podman.md
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 14:58:16.000000 molecule-6.0.0a1/linkcheckerrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-25 14:58:16.000000 molecule-6.0.0a1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.702844 molecule-6.0.0a1/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/molecule/podman/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/molecule/podman/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/tasks/create-fail.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-25 14:58:16.000000 molecule-6.0.0a1/playbooks/snap-pre-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-07-25 14:58:16.000000 molecule-6.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 14:58:16.000000 molecule-6.0.0a1/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:58:37.854848 molecule-6.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/snap/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-25 14:58:16.000000 molecule-6.0.0a1/snap/snapcraft.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.706844 molecule-6.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.794846 molecule-6.0.0a1/src/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.806846 molecule-6.0.0a1/src/molecule/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/idempotence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.806846 molecule-6.0.0a1/src/molecule/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/init/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/init/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/init/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.810846 molecule-6.0.0a1/src/molecule/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/driver.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/init-scenario.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/molecule.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.710844 molecule-6.0.0a1/src/molecule/data/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.810846 molecule-6.0.0a1/src/molecule/data/templates/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/templates/scenario/converge.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/templates/scenario/create.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/templates/scenario/destroy.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/templates/scenario/molecule.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.814847 molecule-6.0.0a1/src/molecule/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.814847 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.818847 molecule-6.0.0a1/src/molecule/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/driver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/driver/delegated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.818847 molecule-6.0.0a1/src/molecule/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/model/schema_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/platforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.818847 molecule-6.0.0a1/src/molecule/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33606 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.818847 molecule-6.0.0a1/src/molecule/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.822847 molecule-6.0.0a1/src/molecule/test/a_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/init/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_idempotence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/cookiecutter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/cookiecutter/test_molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/driver/test_delegated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/lint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_dependency_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_driver_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_platforms_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_provisioner_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_scenario_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_verifier_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_scenarios_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/a_unit/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/verifier/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/verifier/test_testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/b_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/b_functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/b_functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/b_functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/b_functional/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/invalid_role_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/invalid_role_template/bad_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/invalid_role_template/bad_format/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/invalid_role_template/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/playbooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.726844 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.726844 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.726844 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.726844 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.734845 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.734845 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/hosts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.738845 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.734845 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.738845 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.738845 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.738845 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.746845 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.746845 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.750845 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/verifier/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/verifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/verifier/testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.798846 molecule-6.0.0a1/src/molecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.854848 molecule-6.0.0a1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/get-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/opts.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/smoketest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/test-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tox.ini
```

### Comparing `molecule-6.0.0a0/.config/molecule.spec` & `molecule-6.0.0a1/.config/molecule.spec`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.config/requirements-lock.txt` & `molecule-6.0.0a1/.config/requirements-lock.txt`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.config/requirements.txt` & `molecule-6.0.0a1/.config/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 ptyprocess==0.7.0
 pycparser==2.21
 pygments==2.15.1
 pymdown-extensions==10.0.1
 pytest==7.4.0
 pytest-mock==3.11.1
 pytest-plus==0.4.0
+pytest-testinfra==8.1.0
 pytest-xdist==3.3.1
 python-dateutil==2.8.2
 python-slugify==8.0.1
 pyyaml==6.0
 pyyaml-env-tag==0.1
 referencing==0.29.1
 regex==2023.5.5
```

### Comparing `molecule-6.0.0a0/.gitattributes` & `molecule-6.0.0a1/.gitattributes`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.github/ISSUE_TEMPLATE/bug_report.md` & `molecule-6.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.github/ISSUE_TEMPLATE/config.yml` & `molecule-6.0.0a1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.github/dependabot.yml` & `molecule-6.0.0a1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.github/workflows/redirects.yml` & `molecule-6.0.0a1/.github/workflows/redirects.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.github/workflows/release.yml` & `molecule-6.0.0a1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.github/workflows/tox.yml` & `molecule-6.0.0a1/.github/workflows/tox.yml`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # limit potential endless looks like we had with build-containers
     timeout-minutes: 20
     strategy:
       fail-fast: false
       matrix: ${{ fromJson(needs.pre.outputs.matrix) }}
 
     env:
-      PYTEST_REQPASS: 424
+      PYTEST_REQPASS: 445
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # needed by setuptools-scm
           submodules: true
 
       - name: Set pre-commit cache
```

### Comparing `molecule-6.0.0a0/.packit.yaml` & `molecule-6.0.0a1/.packit.yaml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.pre-commit-config.yaml` & `molecule-6.0.0a1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
           - click
           - click-help-colors
           - enrich>=1.2.7
           - filelock
           - jsonschema
           - pexpect
           - pytest-mock
+          - pytest-testinfra
   - repo: https://github.com/jazzband/pip-tools
     rev: 6.14.0
     hooks:
       - id: pip-compile
         entry: pip-compile -q --resolver=backtracking --strip-extras --no-annotate --output-file=.config/requirements.txt pyproject.toml --extra docs --extra test
         files: ^(pyproject\.toml|\.config\/.*)$
       - id: pip-compile
```

### Comparing `molecule-6.0.0a0/.vscode/settings.json` & `molecule-6.0.0a1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/.yamllint` & `molecule-6.0.0a1/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/DCO_1_1.md` & `molecule-6.0.0a1/DCO_1_1.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/LICENSE` & `molecule-6.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/PKG-INFO` & `molecule-6.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 6.0.0a0
+Version: 6.0.0a1
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
```

### Comparing `molecule-6.0.0a0/README.md` & `molecule-6.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/bindep.txt` & `molecule-6.0.0a1/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/conftest.py` & `molecule-6.0.0a1/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/_static/images/favicon.ico` & `molecule-6.0.0a1/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/_static/images/logo.png` & `molecule-6.0.0a1/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/_static/images/logo_big.png` & `molecule-6.0.0a1/docs/_static/images/logo_big.png`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/ci.md` & `molecule-6.0.0a1/docs/ci.md`

 * *Files 1% similar despite different names*

```diff
@@ -397,17 +397,21 @@
 platform in `molecule.yml` configuration file. This way, their names
 won't create any conflict.
 
 ```yaml
 ---
 dependency:
   name: galaxy
+driver:
+  name: docker
 platforms:
   - name: instance1-$TOX_ENVNAME
     image: mariadb
   - name: instance2-$TOX_ENVNAME
     image: retr0h/centos7-systemd-ansible:latest
     privileged: True
     command: /usr/sbin/init
 provisioner:
   name: ansible
+verifier:
+  name: testinfra
 ```
```

### Comparing `molecule-6.0.0a0/docs/configuration.md` & `molecule-6.0.0a1/docs/configuration.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # Configuration
 
 ::: molecule.config.Config
 
 ## Prerun
 
-In order to help Ansible find used modules and roles, molecule will
+To help Ansible find used modules and roles, molecule will
 perform a prerun set of actions. These involve installing dependencies
-from `requirements.yml` specified at project level, install a standalone
+from `requirements.yml` specified at the project level, installing a standalone
 role or a collection. The destination is `project_dir/.cache` and the
 code itself was reused from ansible-lint, which has to do the same
 actions. (Note: ansible-lint is not included with molecule.)
 
 This assures that when you include a role inside molecule playbooks,
-Ansible will be able to find that role, and that the include is exactly
+Ansible will be able to find that role and that the include is exactly
 the same as the one you are expecting to use in production.
 
-If for some reason the prerun action does not suits your needs, you can
+If for some reason the prerun action does not suit your needs, you can
 still disable it by adding `prerun: false` inside the
 configuration file.
 
 Keep in mind that you can add this value to the
 `.config/molecule/config.yml` file, in your `$HOME` or at the root of
 your project, in order to avoid adding it to each scenario.
 
 ## Role name check
 
 By default, `Molecule` will check whether the role name follows the name
 standard. If not, it will raise an error.
 
-If computed fully qualified role name does not follow current galaxy
+If the computed fully qualified role name does not follow current galaxy
 requirements, you can ignore it by adding `role_name_check:1` inside the configuration file.
 
 It is strongly recommended to follow the name standard of
 [namespace](https://galaxy.ansible.com/docs/contributing/namespaces.html#galaxy-namespace-limitations)
 and
 [role](https://galaxy.ansible.com/docs/contributing/creating_role.html#role-names).
 
 ## Variable Substitution
 
 ::: molecule.interpolation.Interpolator
 
-There are following environment variables available in `molecule.yml`:
+Following are the environment variables available in `molecule.yml`:
 
 MOLECULE_DEBUG
 
 : If debug is turned on or off
 
 MOLECULE_FILE
 
@@ -53,15 +53,15 @@
 
 MOLECULE_ENV_FILE
 
 : Path to molecule environment file, usually `<role_path>/.env.yml`
 
 MOLECULE_STATE_FILE
 
-: Path to molecule state file, contains state of the instances
+: The path to molecule state file contains the state of the instances
 (created, converged, etc.). Usually
 `~/.cache/molecule/<role-name>/<scenario-name>/state.yml`
 
 MOLECULE_INVENTORY_FILE
 
 : Path to generated inventory file, usually
 `~/.cache/molecule/<role-name>/<scenario-name>/inventory/ansible_inventory.yml`
@@ -245,31 +245,31 @@
   - verify
 ```
 
 `side_effect` without an argument is executing the usual `side_effect` configured in
 `provisioner.playbooks` section of molecule.yml.
 
 `side_effect` can have one or more arguments (separated by spaces) which is
-a playbook (plabyooks) to execute. If the argument for `side_effect` is present,
+a playbook (playbooks) to execute. If the argument for `side_effect` is present,
 it's executed instead. The path to the playbook is relative to the molecule.yml location.
 Normal side effect settings (from `provisioner.playbooks`) are ignored for action with
 argument.
 
-`verify` without an argument is executing usual tests configured in the verifier section
+`verify` without an argument is executing the usual tests configured in the verifier section
 of molecule.yml.
 
 If one or more arguments (separated by spaces) are present, each argument is treated
 as a test name (file or directory) to pass to the verifier (either Ansible or Testinfra).
 The kind of verifier is set in the `verifier` section of molecule.yml and is applied to all
 `verify` actions in the scenario.
 
 The path to tests is relative to the molecule.yml file location. The `additional_files_or_dirs`
-setting for verifier is ignored if the `verify` action has an argument.
+setting for the verifier is ignored if the `verify` action is provided with an argument.
 
-Multiple `side_effect` and `verify` actions can be used to a create a combination
+Multiple `side_effect` and `verify` actions can be used to create a combination
 of playbooks and tests, for example, for end-to-end playbook testing.
 
 Additional `converge` and `idempotence` actions can be used multiple times:
 
 ```yaml
 test_sequence:
   - converge
@@ -290,7 +290,11 @@
 ## Verifier
 
 Molecule handles role testing by invoking configurable verifiers.
 
 ### Ansible
 
 ::: molecule.verifier.ansible.Ansible
+
+### Testinfra
+
+::: molecule.verifier.testinfra.Testinfra
```

### Comparing `molecule-6.0.0a0/docs/contributing.md` & `molecule-6.0.0a1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/examples.md` & `molecule-6.0.0a1/docs/examples.md`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,23 @@
 │   │   └── molecule.yml
 │   └── ubuntu-upstart
 │       └── molecule.yml
 ```
 
 Tests and playbooks can be shared across scenarios.
 
+In this example the `tests` directory lives in a shared
+location and `molecule.yml` points to the shared tests.
+
+```yaml
+verifier:
+  name: testinfra
+  directory: ../resources/tests/
+```
+
 In this second example the actions `create`,
 `destroy`, `converge` and `prepare`
 are loaded from a shared directory.
 
 ```yaml
 provisioner:
   name: ansible
```

### Comparing `molecule-6.0.0a0/docs/faq.md` & `molecule-6.0.0a1/docs/faq.md`

 * *Files 6% similar despite different names*

```diff
@@ -80,20 +80,18 @@
 
 Where `CI_JOB_ID` is the random variable that Gitlab provides.
 
 Molecule will resolve the `INSTANCE_UUID` environment variable when
 creating and looking up the instance name. You can confirm all is in
 working order by running `molecule list`.
 
-## Can I test Ansible Collections with Molecule?
+## Where can I configure my `roles-path` and `collections-paths`?
 
-This is not currently officially supported. Also, collections remain in
-"tech preview" status. However, you can take a look at [this blog
-post](https://www.jeffgeerling.com/blog/2019/how-add-integration-tests-ansible-collection-molecule)
-outlining a workable DIY solution as a stop gap for now.
+As of molecule v6, users are expected to make use of [`ansible.cfg`](https://docs.ansible.com/ansible/latest/reference_appendices/config.html) file to
+alter them when needed.
 
 ## Does Molecule support monorepos?
 
 Yes, roles contained in a
 [monorepo](https://en.wikipedia.org/wiki/Monorepo) with other roles are
 automatically picked up and `ANSIBLE_ROLES_PATH` is set accordingly. See
 [this
```

### Comparing `molecule-6.0.0a0/docs/getting-started.md` & `molecule-6.0.0a1/docs/getting-started.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
   employ when testing your role.
 - `converge.yml` is the playbook file that contains the call for your
   role. Molecule will invoke this playbook with `ansible-playbook` and
   run it against an instance created by the driver.
 - `verify.yml` is the Ansible file used for testing as Ansible is the
   default [verifier](configuration.md#verifier). This allows you to
   write specific tests against the state of the container after your
-  role has finished executing.
+  role has finished executing. Other verifier tools are available
+  Note that [testinfra](https://testinfra.readthedocs.io/en/latest/) was the default verifier prior to molecule version 3.
 
 !!! note
 
     If the `verify.yml` playbook does not explicitly `include_role` your
     role, the `library` and `module_utils` provided by your role are not
     available in the playbook by default. If you need those for testing but
     would like to avoid re-running your role, consider adding an empty task
```

### Comparing `molecule-6.0.0a0/docs/images/favicon.ico` & `molecule-6.0.0a1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/images/logo.png` & `molecule-6.0.0a1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/images/logo.svg` & `molecule-6.0.0a1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/index.md` & `molecule-6.0.0a1/docs/index.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/installation.md` & `molecule-6.0.0a1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/next.md` & `molecule-6.0.0a1/docs/next.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 Molecule "next" is the future major version of molecule, one that is currently
 available from the main branch. One of the main goals of the new version is to
 reduce the amount of magic and just rely on ansible core features.
 
 # Implemented changes
 
 - `roles-path` and `collections-paths` are no longer configurable for
-  dependencies. Users are expected to make use of `ansible.cfg` file to
+  dependencies. Users are expected to make use of [`ansible.cfg`](https://docs.ansible.com/ansible/latest/reference_appendices/config.html) file to
   alter them when needed.
-- testinfra verifier driver was removed but current users should be able to
-  keep calling their testinfra tests by using `command` or `shell` ansible
-  modules from within `verify.yml` playbook.
+
+- `molecule init` command is now only available to create a scenario
+  using `molecule init scenario`.
+  Users will no longer be able to create a role.
+  Instead, users can make use of [`ansible-galaxy`](https://docs.ansible.com/ansible/latest/galaxy/dev_guide.html#) to [create a role](https://docs.ansible.com/ansible/latest/galaxy/dev_guide.html#creating-roles-for-galaxy).
 
 # Planned changes
 
-- Removal of provisioning drivers support and documenting, with examples, how to easily migrate to a self-provisioning approach.
 - Refactoring how dependencies are installed
 - Bringing ephemeral directory under scenario folder instead of the current
   inconvenient location under `~/.cache/molecule/...`
-- Addition of a minimal `ansible.cfg` file under scenario folder that can
-  be used to tell ansible from where to load testing content. This is to replace
+- Addition of a minimal `ansible.cfg` file under the scenario folder that can
+  be used to tell Ansible from where to load testing content. This is to replace
   current Molecule magic around roles, collections and library paths and
-  test inventory location. Once done you will be able to run molecule playbooks with ansible directly without
+  test inventory location. Once done you will be able to run molecule playbooks with Ansible directly without
   having to define these folders.
```

### Comparing `molecule-6.0.0a0/docs/podman.md` & `molecule-6.0.0a1/docs/podman.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/docs/usage.md` & `molecule-6.0.0a1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/mkdocs.yml` & `molecule-6.0.0a1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/molecule/default/create.yml` & `molecule-6.0.0a1/molecule/default/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/molecule/default/destroy.yml` & `molecule-6.0.0a1/molecule/default/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/molecule/podman/converge.yml` & `molecule-6.0.0a1/molecule/podman/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/molecule/podman/create.yml` & `molecule-6.0.0a1/molecule/podman/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/molecule/podman/destroy.yml` & `molecule-6.0.0a1/molecule/podman/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/playbooks/snap-pre-run.yaml` & `molecule-6.0.0a1/playbooks/snap-pre-run.yaml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/pyproject.toml` & `molecule-6.0.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -43,18 +43,19 @@
 documentation = "https://molecule.readthedocs.io/"
 repository = "https://github.com/ansible-community/molecule"
 changelog = "https://github.com/ansible-community/molecule/releases"
 
 [project.scripts]
 molecule = "molecule.__main__:main"
 
-[project.entry-points."molecule.driver.next"]
+[project.entry-points."molecule.driver"]
 default = "molecule.driver.delegated:Delegated"
 
-[project.entry-points."molecule.verifier.next"]
+[project.entry-points."molecule.verifier"]
+testinfra = "molecule.verifier.testinfra:Testinfra"
 ansible = "molecule.verifier.ansible:Ansible"
 
 [tool.coverage.run]
 source = ["src"]
 # branch = true
 parallel = true
 concurrency = ["multiprocessing", "thread"]
@@ -92,14 +93,15 @@
 no_incremental = true
 
 [[tool.mypy.overrides]]
 module = [
   "click_help_colors", # https://github.com/click-contrib/click-help-colors/issues/20
   "pexpect", # https://github.com/pexpect/pexpect/issues/759
   "pluggy", # https://github.com/pytest-dev/pluggy/pull/414
+  "testinfra.*", # https://github.com/pytest-dev/pytest-testinfra/issues/619
   "pytest_mock",
 ]
 ignore_missing_imports = true
 ignore_errors = true
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
```

### Comparing `molecule-6.0.0a0/snap/snapcraft.yaml` & `molecule-6.0.0a1/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/__init__.py` & `molecule-6.0.0a1/src/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/__main__.py` & `molecule-6.0.0a1/src/molecule/__main__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/api.py` & `molecule-6.0.0a1/src/molecule/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     """A warning noting an unsupported runtime environment."""
 
 
 @cache
 def drivers(config=None) -> UserListMap:
     """Return list of active drivers."""
     plugins = UserListMap()
-    pm = pluggy.PluginManager("molecule.driver.next")
+    pm = pluggy.PluginManager("molecule.driver")
     try:
-        pm.load_setuptools_entrypoints("molecule.driver.next")
+        pm.load_setuptools_entrypoints("molecule.driver")
     except (Exception, SystemExit):
         # These are not fatal because a broken driver should not make the entire
         # tool unusable.
         LOG.error("Failed to load driver entry point %s", traceback.format_exc())
     for p in pm.get_plugins():
         try:
             plugins.append(p(config))
@@ -64,17 +64,17 @@
     return plugins
 
 
 @cache
 def verifiers(config=None) -> UserListMap:
     """Return list of active verifiers."""
     plugins = UserListMap()
-    pm = pluggy.PluginManager("molecule.verifier.next")
+    pm = pluggy.PluginManager("molecule.verifier")
     try:
-        pm.load_setuptools_entrypoints("molecule.verifier.next")
+        pm.load_setuptools_entrypoints("molecule.verifier")
     except Exception:
         # These are not fatal because a broken verifier should not make the entire
         # tool unusable.
         LOG.error("Failed to load verifier entry point %s", traceback.format_exc())
     for p in pm.get_plugins():
         try:
             plugins.append(p(config))
```

### Comparing `molecule-6.0.0a0/src/molecule/command/__init__.py` & `molecule-6.0.0a1/src/molecule/command/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/base.py` & `molecule-6.0.0a1/src/molecule/command/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/check.py` & `molecule-6.0.0a1/src/molecule/command/check.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/cleanup.py` & `molecule-6.0.0a1/src/molecule/command/cleanup.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/converge.py` & `molecule-6.0.0a1/src/molecule/command/converge.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/create.py` & `molecule-6.0.0a1/src/molecule/command/create.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/dependency.py` & `molecule-6.0.0a1/src/molecule/command/dependency.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/destroy.py` & `molecule-6.0.0a1/src/molecule/command/destroy.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/drivers.py` & `molecule-6.0.0a1/src/molecule/command/drivers.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/idempotence.py` & `molecule-6.0.0a1/src/molecule/command/idempotence.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/init/base.py` & `molecule-6.0.0a1/src/molecule/command/init/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/init/init.py` & `molecule-6.0.0a1/src/molecule/command/init/init.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/init/scenario.py` & `molecule-6.0.0a1/src/molecule/command/init/scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/list.py` & `molecule-6.0.0a1/src/molecule/command/list.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/login.py` & `molecule-6.0.0a1/src/molecule/command/login.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/matrix.py` & `molecule-6.0.0a1/src/molecule/command/matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/prepare.py` & `molecule-6.0.0a1/src/molecule/command/prepare.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/reset.py` & `molecule-6.0.0a1/src/molecule/command/reset.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/side_effect.py` & `molecule-6.0.0a1/src/molecule/command/side_effect.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/syntax.py` & `molecule-6.0.0a1/src/molecule/command/syntax.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/test.py` & `molecule-6.0.0a1/src/molecule/command/test.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/command/verify.py` & `molecule-6.0.0a1/src/molecule/command/verify.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/config.py` & `molecule-6.0.0a1/src/molecule/config.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/console.py` & `molecule-6.0.0a1/src/molecule/console.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/data/driver.json` & `molecule-6.0.0a1/src/molecule/data/driver.json`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/data/init-scenario.yml` & `molecule-6.0.0a1/src/molecule/data/init-scenario.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/data/molecule.json` & `molecule-6.0.0a1/src/molecule/data/molecule.json`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/data/templates/scenario/create.yml.j2` & `molecule-6.0.0a1/src/molecule/data/templates/scenario/create.yml.j2`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/data/templates/scenario/destroy.yml.j2` & `molecule-6.0.0a1/src/molecule/data/templates/scenario/destroy.yml.j2`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/__init__.py` & `molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/base.py` & `molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/collections.py` & `molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/collections.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/dependency/ansible_galaxy/roles.py` & `molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/roles.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/dependency/base.py` & `molecule-6.0.0a1/src/molecule/dependency/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/dependency/shell.py` & `molecule-6.0.0a1/src/molecule/dependency/shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/driver/base.py` & `molecule-6.0.0a1/src/molecule/driver/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,25 @@
     def name(self, value):  # pragma: no cover
         """Driver name setter and returns None.
 
         :returns: None
         """
 
     @property
+    def testinfra_options(self):
+        """Testinfra specific options and returns a dict.
+
+        :returns: dict
+        """
+        return {
+            "connection": "ansible",
+            "ansible-inventory": self._config.provisioner.inventory_directory,
+        }
+
+    @property
     @abstractmethod
     def login_cmd_template(self):  # pragma: no cover
         """Get the login command template to be populated by ``login_options`` as \
         a string.
 
         :returns: str
         """
```

### Comparing `molecule-6.0.0a0/src/molecule/driver/delegated.py` & `molecule-6.0.0a1/src/molecule/driver/delegated.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,16 @@
                 if d.get("identity_file", None):
                     conn_dict["ansible_private_key_file"] = d.get("identity_file")
                     conn_dict["ansible_ssh_common_args"] = " ".join(
                         self.ssh_connection_options,
                     )
                 if d.get("password", None):
                     conn_dict["ansible_password"] = d.get("password")
+                    # Based on testinfra documentation, ansible password must be passed via ansible_ssh_pass
+                    # issue to fix this can be found https://github.com/pytest-dev/pytest-testinfra/issues/580
                     conn_dict["ansible_ssh_pass"] = d.get("password")
 
                 return conn_dict
 
             except StopIteration:
                 return {}
             except OSError:
```

### Comparing `molecule-6.0.0a0/src/molecule/interpolation.py` & `molecule-6.0.0a1/src/molecule/interpolation.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,30 @@
         self.string = string
         self.place = place
 
 
 class Interpolator:
     """Configuration options may contain environment variables.
 
+    For example, suppose the shell contains ``VERIFIER_NAME=testinfra`` and
+    the following molecule.yml is supplied.
+
+    ```yaml
+        verifier:
+          - name: ${VERIFIER_NAME}
+    ```
+
+    Molecule will substitute ``$VERIFIER_NAME`` with the value of the
+    ``VERIFIER_NAME`` environment variable.
+
+    !!! warning
+
+        If an environment variable is not set, Molecule substitutes with an
+        empty string.
+
     Both ``$VARIABLE`` and ``${VARIABLE}`` syntax are supported. Extended
     shell-style features, such as ``${VARIABLE-default}`` and
     ``${VARIABLE:-default}`` are also supported. Even the default as another
     environment variable is supported like ``${VARIABLE-$DEFAULT}`` or
     ``${VARIABLE:-$DEFAULT}``. An empty string is returned when
     both variables are undefined.
```

### Comparing `molecule-6.0.0a0/src/molecule/logger.py` & `molecule-6.0.0a1/src/molecule/logger.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/model/schema_v3.py` & `molecule-6.0.0a1/src/molecule/model/schema_v3.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/platforms.py` & `molecule-6.0.0a1/src/molecule/platforms.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/provisioner/ansible.py` & `molecule-6.0.0a1/src/molecule/provisioner/ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/provisioner/ansible_playbook.py` & `molecule-6.0.0a1/src/molecule/provisioner/ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/provisioner/ansible_playbooks.py` & `molecule-6.0.0a1/src/molecule/provisioner/ansible_playbooks.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/provisioner/base.py` & `molecule-6.0.0a1/src/molecule/provisioner/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/scenario.py` & `molecule-6.0.0a1/src/molecule/scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/scenarios.py` & `molecule-6.0.0a1/src/molecule/scenarios.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/shell.py` & `molecule-6.0.0a1/src/molecule/shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/state.py` & `molecule-6.0.0a1/src/molecule/state.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/status.py` & `molecule-6.0.0a1/src/molecule/status.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/conftest.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/init/test_scenario.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/init/test_scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_base.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_check.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_check.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_cleanup.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_converge.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_converge.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_create.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_create.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_dependency.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_dependency.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_destroy.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_destroy.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_idempotence.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_idempotence.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_list.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_list.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_login.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_login.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_matrix.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_prepare.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_prepare.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_side_effect.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_side_effect.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_syntax.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_syntax.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_test.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_test.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/command/test_verify.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_verify.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/conftest.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/dependency/test_shell.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/dependency/test_shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/driver/test_delegated.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/driver/test_delegated.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,21 @@
     return delegated.Delegated(config_instance)
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
+def test_testinfra_options_property(_instance):
+    assert {
+        "connection": "ansible",
+        "ansible-inventory": _instance._config.provisioner.inventory_directory,
+    } == _instance.testinfra_options
+
+
 def test_name_property(_instance):
     assert _instance.name == "default"
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_driver_unmanaged_section_data"],
```

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/conftest.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_dependency_section.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_dependency_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_driver_section.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_driver_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_platforms_section.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_platforms_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_provisioner_section.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_provisioner_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_scenario_section.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_scenario_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_schema.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_schema.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/model/v2/test_verifier_section.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_verifier_section.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,29 @@
 #  DEALINGS IN THE SOFTWARE.
 
 import pytest
 
 from molecule.model import schema_v3
 
 
+@pytest.fixture()
+def _model_verifier_section_data():
+    return {
+        "verifier": {
+            "name": "testinfra",
+            "enabled": True,
+            "directory": "foo",
+            "options": {"foo": "bar"},
+            "env": {"FOO": "foo", "FOO_BAR": "foo_bar"},
+            "additional_files_or_dirs": ["foo"],
+        },
+    }
+
+
+@pytest.mark.parametrize("_config", ["_model_verifier_section_data"], indirect=True)
 def test_verifier(_config):
     assert not schema_v3.validate(_config)
 
 
 @pytest.fixture()
 def _model_verifier_errors_section_data():
     return {
@@ -44,20 +59,26 @@
 def test_verifier_has_errors(_config):
     x = ["0 is not one of ['ansible', 'goss', 'inspec', 'testinfra']"]
 
     assert x == schema_v3.validate(_config)
 
 
 @pytest.fixture()
+def _model_verifier_allows_testinfra_section_data():
+    return {"verifier": {"name": "testinfra"}}
+
+
+@pytest.fixture()
 def _model_verifier_allows_ansible_section_data():
     return {"verifier": {"name": "ansible"}}
 
 
 @pytest.mark.parametrize(
     "_config",
     [
+        ("_model_verifier_allows_testinfra_section_data"),
         ("_model_verifier_allows_ansible_section_data"),
     ],
     indirect=True,
 )
 def test_verifier_allows_name(_config):
     assert not schema_v3.validate(_config)
```

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_api.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,10 +34,10 @@
     for result in results:
         assert isinstance(result, api.Driver)
 
     assert "default" in results
 
 
 def test_api_verifiers():
-    x = ["ansible"]
+    x = ["testinfra", "ansible"]
 
     assert all(elem in api.verifiers() for elem in x)
```

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_config.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_config.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_interpolation.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_logger.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_platforms.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_platforms.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_scenario.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_scenarios.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_scenarios_ordered.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_scenarios_ordered.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_shell.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_state.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_state.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_status.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_status.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_text.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_text.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/test_util.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/test_util.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/a_unit/verifier/test_ansible.py` & `molecule-6.0.0a1/src/molecule/test/a_unit/verifier/test_ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/b_functional/conftest.py` & `molecule-6.0.0a1/src/molecule/test/b_functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/b_functional/test_command.py` & `molecule-6.0.0a1/src/molecule/test/b_functional/test_command.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/conftest.py` & `molecule-6.0.0a1/src/molecule/test/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/resources/schema_instance_files/valid/molecule.yml` & `molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/valid/molecule.yml`

 * *Files 8% similar despite different names*

```diff
@@ -64,8 +64,8 @@
     - prepare
     - converge
     - check
     - verify
     - destroy
 
 verifier:
-  name: ansible
+  name: testinfra
```

### Comparing `molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml` & `molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml` & `molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py` & `molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 """Testinfra tests."""
 
+import os
+
+import testinfra.utils.ansible_runner
+
+testinfra_hosts = testinfra.utils.ansible_runner.AnsibleRunner(
+    os.environ["MOLECULE_INVENTORY_FILE"],
+).get_hosts("all")
+
 
 def test_hostname(host):
     """Validate hostname."""
     assert host.check_output("hostname -s") == "instance"
 
 
 def test_etc_molecule_directory(host):
```

### Comparing `molecule-6.0.0a0/src/molecule/text.py` & `molecule-6.0.0a1/src/molecule/text.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/util.py` & `molecule-6.0.0a1/src/molecule/util.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/verifier/ansible.py` & `molecule-6.0.0a1/src/molecule/verifier/ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule/verifier/base.py` & `molecule-6.0.0a1/src/molecule/verifier/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/src/molecule.egg-info/PKG-INFO` & `molecule-6.0.0a1/src/molecule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 6.0.0a0
+Version: 6.0.0a1
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
```

### Comparing `molecule-6.0.0a0/src/molecule.egg-info/SOURCES.txt` & `molecule-6.0.0a1/src/molecule.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -179,14 +179,16 @@
 src/molecule/test/a_unit/command/test_prepare.py
 src/molecule/test/a_unit/command/test_side_effect.py
 src/molecule/test/a_unit/command/test_syntax.py
 src/molecule/test/a_unit/command/test_test.py
 src/molecule/test/a_unit/command/test_verify.py
 src/molecule/test/a_unit/command/init/__init__.py
 src/molecule/test/a_unit/command/init/test_scenario.py
+src/molecule/test/a_unit/cookiecutter/__init__.py
+src/molecule/test/a_unit/cookiecutter/test_molecule.py
 src/molecule/test/a_unit/dependency/__init__.py
 src/molecule/test/a_unit/dependency/test_shell.py
 src/molecule/test/a_unit/dependency/ansible_galaxy/__init__.py
 src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py
 src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py
 src/molecule/test/a_unit/driver/__init__.py
 src/molecule/test/a_unit/driver/test_delegated.py
@@ -203,14 +205,15 @@
 src/molecule/test/a_unit/model/v2/test_verifier_section.py
 src/molecule/test/a_unit/provisioner/__init__.py
 src/molecule/test/a_unit/provisioner/test_ansible.py
 src/molecule/test/a_unit/provisioner/test_ansible_playbook.py
 src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py
 src/molecule/test/a_unit/verifier/__init__.py
 src/molecule/test/a_unit/verifier/test_ansible.py
+src/molecule/test/a_unit/verifier/test_testinfra.py
 src/molecule/test/b_functional/.ansible-lint
 src/molecule/test/b_functional/__init__.py
 src/molecule/test/b_functional/conftest.py
 src/molecule/test/b_functional/test_command.py
 src/molecule/test/resources/.yamllint
 src/molecule/test/resources/molecule.yml
 src/molecule/test/resources/invalid_role_template/cookiecutter.json
@@ -222,17 +225,19 @@
 src/molecule/test/resources/roles/molecule/tasks/main.yml
 src/molecule/test/resources/sample-collection/galaxy.yml
 src/molecule/test/resources/sample-collection/molecule/default/converge.yml
 src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
 src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
 src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
 src/molecule/test/resources/schema_instance_files/valid/molecule.yml
+src/molecule/test/scenarios/.flake8
 src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
 src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
 src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
+src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
 src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
 src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
 src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
 src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
 src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
 src/molecule/test/scenarios/driver/delegated/meta/main.yml
 src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
@@ -248,29 +253,40 @@
 src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
 src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
 src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
 src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
 src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
 src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
 src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
+src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
+src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
 src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
 src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
 src/molecule/test/scenarios/idempotence/tasks/main.yml
 src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
 src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
 src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
 src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
 src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
 src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
 src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
 src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
 src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
 src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
 src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
+src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
+src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
+src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
+src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
+src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
+src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
+src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
+src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
 src/molecule/verifier/__init__.py
 src/molecule/verifier/ansible.py
 src/molecule/verifier/base.py
+src/molecule/verifier/testinfra.py
 tools/get-version.sh
 tools/opts.txt
 tools/smoketest.sh
 tools/test-setup.sh
 tools/update-version.sh
```

### Comparing `molecule-6.0.0a0/src/molecule.egg-info/requires.txt` & `molecule-6.0.0a1/src/molecule.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -47,10 +47,11 @@
 ansible-lint>=6.12.1
 ansi2html>=1.8.0
 coverage>=7.0.3
 filelock>=3.9.0
 pexpect<5,>=4.8.0
 pytest-mock>=3.10.0
 pytest-plus>=0.4.0
+pytest-testinfra>=7.0.0
 pytest-xdist>=3.1.0
 pytest>=7.2.0
 check-jsonschema
```

### Comparing `molecule-6.0.0a0/tools/test-setup.sh` & `molecule-6.0.0a1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a0/tox.ini` & `molecule-6.0.0a1/tox.ini`

 * *Files identical despite different names*

