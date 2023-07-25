# Comparing `tmp/python-pfconclient-3.0.0.tar.gz` & `tmp/python-pfconclient-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pfconclient-3.0.0.tar", last modified: Sat Jan 22 00:26:53 2022, max compression
+gzip compressed data, was "python-pfconclient-3.1.0.tar", last modified: Tue Jul 25 16:30:13 2023, max compression
```

## Comparing `python-pfconclient-3.0.0.tar` & `python-pfconclient-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2022-01-22 00:26:53.900071 python-pfconclient-3.0.0/
--rw-r--r--   0 jbernal    (501) staff       (20)     9143 2022-01-22 00:26:53.899817 python-pfconclient-3.0.0/PKG-INFO
--rw-r--r--   0 jbernal    (501) staff       (20)     7037 2022-01-22 00:21:35.000000 python-pfconclient-3.0.0/README.rst
-drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2022-01-22 00:26:53.897667 python-pfconclient-3.0.0/bin/
--rwxr-xr-x   0 jbernal    (501) staff       (20)     8829 2022-01-21 03:54:18.000000 python-pfconclient-3.0.0/bin/pfconclient
-drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2022-01-22 00:26:53.898223 python-pfconclient-3.0.0/pfconclient/
--rwxr-xr-x   0 jbernal    (501) staff       (20)        0 2020-05-04 16:56:02.000000 python-pfconclient-3.0.0/pfconclient/__init__.py
--rwxr-xr-x   0 jbernal    (501) staff       (20)     9061 2022-01-21 03:54:18.000000 python-pfconclient-3.0.0/pfconclient/client.py
--rwxr-xr-x   0 jbernal    (501) staff       (20)      247 2022-01-21 01:15:14.000000 python-pfconclient-3.0.0/pfconclient/exceptions.py
-drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2022-01-22 00:26:53.899428 python-pfconclient-3.0.0/python_pfconclient.egg-info/
--rw-r--r--   0 jbernal    (501) staff       (20)     9143 2022-01-22 00:26:53.000000 python-pfconclient-3.0.0/python_pfconclient.egg-info/PKG-INFO
--rw-r--r--   0 jbernal    (501) staff       (20)      357 2022-01-22 00:26:53.000000 python-pfconclient-3.0.0/python_pfconclient.egg-info/SOURCES.txt
--rw-r--r--   0 jbernal    (501) staff       (20)        1 2022-01-22 00:26:53.000000 python-pfconclient-3.0.0/python_pfconclient.egg-info/dependency_links.txt
--rw-r--r--   0 jbernal    (501) staff       (20)        1 2021-01-08 19:12:41.000000 python-pfconclient-3.0.0/python_pfconclient.egg-info/not-zip-safe
--rw-r--r--   0 jbernal    (501) staff       (20)       17 2022-01-22 00:26:53.000000 python-pfconclient-3.0.0/python_pfconclient.egg-info/requires.txt
--rw-r--r--   0 jbernal    (501) staff       (20)       12 2022-01-22 00:26:53.000000 python-pfconclient-3.0.0/python_pfconclient.egg-info/top_level.txt
--rw-r--r--   0 jbernal    (501) staff       (20)       38 2022-01-22 00:26:53.900151 python-pfconclient-3.0.0/setup.cfg
--rw-r--r--   0 jbernal    (501) staff       (20)      829 2022-01-22 00:11:10.000000 python-pfconclient-3.0.0/setup.py
+drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-25 16:30:13.877142 python-pfconclient-3.1.0/
+-rw-r--r--   0 jbernal    (501) staff       (20)     9002 2023-07-25 16:30:13.876743 python-pfconclient-3.1.0/PKG-INFO
+-rw-r--r--   0 jbernal    (501) staff       (20)     6928 2023-07-21 22:52:15.000000 python-pfconclient-3.1.0/README.rst
+drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-25 16:30:13.873203 python-pfconclient-3.1.0/bin/
+-rwxr-xr-x   0 jbernal    (501) staff       (20)     8796 2023-07-21 22:52:15.000000 python-pfconclient-3.1.0/bin/pfconclient
+drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-25 16:30:13.873926 python-pfconclient-3.1.0/pfconclient/
+-rwxr-xr-x   0 jbernal    (501) staff       (20)        0 2020-05-04 16:56:02.000000 python-pfconclient-3.1.0/pfconclient/__init__.py
+-rwxr-xr-x   0 jbernal    (501) staff       (20)    10138 2023-07-25 03:51:12.000000 python-pfconclient-3.1.0/pfconclient/client.py
+-rwxr-xr-x   0 jbernal    (501) staff       (20)      247 2022-01-21 01:15:14.000000 python-pfconclient-3.1.0/pfconclient/exceptions.py
+drwxr-xr-x   0 jbernal    (501) staff       (20)        0 2023-07-25 16:30:13.876080 python-pfconclient-3.1.0/python_pfconclient.egg-info/
+-rw-r--r--   0 jbernal    (501) staff       (20)     9002 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/PKG-INFO
+-rw-r--r--   0 jbernal    (501) staff       (20)      357 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/SOURCES.txt
+-rw-r--r--   0 jbernal    (501) staff       (20)        1 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/dependency_links.txt
+-rw-r--r--   0 jbernal    (501) staff       (20)        1 2021-01-08 19:12:41.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/not-zip-safe
+-rw-r--r--   0 jbernal    (501) staff       (20)       17 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/requires.txt
+-rw-r--r--   0 jbernal    (501) staff       (20)       12 2023-07-25 16:30:13.000000 python-pfconclient-3.1.0/python_pfconclient.egg-info/top_level.txt
+-rw-r--r--   0 jbernal    (501) staff       (20)       38 2023-07-25 16:30:13.877248 python-pfconclient-3.1.0/setup.cfg
+-rw-r--r--   0 jbernal    (501) staff       (20)      829 2023-07-25 16:27:24.000000 python-pfconclient-3.1.0/setup.py
```

### Comparing `python-pfconclient-3.0.0/PKG-INFO` & `python-pfconclient-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-pfconclient
-Version: 3.0.0
+Version: 3.1.0
 Summary: (Python) client for the Pfcon API
 Home-page: https://github.com/FNNDSC/python-pfconclient
 Author: FNNDSC
 Author-email: dev@babymri.org
 License: MIT
 Description: ##################
         python-pfconclient
