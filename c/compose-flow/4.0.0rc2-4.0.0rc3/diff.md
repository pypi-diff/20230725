# Comparing `tmp/compose-flow-4.0.0rc2.tar.gz` & `tmp/compose-flow-4.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose-flow-4.0.0rc2.tar", last modified: Tue Jul 25 18:45:10 2023, max compression
+gzip compressed data, was "compose-flow-4.0.0rc3.tar", last modified: Tue Jul 25 19:25:20 2023, max compression
```

## Comparing `compose-flow-4.0.0rc2.tar` & `compose-flow-4.0.0rc3.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/
--rw-r--r--   0 root         (0) docker     (999)       49 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/.dockerignore
--rw-r--r--   0 root         (0) docker     (999)      104 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/.gitignore
--rw-r--r--   0 root         (0) docker     (999)     2642 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/Dockerfile
--rw-r--r--   0 root         (0) docker     (999)      508 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/Jenkinsfile
--rw-r--r--   0 root         (0) docker     (999)    11357 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/LICENSE
--rw-r--r--   0 root         (0) docker     (999)       34 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) docker     (999)     1970 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) docker     (999)      345 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/Pipfile
--rw-r--r--   0 root         (0) docker     (999)    71739 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/Pipfile.lock
--rw-r--r--   0 root         (0) docker     (999)     1691 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/README.md
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/compose/
--rw-r--r--   0 root         (0) docker     (999)     1171 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/compose-flow.yml
--rw-r--r--   0 root         (0) docker     (999)       54 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/docker-compose.mount.yml
--rw-r--r--   0 root         (0) docker     (999)       78 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/docker-compose.publish.yml
--rw-r--r--   0 root         (0) docker     (999)      157 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/docker-compose.results.yml
--rw-r--r--   0 root         (0) docker     (999)       73 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/compose/docker-compose.yml
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/docs/
--rw-r--r--   0 root         (0) docker     (999)     9824 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/docs/advanced.md
--rw-r--r--   0 root         (0) docker     (999)     9328 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/docs/k8s.md
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.433369 compose-flow-4.0.0rc2/files/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.433369 compose-flow-4.0.0rc2/files/home/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/files/home/swarmclient/
--rw-r--r--   0 root         (0) docker     (999)      142 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/files/home/swarmclient/.pypirc
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.433369 compose-flow-4.0.0rc2/files/usr/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.433369 compose-flow-4.0.0rc2/files/usr/local/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/files/usr/local/bin/
--rw-r--r--   0 root         (0) docker     (999)      210 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/files/usr/local/bin/entrypoint.sh
--rw-r--r--   0 root         (0) docker     (999)      132 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/pylama.ini
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.441369 compose-flow-4.0.0rc2/scripts/
--rw-r--r--   0 root         (0) docker     (999)       71 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/black.sh
--rw-r--r--   0 root         (0) docker     (999)      671 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/dump_swarm_config.py
--rwxr-xr-x   0 root         (0) docker     (999)      245 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/lock.sh
--rw-r--r--   0 root         (0) docker     (999)      304 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/publish.sh
--rw-r--r--   0 root         (0) docker     (999)      101 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/tag_and_publish.sh
--rw-r--r--   0 root         (0) docker     (999)      119 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/scripts/watch-tests.sh
--rw-r--r--   0 root         (0) docker     (999)       83 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/setup.cfg
--rw-r--r--   0 root         (0) docker     (999)     2169 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/setup.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/src/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.441369 compose-flow-4.0.0rc2/src/compose_flow/
--rw-r--r--   0 root         (0) docker     (999)        0 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/__init__.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.441369 compose-flow-4.0.0rc2/src/compose_flow/commands/
--rw-r--r--   0 root         (0) docker     (999)       31 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/__init__.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.445370 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/
--rw-r--r--   0 root         (0) docker     (999)     3141 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/__init__.py
--rw-r--r--   0 root         (0) docker     (999)     5042 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/base.py
--rw-r--r--   0 root         (0) docker     (999)      212 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/build.py
--rw-r--r--   0 root         (0) docker     (999)     1477 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/compose.py
--rw-r--r--   0 root         (0) docker     (999)     3250 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/deploy.py
--rw-r--r--   0 root         (0) docker     (999)      272 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/docker.py
--rw-r--r--   0 root         (0) docker     (999)    14787 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/env.py
--rw-r--r--   0 root         (0) docker     (999)      496 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/helm.py
--rw-r--r--   0 root         (0) docker     (999)      435 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/help.py
--rw-r--r--   0 root         (0) docker     (999)     1230 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/kompose.py
--rw-r--r--   0 root         (0) docker     (999)      503 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/kubectl.py
--rw-r--r--   0 root         (0) docker     (999)     1577 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/passthrough_base.py
--rw-r--r--   0 root         (0) docker     (999)     3672 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/pod.py
--rw-r--r--   0 root         (0) docker     (999)    14763 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/profile.py
--rw-r--r--   0 root         (0) docker     (999)     2722 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/publish.py
--rw-r--r--   0 root         (0) docker     (999)      490 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/rancher.py
--rw-r--r--   0 root         (0) docker     (999)     6611 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/remote.py
--rw-r--r--   0 root         (0) docker     (999)     1770 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/remote_config.py
--rw-r--r--   0 root         (0) docker     (999)     6227 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/service.py
--rw-r--r--   0 root         (0) docker     (999)     2501 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/swarm.py
--rw-r--r--   0 root         (0) docker     (999)     2608 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/task.py
--rw-r--r--   0 root         (0) docker     (999)      509 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/workflow_config.py
--rw-r--r--   0 root         (0) docker     (999)     9950 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/commands/workflow.py
--rw-r--r--   0 root         (0) docker     (999)     2315 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/compose.py
--rw-r--r--   0 root         (0) docker     (999)     3539 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/config.py
--rw-r--r--   0 root         (0) docker     (999)     3445 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/docker.py
--rw-r--r--   0 root         (0) docker     (999)     3688 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/docker_image.py
--rw-r--r--   0 root         (0) docker     (999)      641 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/entrypoints.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.445370 compose-flow-4.0.0rc2/src/compose_flow/environment/
--rw-r--r--   0 root         (0) docker     (999)        0 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/__init__.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.445370 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/
--rw-r--r--   0 root         (0) docker     (999)      381 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/__init__.py
--rw-r--r--   0 root         (0) docker     (999)     1078 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/base_backend.py
--rw-r--r--   0 root         (0) docker     (999)     1227 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/kube_backend.py
--rw-r--r--   0 root         (0) docker     (999)     1467 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/local_backend.py
--rw-r--r--   0 root         (0) docker     (999)     1218 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/rancher_backend.py
--rw-r--r--   0 root         (0) docker     (999)     3737 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/environment/backends/swarm_backend.py
--rw-r--r--   0 root         (0) docker     (999)     2789 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/errors.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.445370 compose-flow-4.0.0rc2/src/compose_flow/kube/
--rw-r--r--   0 root         (0) docker     (999)        0 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/kube/__init__.py
--rw-r--r--   0 root         (0) docker     (999)     8131 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/kube/checks.py
--rw-r--r--   0 root         (0) docker     (999)    23354 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/kube/mixins.py
--rw-r--r--   0 root         (0) docker     (999)      708 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/settings.py
--rw-r--r--   0 root         (0) docker     (999)      895 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/shell.py
--rw-r--r--   0 root         (0) docker     (999)     6019 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/compose_flow/utils.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.441369 compose-flow-4.0.0rc2/src/compose_flow.egg-info/
--rw-r--r--   0 root         (0) docker     (999)     1970 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) docker     (999)     4345 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) docker     (999)        1 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) docker     (999)       71 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) docker     (999)       75 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/requires.txt
--rw-r--r--   0 root         (0) docker     (999)       19 2023-07-25 18:45:10.000000 compose-flow-4.0.0rc2/src/compose_flow.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.449370 compose-flow-4.0.0rc2/src/tests/
--rw-r--r--   0 root         (0) docker     (999)      487 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/__init__.py
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.437369 compose-flow-4.0.0rc2/src/tests/files/
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.449370 compose-flow-4.0.0rc2/src/tests/files/answers/
--rw-r--r--   0 root         (0) docker     (999)      137 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/answers/good-resources-answers.yaml
--rw-r--r--   0 root         (0) docker     (999)       47 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/answers/multidoc-answers.yaml
--rw-r--r--   0 root         (0) docker     (999)       90 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/answers/no-limits-answers.yaml
--rw-r--r--   0 root         (0) docker     (999)       86 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/answers/no-requests-answers.yaml
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.449370 compose-flow-4.0.0rc2/src/tests/files/manifests/
--rw-r--r--   0 root         (0) docker     (999)       97 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/external-zalando-ingress.yaml
--rw-r--r--   0 root         (0) docker     (999)     2115 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/good-cronjob.yaml
--rw-r--r--   0 root         (0) docker     (999)     1452 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/good-init-deployment.yaml
--rw-r--r--   0 root         (0) docker     (999)      919 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/good-job.yaml
--rw-r--r--   0 root         (0) docker     (999)       90 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/internal-zalando-ingress.yaml
--rw-r--r--   0 root         (0) docker     (999)      211 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/invalid-ingress-multidoc.yaml
--rw-r--r--   0 root         (0) docker     (999)       24 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/invalid-zalando-ingress.yaml
--rw-r--r--   0 root         (0) docker     (999)       78 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/nginx-ingress.yaml
--rw-r--r--   0 root         (0) docker     (999)     2233 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/no-limits-deployment.yaml
--rw-r--r--   0 root         (0) docker     (999)      272 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/manifests/no-resources-job.yaml
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/src/tests/files/profiles/
--rw-r--r--   0 root         (0) docker     (999)       68 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/global_no_constraints.yml
--rw-r--r--   0 root         (0) docker     (999)      205 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/limit_and_reservation.yml
--rw-r--r--   0 root         (0) docker     (999)      105 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/limit_no_reservation.yml
--rw-r--r--   0 root         (0) docker     (999)       37 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/no_constraints.yml
--rw-r--r--   0 root         (0) docker     (999)      143 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/no_node_constraints.yml
--rw-r--r--   0 root         (0) docker     (999)      111 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/reservation_no_limit.yml
--rw-r--r--   0 root         (0) docker     (999)       66 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/resources_nothing_set.yml
--rw-r--r--   0 root         (0) docker     (999)      119 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/profiles/with_node_constraints.yml
-drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 18:45:10.453370 compose-flow-4.0.0rc2/src/tests/files/values/
--rw-r--r--   0 root         (0) docker     (999)       93 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/values/good-resources-values.yaml
--rw-r--r--   0 root         (0) docker     (999)       69 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/files/values/multidoc-values.yaml
--rw-r--r--   0 root         (0) docker     (999)     3203 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_backends.py
--rw-r--r--   0 root         (0) docker     (999)      695 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_base.py
--rw-r--r--   0 root         (0) docker     (999)     7664 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_deploy.py
--rw-r--r--   0 root         (0) docker     (999)      813 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_docker.py
--rw-r--r--   0 root         (0) docker     (999)     5524 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_docker_image.py
--rw-r--r--   0 root         (0) docker     (999)     6417 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_env.py
--rw-r--r--   0 root         (0) docker     (999)     6254 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_kube_checks.py
--rw-r--r--   0 root         (0) docker     (999)      606 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_kube_mixins.py
--rw-r--r--   0 root         (0) docker     (999)      719 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_passthrough.py
--rw-r--r--   0 root         (0) docker     (999)     3813 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_pod.py
--rw-r--r--   0 root         (0) docker     (999)     8457 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_profile.py
--rw-r--r--   0 root         (0) docker     (999)     5287 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_publish.py
--rw-r--r--   0 root         (0) docker     (999)     1454 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_remote.py
--rw-r--r--   0 root         (0) docker     (999)      903 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_service.py
--rw-r--r--   0 root         (0) docker     (999)      468 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_shell.py
--rw-r--r--   0 root         (0) docker     (999)      976 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_task.py
--rw-r--r--   0 root         (0) docker     (999)      923 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_utils.py
--rw-r--r--   0 root         (0) docker     (999)     6266 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/test_workflow.py
--rw-r--r--   0 root         (0) docker     (999)      408 2023-07-25 18:43:54.000000 compose-flow-4.0.0rc2/src/tests/utils.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.076285 compose-flow-4.0.0rc3/
+-rw-r--r--   0 root         (0) docker     (999)       49 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/.dockerignore
+-rw-r--r--   0 root         (0) docker     (999)      104 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/.gitignore
+-rw-r--r--   0 root         (0) docker     (999)     2642 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/Dockerfile
+-rw-r--r--   0 root         (0) docker     (999)      508 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/Jenkinsfile
+-rw-r--r--   0 root         (0) docker     (999)    11357 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/LICENSE
+-rw-r--r--   0 root         (0) docker     (999)       34 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) docker     (999)     1970 2023-07-25 19:25:20.076285 compose-flow-4.0.0rc3/PKG-INFO
+-rw-r--r--   0 root         (0) docker     (999)      345 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/Pipfile
+-rw-r--r--   0 root         (0) docker     (999)    71739 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/Pipfile.lock
+-rw-r--r--   0 root         (0) docker     (999)     1691 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/README.md
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.056285 compose-flow-4.0.0rc3/compose/
+-rw-r--r--   0 root         (0) docker     (999)     1171 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/compose/compose-flow.yml
+-rw-r--r--   0 root         (0) docker     (999)       54 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/compose/docker-compose.mount.yml
+-rw-r--r--   0 root         (0) docker     (999)       78 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/compose/docker-compose.publish.yml
+-rw-r--r--   0 root         (0) docker     (999)      157 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/compose/docker-compose.results.yml
+-rw-r--r--   0 root         (0) docker     (999)       73 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/compose/docker-compose.yml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.056285 compose-flow-4.0.0rc3/docs/
+-rw-r--r--   0 root         (0) docker     (999)     9824 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/docs/advanced.md
+-rw-r--r--   0 root         (0) docker     (999)     9328 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/docs/k8s.md
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.052285 compose-flow-4.0.0rc3/files/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.052285 compose-flow-4.0.0rc3/files/home/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.056285 compose-flow-4.0.0rc3/files/home/swarmclient/
+-rw-r--r--   0 root         (0) docker     (999)      142 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/files/home/swarmclient/.pypirc
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.052285 compose-flow-4.0.0rc3/files/usr/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.052285 compose-flow-4.0.0rc3/files/usr/local/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.056285 compose-flow-4.0.0rc3/files/usr/local/bin/
+-rw-r--r--   0 root         (0) docker     (999)      210 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/files/usr/local/bin/entrypoint.sh
+-rw-r--r--   0 root         (0) docker     (999)      132 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/pylama.ini
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.060285 compose-flow-4.0.0rc3/scripts/
+-rw-r--r--   0 root         (0) docker     (999)       71 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/scripts/black.sh
+-rw-r--r--   0 root         (0) docker     (999)      671 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/scripts/dump_swarm_config.py
+-rwxr-xr-x   0 root         (0) docker     (999)      245 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/scripts/lock.sh
+-rw-r--r--   0 root         (0) docker     (999)      304 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/scripts/publish.sh
+-rw-r--r--   0 root         (0) docker     (999)      101 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/scripts/tag_and_publish.sh
+-rw-r--r--   0 root         (0) docker     (999)      119 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/scripts/watch-tests.sh
+-rw-r--r--   0 root         (0) docker     (999)       83 2023-07-25 19:25:20.076285 compose-flow-4.0.0rc3/setup.cfg
+-rw-r--r--   0 root         (0) docker     (999)     2169 2023-07-25 19:25:19.000000 compose-flow-4.0.0rc3/setup.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.052285 compose-flow-4.0.0rc3/src/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.060285 compose-flow-4.0.0rc3/src/compose_flow/
+-rw-r--r--   0 root         (0) docker     (999)        0 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.064285 compose-flow-4.0.0rc3/src/compose_flow/commands/
+-rw-r--r--   0 root         (0) docker     (999)       31 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.068285 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/
+-rw-r--r--   0 root         (0) docker     (999)     3141 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/__init__.py
+-rw-r--r--   0 root         (0) docker     (999)     5042 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/base.py
+-rw-r--r--   0 root         (0) docker     (999)      212 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/build.py
+-rw-r--r--   0 root         (0) docker     (999)     1477 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/compose.py
+-rw-r--r--   0 root         (0) docker     (999)     3250 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/deploy.py
+-rw-r--r--   0 root         (0) docker     (999)      272 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/docker.py
+-rw-r--r--   0 root         (0) docker     (999)    14787 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/env.py
+-rw-r--r--   0 root         (0) docker     (999)      496 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/helm.py
+-rw-r--r--   0 root         (0) docker     (999)      435 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/help.py
+-rw-r--r--   0 root         (0) docker     (999)     1230 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/kompose.py
+-rw-r--r--   0 root         (0) docker     (999)      503 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/kubectl.py
+-rw-r--r--   0 root         (0) docker     (999)     1577 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/passthrough_base.py
+-rw-r--r--   0 root         (0) docker     (999)     3672 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/pod.py
+-rw-r--r--   0 root         (0) docker     (999)    14763 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/profile.py
+-rw-r--r--   0 root         (0) docker     (999)     2722 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/publish.py
+-rw-r--r--   0 root         (0) docker     (999)      490 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/rancher.py
+-rw-r--r--   0 root         (0) docker     (999)     6611 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/remote.py
+-rw-r--r--   0 root         (0) docker     (999)     1770 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/remote_config.py
+-rw-r--r--   0 root         (0) docker     (999)     6227 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/service.py
+-rw-r--r--   0 root         (0) docker     (999)     2501 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/swarm.py
+-rw-r--r--   0 root         (0) docker     (999)     2608 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/task.py
+-rw-r--r--   0 root         (0) docker     (999)      509 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/workflow_config.py
+-rw-r--r--   0 root         (0) docker     (999)     9950 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/commands/workflow.py
+-rw-r--r--   0 root         (0) docker     (999)     2315 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/compose.py
+-rw-r--r--   0 root         (0) docker     (999)     3539 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/config.py
+-rw-r--r--   0 root         (0) docker     (999)     3467 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/docker.py
+-rw-r--r--   0 root         (0) docker     (999)     3688 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/docker_image.py
+-rw-r--r--   0 root         (0) docker     (999)      641 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/entrypoints.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.068285 compose-flow-4.0.0rc3/src/compose_flow/environment/
+-rw-r--r--   0 root         (0) docker     (999)        0 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/environment/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.068285 compose-flow-4.0.0rc3/src/compose_flow/environment/backends/
+-rw-r--r--   0 root         (0) docker     (999)      381 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/environment/backends/__init__.py
+-rw-r--r--   0 root         (0) docker     (999)     1078 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/environment/backends/base_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     1227 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/environment/backends/kube_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     1467 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/environment/backends/local_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     1218 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/environment/backends/rancher_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     3737 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/environment/backends/swarm_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     2789 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/errors.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.068285 compose-flow-4.0.0rc3/src/compose_flow/kube/
+-rw-r--r--   0 root         (0) docker     (999)        0 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/kube/__init__.py
+-rw-r--r--   0 root         (0) docker     (999)     8131 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/kube/checks.py
+-rw-r--r--   0 root         (0) docker     (999)    23319 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/kube/mixins.py
+-rw-r--r--   0 root         (0) docker     (999)      708 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/settings.py
+-rw-r--r--   0 root         (0) docker     (999)      895 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/shell.py
+-rw-r--r--   0 root         (0) docker     (999)     6019 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/compose_flow/utils.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.064285 compose-flow-4.0.0rc3/src/compose_flow.egg-info/
+-rw-r--r--   0 root         (0) docker     (999)     1970 2023-07-25 19:25:19.000000 compose-flow-4.0.0rc3/src/compose_flow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) docker     (999)     4345 2023-07-25 19:25:20.000000 compose-flow-4.0.0rc3/src/compose_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) docker     (999)        1 2023-07-25 19:25:19.000000 compose-flow-4.0.0rc3/src/compose_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) docker     (999)       71 2023-07-25 19:25:19.000000 compose-flow-4.0.0rc3/src/compose_flow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) docker     (999)       75 2023-07-25 19:25:19.000000 compose-flow-4.0.0rc3/src/compose_flow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) docker     (999)       19 2023-07-25 19:25:19.000000 compose-flow-4.0.0rc3/src/compose_flow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.072285 compose-flow-4.0.0rc3/src/tests/
+-rw-r--r--   0 root         (0) docker     (999)      487 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.052285 compose-flow-4.0.0rc3/src/tests/files/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.072285 compose-flow-4.0.0rc3/src/tests/files/answers/
+-rw-r--r--   0 root         (0) docker     (999)      137 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/answers/good-resources-answers.yaml
+-rw-r--r--   0 root         (0) docker     (999)       47 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/answers/multidoc-answers.yaml
+-rw-r--r--   0 root         (0) docker     (999)       90 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/answers/no-limits-answers.yaml
+-rw-r--r--   0 root         (0) docker     (999)       86 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/answers/no-requests-answers.yaml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.076285 compose-flow-4.0.0rc3/src/tests/files/manifests/
+-rw-r--r--   0 root         (0) docker     (999)       97 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/external-zalando-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)     2115 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/good-cronjob.yaml
+-rw-r--r--   0 root         (0) docker     (999)     1452 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/good-init-deployment.yaml
+-rw-r--r--   0 root         (0) docker     (999)      919 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/good-job.yaml
+-rw-r--r--   0 root         (0) docker     (999)       90 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/internal-zalando-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)      211 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/invalid-ingress-multidoc.yaml
+-rw-r--r--   0 root         (0) docker     (999)       24 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/invalid-zalando-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)       78 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/nginx-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)     2233 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/no-limits-deployment.yaml
+-rw-r--r--   0 root         (0) docker     (999)      272 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/manifests/no-resources-job.yaml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.076285 compose-flow-4.0.0rc3/src/tests/files/profiles/
+-rw-r--r--   0 root         (0) docker     (999)       68 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/profiles/global_no_constraints.yml
+-rw-r--r--   0 root         (0) docker     (999)      205 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/profiles/limit_and_reservation.yml
+-rw-r--r--   0 root         (0) docker     (999)      105 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/profiles/limit_no_reservation.yml
+-rw-r--r--   0 root         (0) docker     (999)       37 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/profiles/no_constraints.yml
+-rw-r--r--   0 root         (0) docker     (999)      143 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/profiles/no_node_constraints.yml
+-rw-r--r--   0 root         (0) docker     (999)      111 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/profiles/reservation_no_limit.yml
+-rw-r--r--   0 root         (0) docker     (999)       66 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/profiles/resources_nothing_set.yml
+-rw-r--r--   0 root         (0) docker     (999)      119 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/profiles/with_node_constraints.yml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-25 19:25:20.076285 compose-flow-4.0.0rc3/src/tests/files/values/
+-rw-r--r--   0 root         (0) docker     (999)       93 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/values/good-resources-values.yaml
+-rw-r--r--   0 root         (0) docker     (999)       69 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/files/values/multidoc-values.yaml
+-rw-r--r--   0 root         (0) docker     (999)     3203 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_backends.py
+-rw-r--r--   0 root         (0) docker     (999)      695 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_base.py
+-rw-r--r--   0 root         (0) docker     (999)     7664 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_deploy.py
+-rw-r--r--   0 root         (0) docker     (999)      813 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_docker.py
+-rw-r--r--   0 root         (0) docker     (999)     5524 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_docker_image.py
+-rw-r--r--   0 root         (0) docker     (999)     6417 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_env.py
+-rw-r--r--   0 root         (0) docker     (999)     6254 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_kube_checks.py
+-rw-r--r--   0 root         (0) docker     (999)      606 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_kube_mixins.py
+-rw-r--r--   0 root         (0) docker     (999)      719 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_passthrough.py
+-rw-r--r--   0 root         (0) docker     (999)     3813 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_pod.py
+-rw-r--r--   0 root         (0) docker     (999)     8457 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_profile.py
+-rw-r--r--   0 root         (0) docker     (999)     5287 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_publish.py
+-rw-r--r--   0 root         (0) docker     (999)     1454 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_remote.py
+-rw-r--r--   0 root         (0) docker     (999)      903 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_service.py
+-rw-r--r--   0 root         (0) docker     (999)      468 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_shell.py
+-rw-r--r--   0 root         (0) docker     (999)      976 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_task.py
+-rw-r--r--   0 root         (0) docker     (999)      923 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_utils.py
+-rw-r--r--   0 root         (0) docker     (999)     6266 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/test_workflow.py
+-rw-r--r--   0 root         (0) docker     (999)      408 2023-07-25 19:24:15.000000 compose-flow-4.0.0rc3/src/tests/utils.py
```

### Comparing `compose-flow-4.0.0rc2/Dockerfile` & `compose-flow-4.0.0rc3/Dockerfile`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/LICENSE` & `compose-flow-4.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/PKG-INFO` & `compose-flow-4.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-flow
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: codified workflows for docker compose
 Home-page: https://github.com/openslate/compose-flow
 Author: DoubleVerify
 Author-email: code@doubleverify.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `compose-flow-4.0.0rc2/Pipfile.lock` & `compose-flow-4.0.0rc3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/README.md` & `compose-flow-4.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/compose/compose-flow.yml` & `compose-flow-4.0.0rc3/compose/compose-flow.yml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/docs/advanced.md` & `compose-flow-4.0.0rc3/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/docs/k8s.md` & `compose-flow-4.0.0rc3/docs/k8s.md`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/scripts/dump_swarm_config.py` & `compose-flow-4.0.0rc3/scripts/dump_swarm_config.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/setup.py` & `compose-flow-4.0.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/__init__.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/base.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/compose.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/compose.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/deploy.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/deploy.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/env.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/env.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/kompose.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/kompose.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/passthrough_base.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/passthrough_base.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/pod.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/pod.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/profile.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/profile.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/publish.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/publish.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/remote.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/remote.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/remote_config.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/remote_config.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/service.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/swarm.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/swarm.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/subcommands/task.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/subcommands/task.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/commands/workflow.py` & `compose-flow-4.0.0rc3/src/compose_flow/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/compose.py` & `compose-flow-4.0.0rc3/src/compose_flow/compose.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/config.py` & `compose-flow-4.0.0rc3/src/compose_flow/config.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/docker.py` & `compose-flow-4.0.0rc3/src/compose_flow/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,8 +140,8 @@
     except shell.ErrorReturnCode_1 as exc:
         exc_s = f"{exc}".lower()
         if "cannot connect to the docker daemon" in exc_s:
             raise NotConnected()
 
         raise DockerError(exc)
 
-    return proc
+    return proc.stdout.decode("utf8")
```

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/docker_image.py` & `compose-flow-4.0.0rc3/src/compose_flow/docker_image.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/entrypoints.py` & `compose-flow-4.0.0rc3/src/compose_flow/entrypoints.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/base_backend.py` & `compose-flow-4.0.0rc3/src/compose_flow/environment/backends/base_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/kube_backend.py` & `compose-flow-4.0.0rc3/src/compose_flow/environment/backends/kube_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/local_backend.py` & `compose-flow-4.0.0rc3/src/compose_flow/environment/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/rancher_backend.py` & `compose-flow-4.0.0rc3/src/compose_flow/environment/backends/rancher_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/environment/backends/swarm_backend.py` & `compose-flow-4.0.0rc3/src/compose_flow/environment/backends/swarm_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/errors.py` & `compose-flow-4.0.0rc3/src/compose_flow/errors.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/kube/checks.py` & `compose-flow-4.0.0rc3/src/compose_flow/kube/checks.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/kube/mixins.py` & `compose-flow-4.0.0rc3/src/compose_flow/kube/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     def _check_kube_context(self):
         """
         Checks to see if there is a kubecontext configured
         """
         try:
             self.execute("kubectl config current-context")
         except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-            message = exc.stderr.decode("utf8").strip().lower()
