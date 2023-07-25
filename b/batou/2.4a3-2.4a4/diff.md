# Comparing `tmp/batou-2.4a3.tar.gz` & `tmp/batou-2.4a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou-2.4a3.tar", last modified: Mon Jul 17 14:28:24 2023, max compression
+gzip compressed data, was "batou-2.4a4.tar", last modified: Tue Jul 25 08:08:09 2023, max compression
```

## Comparing `batou-2.4a3.tar` & `batou-2.4a4.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.793388 batou-2.4a3/
--rw-r--r--   0 elikoga    (501) staff       (20)    31241 2023-07-17 14:28:24.000000 batou-2.4a3/CHANGES.history.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     1608 2023-07-17 14:28:24.000000 batou-2.4a3/LICENSE.txt
--rw-r--r--   0 elikoga    (501) staff       (20)      212 2023-07-17 14:28:24.000000 batou-2.4a3/MANIFEST.in
--rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-07-17 14:28:24.793466 batou-2.4a3/PKG-INFO
--rw-r--r--   0 elikoga    (501) staff       (20)     2636 2023-07-17 14:28:24.000000 batou-2.4a3/README.md
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.713760 batou-2.4a3/doc/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.720112 batou-2.4a3/doc/source/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.770774 batou-2.4a3/doc/source/api/
--rw-r--r--   0 elikoga    (501) staff       (20)      886 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/api/component.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     1717 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/api/environment.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       48 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/api/templates.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       63 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/api/utilities.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.770966 batou-2.4a3/doc/source/cli/
--rw-r--r--   0 elikoga    (501) staff       (20)     4211 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/cli/index.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.771745 batou-2.4a3/doc/source/components/
--rw-r--r--   0 elikoga    (501) staff       (20)     1025 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/components/cmmi.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     2941 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/components/downloads-vcs.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     5657 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/components/files.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     4820 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/components/python.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     3050 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/components/services.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.772334 batou-2.4a3/doc/source/dev/
--rw-r--r--   0 elikoga    (501) staff       (20)      718 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/dev/authors.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     8555 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/dev/contributing.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     1711 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/dev/testing.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     2809 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/dev/todo.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     8500 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/index.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     4799 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/upgrading.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.773215 batou-2.4a3/doc/source/user/
--rw-r--r--   0 elikoga    (501) staff       (20)    10870 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/user/advanced.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     2565 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/user/install.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     3848 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/user/installation-deb.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     3798 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/user/installation-rpm.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     2907 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/user/intro.txt
--rw-r--r--   0 elikoga    (501) staff       (20)    47489 2023-07-17 14:28:24.000000 batou-2.4a3/doc/source/user/quickstart.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.715406 batou-2.4a3/examples/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.773558 batou-2.4a3/examples/api/
--rw-r--r--   0 elikoga    (501) staff       (20)      349 2023-07-17 14:28:24.000000 batou-2.4a3/examples/api/index.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/api/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.773705 batou-2.4a3/examples/django/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/django/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.774637 batou-2.4a3/examples/durations/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/durations/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.774794 batou-2.4a3/examples/errors/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/errors/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.774961 batou-2.4a3/examples/errors2/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/errors2/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.775118 batou-2.4a3/examples/ignores/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/ignores/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.775266 batou-2.4a3/examples/largetempl/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/largetempl/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.775414 batou-2.4a3/examples/package/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/package/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.775569 batou-2.4a3/examples/sync_async/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/sync_async/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.775720 batou-2.4a3/examples/tutorial-buildout/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/tutorial-buildout/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.775866 batou-2.4a3/examples/tutorial-component/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/tutorial-component/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.776008 batou-2.4a3/examples/tutorial-helloworld/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/tutorial-helloworld/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.776164 batou-2.4a3/examples/tutorial-parallelize/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/tutorial-parallelize/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.776326 batou-2.4a3/examples/tutorial-provision-container/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/tutorial-provision-container/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.776478 batou-2.4a3/examples/tutorial-secrets/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.715223 batou-2.4a3/examples/tutorial-secrets/environments/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.776635 batou-2.4a3/examples/tutorial-secrets/environments/age/
--rw-r--r--   0 elikoga    (501) staff       (20)     2431 2023-07-17 14:28:24.000000 batou-2.4a3/examples/tutorial-secrets/environments/age/age_keys.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/tutorial-secrets/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.776790 batou-2.4a3/examples/vagrant/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/vagrant/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.776938 batou-2.4a3/examples/vagrant-multi/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/vagrant-multi/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.777093 batou-2.4a3/examples/venvs/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.777248 batou-2.4a3/examples/venvs/environments/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/venvs/environments/requirements.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-17 14:28:24.000000 batou-2.4a3/examples/venvs/requirements.txt
--rw-r--r--   0 elikoga    (501) staff       (20)      129 2023-07-17 14:28:24.000000 batou-2.4a3/pyproject.toml
--rw-r--r--   0 elikoga    (501) staff       (20)      275 2023-07-17 14:28:24.000000 batou-2.4a3/requirements-dev.txt
--rw-r--r--   0 elikoga    (501) staff       (20)      139 2023-07-17 14:28:24.793700 batou-2.4a3/setup.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)     2187 2023-07-17 14:28:24.000000 batou-2.4a3/setup.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.715642 batou-2.4a3/src/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.780345 batou-2.4a3/src/batou/
--rw-r--r--   0 elikoga    (501) staff       (20)    21062 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)      997 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/_output.py
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/agent.py
--rw-r--r--   0 elikoga    (501) staff       (20)      163 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/c.py
--rw-r--r--   0 elikoga    (501) staff       (20)    40510 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/component.py
--rw-r--r--   0 elikoga    (501) staff       (20)      795 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/conftest.py
--rw-r--r--   0 elikoga    (501) staff       (20)    14630 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/deploy.py
--rw-r--r--   0 elikoga    (501) staff       (20)    20522 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/environment.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1507 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/fixtures.py
--rw-r--r--   0 elikoga    (501) staff       (20)    11006 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/host.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.781416 batou-2.4a3/src/batou/init-template/
--rw-r--r--   0 elikoga    (501) staff       (20)       44 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/init-template/.hgignore
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.715814 batou-2.4a3/src/batou/init-template/components/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.781521 batou-2.4a3/src/batou/init-template/components/example/
--rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/init-template/components/example/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.781628 batou-2.4a3/src/batou/init-template/environments/
--rw-r--r--   0 elikoga    (501) staff       (20)       66 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/init-template/environments/dev.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      411 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/insecure-private.key
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.783692 batou-2.4a3/src/batou/lib/
--rw-r--r--   0 elikoga    (501) staff       (20)       29 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3983 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/appenv.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6457 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/archive.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3297 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/buildout.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2211 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/cmmi.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2524 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/cron.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1224 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/debian.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2286 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/download.py
--rw-r--r--   0 elikoga    (501) staff       (20)    22046 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/file.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6368 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/git.py
--rw-r--r--   0 elikoga    (501) staff       (20)      854 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/goceptnet.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1388 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/logrotate.py
--rw-r--r--   0 elikoga    (501) staff       (20)     4541 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/mercurial.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3647 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/mysql.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2814 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/nagios.py
--rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/package.py
--rw-r--r--   0 elikoga    (501) staff       (20)     8150 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/python.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.784556 batou-2.4a3/src/batou/lib/resources/
--rw-r--r--   0 elikoga    (501) staff       (20)     2120 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/resources/check_supervisor.py.in
--rw-r--r--   0 elikoga    (501) staff       (20)      244 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/resources/crontab
--rw-r--r--   0 elikoga    (501) staff       (20)      548 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/resources/init.sh
--rw-r--r--   0 elikoga    (501) staff       (20)      299 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/resources/logrotate.in
--rw-r--r--   0 elikoga    (501) staff       (20)      840 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/resources/nagios.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      153 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/resources/nrpe.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      380 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/resources/supervisor.buildout.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      609 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/resources/supervisor.conf
--rw-r--r--   0 elikoga    (501) staff       (20)      932 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/service.py
--rw-r--r--   0 elikoga    (501) staff       (20)    10273 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/supervisor.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1172 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/svn.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.786317 batou-2.4a3/src/batou/lib/tests/
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3083 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_appenv.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3858 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_archive.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1689 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_buildout.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3261 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_cmmi.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2110 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_cron.py
--rw-r--r--   0 elikoga    (501) staff       (20)      639 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_debian.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2158 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_download.py
--rw-r--r--   0 elikoga    (501) staff       (20)    31505 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_file.py
--rw-r--r--   0 elikoga    (501) staff       (20)    10383 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_git.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6165 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_mercurial.py
--rw-r--r--   0 elikoga    (501) staff       (20)      121 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_mysql.py
--rw-r--r--   0 elikoga    (501) staff       (20)      847 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_nagios.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1165 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_python.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1693 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_service.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3106 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_supervisor.py
--rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/lib/tests/test_svn.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6247 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/main.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.786434 batou-2.4a3/src/batou/migrate/
--rw-r--r--   0 elikoga    (501) staff       (20)     3377 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/migrate/__init__.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.787057 batou-2.4a3/src/batou/migrate/migrations/
--rw-r--r--   0 elikoga    (501) staff       (20)      389 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/migrate/migrations/2300.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1775 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/migrate/migrations/2301.py
--rw-r--r--   0 elikoga    (501) staff       (20)      874 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/migrate/migrations/2302.py
--rw-r--r--   0 elikoga    (501) staff       (20)      790 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/migrate/migrations/2303.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1282 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/migrate/migrations/2400.py
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/migrate/migrations/__init__.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.787234 batou-2.4a3/src/batou/migrate/tests/
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/migrate/tests/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     4532 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/migrate/tests/test_migrate.py
--rw-r--r--   0 elikoga    (501) staff       (20)    12756 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/provision.py
--rw-r--r--   0 elikoga    (501) staff       (20)    11713 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/remote_core.py
--rw-r--r--   0 elikoga    (501) staff       (20)    11793 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/repository.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6424 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/resources.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.787666 batou-2.4a3/src/batou/secrets/
--rw-r--r--   0 elikoga    (501) staff       (20)    22033 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/secrets/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3935 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/secrets/edit.py
--rw-r--r--   0 elikoga    (501) staff       (20)    12969 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/secrets/encryption.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2695 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/secrets/manage.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.788090 batou-2.4a3/src/batou/secrets/tests/
--rw-r--r--   0 elikoga    (501) staff       (20)       23 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/secrets/tests/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/secrets/tests/test_editor.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1566 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/secrets/tests/test_manage.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2736 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/secrets/tests/test_secrets.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2429 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/template.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.790151 batou-2.4a3/src/batou/tests/
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)      666 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/conftest.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3012 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/ellipsis.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.718845 batou-2.4a3/src/batou/tests/fixture/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.790276 batou-2.4a3/src/batou/tests/fixture/basic_service/
--rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/basic_service/.batou.json
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.716843 batou-2.4a3/src/batou/tests/fixture/basic_service/components/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.790405 batou-2.4a3/src/batou/tests/fixture/basic_service/components/zeo/
--rw-r--r--   0 elikoga    (501) staff       (20)      178 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/basic_service/components/zeo/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.790530 batou-2.4a3/src/batou/tests/fixture/basic_service/components/zope/
--rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/basic_service/components/zope/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.717086 batou-2.4a3/src/batou/tests/fixture/basic_service/environments/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.790654 batou-2.4a3/src/batou/tests/fixture/basic_service/environments/dev/
--rw-r--r--   0 elikoga    (501) staff       (20)       79 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.790783 batou-2.4a3/src/batou/tests/fixture/basic_service/environments/production/
--rw-r--r--   0 elikoga    (501) staff       (20)      128 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.790909 batou-2.4a3/src/batou/tests/fixture/component/
--rw-r--r--   0 elikoga    (501) staff       (20)       40 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/component/haproxy.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.791029 batou-2.4a3/src/batou/tests/fixture/sample_service/
--rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/.batou.json
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.717390 batou-2.4a3/src/batou/tests/fixture/sample_service/components/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.791147 batou-2.4a3/src/batou/tests/fixture/sample_service/components/hello/
--rw-r--r--   0 elikoga    (501) staff       (20)      973 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/components/hello/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.718291 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.791281 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
--rw-r--r--   0 elikoga    (501) staff       (20)      144 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.791417 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
--rw-r--r--   0 elikoga    (501) staff       (20)       88 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.791546 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
--rw-r--r--   0 elikoga    (501) staff       (20)      110 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.791678 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-resolver/
--rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.791805 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
--rw-r--r--   0 elikoga    (501) staff       (20)       90 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.791934 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
--rw-r--r--   0 elikoga    (501) staff       (20)      191 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.792070 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
--rw-r--r--   0 elikoga    (501) staff       (20)       94 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.792204 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
--rw-r--r--   0 elikoga    (501) staff       (20)       85 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.792331 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
--rw-r--r--   0 elikoga    (501) staff       (20)       64 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.792462 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
--rw-r--r--   0 elikoga    (501) staff       (20)       26 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.792591 batou-2.4a3/src/batou/tests/fixture/service_early_resource/
--rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/service_early_resource/.batou.json
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.718617 batou-2.4a3/src/batou/tests/fixture/service_early_resource/components/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.792723 batou-2.4a3/src/batou/tests/fixture/service_early_resource/components/zeo/
--rw-r--r--   0 elikoga    (501) staff       (20)      346 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.792862 batou-2.4a3/src/batou/tests/fixture/service_early_resource/components/zope/
--rw-r--r--   0 elikoga    (501) staff       (20)      116 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/service_early_resource/components/zope/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.718761 batou-2.4a3/src/batou/tests/fixture/service_early_resource/environments/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.792998 batou-2.4a3/src/batou/tests/fixture/service_early_resource/environments/dev/
--rw-r--r--   0 elikoga    (501) staff       (20)       62 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.793258 batou-2.4a3/src/batou/tests/fixture/template/
--rw-r--r--   0 elikoga    (501) staff       (20)       84 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/template/haproxy.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      119 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/fixture/template/haproxy.cfg.jinja2
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_bootstrap.py
--rw-r--r--   0 elikoga    (501) staff       (20)    18479 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_component.py
--rw-r--r--   0 elikoga    (501) staff       (20)     4776 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_config.py
--rw-r--r--   0 elikoga    (501) staff       (20)     5707 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_dependencies.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1725 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_deploy.py
--rw-r--r--   0 elikoga    (501) staff       (20)    10550 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_endtoend.py
--rw-r--r--   0 elikoga    (501) staff       (20)     8674 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_environment.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2305 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_exceptions.py
--rw-r--r--   0 elikoga    (501) staff       (20)      606 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_host.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1488 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_main.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1326 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_remote.py
--rw-r--r--   0 elikoga    (501) staff       (20)     9398 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_remote_core.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3648 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_repository.py
--rw-r--r--   0 elikoga    (501) staff       (20)      743 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_resources.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2602 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_template.py
--rw-r--r--   0 elikoga    (501) staff       (20)    14060 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_utils.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1169 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/tests/test_vfs.py
--rw-r--r--   0 elikoga    (501) staff       (20)    18387 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/utils.py
--rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/version.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     1009 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou/vfs.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-17 14:28:24.781312 batou-2.4a3/src/batou.egg-info/
--rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou.egg-info/PKG-INFO
--rw-r--r--   0 elikoga    (501) staff       (20)     6796 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou.egg-info/SOURCES.txt
--rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou.egg-info/dependency_links.txt
--rw-r--r--   0 elikoga    (501) staff       (20)      241 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou.egg-info/entry_points.txt
--rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou.egg-info/not-zip-safe
--rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou.egg-info/requires.txt
--rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-07-17 14:28:24.000000 batou-2.4a3/src/batou.egg-info/top_level.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.291863 batou-2.4a4/
+-rw-r--r--   0 elikoga    (501) staff       (20)    31241 2023-07-25 08:08:08.000000 batou-2.4a4/CHANGES.history.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1608 2023-07-25 08:08:08.000000 batou-2.4a4/LICENSE.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      212 2023-07-25 08:08:08.000000 batou-2.4a4/MANIFEST.in
+-rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-07-25 08:08:09.291928 batou-2.4a4/PKG-INFO
+-rw-r--r--   0 elikoga    (501) staff       (20)     2636 2023-07-25 08:08:08.000000 batou-2.4a4/README.md
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.222356 batou-2.4a4/doc/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.266852 batou-2.4a4/doc/source/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.267434 batou-2.4a4/doc/source/api/
+-rw-r--r--   0 elikoga    (501) staff       (20)      886 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/api/component.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1717 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/api/environment.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       48 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/api/templates.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       63 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/api/utilities.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.267580 batou-2.4a4/doc/source/cli/
+-rw-r--r--   0 elikoga    (501) staff       (20)     4211 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/cli/index.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.268321 batou-2.4a4/doc/source/components/
+-rw-r--r--   0 elikoga    (501) staff       (20)     1025 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/components/cmmi.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2941 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/components/downloads-vcs.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     5657 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/components/files.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     4820 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/components/python.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     3050 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/components/services.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.268917 batou-2.4a4/doc/source/dev/
+-rw-r--r--   0 elikoga    (501) staff       (20)      718 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/dev/authors.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     8555 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/dev/contributing.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1711 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/dev/testing.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2809 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/dev/todo.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     8500 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/index.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     4799 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/upgrading.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.269821 batou-2.4a4/doc/source/user/
+-rw-r--r--   0 elikoga    (501) staff       (20)    10870 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/user/advanced.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2565 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/user/install.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     3848 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/user/installation-deb.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     3798 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/user/installation-rpm.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2907 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/user/intro.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)    47489 2023-07-25 08:08:08.000000 batou-2.4a4/doc/source/user/quickstart.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.223971 batou-2.4a4/examples/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.270148 batou-2.4a4/examples/api/
+-rw-r--r--   0 elikoga    (501) staff       (20)      349 2023-07-25 08:08:08.000000 batou-2.4a4/examples/api/index.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/api/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.270295 batou-2.4a4/examples/django/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/django/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.270435 batou-2.4a4/examples/durations/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/durations/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.270570 batou-2.4a4/examples/errors/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/errors/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.270699 batou-2.4a4/examples/errors2/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/errors2/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.270830 batou-2.4a4/examples/ignores/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/ignores/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.270963 batou-2.4a4/examples/largetempl/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/largetempl/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.271105 batou-2.4a4/examples/package/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/package/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.271245 batou-2.4a4/examples/sync_async/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/sync_async/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.271375 batou-2.4a4/examples/tutorial-buildout/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/tutorial-buildout/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.271504 batou-2.4a4/examples/tutorial-component/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/tutorial-component/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.271640 batou-2.4a4/examples/tutorial-helloworld/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/tutorial-helloworld/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.271776 batou-2.4a4/examples/tutorial-parallelize/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/tutorial-parallelize/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.271907 batou-2.4a4/examples/tutorial-provision-container/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/tutorial-provision-container/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.272038 batou-2.4a4/examples/tutorial-secrets/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.223783 batou-2.4a4/examples/tutorial-secrets/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.272177 batou-2.4a4/examples/tutorial-secrets/environments/age/
+-rw-r--r--   0 elikoga    (501) staff       (20)     2431 2023-07-25 08:08:08.000000 batou-2.4a4/examples/tutorial-secrets/environments/age/age_keys.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/tutorial-secrets/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.272317 batou-2.4a4/examples/vagrant/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/vagrant/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.272449 batou-2.4a4/examples/vagrant-multi/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/vagrant-multi/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.272579 batou-2.4a4/examples/venvs/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.272720 batou-2.4a4/examples/venvs/environments/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/venvs/environments/requirements.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-25 08:08:08.000000 batou-2.4a4/examples/venvs/requirements.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      129 2023-07-25 08:08:08.000000 batou-2.4a4/pyproject.toml
+-rw-r--r--   0 elikoga    (501) staff       (20)      277 2023-07-25 08:08:08.000000 batou-2.4a4/requirements-dev.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      139 2023-07-25 08:08:09.292175 batou-2.4a4/setup.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)     2187 2023-07-25 08:08:08.000000 batou-2.4a4/setup.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.224209 batou-2.4a4/src/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.275456 batou-2.4a4/src/batou/
+-rw-r--r--   0 elikoga    (501) staff       (20)    21062 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      997 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/_output.py
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/agent.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      163 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/c.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    40510 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/component.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      795 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/conftest.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    14630 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/deploy.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    20522 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/environment.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1507 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/fixtures.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    11006 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/host.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.276557 batou-2.4a4/src/batou/init-template/
+-rw-r--r--   0 elikoga    (501) staff       (20)       44 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/init-template/.hgignore
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.224386 batou-2.4a4/src/batou/init-template/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.276717 batou-2.4a4/src/batou/init-template/components/example/
+-rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/init-template/components/example/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.276869 batou-2.4a4/src/batou/init-template/environments/
+-rw-r--r--   0 elikoga    (501) staff       (20)       66 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/init-template/environments/dev.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      411 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/insecure-private.key
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.279736 batou-2.4a4/src/batou/lib/
+-rw-r--r--   0 elikoga    (501) staff       (20)       29 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3983 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/appenv.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6457 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/archive.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3297 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/buildout.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2211 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/cmmi.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2524 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/cron.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1224 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/debian.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2286 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/download.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    22046 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/file.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6368 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/git.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      854 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/goceptnet.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1388 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/logrotate.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     4541 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/mercurial.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3647 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/mysql.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2814 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/nagios.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/package.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     8150 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/python.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.280887 batou-2.4a4/src/batou/lib/resources/
+-rw-r--r--   0 elikoga    (501) staff       (20)     2120 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/resources/check_supervisor.py.in
+-rw-r--r--   0 elikoga    (501) staff       (20)      244 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/resources/crontab
+-rw-r--r--   0 elikoga    (501) staff       (20)      548 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/resources/init.sh
+-rw-r--r--   0 elikoga    (501) staff       (20)      299 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/resources/logrotate.in
+-rw-r--r--   0 elikoga    (501) staff       (20)      840 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/resources/nagios.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      153 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/resources/nrpe.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      380 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/resources/supervisor.buildout.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      609 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/resources/supervisor.conf
+-rw-r--r--   0 elikoga    (501) staff       (20)      932 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/service.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    10273 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/supervisor.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1172 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/svn.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.283328 batou-2.4a4/src/batou/lib/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3083 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_appenv.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3858 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_archive.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1689 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_buildout.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3261 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_cmmi.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2110 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_cron.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      639 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_debian.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2158 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_download.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    31505 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_file.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    10383 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_git.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6165 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_mercurial.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      121 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_mysql.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      847 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_nagios.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1165 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_python.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1693 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_service.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3106 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_supervisor.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/lib/tests/test_svn.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6247 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/main.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.283477 batou-2.4a4/src/batou/migrate/
+-rw-r--r--   0 elikoga    (501) staff       (20)     3377 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/migrate/__init__.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.284295 batou-2.4a4/src/batou/migrate/migrations/
+-rw-r--r--   0 elikoga    (501) staff       (20)      389 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/migrate/migrations/2300.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1775 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/migrate/migrations/2301.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      874 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/migrate/migrations/2302.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      790 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/migrate/migrations/2303.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1282 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/migrate/migrations/2400.py
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/migrate/migrations/__init__.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.284537 batou-2.4a4/src/batou/migrate/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/migrate/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     4532 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/migrate/tests/test_migrate.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    12756 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/provision.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    11713 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/remote_core.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    11793 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/repository.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6424 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/resources.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.285118 batou-2.4a4/src/batou/secrets/
+-rw-r--r--   0 elikoga    (501) staff       (20)    22033 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/secrets/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3935 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/secrets/edit.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    13507 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/secrets/encryption.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2695 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/secrets/manage.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.285694 batou-2.4a4/src/batou/secrets/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)       23 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/secrets/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/secrets/tests/test_editor.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1566 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/secrets/tests/test_manage.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2736 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/secrets/tests/test_secrets.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2429 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/template.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.288388 batou-2.4a4/src/batou/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      666 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/conftest.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3012 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/ellipsis.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.264972 batou-2.4a4/src/batou/tests/fixture/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.288523 batou-2.4a4/src/batou/tests/fixture/basic_service/
+-rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/basic_service/.batou.json
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.225306 batou-2.4a4/src/batou/tests/fixture/basic_service/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.288663 batou-2.4a4/src/batou/tests/fixture/basic_service/components/zeo/
+-rw-r--r--   0 elikoga    (501) staff       (20)      178 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/basic_service/components/zeo/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.288802 batou-2.4a4/src/batou/tests/fixture/basic_service/components/zope/
+-rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/basic_service/components/zope/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.225488 batou-2.4a4/src/batou/tests/fixture/basic_service/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.288938 batou-2.4a4/src/batou/tests/fixture/basic_service/environments/dev/
+-rw-r--r--   0 elikoga    (501) staff       (20)       79 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.289083 batou-2.4a4/src/batou/tests/fixture/basic_service/environments/production/
+-rw-r--r--   0 elikoga    (501) staff       (20)      128 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.289229 batou-2.4a4/src/batou/tests/fixture/component/
+-rw-r--r--   0 elikoga    (501) staff       (20)       40 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/component/haproxy.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.289369 batou-2.4a4/src/batou/tests/fixture/sample_service/
+-rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/.batou.json
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.225722 batou-2.4a4/src/batou/tests/fixture/sample_service/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.289502 batou-2.4a4/src/batou/tests/fixture/sample_service/components/hello/
+-rw-r--r--   0 elikoga    (501) staff       (20)      973 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/components/hello/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.264339 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.289645 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
+-rw-r--r--   0 elikoga    (501) staff       (20)      144 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.289788 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
+-rw-r--r--   0 elikoga    (501) staff       (20)       88 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.289935 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
+-rw-r--r--   0 elikoga    (501) staff       (20)      110 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.290072 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-resolver/
+-rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.290211 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
+-rw-r--r--   0 elikoga    (501) staff       (20)       90 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.290355 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
+-rw-r--r--   0 elikoga    (501) staff       (20)      191 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.290495 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
+-rw-r--r--   0 elikoga    (501) staff       (20)       94 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.290631 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
+-rw-r--r--   0 elikoga    (501) staff       (20)       85 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.290770 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
+-rw-r--r--   0 elikoga    (501) staff       (20)       64 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.290908 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
+-rw-r--r--   0 elikoga    (501) staff       (20)       26 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.291045 batou-2.4a4/src/batou/tests/fixture/service_early_resource/
+-rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/service_early_resource/.batou.json
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.264703 batou-2.4a4/src/batou/tests/fixture/service_early_resource/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.291182 batou-2.4a4/src/batou/tests/fixture/service_early_resource/components/zeo/
+-rw-r--r--   0 elikoga    (501) staff       (20)      346 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.291316 batou-2.4a4/src/batou/tests/fixture/service_early_resource/components/zope/
+-rw-r--r--   0 elikoga    (501) staff       (20)      116 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/service_early_resource/components/zope/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.264881 batou-2.4a4/src/batou/tests/fixture/service_early_resource/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.291453 batou-2.4a4/src/batou/tests/fixture/service_early_resource/environments/dev/
+-rw-r--r--   0 elikoga    (501) staff       (20)       62 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.291731 batou-2.4a4/src/batou/tests/fixture/template/
+-rw-r--r--   0 elikoga    (501) staff       (20)       84 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/template/haproxy.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      119 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/fixture/template/haproxy.cfg.jinja2
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_bootstrap.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    18479 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_component.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     4776 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_config.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     5707 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_dependencies.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1725 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_deploy.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    10550 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_endtoend.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     8674 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_environment.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2305 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_exceptions.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      606 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_host.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1488 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_main.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1326 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_remote.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     9398 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_remote_core.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3648 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_repository.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      743 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_resources.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2602 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_template.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    14060 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_utils.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1169 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/tests/test_vfs.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    18387 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/utils.py
+-rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/version.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1009 2023-07-25 08:08:08.000000 batou-2.4a4/src/batou/vfs.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-25 08:08:09.276410 batou-2.4a4/src/batou.egg-info/
+-rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-07-25 08:08:09.000000 batou-2.4a4/src/batou.egg-info/PKG-INFO
+-rw-r--r--   0 elikoga    (501) staff       (20)     6796 2023-07-25 08:08:09.000000 batou-2.4a4/src/batou.egg-info/SOURCES.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-07-25 08:08:09.000000 batou-2.4a4/src/batou.egg-info/dependency_links.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      241 2023-07-25 08:08:09.000000 batou-2.4a4/src/batou.egg-info/entry_points.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-07-25 08:08:09.000000 batou-2.4a4/src/batou.egg-info/not-zip-safe
+-rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-07-25 08:08:09.000000 batou-2.4a4/src/batou.egg-info/requires.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-07-25 08:08:09.000000 batou-2.4a4/src/batou.egg-info/top_level.txt
```

### Comparing `batou-2.4a3/CHANGES.history.txt` & `batou-2.4a4/CHANGES.history.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/LICENSE.txt` & `batou-2.4a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/PKG-INFO` & `batou-2.4a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.4a3
+Version: 2.4a4
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Platform: UNKNOWN
```

### Comparing `batou-2.4a3/README.md` & `batou-2.4a4/README.md`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/api/component.txt` & `batou-2.4a4/doc/source/api/component.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/api/environment.txt` & `batou-2.4a4/doc/source/api/environment.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/cli/index.txt` & `batou-2.4a4/doc/source/cli/index.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/components/cmmi.txt` & `batou-2.4a4/doc/source/components/cmmi.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/components/downloads-vcs.txt` & `batou-2.4a4/doc/source/components/downloads-vcs.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/components/files.txt` & `batou-2.4a4/doc/source/components/files.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/components/python.txt` & `batou-2.4a4/doc/source/components/python.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/components/services.txt` & `batou-2.4a4/doc/source/components/services.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/dev/authors.txt` & `batou-2.4a4/doc/source/dev/authors.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/dev/contributing.txt` & `batou-2.4a4/doc/source/dev/contributing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/dev/testing.txt` & `batou-2.4a4/doc/source/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/dev/todo.txt` & `batou-2.4a4/doc/source/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/index.txt` & `batou-2.4a4/doc/source/index.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/upgrading.txt` & `batou-2.4a4/doc/source/upgrading.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/user/advanced.txt` & `batou-2.4a4/doc/source/user/advanced.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/user/install.txt` & `batou-2.4a4/doc/source/user/install.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/user/installation-deb.txt` & `batou-2.4a4/doc/source/user/installation-deb.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/user/installation-rpm.txt` & `batou-2.4a4/doc/source/user/installation-rpm.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/user/intro.txt` & `batou-2.4a4/doc/source/user/intro.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/doc/source/user/quickstart.txt` & `batou-2.4a4/doc/source/user/quickstart.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/examples/tutorial-secrets/environments/age/age_keys.txt` & `batou-2.4a4/examples/tutorial-secrets/environments/age/age_keys.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/setup.py` & `batou-2.4a4/setup.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/__init__.py` & `batou-2.4a4/src/batou/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/_output.py` & `batou-2.4a4/src/batou/_output.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/component.py` & `batou-2.4a4/src/batou/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/conftest.py` & `batou-2.4a4/src/batou/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/deploy.py` & `batou-2.4a4/src/batou/deploy.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/environment.py` & `batou-2.4a4/src/batou/environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/fixtures.py` & `batou-2.4a4/src/batou/fixtures.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/host.py` & `batou-2.4a4/src/batou/host.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/appenv.py` & `batou-2.4a4/src/batou/lib/appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/archive.py` & `batou-2.4a4/src/batou/lib/archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/buildout.py` & `batou-2.4a4/src/batou/lib/buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/cmmi.py` & `batou-2.4a4/src/batou/lib/cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/cron.py` & `batou-2.4a4/src/batou/lib/cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/debian.py` & `batou-2.4a4/src/batou/lib/debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/download.py` & `batou-2.4a4/src/batou/lib/download.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/file.py` & `batou-2.4a4/src/batou/lib/file.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/git.py` & `batou-2.4a4/src/batou/lib/git.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/goceptnet.py` & `batou-2.4a4/src/batou/lib/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/logrotate.py` & `batou-2.4a4/src/batou/lib/logrotate.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/mercurial.py` & `batou-2.4a4/src/batou/lib/mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/mysql.py` & `batou-2.4a4/src/batou/lib/mysql.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/nagios.py` & `batou-2.4a4/src/batou/lib/nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/package.py` & `batou-2.4a4/src/batou/lib/package.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/python.py` & `batou-2.4a4/src/batou/lib/python.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/resources/check_supervisor.py.in` & `batou-2.4a4/src/batou/lib/resources/check_supervisor.py.in`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/resources/init.sh` & `batou-2.4a4/src/batou/lib/resources/init.sh`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/resources/nagios.cfg` & `batou-2.4a4/src/batou/lib/resources/nagios.cfg`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/resources/supervisor.conf` & `batou-2.4a4/src/batou/lib/resources/supervisor.conf`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/service.py` & `batou-2.4a4/src/batou/lib/service.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/supervisor.py` & `batou-2.4a4/src/batou/lib/supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/svn.py` & `batou-2.4a4/src/batou/lib/svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_appenv.py` & `batou-2.4a4/src/batou/lib/tests/test_appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_archive.py` & `batou-2.4a4/src/batou/lib/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_buildout.py` & `batou-2.4a4/src/batou/lib/tests/test_buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_cmmi.py` & `batou-2.4a4/src/batou/lib/tests/test_cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_cron.py` & `batou-2.4a4/src/batou/lib/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_debian.py` & `batou-2.4a4/src/batou/lib/tests/test_debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_download.py` & `batou-2.4a4/src/batou/lib/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_file.py` & `batou-2.4a4/src/batou/lib/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_git.py` & `batou-2.4a4/src/batou/lib/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_mercurial.py` & `batou-2.4a4/src/batou/lib/tests/test_mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_nagios.py` & `batou-2.4a4/src/batou/lib/tests/test_nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_python.py` & `batou-2.4a4/src/batou/lib/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_service.py` & `batou-2.4a4/src/batou/lib/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_supervisor.py` & `batou-2.4a4/src/batou/lib/tests/test_supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/lib/tests/test_svn.py` & `batou-2.4a4/src/batou/lib/tests/test_svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/main.py` & `batou-2.4a4/src/batou/main.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/migrate/__init__.py` & `batou-2.4a4/src/batou/migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/migrate/migrations/2301.py` & `batou-2.4a4/src/batou/migrate/migrations/2301.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/migrate/migrations/2302.py` & `batou-2.4a4/src/batou/migrate/migrations/2302.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/migrate/migrations/2303.py` & `batou-2.4a4/src/batou/migrate/migrations/2303.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/migrate/migrations/2400.py` & `batou-2.4a4/src/batou/migrate/migrations/2400.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/migrate/tests/test_migrate.py` & `batou-2.4a4/src/batou/migrate/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/provision.py` & `batou-2.4a4/src/batou/provision.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/remote_core.py` & `batou-2.4a4/src/batou/remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/repository.py` & `batou-2.4a4/src/batou/repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/resources.py` & `batou-2.4a4/src/batou/resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/secrets/__init__.py` & `batou-2.4a4/src/batou/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/secrets/edit.py` & `batou-2.4a4/src/batou/secrets/edit.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/secrets/encryption.py` & `batou-2.4a4/src/batou/secrets/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,15 +334,24 @@
                                 )
                             )
                         )
                         continue
                     # also assert, that output is empty from now on
                     buffer = b""
                     while True:
-                        chunk = os.read(fd, 1024)
+                        try:
+                            chunk = os.read(fd, 1024)
+                        except OSError as err:  # noqa
+                            if err.errno == errno.EIO:
+                                # work arond suspected pty "feature", where
+                                # reading from the file descriptor
+                                # when there is no data raises instead of
+                                # returning an empty string, see
+                                # https://bugs.python.org/issue5380
+                                chunk = None
                         if not chunk:
                             break
                         buffer += chunk
                     if buffer:
                         magic_bytes = b"\x1b[F\x1b[K"
                         if buffer.startswith(magic_bytes):
                             buffer = buffer[len(magic_bytes) :]
```