@@ -86,47 +86,43 @@
         
         
         Run ``fs`` plugin until finished using any local input directory and get the resulting files in a local output directory:
         
         .. code-block:: python
         
             job_descriptors = {
-                'cmd_args': '--saveinputmeta --saveoutputmeta --dir cube/uploads',
-                'cmd_path_flags': '--dir',  # comma separated list of flags with arguments of type 'path' or 'unextpath'
+                'args': ['--saveinputmeta', '--saveoutputmeta', '--dir', 'cube/uploads'],
+                'args_path_flags': ['--dir'],  # list of flags with arguments of type 'path' or 'unextpath'
                 'auid': 'cube',
                 'number_of_workers': 1,
                 'cpu_limit': 1000,
                 'memory_limit': 200,
                 'gpu_limit': 0,
                 'image': 'fnndsc/pl-simplefsapp',
-                'selfexec': 'simplefsapp',
-                'selfpath': '/usr/local/bin',
-                'execshell': 'python3',
+                'entrypoint': ['python3', '/usr/local/bin/simplefsapp'],
                 'type': 'fs'
             }
             job_id = 'chris-jid-1'
             inputdir = '/tmp/sbin/in'
             outputdir = '/tmp/sbin/out/chris-jid-1'
             cl.run_job(job_id, job_descriptors, inputdir, outputdir)
         
         Run ``ds`` plugin until finished using the local output directory of a previous plugin as its input directory and get the resulting files in a local output directory:
         
         .. code-block:: python
         
             job_descriptors = {
-                'cmd_args': '--saveinputmeta --saveoutputmeta --prefix lolo',
+                'args': ['--saveinputmeta', '--saveoutputmeta', '--prefix', 'lolo'],
                 'auid': 'cube',
                 'number_of_workers': 1,
                 'cpu_limit': 1000,
                 'memory_limit': 200,
                 'gpu_limit': 0,
                 'image': 'fnndsc/pl-simpledsapp',
-                'selfexec': 'simpledsapp',
-                'selfpath': '/usr/local/bin',
-                'execshell': 'python3',
+                'entrypoint': ['python3', '/usr/local/bin/simpledsapp'],
                 'type': 'ds'
             }
             job_id = 'chris-jid-2'
             inputdir = '/tmp/sbin/out/chris-jid-1'
             outputdir = '/tmp/sbin/out/chris-jid-2'
             cl.run_job(job_id, job_descriptors, inputdir, outputdir)
         