+            message = str(exc).lower()
 
             if "current-context is not set" in message:
                 raise errors.MissingKubeContext(
                     "No current context configured in kubectl!"
                 )
 
     def _check_kube_namespace(self):
@@ -110,15 +110,15 @@
         Checks for existence of the target namespace for native kubectl.
 
         If not found, attempt to create it.
         """
         try:
             self.execute(f"{self.kubectl_command} get namespace {self.namespace}")
         except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-            message = exc.strip().lower()
+            message = str(exc).lower()
 
             if f'namespaces "{self.namespace}" not found' in message:
                 self.logger.warning(
                     "Namespace '%s' not found - attempting to create it...",
                     self.namespace,
                 )
                 self.execute(
@@ -154,15 +154,15 @@
         """
         Reads environment from a Secret
         """
         try:
             raw_secret = self._get_secret(name)
             self.secret_exists = True
         except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-            message = exc.stderr.decode("utf8").strip().lower()
+            message = str(exc).lower()
 
             if f'secrets "{self.secret_name}" not found' in message:
                 self.secret_exists = False
                 raise errors.NoSuchConfig(
                     f"secret name={self.secret_name} in namespace={self.namespace} not found"
                 )
 
@@ -185,15 +185,15 @@
         patch_string = f'{{"data": {{"{self.env_key}": "{b64_env}"}}}}'
         if not self.secret_exists:
             try:
                 self.execute(
                     f"{self.kubectl_command} create secret generic --namespace {self.namespace} {self.secret_name}"
                 )
             except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-                message = exc.strip().lower()
+                message = str(exc).lower()
 
                 if f'secrets "{self.secret_name}" already exists' not in message:
                     raise
 
         self.execute(
             f"{self.kubectl_command} patch secrets --namespace {self.namespace} {self.secret_name} --patch '{patch_string}'"
         )
@@ -230,15 +230,15 @@
     @lru_cache()
     def cluster_listing(self):
         cluster_ls_command = f"rancher cluster ls --format '{CLUSTER_LS_FORMAT}'"
         output = str(self.execute(cluster_ls_command)).strip()
         for err in NONFATAL_ERROR_MESSAGES:
             if err in output:
                 output = output.replace(err, "")
-        return yaml.load(output)
+        return yaml.load(output, Loader=yaml.FullLoader)
 
     @property
     def cluster_name(self):
         """
         Get the cluster name for the specified target environment.
 
         If profile_name is in the compose-flow.yml Rancher cluster mapping,
