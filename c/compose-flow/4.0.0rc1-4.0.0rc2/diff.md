# Comparing `tmp/compose-flow-4.0.0rc1.tar.gz` & `tmp/compose-flow-4.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose-flow-4.0.0rc1.tar", last modified: Thu Jul 20 18:57:44 2023, max compression
+gzip compressed data, was "compose-flow-4.0.0rc2.tar", last modified: Tue Jul 25 18:45:10 2023, max compression
```

## Comparing `compose-flow-4.0.0rc1.tar` & `compose-flow-4.0.0rc2.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/
--rw-r--r--   0 root         (0) docker     (999)       49 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/.dockerignore
--rw-r--r--   0 root         (0) docker     (999)      105 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/.gitignore
--rw-r--r--   0 root         (0) docker     (999)     2642 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/Dockerfile
--rw-r--r--   0 root         (0) docker     (999)      508 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/Jenkinsfile
--rw-r--r--   0 root         (0) docker     (999)    11357 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) docker     (999)       34 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) docker     (999)     1964 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) docker     (999)      339 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/Pipfile
--rw-r--r--   0 root         (0) docker     (999)    73192 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/Pipfile.lock
--rw-r--r--   0 root         (0) docker     (999)     1691 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/README.md
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/compose/
--rw-r--r--   0 root         (0) docker     (999)     1171 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/compose-flow.yml
--rw-r--r--   0 root         (0) docker     (999)       54 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/docker-compose.mount.yml
--rw-r--r--   0 root         (0) docker     (999)       78 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/docker-compose.publish.yml
--rw-r--r--   0 root         (0) docker     (999)      157 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/docker-compose.results.yml
--rw-r--r--   0 root         (0) docker     (999)       73 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/docker-compose.yml
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/docs/
--rw-r--r--   0 root         (0) docker     (999)     9824 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/docs/advanced.md
--rw-r--r--   0 root         (0) docker     (999)     9328 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/docs/k8s.md
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/files/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/files/home/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/files/home/swarmclient/
--rw-r--r--   0 root         (0) docker     (999)      142 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/files/home/swarmclient/.pypirc
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/files/usr/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/files/usr/local/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/files/usr/local/bin/
--rw-r--r--   0 root         (0) docker     (999)      210 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/files/usr/local/bin/entrypoint.sh
--rw-r--r--   0 root         (0) docker     (999)      132 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/pylama.ini
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/scripts/
--rw-r--r--   0 root         (0) docker     (999)       71 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/black.sh
--rw-r--r--   0 root         (0) docker     (999)      715 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/dump_swarm_config.py
--rwxr-xr-x   0 root         (0) docker     (999)      245 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/lock.sh
--rw-r--r--   0 root         (0) docker     (999)      304 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/publish.sh
--rw-r--r--   0 root         (0) docker     (999)      101 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/tag_and_publish.sh
--rw-r--r--   0 root         (0) docker     (999)      119 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/watch-tests.sh
--rw-r--r--   0 root         (0) docker     (999)       83 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) docker     (999)     2131 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/setup.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/src/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.862718 compose-flow-4.0.0rc1/src/compose_flow/
--rw-r--r--   0 root         (0) docker     (999)        0 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/__init__.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.862718 compose-flow-4.0.0rc1/src/compose_flow/commands/
--rw-r--r--   0 root         (0) docker     (999)       31 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/__init__.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.866718 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/
--rw-r--r--   0 root         (0) docker     (999)     3141 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/__init__.py
--rw-r--r--   0 root         (0) docker     (999)     5042 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/base.py
--rw-r--r--   0 root         (0) docker     (999)      212 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/build.py
--rw-r--r--   0 root         (0) docker     (999)     1477 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/compose.py
--rw-r--r--   0 root         (0) docker     (999)     3250 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/deploy.py
--rw-r--r--   0 root         (0) docker     (999)      272 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/docker.py
--rw-r--r--   0 root         (0) docker     (999)    14787 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/env.py
--rw-r--r--   0 root         (0) docker     (999)      496 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/helm.py
--rw-r--r--   0 root         (0) docker     (999)      435 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/help.py
--rw-r--r--   0 root         (0) docker     (999)     1230 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/kompose.py
--rw-r--r--   0 root         (0) docker     (999)      503 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/kubectl.py
--rw-r--r--   0 root         (0) docker     (999)     1600 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/passthrough_base.py
--rw-r--r--   0 root         (0) docker     (999)     3672 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/pod.py
--rw-r--r--   0 root         (0) docker     (999)    14763 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/profile.py
--rw-r--r--   0 root         (0) docker     (999)     2722 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/publish.py
--rw-r--r--   0 root         (0) docker     (999)      490 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/rancher.py
--rw-r--r--   0 root         (0) docker     (999)     6633 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/remote.py
--rw-r--r--   0 root         (0) docker     (999)     1770 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/remote_config.py
--rw-r--r--   0 root         (0) docker     (999)     6271 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/service.py
--rw-r--r--   0 root         (0) docker     (999)     2501 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/swarm.py
--rw-r--r--   0 root         (0) docker     (999)     2608 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/task.py
--rw-r--r--   0 root         (0) docker     (999)      509 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/workflow_config.py
--rw-r--r--   0 root         (0) docker     (999)     9950 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/workflow.py
--rw-r--r--   0 root         (0) docker     (999)     2315 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/compose.py
--rw-r--r--   0 root         (0) docker     (999)     3539 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/config.py
--rw-r--r--   0 root         (0) docker     (999)     3467 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/docker.py
--rw-r--r--   0 root         (0) docker     (999)     3688 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/docker_image.py
--rw-r--r--   0 root         (0) docker     (999)      641 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/entrypoints.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.866718 compose-flow-4.0.0rc1/src/compose_flow/environment/
--rw-r--r--   0 root         (0) docker     (999)        0 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/__init__.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.866718 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/
--rw-r--r--   0 root         (0) docker     (999)      381 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/__init__.py
--rw-r--r--   0 root         (0) docker     (999)     1078 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/base_backend.py
--rw-r--r--   0 root         (0) docker     (999)     1227 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/kube_backend.py
--rw-r--r--   0 root         (0) docker     (999)     1467 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/local_backend.py
--rw-r--r--   0 root         (0) docker     (999)     1218 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/rancher_backend.py
--rw-r--r--   0 root         (0) docker     (999)     3759 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/swarm_backend.py
--rw-r--r--   0 root         (0) docker     (999)     2789 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/errors.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.866718 compose-flow-4.0.0rc1/src/compose_flow/kube/
--rw-r--r--   0 root         (0) docker     (999)        0 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/kube/__init__.py
--rw-r--r--   0 root         (0) docker     (999)     8131 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/kube/checks.py
--rw-r--r--   0 root         (0) docker     (999)    23597 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/kube/mixins.py
--rw-r--r--   0 root         (0) docker     (999)      708 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/settings.py
--rw-r--r--   0 root         (0) docker     (999)      895 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/shell.py
--rw-r--r--   0 root         (0) docker     (999)     6180 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/utils.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.862718 compose-flow-4.0.0rc1/src/compose_flow.egg-info/
--rw-r--r--   0 root         (0) docker     (999)     1964 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) docker     (999)     4345 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) docker     (999)        1 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) docker     (999)       71 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) docker     (999)       68 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/requires.txt
--rw-r--r--   0 root         (0) docker     (999)       19 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.870718 compose-flow-4.0.0rc1/src/tests/
--rw-r--r--   0 root         (0) docker     (999)      487 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/__init__.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/src/tests/files/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.870718 compose-flow-4.0.0rc1/src/tests/files/answers/
--rw-r--r--   0 root         (0) docker     (999)      137 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/answers/good-resources-answers.yaml
--rw-r--r--   0 root         (0) docker     (999)       47 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/answers/multidoc-answers.yaml
--rw-r--r--   0 root         (0) docker     (999)       90 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/answers/no-limits-answers.yaml
--rw-r--r--   0 root         (0) docker     (999)       86 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/answers/no-requests-answers.yaml
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.870718 compose-flow-4.0.0rc1/src/tests/files/manifests/
--rw-r--r--   0 root         (0) docker     (999)       97 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/external-zalando-ingress.yaml
--rw-r--r--   0 root         (0) docker     (999)     2115 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/good-cronjob.yaml
--rw-r--r--   0 root         (0) docker     (999)     1452 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/good-init-deployment.yaml
--rw-r--r--   0 root         (0) docker     (999)      919 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/good-job.yaml
--rw-r--r--   0 root         (0) docker     (999)       90 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/internal-zalando-ingress.yaml
--rw-r--r--   0 root         (0) docker     (999)      211 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/invalid-ingress-multidoc.yaml
--rw-r--r--   0 root         (0) docker     (999)       24 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/invalid-zalando-ingress.yaml
--rw-r--r--   0 root         (0) docker     (999)       78 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/nginx-ingress.yaml
--rw-r--r--   0 root         (0) docker     (999)     2233 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/no-limits-deployment.yaml
--rw-r--r--   0 root         (0) docker     (999)      272 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/no-resources-job.yaml
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/src/tests/files/profiles/
--rw-r--r--   0 root         (0) docker     (999)       68 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/global_no_constraints.yml
--rw-r--r--   0 root         (0) docker     (999)      205 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/limit_and_reservation.yml
--rw-r--r--   0 root         (0) docker     (999)      105 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/limit_no_reservation.yml
--rw-r--r--   0 root         (0) docker     (999)       37 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/no_constraints.yml
--rw-r--r--   0 root         (0) docker     (999)      143 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/no_node_constraints.yml
--rw-r--r--   0 root         (0) docker     (999)      111 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/reservation_no_limit.yml
--rw-r--r--   0 root         (0) docker     (999)       66 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/resources_nothing_set.yml
--rw-r--r--   0 root         (0) docker     (999)      119 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/with_node_constraints.yml
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/src/tests/files/values/
--rw-r--r--   0 root         (0) docker     (999)       93 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/values/good-resources-values.yaml
--rw-r--r--   0 root         (0) docker     (999)       69 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/values/multidoc-values.yaml
--rw-r--r--   0 root         (0) docker     (999)     3203 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_backends.py
--rw-r--r--   0 root         (0) docker     (999)      695 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_base.py
--rw-r--r--   0 root         (0) docker     (999)     7664 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_deploy.py
--rw-r--r--   0 root         (0) docker     (999)      813 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_docker.py
--rw-r--r--   0 root         (0) docker     (999)     5524 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_docker_image.py
--rw-r--r--   0 root         (0) docker     (999)     6417 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_env.py
--rw-r--r--   0 root         (0) docker     (999)     6254 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_kube_checks.py
--rw-r--r--   0 root         (0) docker     (999)      606 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_kube_mixins.py
--rw-r--r--   0 root         (0) docker     (999)      719 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_passthrough.py
--rw-r--r--   0 root         (0) docker     (999)     3813 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_pod.py
--rw-r--r--   0 root         (0) docker     (999)     8457 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_profile.py
--rw-r--r--   0 root         (0) docker     (999)     5287 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_publish.py
--rw-r--r--   0 root         (0) docker     (999)     1454 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_remote.py
--rw-r--r--   0 root         (0) docker     (999)      903 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_service.py
--rw-r--r--   0 root         (0) docker     (999)      468 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_shell.py
--rw-r--r--   0 root         (0) docker     (999)      976 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_task.py
--rw-r--r--   0 root         (0) docker     (999)      923 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_utils.py
--rw-r--r--   0 root         (0) docker     (999)     6266 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_workflow.py
--rw-r--r--   0 root         (0) docker     (999)      408 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/utils.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/
+-rw-r--r--   0 root         (0) docker     (999)       49 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/.dockerignore
+-rw-r--r--   0 root         (0) docker     (999)      104 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/.gitignore
+-rw-r--r--   0 root         (0) docker     (999)     2642 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/Dockerfile
+-rw-r--r--   0 root         (0) docker     (999)      508 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/Jenkinsfile
+-rw-r--r--   0 root         (0) docker     (999)    11357 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/LICENSE
+-rw-r--r--   0 root         (0) docker     (999)       34 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) docker     (999)     1970 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) docker     (999)      345 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/Pipfile
+-rw-r--r--   0 root         (0) docker     (999)    71739 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/Pipfile.lock
+-rw-r--r--   0 root         (0) docker     (999)     1691 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/README.md
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/compose/
+-rw-r--r--   0 root         (0) docker     (999)     1171 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/compose-flow.yml
+-rw-r--r--   0 root         (0) docker     (999)       54 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/docker-compose.mount.yml
+-rw-r--r--   0 root         (0) docker     (999)       78 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/docker-compose.publish.yml
+-rw-r--r--   0 root         (0) docker     (999)      157 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/docker-compose.results.yml
+-rw-r--r--   0 root         (0) docker     (999)       73 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/docker-compose.yml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/docs/
+-rw-r--r--   0 root         (0) docker     (999)     9824 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/docs/advanced.md
+-rw-r--r--   0 root         (0) docker     (999)     9328 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/docs/k8s.md
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.433369 compose-flow-4.0.0rc2/files/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.433369 compose-flow-4.0.0rc2/files/home/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/files/home/swarmclient/
+-rw-r--r--   0 root         (0) docker     (999)      142 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/files/home/swarmclient/.pypirc
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.433369 compose-flow-4.0.0rc2/files/usr/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.433369 compose-flow-4.0.0rc2/files/usr/local/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/files/usr/local/bin/
+-rw-r--r--   0 root         (0) docker     (999)      210 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/files/usr/local/bin/entrypoint.sh
+-rw-r--r--   0 root         (0) docker     (999)      132 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/pylama.ini
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.441369 compose-flow-4.0.0rc2/scripts/
+-rw-r--r--   0 root         (0) docker     (999)       71 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/black.sh
+-rw-r--r--   0 root         (0) docker     (999)      671 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/dump_swarm_config.py
+-rwxr-xr-x   0 root         (0) docker     (999)      245 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/lock.sh
+-rw-r--r--   0 root         (0) docker     (999)      304 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/publish.sh
+-rw-r--r--   0 root         (0) docker     (999)      101 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/tag_and_publish.sh
+-rw-r--r--   0 root         (0) docker     (999)      119 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/watch-tests.sh
+-rw-r--r--   0 root         (0) docker     (999)       83 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) docker     (999)     2169 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/setup.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/src/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.441369 compose-flow-4.0.0rc2/src/compose_flow/
+-rw-r--r--   0 root         (0) docker     (999)        0 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.441369 compose-flow-4.0.0rc2/src/compose_flow/commands/
+-rw-r--r--   0 root         (0) docker     (999)       31 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.445370 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/
+-rw-r--r--   0 root         (0) docker     (999)     3141 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/__init__.py
+-rw-r--r--   0 root         (0) docker     (999)     5042 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/base.py
+-rw-r--r--   0 root         (0) docker     (999)      212 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/build.py
+-rw-r--r--   0 root         (0) docker     (999)     1477 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/compose.py
+-rw-r--r--   0 root         (0) docker     (999)     3250 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/deploy.py
+-rw-r--r--   0 root         (0) docker     (999)      272 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/docker.py
+-rw-r--r--   0 root         (0) docker     (999)    14787 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/env.py
+-rw-r--r--   0 root         (0) docker     (999)      496 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/helm.py
+-rw-r--r--   0 root         (0) docker     (999)      435 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/help.py
+-rw-r--r--   0 root         (0) docker     (999)     1230 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/kompose.py
+-rw-r--r--   0 root         (0) docker     (999)      503 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/kubectl.py
+-rw-r--r--   0 root         (0) docker     (999)     1577 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/passthrough_base.py
+-rw-r--r--   0 root         (0) docker     (999)     3672 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/pod.py
+-rw-r--r--   0 root         (0) docker     (999)    14763 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/profile.py
+-rw-r--r--   0 root         (0) docker     (999)     2722 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/publish.py
+-rw-r--r--   0 root         (0) docker     (999)      490 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/rancher.py
+-rw-r--r--   0 root         (0) docker     (999)     6611 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/remote.py
+-rw-r--r--   0 root         (0) docker     (999)     1770 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/remote_config.py
+-rw-r--r--   0 root         (0) docker     (999)     6227 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/service.py
+-rw-r--r--   0 root         (0) docker     (999)     2501 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/swarm.py
+-rw-r--r--   0 root         (0) docker     (999)     2608 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/task.py
+-rw-r--r--   0 root         (0) docker     (999)      509 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/workflow_config.py
+-rw-r--r--   0 root         (0) docker     (999)     9950 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/workflow.py
+-rw-r--r--   0 root         (0) docker     (999)     2315 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/compose.py
+-rw-r--r--   0 root         (0) docker     (999)     3539 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/config.py
+-rw-r--r--   0 root         (0) docker     (999)     3445 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/docker.py
+-rw-r--r--   0 root         (0) docker     (999)     3688 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/docker_image.py
+-rw-r--r--   0 root         (0) docker     (999)      641 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/entrypoints.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.445370 compose-flow-4.0.0rc2/src/compose_flow/environment/
+-rw-r--r--   0 root         (0) docker     (999)        0 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.445370 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/
+-rw-r--r--   0 root         (0) docker     (999)      381 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/__init__.py
+-rw-r--r--   0 root         (0) docker     (999)     1078 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/base_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     1227 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/kube_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     1467 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/local_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     1218 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/rancher_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     3737 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/swarm_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     2789 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/errors.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.445370 compose-flow-4.0.0rc2/src/compose_flow/kube/
+-rw-r--r--   0 root         (0) docker     (999)        0 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/kube/__init__.py
+-rw-r--r--   0 root         (0) docker     (999)     8131 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/kube/checks.py
+-rw-r--r--   0 root         (0) docker     (999)    23354 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/kube/mixins.py
+-rw-r--r--   0 root         (0) docker     (999)      708 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/settings.py
+-rw-r--r--   0 root         (0) docker     (999)      895 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/shell.py
+-rw-r--r--   0 root         (0) docker     (999)     6019 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/utils.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.441369 compose-flow-4.0.0rc2/src/compose_flow.egg-info/
+-rw-r--r--   0 root         (0) docker     (999)     1970 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) docker     (999)     4345 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) docker     (999)        1 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) docker     (999)       71 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) docker     (999)       75 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) docker     (999)       19 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.449370 compose-flow-4.0.0rc2/src/tests/
+-rw-r--r--   0 root         (0) docker     (999)      487 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/src/tests/files/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.449370 compose-flow-4.0.0rc2/src/tests/files/answers/
+-rw-r--r--   0 root         (0) docker     (999)      137 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/answers/good-resources-answers.yaml
+-rw-r--r--   0 root         (0) docker     (999)       47 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/answers/multidoc-answers.yaml
+-rw-r--r--   0 root         (0) docker     (999)       90 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/answers/no-limits-answers.yaml
+-rw-r--r--   0 root         (0) docker     (999)       86 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/answers/no-requests-answers.yaml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.449370 compose-flow-4.0.0rc2/src/tests/files/manifests/
+-rw-r--r--   0 root         (0) docker     (999)       97 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/external-zalando-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)     2115 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/good-cronjob.yaml
+-rw-r--r--   0 root         (0) docker     (999)     1452 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/good-init-deployment.yaml
+-rw-r--r--   0 root         (0) docker     (999)      919 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/good-job.yaml
+-rw-r--r--   0 root         (0) docker     (999)       90 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/internal-zalando-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)      211 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/invalid-ingress-multidoc.yaml
+-rw-r--r--   0 root         (0) docker     (999)       24 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/invalid-zalando-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)       78 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/nginx-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)     2233 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/no-limits-deployment.yaml
+-rw-r--r--   0 root         (0) docker     (999)      272 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/no-resources-job.yaml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/src/tests/files/profiles/
+-rw-r--r--   0 root         (0) docker     (999)       68 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/global_no_constraints.yml
+-rw-r--r--   0 root         (0) docker     (999)      205 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/limit_and_reservation.yml
+-rw-r--r--   0 root         (0) docker     (999)      105 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/limit_no_reservation.yml
+-rw-r--r--   0 root         (0) docker     (999)       37 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/no_constraints.yml
+-rw-r--r--   0 root         (0) docker     (999)      143 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/no_node_constraints.yml
+-rw-r--r--   0 root         (0) docker     (999)      111 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/reservation_no_limit.yml
+-rw-r--r--   0 root         (0) docker     (999)       66 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/resources_nothing_set.yml
+-rw-r--r--   0 root         (0) docker     (999)      119 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/with_node_constraints.yml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/src/tests/files/values/
+-rw-r--r--   0 root         (0) docker     (999)       93 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/values/good-resources-values.yaml
+-rw-r--r--   0 root         (0) docker     (999)       69 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/values/multidoc-values.yaml
+-rw-r--r--   0 root         (0) docker     (999)     3203 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_backends.py
+-rw-r--r--   0 root         (0) docker     (999)      695 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_base.py
+-rw-r--r--   0 root         (0) docker     (999)     7664 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_deploy.py
+-rw-r--r--   0 root         (0) docker     (999)      813 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_docker.py
+-rw-r--r--   0 root         (0) docker     (999)     5524 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_docker_image.py
+-rw-r--r--   0 root         (0) docker     (999)     6417 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_env.py
+-rw-r--r--   0 root         (0) docker     (999)     6254 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_kube_checks.py
+-rw-r--r--   0 root         (0) docker     (999)      606 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_kube_mixins.py
+-rw-r--r--   0 root         (0) docker     (999)      719 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_passthrough.py
+-rw-r--r--   0 root         (0) docker     (999)     3813 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_pod.py
+-rw-r--r--   0 root         (0) docker     (999)     8457 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_profile.py
+-rw-r--r--   0 root         (0) docker     (999)     5287 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_publish.py
+-rw-r--r--   0 root         (0) docker     (999)     1454 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_remote.py
+-rw-r--r--   0 root         (0) docker     (999)      903 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_service.py
+-rw-r--r--   0 root         (0) docker     (999)      468 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_shell.py
+-rw-r--r--   0 root         (0) docker     (999)      976 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_task.py
+-rw-r--r--   0 root         (0) docker     (999)      923 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_utils.py
+-rw-r--r--   0 root         (0) docker     (999)     6266 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_workflow.py
+-rw-r--r--   0 root         (0) docker     (999)      408 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/utils.py
```

### Comparing `compose-flow-4.0.0rc1/Dockerfile` & `compose-flow-4.0.0rc2/Dockerfile`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/LICENSE` & `compose-flow-4.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/PKG-INFO` & `compose-flow-4.0.0rc2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: compose-flow
-Version: 4.0.0rc1
-Summary: codified workflows for docker compose
-Home-page: https://github.com/openslate/compose-flow
-Author: OpenSlate
-Author-email: code@openslate.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Compose Flow
 
 This utility is built on top of [Docker Compose](https://docs.docker.com/compose/) and [Swarm Mode](https://docs.docker.com/engine/swarm/).  It establishes workflow conventions that are easily shared between team members -- and butlers -- who need to manage and deploy services, including:
 
 - managing [Stacks](https://docs.docker.com/get-started/part5/#prerequisites) across multiple Swarms (e.g. separate dev and prod Swarms)
 - connecting to and working with service containers
 - building and publishing images
```