@@ -145,34 +141,34 @@
             $> pfconclient http://localhost:30006/api/v1/ auth --pfcon_user pfcon --pfcon_password pfcon1234
         
         
         Run ``fs`` plugin until finished using any local input directory and get the resulting files in a local output directory:
         
         .. code-block:: bash
         
-            $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-3 --cmd_args '--saveinputmeta --saveoutputmeta --dir cube/uploads' --cmd_path_flags='--dir' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simplefsapp --selfexec simplefsapp --selfpath /usr/local/bin --execshell python3 --type fs /tmp/sbin/in /tmp/sbin/out/chris-jid-3
+            $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-3 --args '--saveinputmeta --saveoutputmeta --dir cube/uploads' --args_path_flags='--dir' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simplefsapp --selfexec simplefsapp --selfpath /usr/local/bin --execshell python3 --type fs /tmp/sbin/in /tmp/sbin/out/chris-jid-3
         
         
         Run ``ds`` plugin until finished using the local output directory of a previous plugin as its input directory and get the resulting files in a local output directory:
         
         .. code-block:: bash
         
-            $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-4 --cmd_args '--saveinputmeta --saveoutputmeta --prefix lolo' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simpledsapp --selfexec simpledsapp --selfpath /usr/local/bin --execshell python3 --type ds /tmp/sbin/out/chris-jid-3 /tmp/sbin/out/chris-jid-4
+            $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-4 --args '--saveinputmeta --saveoutputmeta --prefix lolo' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simpledsapp --selfexec simpledsapp --selfpath /usr/local/bin --execshell python3 --type ds /tmp/sbin/out/chris-jid-3 /tmp/sbin/out/chris-jid-4
         
         
         Visit the `standalone CLI client`_ wiki page to learn more about the CLI client.
         
         .. _`standalone CLI client`: https://github.com/FNNDSC/python-pfconclient/wiki/Standalone-CLI-client-tool
         
         
         Arguments of type ``path`` or ``unextpath``
         ===========================================
         
-        If a plugin's ``cmd_args`` string contains flags with arguments of type ``path`` or ``unextpath`` then those flags should be included
-        in the optional ``cmd_path_flags`` string. This string represents a comma separated list of flags. This way ``pfcon`` server will
+        If a plugin's ``args`` list contains flags with arguments of type ``path`` or ``unextpath`` then those flags should be included
+        in the optional ``args_path_flags`` list. This string represents a list of flags. This way ``pfcon`` server will
         know that it has to substitute the local path specified by the flag by an actual path in the cloud.
         
         
         Development and testing
         -----------------------
         
         Optionally setup a virtual environment