@@ -460,15 +460,15 @@
         creation_command = f"rancher namespaces create {namespace}"
 
         print(f"Creating namespace {namespace} in project {self.project_name}")
         if not dry_run:
             try:
                 self.execute(creation_command)
             except sh.ErrorReturnCode_1 as exc:  # pylint: disable=E1101
-                message = exc.strip()
+                message = str(exc)
                 if "code=AlreadyExists" in message:
                     raise errors.RancherNamespaceAlreadyExists(
                         f"Namespace {namespace} already exists in another project!"
                     )
                 else:
                     raise
```

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/settings.py` & `compose-flow-4.0.0rc3/src/compose_flow/settings.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/shell.py` & `compose-flow-4.0.0rc3/src/compose_flow/shell.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow/utils.py` & `compose-flow-4.0.0rc3/src/compose_flow/utils.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/compose_flow.egg-info/PKG-INFO` & `compose-flow-4.0.0rc3/src/compose_flow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-flow
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: codified workflows for docker compose
 Home-page: https://github.com/openslate/compose-flow
 Author: DoubleVerify
 Author-email: code@doubleverify.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `compose-flow-4.0.0rc2/src/compose_flow.egg-info/SOURCES.txt` & `compose-flow-4.0.0rc3/src/compose_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/files/manifests/good-cronjob.yaml` & `compose-flow-4.0.0rc3/src/tests/files/manifests/good-cronjob.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/files/manifests/good-init-deployment.yaml` & `compose-flow-4.0.0rc3/src/tests/files/manifests/good-init-deployment.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/files/manifests/good-job.yaml` & `compose-flow-4.0.0rc3/src/tests/files/manifests/good-job.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/files/manifests/no-limits-deployment.yaml` & `compose-flow-4.0.0rc3/src/tests/files/manifests/no-limits-deployment.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_backends.py` & `compose-flow-4.0.0rc3/src/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_base.py` & `compose-flow-4.0.0rc3/src/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_deploy.py` & `compose-flow-4.0.0rc3/src/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_docker.py` & `compose-flow-4.0.0rc3/src/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_docker_image.py` & `compose-flow-4.0.0rc3/src/tests/test_docker_image.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_env.py` & `compose-flow-4.0.0rc3/src/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_kube_checks.py` & `compose-flow-4.0.0rc3/src/tests/test_kube_checks.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_kube_mixins.py` & `compose-flow-4.0.0rc3/src/tests/test_kube_mixins.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_passthrough.py` & `compose-flow-4.0.0rc3/src/tests/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_pod.py` & `compose-flow-4.0.0rc3/src/tests/test_pod.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_profile.py` & `compose-flow-4.0.0rc3/src/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_publish.py` & `compose-flow-4.0.0rc3/src/tests/test_publish.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_remote.py` & `compose-flow-4.0.0rc3/src/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_service.py` & `compose-flow-4.0.0rc3/src/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_task.py` & `compose-flow-4.0.0rc3/src/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_utils.py` & `compose-flow-4.0.0rc3/src/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `compose-flow-4.0.0rc2/src/tests/test_workflow.py` & `compose-flow-4.0.0rc3/src/tests/test_workflow.py`

 * *Files identical despite different names*