### Comparing `compose-flow-4.0.0rc1/Pipfile.lock` & `compose-flow-4.0.0rc2/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9858743686868686%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'cdb48d3d46a152c6bf5eaa21d821d5988f225693491ae25e67eff5555bbcba4f'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082', "*

 * *              "'sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9'], "*

 * *              "'version': '==2023.7.22'}, 'pyyaml': {'hashes': "*

 * *              "['sha256:06a0d7ba600ce0b2d2fe2e78453a470b5a6e000a985dd4a4e54e436cc36b0e97', "*

 * *          […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "7dd6933e48750b1df28fb1c9a69a8105d8579ec6b28627c3f28ae114bb410840"
+            "sha256": "cdb48d3d46a152c6bf5eaa21d821d5988f225693491ae25e67eff5555bbcba4f"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
@@ -55,19 +55,19 @@
                 "sha256:f716a1b57698a5b19062f3146cb5ce3549904028a2f267c2c0cf584eea3ad75b"
             ],
             "index": "pypi",
             "version": "==23.0.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -439,46 +439,30 @@
                 "sha256:41e12e0318bebc859fcc4d97d4db8d20ad21721a6aa5047dd59f090391cb549a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.21.1"
         },
         "pyyaml": {
             "hashes": [
-                "sha256:08682f6b72c722394747bddaf0aa62277e02557c0fd1c42cb853016a38f8dedf",
-                "sha256:0f5f5786c0e09baddcd8b4b45f20a7b5d61a7e7e99846e3c799b05c7c53fa696",
-                "sha256:129def1b7c1bf22faffd67b8f3724645203b79d8f4cc81f674654d9902cb4393",
-                "sha256:294db365efa064d00b8d1ef65d8ea2c3426ac366c0c4368d930bf1c5fb497f77",
-                "sha256:3b2b1824fe7112845700f815ff6a489360226a5609b96ec2190a45e62a9fc922",
-                "sha256:3bd0e463264cf257d1ffd2e40223b197271046d09dadf73a0fe82b9c1fc385a5",
-                "sha256:4465124ef1b18d9ace298060f4eccc64b0850899ac4ac53294547536533800c8",
-                "sha256:49d4cdd9065b9b6e206d0595fee27a96b5dd22618e7520c33204a4a3239d5b10",
-                "sha256:4e0583d24c881e14342eaf4ec5fbc97f934b999a6828693a99157fde912540cc",
-                "sha256:5accb17103e43963b80e6f837831f38d314a0495500067cb25afab2e8d7a4018",
-                "sha256:607774cbba28732bfa802b54baa7484215f530991055bb562efbed5b2f20a45e",
-                "sha256:6c78645d400265a062508ae399b60b8c167bf003db364ecb26dcab2bda048253",
-                "sha256:72a01f726a9c7851ca9bfad6fd09ca4e090a023c00945ea05ba1638c09dc3347",
-                "sha256:74c1485f7707cf707a7aef42ef6322b8f97921bd89be2ab6317fd782c2d53183",
-                "sha256:895f61ef02e8fed38159bb70f7e100e00f471eae2bc838cd0f4ebb21e28f8541",
-                "sha256:8c1be557ee92a20f184922c7b6424e8ab6691788e6d86137c5d93c1a6ec1b8fb",
-                "sha256:bb4191dfc9306777bc594117aee052446b3fa88737cd13b7188d0e7aa8162185",
-                "sha256:bfb51918d4ff3d77c1c856a9699f8492c612cde32fd3bcd344af9be34999bfdc",
-                "sha256:c20cfa2d49991c8b4147af39859b167664f2ad4561704ee74c1de03318e898db",
-                "sha256:cb333c16912324fd5f769fff6bc5de372e9e7a202247b48870bc251ed40239aa",
-                "sha256:d2d9808ea7b4af864f35ea216be506ecec180628aced0704e34aca0b040ffe46",
-                "sha256:d483ad4e639292c90170eb6f7783ad19490e7a8defb3e46f97dfe4bacae89122",
-                "sha256:dd5de0646207f053eb0d6c74ae45ba98c3395a571a2891858e87df7c9b9bd51b",
-                "sha256:e1d4970ea66be07ae37a3c2e48b5ec63f7ba6804bdddfdbd3cfd954d25a82e63",
-                "sha256:e4fac90784481d221a8e4b1162afa7c47ed953be40d31ab4629ae917510051df",
-                "sha256:fa5ae20527d8e831e8230cbffd9f8fe952815b2b7dae6ffec25318803a7528fc",
-                "sha256:fd7f6999a8070df521b6384004ef42833b9bd62cfee11a09bda1079b4b704247",
-                "sha256:fdc842473cd33f45ff6bce46aea678a54e3d21f1b61a7750ce3c498eedfe25d6",
-                "sha256:fe69978f3f768926cfa37b867e3843918e012cf83f680806599ddce33c2c68b0"
+                "sha256:06a0d7ba600ce0b2d2fe2e78453a470b5a6e000a985dd4a4e54e436cc36b0e97",
+                "sha256:240097ff019d7c70a4922b6869d8a86407758333f02203e0fc6ff79c5dcede76",
+                "sha256:4f4b913ca1a7319b33cfb1369e91e50354d6f07a135f3b901aca02aa95940bd2",
+                "sha256:6034f55dab5fea9e53f436aa68fa3ace2634918e8b5994d82f3621c04ff5ed2e",
+                "sha256:69f00dca373f240f842b2931fb2c7e14ddbacd1397d57157a9b005a6a9942648",
+                "sha256:73f099454b799e05e5ab51423c7bcf361c58d3206fa7b0d555426b1f4d9a3eaf",
+                "sha256:74809a57b329d6cc0fdccee6318f44b9b8649961fa73144a98735b0aaf029f1f",
+                "sha256:7739fc0fa8205b3ee8808aea45e968bc90082c10aef6ea95e855e10abf4a37b2",
+                "sha256:95f71d2af0ff4227885f7a6605c37fd53d3a106fcab511b8860ecca9fcf400ee",
+                "sha256:ad9c67312c84def58f3c04504727ca879cb0013b2517c85a9a253f0cb6380c0a",
+                "sha256:b8eac752c5e14d3eca0e6dd9199cd627518cb5ec06add0de9d32baeee6fe645d",
+                "sha256:cc8955cfbfc7a115fa81d85284ee61147059a753344bc51098f3ccd69b0d7e0c",
+                "sha256:d13155f591e6fcc1ec3b30685d50bf0711574e2c0dfffd7644babf8b5102ca1a"
             ],
             "index": "pypi",
-            "version": "==5.4.1"
+            "version": "==5.3.1"
         },
         "requests": {
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "markers": "python_version >= '3.7'",
@@ -597,19 +581,19 @@
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
-                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.5.7"
+            "version": "==2023.7.22"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
                 "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
                 "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
                 "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
@@ -694,19 +678,19 @@
                 "sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.1.6"
         },
         "dill": {
             "hashes": [
-                "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
-                "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
+                "sha256:76b122c08ef4ce2eedcd4d1abd8e641114bfc6c2867f49f3c41facf65bf19f5e",
+                "sha256:cc1c8b182eb3013e24bd475ff2e9295af86c1a38eb1aff128dac8962a9ce3c03"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==0.3.6"
+            "version": "==0.3.7"
         },
         "docutils": {
             "hashes": [
                 "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
@@ -816,19 +800,19 @@
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "more-itertools": {
             "hashes": [
-                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
-                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
+                "sha256:928d514ffd22b5b0a8fce326d57f423a55d2ff783b093bab217eda71e732330f",
+                "sha256:cd65437d7c4b615ab81c0640c0480bc29a550ea032891977681efd28344d51e1"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==9.1.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==10.0.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
```

### Comparing `compose-flow-4.0.0rc1/README.md` & `compose-flow-4.0.0rc2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: compose-flow
+Version: 4.0.0rc2
+Summary: codified workflows for docker compose
+Home-page: https://github.com/openslate/compose-flow
+Author: DoubleVerify
+Author-email: code@doubleverify.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Compose Flow
 
 This utility is built on top of [Docker Compose](https://docs.docker.com/compose/) and [Swarm Mode](https://docs.docker.com/engine/swarm/).  It establishes workflow conventions that are easily shared between team members -- and butlers -- who need to manage and deploy services, including:
 
 - managing [Stacks](https://docs.docker.com/get-started/part5/#prerequisites) across multiple Swarms (e.g. separate dev and prod Swarms)
 - connecting to and working with service containers
 - building and publishing images
```

### Comparing `compose-flow-4.0.0rc1/compose/compose-flow.yml` & `compose-flow-4.0.0rc2/compose/compose-flow.yml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/docs/advanced.md` & `compose-flow-4.0.0rc2/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/docs/k8s.md` & `compose-flow-4.0.0rc2/docs/k8s.md`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/scripts/dump_swarm_config.py` & `compose-flow-4.0.0rc2/scripts/dump_swarm_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 parser = argparse.ArgumentParser()
 parser.add_argument("root")
 
 args = parser.parse_args()
 
 
 proc = shell.execute('docker config ls --format "{{ .Name }}"', os.environ)
-for config_name in proc.stdout.decode("utf8").splitlines():
+for config_name in proc.splitlines():
     proc = shell.execute(
         f'docker config inspect {config_name} --format "{{{{ json .Spec.Data }}}}"',
         os.environ,
     )
-    buf_b64 = proc.stdout.decode("utf8").replace('"', "")
+    buf_b64 = proc.replace('"', "")
 
     if not os.path.exists(args.root):
         os.makedirs(args.root)
 
     path = os.path.join(args.root, config_name)
     with open(path, "wb") as fh:
         fh.write(base64.b64decode(buf_b64))
```

### Comparing `compose-flow-4.0.0rc1/setup.py` & `compose-flow-4.0.0rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,18 +55,19 @@
 
     return install_requires
 
 
 setup(
     name="compose-flow",
     url="https://github.com/openslate/compose-flow",
-    author="OpenSlate",
-    author_email="code@openslate.com",
+    author="DoubleVerify",
+    author_email="code@doubleverify.com",
     use_scm_version=True,
     description="codified workflows for docker compose",
+    license_files=("LICENSE",),
     long_description=readme(),
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=packages,
     entry_points={
         "console_scripts": ["compose-flow = compose_flow.entrypoints:compose_flow"]
     },
```

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/__init__.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/base.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/compose.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/compose.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/deploy.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/deploy.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/env.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/env.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/kompose.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/kompose.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/passthrough_base.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/passthrough_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,12 +42,12 @@
         command_s = " ".join([x if " " not in x else repr(x) for x in command])
 
         self.logger.info(command_s)
 
         if not args.dry_run:
             res = self.execute(command_s, _fg=True)
             if res and log_output:
-                self.logger.info(res.stdout.decode("utf-8").strip())
+                self.logger.info(res.strip())
 
     @property
     def logger(self) -> logging.Logger:
         return logging.getLogger(f"{__name__}.{self.__class__.__name__}")
```

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/pod.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/pod.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/profile.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/profile.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/publish.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/publish.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/remote.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         try:
             # very low-level command that does not need workflow environment
             proc = self.execute(f'pgrep -f "{pgrep_search}"', _env=os.environ)
         except shell.ErrorReturnCode_1:
             pass
         else:
-            for item in proc.stdout.decode("utf8").strip().splitlines():
+            for item in proc.strip().splitlines():
                 yield int(item)
 
     def get_socket(self):
         remote_host = self.get_remote_host()
         if not remote_host:
             raise EnvError("DOCKER_HOST not defined")
```

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/remote_config.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/remote_config.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/service.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
         # note; because this is being cached, create a list
         # instead of a generator becuase a generator can only
         # be iterated once
         items = []
 
         try:
-            output = proc.stdout.decode("utf8").splitlines()[1:]
+            output = proc.splitlines()[1:]
 
             # check to see there's at least one container listed
             output[0]
         except IndexError:
             raise errors.NoContainer()
         else:
             for item in output:
@@ -149,15 +149,15 @@
 
     def list_services(self):
         """
         Lists all the services for this stack
         """
         proc = self.execute(f"docker stack services {self.workflow.config_name}")
 
-        return proc.stdout.decode("utf8")
+        return proc
 
     def run_service(self):
         args = self.workflow.args
         line = self.select_container()
 
         container_info = line.strip()
         container_info_split = container_info.split()
```

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/swarm.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/swarm.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/task.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/task.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/commands/workflow.py` & `compose-flow-4.0.0rc2/src/compose_flow/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/compose.py` & `compose-flow-4.0.0rc2/src/compose_flow/compose.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/config.py` & `compose-flow-4.0.0rc2/src/compose_flow/config.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/docker.py` & `compose-flow-4.0.0rc2/src/compose_flow/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,8 +140,8 @@
     except shell.ErrorReturnCode_1 as exc:
         exc_s = f"{exc}".lower()
         if "cannot connect to the docker daemon" in exc_s:
             raise NotConnected()
 
         raise DockerError(exc)
 
-    return proc.stdout.decode("utf8")
+    return proc
```

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/docker_image.py` & `compose-flow-4.0.0rc2/src/compose_flow/docker_image.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/entrypoints.py` & `compose-flow-4.0.0rc2/src/compose_flow/entrypoints.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/base_backend.py` & `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/base_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/kube_backend.py` & `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/kube_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/local_backend.py` & `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/rancher_backend.py` & `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/rancher_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/swarm_backend.py` & `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/swarm_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def _check_swarm(self):
         """
         Checks to see if Docker is setup as a swarm
         """
         try:
             self.execute("docker config ls")  # pylint: disable=E1101
         except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-            message = exc.stderr.decode("utf8").strip().lower()
+            message = exc.strip().lower()
 
             if "this node is not a swarm manager" in message:
                 self.init_swarm(prompt=True)
             else:
                 raise
 
     def init_swarm(self, prompt: bool = False) -> None:
```

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/errors.py` & `compose-flow-4.0.0rc2/src/compose_flow/errors.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/kube/checks.py` & `compose-flow-4.0.0rc2/src/compose_flow/kube/checks.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/kube/mixins.py` & `compose-flow-4.0.0rc2/src/compose_flow/kube/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         Checks for existence of the target namespace for native kubectl.
 
         If not found, attempt to create it.
         """
         try:
             self.execute(f"{self.kubectl_command} get namespace {self.namespace}")
         except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-            message = exc.stderr.decode("utf8").strip().lower()
+            message = exc.strip().lower()
 
             if f'namespaces "{self.namespace}" not found' in message:
                 self.logger.warning(
                     "Namespace '%s' not found - attempting to create it...",
                     self.namespace,
                 )
                 self.execute(
@@ -127,20 +127,15 @@
 
     def _check_rancher_namespace(self):
         """
         Checks for existence of the target namespace for Rancher.
 
         If not found, attempt to create it.
         """
-        namespaces = (
-            self.execute("rancher namespace ls --quiet")
-            .stdout.decode("utf8")
-            .strip()
-            .split("\n")
-        )
+        namespaces = self.execute("rancher namespace ls --quiet").strip().split("\n")
 
         if self.namespace not in namespaces:
             self.logger.warning(
                 "Namespace '%s' not found - attempting to create it...", self.namespace
             )
             self.execute(f"rancher namespaces create {self.namespace}")
 
@@ -190,15 +185,15 @@
         patch_string = f'{{"data": {{"{self.env_key}": "{b64_env}"}}}}'
         if not self.secret_exists:
             try:
                 self.execute(
                     f"{self.kubectl_command} create secret generic --namespace {self.namespace} {self.secret_name}"
                 )
             except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-                message = exc.stderr.decode("utf8").strip().lower()
+                message = exc.strip().lower()
 
                 if f'secrets "{self.secret_name}" already exists' not in message:
                     raise
 
         self.execute(
             f"{self.kubectl_command} patch secrets --namespace {self.namespace} {self.secret_name} --patch '{patch_string}'"
         )
@@ -299,34 +294,29 @@
         """
         Switch Rancher CLI context to target specified cluster based on environment
         and specified project name from compose-flow.yml
         """
         # Get the project name specified in compose-flow.yml
         target_project_name = self.project_name
 
-        current_context = (
-            self.execute("rancher context current")
-            .stdout.decode("utf8")
-            .strip()
-            .split(" ")
-        )
+        current_context = self.execute("rancher context current").strip().split(" ")
         correct_cluster = current_context[0] == f"Cluster:{self.cluster_name}"
         correct_project = current_context[1] == f"Project:{target_project_name}"
 
         if correct_cluster and correct_project:
             # Don't do anything if context is already correct
             return
 
         base_context_switch_command = "rancher context switch "
         name_context_switch_command = base_context_switch_command + target_project_name
         try:
             self.logger.info(name_context_switch_command)
             self.execute(name_context_switch_command)
         except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-            stderr = str(exc.stderr)
+            stderr = str(exc)
             if "Multiple resources of type project found for name" in stderr:
                 self.logger.info(
                     "Multiple clusters have a project called %s - "
                     "switching context by Project ID",
                     target_project_name,
                 )
                 # Choose the one that matches target cluster ID
@@ -470,15 +460,15 @@
         creation_command = f"rancher namespaces create {namespace}"
 
         print(f"Creating namespace {namespace} in project {self.project_name}")
         if not dry_run:
             try:
                 self.execute(creation_command)
             except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-                message = exc.stderr.decode("utf8").strip()
+                message = exc.strip()
                 if "code=AlreadyExists" in message:
                     raise errors.RancherNamespaceAlreadyExists(
                         f"Namespace {namespace} already exists in another project!"
                     )
                 else:
                     raise
```

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/settings.py` & `compose-flow-4.0.0rc2/src/compose_flow/settings.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/shell.py` & `compose-flow-4.0.0rc2/src/compose_flow/shell.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/compose_flow/utils.py` & `compose-flow-4.0.0rc2/src/compose_flow/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,27 +59,24 @@
         print_warning: when `tag-version` results in error, print a warning
     """
     # inject the version from tag-version command into the loaded environment
     tag_version = default or "unknown"
     try:
         proc = shell.execute("tag-version version --format docker", os.environ)
     except Exception as exc:
-        try:
-            error_message = exc.stderr.decode("utf8")  # pylint: disable=E1101
-        except:
-            error_message = exc.stderr  # pylint: disable=E1101
+        error_message = str(exc)
 
         if "not clean" in error_message:
             tag_version = f"{tag_version}-dirty"
 
         raise TagVersionError(
             "Warning: tag-version failed", shell_exception=exc, tag_version=tag_version
         )
     else:
-        tag_version = proc.stdout.decode("utf8").strip()
+        tag_version = proc.strip()
 
     return tag_version
 
 
 # https://gist.github.com/mahmoud/db02d16ac89fa401b968
 def remerge(target_list, sourced=False):
     """Takes a list of containers (e.g., dicts) and merges them using
```

### Comparing `compose-flow-4.0.0rc1/src/compose_flow.egg-info/PKG-INFO` & `compose-flow-4.0.0rc2/src/compose_flow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: compose-flow
-Version: 4.0.0rc1
+Version: 4.0.0rc2
 Summary: codified workflows for docker compose
 Home-page: https://github.com/openslate/compose-flow
-Author: OpenSlate
-Author-email: code@openslate.com
+Author: DoubleVerify
+Author-email: code@doubleverify.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Compose Flow
 
 This utility is built on top of [Docker Compose](https://docs.docker.com/compose/) and [Swarm Mode](https://docs.docker.com/engine/swarm/).  It establishes workflow conventions that are easily shared between team members -- and butlers -- who need to manage and deploy services, including:
```

### Comparing `compose-flow-4.0.0rc1/src/compose_flow.egg-info/SOURCES.txt` & `compose-flow-4.0.0rc2/src/compose_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/files/manifests/good-cronjob.yaml` & `compose-flow-4.0.0rc2/src/tests/files/manifests/good-cronjob.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/files/manifests/good-init-deployment.yaml` & `compose-flow-4.0.0rc2/src/tests/files/manifests/good-init-deployment.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/files/manifests/good-job.yaml` & `compose-flow-4.0.0rc2/src/tests/files/manifests/good-job.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/files/manifests/no-limits-deployment.yaml` & `compose-flow-4.0.0rc2/src/tests/files/manifests/no-limits-deployment.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_backends.py` & `compose-flow-4.0.0rc2/src/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_base.py` & `compose-flow-4.0.0rc2/src/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_deploy.py` & `compose-flow-4.0.0rc2/src/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_docker.py` & `compose-flow-4.0.0rc2/src/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_docker_image.py` & `compose-flow-4.0.0rc2/src/tests/test_docker_image.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_env.py` & `compose-flow-4.0.0rc2/src/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_kube_checks.py` & `compose-flow-4.0.0rc2/src/tests/test_kube_checks.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_kube_mixins.py` & `compose-flow-4.0.0rc2/src/tests/test_kube_mixins.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_passthrough.py` & `compose-flow-4.0.0rc2/src/tests/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_pod.py` & `compose-flow-4.0.0rc2/src/tests/test_pod.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_profile.py` & `compose-flow-4.0.0rc2/src/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_publish.py` & `compose-flow-4.0.0rc2/src/tests/test_publish.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_remote.py` & `compose-flow-4.0.0rc2/src/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_service.py` & `compose-flow-4.0.0rc2/src/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_task.py` & `compose-flow-4.0.0rc2/src/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_utils.py` & `compose-flow-4.0.0rc2/src/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc1/src/tests/test_workflow.py` & `compose-flow-4.0.0rc2/src/tests/test_workflow.py`

 * *Files identical despite different names*