```

### Comparing `python-pfconclient-3.0.0/README.rst` & `python-pfconclient-3.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -78,47 +78,43 @@
 
 
 Run ``fs`` plugin until finished using any local input directory and get the resulting files in a local output directory:
 
 .. code-block:: python
 
     job_descriptors = {
-        'cmd_args': '--saveinputmeta --saveoutputmeta --dir cube/uploads',
-        'cmd_path_flags': '--dir',  # comma separated list of flags with arguments of type 'path' or 'unextpath'
+        'args': ['--saveinputmeta', '--saveoutputmeta', '--dir', 'cube/uploads'],
+        'args_path_flags': ['--dir'],  # list of flags with arguments of type 'path' or 'unextpath'
         'auid': 'cube',
         'number_of_workers': 1,
         'cpu_limit': 1000,
         'memory_limit': 200,
         'gpu_limit': 0,
         'image': 'fnndsc/pl-simplefsapp',
-        'selfexec': 'simplefsapp',
-        'selfpath': '/usr/local/bin',
-        'execshell': 'python3',
+        'entrypoint': ['python3', '/usr/local/bin/simplefsapp'],
         'type': 'fs'
     }
     job_id = 'chris-jid-1'
     inputdir = '/tmp/sbin/in'
     outputdir = '/tmp/sbin/out/chris-jid-1'
     cl.run_job(job_id, job_descriptors, inputdir, outputdir)
 
 Run ``ds`` plugin until finished using the local output directory of a previous plugin as its input directory and get the resulting files in a local output directory:
 
 .. code-block:: python
 
     job_descriptors = {
-        'cmd_args': '--saveinputmeta --saveoutputmeta --prefix lolo',
+        'args': ['--saveinputmeta', '--saveoutputmeta', '--prefix', 'lolo'],
         'auid': 'cube',
         'number_of_workers': 1,
         'cpu_limit': 1000,
         'memory_limit': 200,
         'gpu_limit': 0,
         'image': 'fnndsc/pl-simpledsapp',
-        'selfexec': 'simpledsapp',
-        'selfpath': '/usr/local/bin',
-        'execshell': 'python3',
+        'entrypoint': ['python3', '/usr/local/bin/simpledsapp'],
         'type': 'ds'
     }
     job_id = 'chris-jid-2'
     inputdir = '/tmp/sbin/out/chris-jid-1'
     outputdir = '/tmp/sbin/out/chris-jid-2'
     cl.run_job(job_id, job_descriptors, inputdir, outputdir)
 
@@ -137,34 +133,34 @@
     $> pfconclient http://localhost:30006/api/v1/ auth --pfcon_user pfcon --pfcon_password pfcon1234
 
 
 Run ``fs`` plugin until finished using any local input directory and get the resulting files in a local output directory:
 
 .. code-block:: bash
 
-    $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-3 --cmd_args '--saveinputmeta --saveoutputmeta --dir cube/uploads' --cmd_path_flags='--dir' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simplefsapp --selfexec simplefsapp --selfpath /usr/local/bin --execshell python3 --type fs /tmp/sbin/in /tmp/sbin/out/chris-jid-3
+    $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-3 --args '--saveinputmeta --saveoutputmeta --dir cube/uploads' --args_path_flags='--dir' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simplefsapp --selfexec simplefsapp --selfpath /usr/local/bin --execshell python3 --type fs /tmp/sbin/in /tmp/sbin/out/chris-jid-3
 
 
 Run ``ds`` plugin until finished using the local output directory of a previous plugin as its input directory and get the resulting files in a local output directory:
 
 .. code-block:: bash
 
-    $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-4 --cmd_args '--saveinputmeta --saveoutputmeta --prefix lolo' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simpledsapp --selfexec simpledsapp --selfpath /usr/local/bin --execshell python3 --type ds /tmp/sbin/out/chris-jid-3 /tmp/sbin/out/chris-jid-4
+    $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-4 --args '--saveinputmeta --saveoutputmeta --prefix lolo' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simpledsapp --selfexec simpledsapp --selfpath /usr/local/bin --execshell python3 --type ds /tmp/sbin/out/chris-jid-3 /tmp/sbin/out/chris-jid-4
 
 
 Visit the `standalone CLI client`_ wiki page to learn more about the CLI client.
 
 .. _`standalone CLI client`: https://github.com/FNNDSC/python-pfconclient/wiki/Standalone-CLI-client-tool
 
 
 Arguments of type ``path`` or ``unextpath``
 ===========================================
 