### Comparing `batou-2.4a3/src/batou/secrets/manage.py` & `batou-2.4a4/src/batou/secrets/manage.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/secrets/tests/test_editor.py` & `batou-2.4a4/src/batou/secrets/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/secrets/tests/test_manage.py` & `batou-2.4a4/src/batou/secrets/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/secrets/tests/test_secrets.py` & `batou-2.4a4/src/batou/secrets/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/template.py` & `batou-2.4a4/src/batou/template.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/conftest.py` & `batou-2.4a4/src/batou/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/ellipsis.py` & `batou-2.4a4/src/batou/tests/ellipsis.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/fixture/sample_service/components/hello/component.py` & `batou-2.4a4/src/batou/tests/fixture/sample_service/components/hello/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_component.py` & `batou-2.4a4/src/batou/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_config.py` & `batou-2.4a4/src/batou/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_dependencies.py` & `batou-2.4a4/src/batou/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_deploy.py` & `batou-2.4a4/src/batou/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_endtoend.py` & `batou-2.4a4/src/batou/tests/test_endtoend.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_environment.py` & `batou-2.4a4/src/batou/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_exceptions.py` & `batou-2.4a4/src/batou/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_host.py` & `batou-2.4a4/src/batou/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_main.py` & `batou-2.4a4/src/batou/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_remote.py` & `batou-2.4a4/src/batou/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_remote_core.py` & `batou-2.4a4/src/batou/tests/test_remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_repository.py` & `batou-2.4a4/src/batou/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_resources.py` & `batou-2.4a4/src/batou/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_template.py` & `batou-2.4a4/src/batou/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_utils.py` & `batou-2.4a4/src/batou/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/tests/test_vfs.py` & `batou-2.4a4/src/batou/tests/test_vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/utils.py` & `batou-2.4a4/src/batou/utils.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou/vfs.py` & `batou-2.4a4/src/batou/vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a3/src/batou.egg-info/PKG-INFO` & `batou-2.4a4/src/batou.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.4a3
+Version: 2.4a4
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Platform: UNKNOWN
```

### Comparing `batou-2.4a3/src/batou.egg-info/SOURCES.txt` & `batou-2.4a4/src/batou.egg-info/SOURCES.txt`

 * *Files identical despite different names*