-If a plugin's ``cmd_args`` string contains flags with arguments of type ``path`` or ``unextpath`` then those flags should be included
-in the optional ``cmd_path_flags`` string. This string represents a comma separated list of flags. This way ``pfcon`` server will
+If a plugin's ``args`` list contains flags with arguments of type ``path`` or ``unextpath`` then those flags should be included
+in the optional ``args_path_flags`` list. This string represents a list of flags. This way ``pfcon`` server will
 know that it has to substitute the local path specified by the flag by an actual path in the cloud.
 
 
 Development and testing
 -----------------------
 
 Optionally setup a virtual environment
```

### Comparing `python-pfconclient-3.0.0/bin/pfconclient` & `python-pfconclient-3.1.0/bin/pfconclient`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 # create the parser for the "run" command
 parser_run = subparsers.add_parser('run', help='run a new job until finished')
 parser_run.add_argument('inputdir', help="job input directory")
 parser_run.add_argument('outputdir', help="job output directory")
 run_req_group = parser_run.add_argument_group('required job API parameters')
 run_req_group.add_argument('--jid', help="job id", required=True)
-run_req_group.add_argument('--cmd_args', help='cmd arguments string', required=True)
+run_req_group.add_argument('--args', help='cmd arguments string', required=True)
 run_req_group.add_argument('--auid', help='user id', required=True)
 run_req_group.add_argument('--number_of_workers', help='number of workers',
                               required=True)
 run_req_group.add_argument('--cpu_limit', help='cpu limit', required=True)
 run_req_group.add_argument('--memory_limit', help='memory limit', required=True)
 run_req_group.add_argument('--gpu_limit', help='gpu limit', required=True)
 run_req_group.add_argument('--image', help='docker image', required=True)
@@ -51,27 +51,27 @@
                            required=True)
 run_req_group.add_argument('--execshell',
                            help='execution shell within the docker image',
                            required=True)
 run_req_group.add_argument('--type', help='plugin type', choices=['fs', 'ds'],
                            required=True)
 run_opt_group = parser_run.add_argument_group('optional job API parameters')
-run_opt_group.add_argument('--cmd_path_flags',
+run_opt_group.add_argument('--args_path_flags',
                            help='comma separated list of cmd flags with path argument')
 parser_run.add_argument('--poll_initial_wait',
                         help='initial wait time in seconds to poll for job status')
 parser_run.add_argument('--poll_max_wait',
                         help='maximum wait time in seconds to poll for job status')
 
 # create the parser for the "submit" command
 parser_submit = subparsers.add_parser('submit', help='submit a new job')
 parser_submit.add_argument('inputdir', help="job input directory")
 submit_req_group = parser_submit.add_argument_group('required job API parameters')
 submit_req_group.add_argument('--jid', help="job id", required=True)
-submit_req_group.add_argument('--cmd_args', help='cmd arguments string', required=True)
+submit_req_group.add_argument('--args', help='cmd arguments string', required=True)
 submit_req_group.add_argument('--auid', help='user id', required=True)
 submit_req_group.add_argument('--number_of_workers', help='number of workers', required=True)
 submit_req_group.add_argument('--cpu_limit', help='cpu limit', required=True)
 submit_req_group.add_argument('--memory_limit', help='memory limit', required=True)
 submit_req_group.add_argument('--gpu_limit', help='gpu limit', required=True)
 submit_req_group.add_argument('--image', help='docker image', required=True)
 submit_req_group.add_argument('--selfexec',
@@ -82,15 +82,15 @@
                               required=True)
 submit_req_group.add_argument('--execshell',
                               help='execution shell within the docker image',
                               required=True)
 submit_req_group.add_argument('--type', help='plugin type', choices=['fs', 'ds'],
                               required=True)
 submit_opt_group = parser_submit.add_argument_group('optional job API parameters')
-submit_opt_group.add_argument('--cmd_path_flags',
+submit_opt_group.add_argument('--args_path_flags',
                               help='comma separated list of cmd flags with path argument')
 
 # create the parser for the "status" command
 parser_status = subparsers.add_parser('status', help='get the exec status of a job')
 parser_status.add_argument('--jid', help="job id", required=True)
 
 # create the parser for the "poll" command
@@ -123,25 +123,23 @@
     token = client.Client.get_auth_token(auth_url, args.pfcon_user, args.pfcon_password)
     print(f'\ntoken: {token}\n')
 else:
     client = client.Client(args.url, args.auth_token)
 
     if args.subparser_name == 'run' or args.subparser_name == 'submit':
         d_job_descriptors = {
-            'cmd_args': args.cmd_args,
-            'cmd_path_flags': args.cmd_path_flags if args.cmd_path_flags is not None else '',
+            'entrypoint': [args.execshell, os.path.join(args.selfpath, args.selfexec)],
+            'args': args.args.split(),
+            'args_path_flags': args.args_path_flags if args.args_path_flags is not None else '',
             'auid': args.auid,
             'number_of_workers': args.number_of_workers,
             'cpu_limit': args.cpu_limit,
             'memory_limit': args.memory_limit,
             'gpu_limit': args.gpu_limit,
             'image': args.image,
-            'selfexec': args.selfexec,
-            'selfpath': args.selfpath,
-            'execshell':args.execshell,
             'type': args.type
         }
         if args.subparser_name == 'run':
             if args.poll_initial_wait:
                 client.initial_wait = args.poll_initial_wait
             if args.poll_max_wait:
                 client.max_wait = args.poll_max_wait
```

### Comparing `python-pfconclient-3.0.0/pfconclient/client.py` & `python-pfconclient-3.1.0/pfconclient/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 
 class Client(object):
     """
     A pfcon API client.
     """
 
-    def __init__(self, url, auth_token):
+    def __init__(self, url, auth_token, pfcon_innetwork=False):
         self.url = url
         self.set_auth_token(auth_token)
+        self.pfcon_innetwork = pfcon_innetwork
 
         # initial and maximum wait time (seconds) for exponential-backoff-based retries
         self.initial_wait = 2
         self.max_wait = 2**15
 
     def set_auth_token(self, auth_token):
         if not auth_token:
@@ -52,15 +53,15 @@
         else:
             print(f'Job {job_id} finished with unexpected status: {status}')
         print(f'\nDeleting job {job_id} from the remote...')
         self.delete_job(job_id, timeout)
         print('Done')
         return status
 
-    def submit_job(self, job_id, d_job_descriptors, data_file, timeout=1000):
+    def submit_job(self, job_id, d_job_descriptors, data_file=None, timeout=1000):
         """
         Submit a new job.
         """
         d_job_descriptors['jid'] = job_id
         url = self.url + 'jobs/'
         resp = self.post(url, d_job_descriptors, data_file, timeout)
         return self.get_data_from_response(resp)
@@ -91,14 +92,37 @@
             if status in ('undefined', 'finishedSuccessfully', 'finishedWithError'):
                 break
             else:
                 wait_time = self.initial_wait * 2 ** poll_num
                 poll_num += 1
         return status
 
+    def get_job_json_data(self, job_id, job_output_path, timeout=1000):
+        """
+        Get a job's JSON file content. This only works for pfcon in-network mode
+        """
+        if not self.pfcon_innetwork:
+            raise PfconRequestException('JSON data is only available for PFCON server '
+                                        'operating in-network')
+        url = self.url + 'jobs/' + job_id + '/file/?job_output_path=' + job_output_path
+        resp = self.get(url, timeout)
+        json_content = self.get_data_from_response(resp)
+        return json_content
+
+    def get_job_json_file(self, job_id, job_output_path, local_dir, timeout=1000):
+        """
+        Get and save a job's zip file into a local directory.
+        """
+        if not os.path.exists(local_dir):
+            os.makedirs(local_dir)
+        json_content = self.get_job_json_data(job_id, job_output_path, timeout)
+        fpath = os.path.join(local_dir, job_id + '.json')
+        with open(fpath, 'w') as f:
+            json.dump(json_content, f)
+
     def get_job_zip_data(self, job_id, timeout=1000):
         """
         Get a job's zip file content.
         """
         url = self.url + 'jobs/' + job_id + '/file/'
         resp = self.get(url, timeout)
         zip_content = self.get_data_from_response(resp, 'application/zip')
@@ -160,15 +184,14 @@
         """
         Make a POST request to pfcon.
         """
         headers = {'Authorization': 'Bearer ' + self.auth_token}
         if data_file is None:
             headers['Content-Type'] = 'application/json'
             files = None
-            data = json.dumps(data)
         else:
             # this is a multipart request
             files = {'data_file': data_file}
         try:
             r = requests.post(url, files=files, data=data,
                               headers={'Authorization': 'Bearer ' + self.auth_token},
                               timeout=timeout)
```

### Comparing `python-pfconclient-3.0.0/python_pfconclient.egg-info/PKG-INFO` & `python-pfconclient-3.1.0/python_pfconclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-pfconclient
-Version: 3.0.0
+Version: 3.1.0
 Summary: (Python) client for the Pfcon API
 Home-page: https://github.com/FNNDSC/python-pfconclient
 Author: FNNDSC
 Author-email: dev@babymri.org
 License: MIT
 Description: ##################
         python-pfconclient
@@ -86,47 +86,43 @@
         
         
         Run ``fs`` plugin until finished using any local input directory and get the resulting files in a local output directory:
         
         .. code-block:: python
         
             job_descriptors = {
-                'cmd_args': '--saveinputmeta --saveoutputmeta --dir cube/uploads',
-                'cmd_path_flags': '--dir',  # comma separated list of flags with arguments of type 'path' or 'unextpath'
+                'args': ['--saveinputmeta', '--saveoutputmeta', '--dir', 'cube/uploads'],
+                'args_path_flags': ['--dir'],  # list of flags with arguments of type 'path' or 'unextpath'
                 'auid': 'cube',
                 'number_of_workers': 1,
                 'cpu_limit': 1000,
                 'memory_limit': 200,
                 'gpu_limit': 0,
                 'image': 'fnndsc/pl-simplefsapp',
-                'selfexec': 'simplefsapp',
-                'selfpath': '/usr/local/bin',
-                'execshell': 'python3',
+                'entrypoint': ['python3', '/usr/local/bin/simplefsapp'],
                 'type': 'fs'
             }
             job_id = 'chris-jid-1'
             inputdir = '/tmp/sbin/in'
             outputdir = '/tmp/sbin/out/chris-jid-1'
             cl.run_job(job_id, job_descriptors, inputdir, outputdir)
         
         Run ``ds`` plugin until finished using the local output directory of a previous plugin as its input directory and get the resulting files in a local output directory:
         
         .. code-block:: python
         
             job_descriptors = {
-                'cmd_args': '--saveinputmeta --saveoutputmeta --prefix lolo',
+                'args': ['--saveinputmeta', '--saveoutputmeta', '--prefix', 'lolo'],
                 'auid': 'cube',
                 'number_of_workers': 1,
                 'cpu_limit': 1000,
                 'memory_limit': 200,
                 'gpu_limit': 0,
                 'image': 'fnndsc/pl-simpledsapp',
-                'selfexec': 'simpledsapp',
-                'selfpath': '/usr/local/bin',
-                'execshell': 'python3',
+                'entrypoint': ['python3', '/usr/local/bin/simpledsapp'],
                 'type': 'ds'
             }
             job_id = 'chris-jid-2'
             inputdir = '/tmp/sbin/out/chris-jid-1'
             outputdir = '/tmp/sbin/out/chris-jid-2'
             cl.run_job(job_id, job_descriptors, inputdir, outputdir)
         
@@ -145,34 +141,34 @@
             $> pfconclient http://localhost:30006/api/v1/ auth --pfcon_user pfcon --pfcon_password pfcon1234
         
         
         Run ``fs`` plugin until finished using any local input directory and get the resulting files in a local output directory:
         
         .. code-block:: bash
         
-            $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-3 --cmd_args '--saveinputmeta --saveoutputmeta --dir cube/uploads' --cmd_path_flags='--dir' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simplefsapp --selfexec simplefsapp --selfpath /usr/local/bin --execshell python3 --type fs /tmp/sbin/in /tmp/sbin/out/chris-jid-3
+            $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-3 --args '--saveinputmeta --saveoutputmeta --dir cube/uploads' --args_path_flags='--dir' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simplefsapp --selfexec simplefsapp --selfpath /usr/local/bin --execshell python3 --type fs /tmp/sbin/in /tmp/sbin/out/chris-jid-3
         
         
         Run ``ds`` plugin until finished using the local output directory of a previous plugin as its input directory and get the resulting files in a local output directory:
         
         .. code-block:: bash
         
-            $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-4 --cmd_args '--saveinputmeta --saveoutputmeta --prefix lolo' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simpledsapp --selfexec simpledsapp --selfpath /usr/local/bin --execshell python3 --type ds /tmp/sbin/out/chris-jid-3 /tmp/sbin/out/chris-jid-4
+            $> pfconclient http://localhost:30006/api/v1/ -a <token> run --jid chris-jid-4 --args '--saveinputmeta --saveoutputmeta --prefix lolo' --auid cube --number_of_workers 1 --cpu_limit 1000 --memory_limit 200 --gpu_limit 0 --image fnndsc/pl-simpledsapp --selfexec simpledsapp --selfpath /usr/local/bin --execshell python3 --type ds /tmp/sbin/out/chris-jid-3 /tmp/sbin/out/chris-jid-4
         
         
         Visit the `standalone CLI client`_ wiki page to learn more about the CLI client.
         
         .. _`standalone CLI client`: https://github.com/FNNDSC/python-pfconclient/wiki/Standalone-CLI-client-tool
         
         
         Arguments of type ``path`` or ``unextpath``
         ===========================================
         
-        If a plugin's ``cmd_args`` string contains flags with arguments of type ``path`` or ``unextpath`` then those flags should be included
-        in the optional ``cmd_path_flags`` string. This string represents a comma separated list of flags. This way ``pfcon`` server will
+        If a plugin's ``args`` list contains flags with arguments of type ``path`` or ``unextpath`` then those flags should be included
+        in the optional ``args_path_flags`` list. This string represents a list of flags. This way ``pfcon`` server will
         know that it has to substitute the local path specified by the flag by an actual path in the cloud.
         
         
         Development and testing
         -----------------------
         
         Optionally setup a virtual environment
```

### Comparing `python-pfconclient-3.0.0/setup.py` & `python-pfconclient-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open(path.join(path.dirname(path.abspath(__file__)), 'README.rst')) as f:
     readme = f.read()
 
 setup(
       name             =   'python-pfconclient',
-      version          =   '3.0.0',
+      version          =   '3.1.0',
       description      =   '(Python) client for the Pfcon API',
       long_description =   readme,
       author           =   'FNNDSC',
       author_email     =   'dev@babymri.org',
       url              =   'https://github.com/FNNDSC/python-pfconclient',
       packages         =   ['pfconclient'],
       install_requires =   ['requests>=2.27.1'],
```

