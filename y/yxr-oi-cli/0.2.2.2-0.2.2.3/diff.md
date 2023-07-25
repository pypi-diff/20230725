# Comparing `tmp/yxr_oi_cli-0.2.2.2.tar.gz` & `tmp/yxr_oi_cli-0.2.2.3.tar.gz`

## Comparing `yxr_oi_cli-0.2.2.2.tar` & `yxr_oi_cli-0.2.2.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/py.typed
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/abstract/HtmlTagAbstract.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/abstract/__init__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/__init__.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/account.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/analyze.py
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/completion.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/config.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/constant.py
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/contest.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/init.py
--rwxr-xr-x   0        0        0     1280 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/lang.py
--rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/main.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/problem.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/reg_list.py
--rwxr-xr-x   0        0        0     4684 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/submit.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/template.py
--rwxr-xr-x   0        0        0     3450 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/test.py
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/adaptor/AtCoderAdaptor.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/adaptor/CodeforcesAdaptor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/adaptor/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/cli/adaptor/ojman.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/core/DI.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/core/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/core/problem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/custom/__init__.py
--rw-r--r--   0        0        0    12402 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/custom/Codeforces/Codeforces.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/custom/Codeforces/__init__.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/custom/Codeforces/contestList.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/custom/Codeforces/standing.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/Account.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/Analyze.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/BaseOj.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/Contest.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/FolderState.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/LangKV.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/ParseProblemResult.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/Problem.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/ProblemMeta.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/Result.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/Template.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/TestCase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/model/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/FileUtil.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/HtmlTag.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/HttpUtil.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/HttpUtilCookiesHelper.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/Logger.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/OJUtil.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/Provider2.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/Singleton.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/__init__.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/account.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/analyze.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/async2sync.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/configFolder.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/db.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/diffTool.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/enc.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/force_symlink.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/start_terminal.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/template.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/utc2local.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/wsTool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/consts/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/consts/ids.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/oi_cli2/utils/consts/platforms.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/LICENSE
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/README.md
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/pyproject.toml
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.2/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/py.typed
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/abstract/HtmlTagAbstract.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/abstract/__init__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/__init__.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/account.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/analyze.py
+-rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/completion.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/config.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/constant.py
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/contest.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/init.py
+-rwxr-xr-x   0        0        0     1280 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/lang.py
+-rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/main.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/problem.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/reg_list.py
+-rwxr-xr-x   0        0        0     4732 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/submit.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/template.py
+-rwxr-xr-x   0        0        0     3613 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/test.py
+-rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/adaptor/AtCoderAdaptor.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/adaptor/CodeforcesAdaptor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/adaptor/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/cli/adaptor/ojman.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/core/DI.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/core/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/core/problem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/custom/__init__.py
+-rw-r--r--   0        0        0    13307 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/custom/Codeforces/Codeforces.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/custom/Codeforces/__init__.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/custom/Codeforces/contestList.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/custom/Codeforces/standing.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/Account.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/Analyze.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/BaseOj.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/Contest.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/FolderState.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/LangKV.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/ParseProblemResult.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/Problem.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/ProblemMeta.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/Result.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/Template.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/TestCase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/model/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/FileUtil.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/HtmlTag.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/HttpUtil.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/HttpUtilCookiesHelper.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/Logger.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/OJUtil.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/Provider2.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/Singleton.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/__init__.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/account.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/analyze.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/async2sync.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/configFolder.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/db.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/diffTool.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/enc.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/force_symlink.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/start_terminal.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/template.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/utc2local.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/wsTool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/consts/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/consts/ids.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/oi_cli2/utils/consts/platforms.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/LICENSE
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/README.md
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 yxr_oi_cli-0.2.2.3/PKG-INFO
```

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/abstract/HtmlTagAbstract.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/abstract/HtmlTagAbstract.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/account.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/account.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/analyze.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/completion.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/completion.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/config.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/config.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/constant.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/constant.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 SUBMIT_PY = 'submit.py'
 # LANG_CONFIG_FILE = ROOT_PATH + 'lang.json'
 OT_LOG = 'log/oiTerminal.log'
 USER_CONFIG_FILE = '_userConfig.json'
 COOKIES_FILE = '_cookies.json'
 ACCT_CONFIG_FILE = '_acctConfig.json'  # TODO split config json
 TEMP_CONFIG_FILE = '_tempConfig.json'
+# LOG
+APP_NAME='oiTerminal'
 
 IN_SUFFIX = 'in.'
 OUT_SUFFIX = 'out.'
 
 # CONFIG
 FETCH_RESULT_INTERVAL = 2
 CIPHER_KEY = 'oiTerminal'
```

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/contest.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/contest.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/init.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/init.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/lang.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/lang.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/main.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/main.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/problem.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/problem.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/reg_list.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/reg_list.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/submit.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
   """Make a new submission table."""
   table = Table().grid()
   table.add_column(min_width=12)
   table.add_column()
   table.add_row("Result ID", f"{res.id}")
   # "[red]ERROR" if value < 50 else "[green]SUCCESS"
   table.add_row("Status", Text.from_ansi(f"{status_string(res)}"))
-  table.add_row("Time(s)", f"{res.time_note}")
-  table.add_row("Memory(KB)", f"{res.mem_note}")
+  table.add_row("Time", f"{res.time_note}")
+  table.add_row("Memory", f"{res.mem_note}")
   if res.msg_txt:
     table.add_row("MSG", f"{res.msg_txt}")
   if res.url:
     table.add_row("Url", f"{res.url}")
   return table
 
 
@@ -49,15 +49,16 @@
   await oj.init()
   try:
     result = SubmissionResult()
     with Live(auto_refresh=False) as live:
       async for result in oj.async_get_result_yield(problem_url, time_gap=FETCH_RESULT_INTERVAL):
         live.update(generate_submission_table(result), refresh=True)
   except Exception as e:
-    logging.exception(e)
+    logger: logging.Logger = Provider2().get(DI_LOGGER)
+    logger.exception(e)
   await oj.deinit()
   return result
 
 
 def submit_parser() -> Tuple[str, str, str, Account, str, str]:
   logger: logging.Logger = Provider2().get(DI_LOGGER)
   am: AccountManager = Provider2().get(DI_ACCMAN)
```

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/template.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/template.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/test.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,37 +17,41 @@
 from oi_cli2.utils.template import TemplateManager
 
 console = Console(color_system='256', style=None)
 
 
 def tester(root_folder: str, test_files: List[str], testcase_folder: str, template: Template,
            diff_fn: Callable[[str, str, str], None], logger: logging.Logger):
+  # TODO, 这里似乎传入参数也是 abspath, 两个folder 似乎有点冗余, 还有test_folder
   logger.debug(f'{root_folder},{test_files},{testcase_folder}')
   # makefolder & mv code 2 folder
   os.makedirs(TEST_FOLDER, exist_ok=True)
   for source_file_name in test_files:
     if not os.path.exists(source_file_name):
       raise FileNotFoundError(f"'{source_file_name}' not found!")
     shutil.copy(source_file_name, os.path.join(TEST_FOLDER, source_file_name))
   # compile
   os.chdir(TEST_FOLDER)
+  # TODO 非系统命令diff, 改为 自己实现函数/注入式/支持交互
   if os.system(template.compilation) != 0:
     logger.error('Complete Failed.')
     return
+
   logger.debug('In Exist:' + os.path.join(root_folder, testcase_folder, f"{IN_SUFFIX}{0}"))
 
   # run  "" not better than 'time' in bash but worse is better :-)
   i = 0
   while os.path.isfile(os.path.join(root_folder, testcase_folder, f"{IN_SUFFIX}{i}")):
     std_in_file = os.path.join(root_folder, testcase_folder, f"{IN_SUFFIX}{i}")
     std_out_file = os.path.join(root_folder, testcase_folder, f"{OUT_SUFFIX}{i}")
     user_out_file = os.path.join(root_folder, TEST_FOLDER, f"{OUT_SUFFIX}{i}")
     start_time = datetime.datetime.now()
-    logger.debug(f"{template.execute} < {std_in_file} > {user_out_file}")
-    os.system(f"{template.execute} < {std_in_file} > {user_out_file}")
+    command = f'"{template.execute}" < "{std_in_file}" > "{user_out_file}"'
+    logger.debug(command)
+    os.system(command)
     end_time = datetime.datetime.now()
     print()
     # TODO COMPARE TIME
     print(f"TestCase {i} Time spend: {GREEN}{(end_time - start_time).total_seconds()}s{DEFAULT}")
     diff_fn(std_in_file, std_out_file, user_out_file)
 
     i += 1
@@ -78,15 +82,15 @@
          test_files=[source_file_name],
          testcase_folder=os.path.abspath('.'),
          template=template,
          diff_fn=diff_result_fn,
          logger=logger)
 
   # shutil.rmtree(TEST_FOLDER)
-  logger.debug('test finished')
+  # logger.debug('test finished')
   return True
 
 
 @click.command(name='test')
 def tst_command() -> None:
   try:
     logger: logging.Logger = Provider2().get(DI_LOGGER)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/adaptor/AtCoderAdaptor.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/adaptor/AtCoderAdaptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
   return SubmissionResult(
       id=res.id,
       cur_status=status,
       quick_key=res.url,  # for refetch result
       url=res.url,  # TODO change to webpage url
       state_note=str(res.score),
-      time_note=str(res.time_cost_ms / 1000),
-      mem_note=str(res.mem_cost_kb),
+      time_note=str(res.time_cost_ms / 1000) + ' ms',
+      mem_note=str(res.mem_cost_kb) + ' kb',
       msg_txt=res.msg_txt,
   )
 
 
 class AtCoder(BaseOj):
 
   def __init__(self, http_util: HttpUtil, logger: logging.Logger, account: Account, html_tag: HtmlTagAbstract) -> None:
```

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/adaptor/CodeforcesAdaptor.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/adaptor/CodeforcesAdaptor.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/cli/adaptor/ojman.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/cli/adaptor/ojman.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/core/problem.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/core/problem.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/custom/Codeforces/Codeforces.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/custom/Codeforces/Codeforces.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import logging
 import os
 from typing import Any, Tuple, AsyncIterator
 
 from requests.exceptions import ReadTimeout, ConnectTimeout
 
-from oi_cli2.cli.constant import CIPHER_KEY, GREEN, DEFAULT
+from oi_cli2.cli.constant import APP_NAME, CIPHER_KEY, GREEN, DEFAULT
 from oi_cli2.model.BaseOj import BaseOj
 from oi_cli2.model.ParseProblemResult import ParsedProblemResult
 from oi_cli2.model.LangKV import LangKV
 from oi_cli2.model.Account import Account
 from oi_cli2.model.ProblemMeta import ContestMeta, ProblemMeta, E_STATUS
 from oi_cli2.model.Result import SubmissionResult
 from oi_cli2.model.TestCase import TestCase
@@ -34,14 +34,15 @@
   def __init__(self, http_util: AioHttpHelperInterface, logger: logging.Logger, account: Account) -> None:
     super().__init__()
     assert (account is not None)
     self._base_url = 'https://codeforces.com/'
     self.logger: logging.Logger = logger
     self.account: Account = account
     self.http = http_util
+    self.api_sub_logger:logging.Logger = logging.getLogger(f'{APP_NAME}.yxr-cf-core')
 
   async def init(self) -> None:
     await self.http.open_session()
 
   async def deinit(self) -> None:
     await self.http.close_session()
 
@@ -144,90 +145,110 @@
     contest_id, problem_key = pid2split(sid)
     self.logger.debug(f'{contest_id},{problem_key}')
 
     submit_id, resp = await async_submit(http=self.http,
                                          contest_id=contest_id,
                                          level=problem_key,
                                          file_path=code_path,
-                                         lang_id=language_id)
+                                         lang_id=language_id,
+                                         logger=self.api_sub_logger)
     self.logger.debug(f'submit_id = {submit_id}')
     return bool(submit_id)
 
   async def async_get_result_yield(self, problem_url: str, time_gap: float = 2) -> AsyncIterator[SubmissionResult]:
     contest_id, problem_key = problem_url_parse(problem_url)
 
     # return (end watch?, transform result)
     def custom_handler(result: Any) -> Tuple[bool, SubmissionWSResult]:
       parsed_data = transform_submission(result)
       if parsed_data.msg != 'TESTING':
         return True, parsed_data
+
+
       return False, parsed_data
 
     # TODO move more parse inside codeforces-core ? cf是出错中断形式,状态+数量
     def page_result_transform(res: SubmissionPageResult) -> SubmissionResult:
-      # logging.warn('verdict:' + res.verdict)
+      self.logger.debug('page res:'+str(res))
       cur_status = SubmissionResult.Status.PENDING
       if res.verdict.startswith('Running'):
         cur_status = SubmissionResult.Status.RUNNING
       elif res.verdict.startswith('In queue'):
         cur_status = SubmissionResult.Status.RUNNING
       elif res.verdict.startswith('Accepted'):
         cur_status = SubmissionResult.Status.AC
       elif res.verdict.startswith('Pretests passed'):
         cur_status = SubmissionResult.Status.AC
       elif res.verdict.startswith('Wrong answer'):
         cur_status = SubmissionResult.Status.WA
+      elif res.verdict.startswith('Time limit exceeded'):
+        cur_status = SubmissionResult.Status.TLE
       elif res.verdict.startswith('Runtime error'): # Runtime error on pretest 2
         cur_status = SubmissionResult.Status.RE
       else:
-        logging.error('NOT HANDLE PAGE:', res.verdict)
+        self.logger.error('NOT HANDLE PAGE:'+str(res.verdict))
+
+      if res.url.startswith('/'):
+        res.url = 'https://codeforces.com' + res.url
 
       return SubmissionResult(id=res.id,
                               cur_status=cur_status,
-                              time_note=res.time_ms,
-                              mem_note=res.mem_bytes,
+                              time_note=res.time_ms + ' ms',
+                              mem_note=str(int(res.mem_bytes)/1000) + ' kb',
                               url=res.url,
                               msg_txt=res.verdict)
 
+
+
+
     # TODO move more parse inside codeforces-core ?
     def ws_result_transform(res: SubmissionWSResult) -> SubmissionResult:
-      # logging.warn('res.msg:' + res.msg)
       cur_status = SubmissionResult.Status.PENDING
       if res.msg == 'TESTING':
         cur_status = SubmissionResult.Status.RUNNING
       elif res.msg == 'OK':
         cur_status = SubmissionResult.Status.AC
       elif res.msg == 'WRONG_ANSWER':
         cur_status = SubmissionResult.Status.WA
       else:
-        logging.error('NOT HANDLE WS:' + str(res.msg))
+        self.logger.error('NOT HANDLE WS:' + str(res.msg))
 
       msg_txt = str(res.testcases)
-      if cur_status == SubmissionResult.Status.AC:
+      if cur_status in [SubmissionResult.Status.AC, SubmissionResult.Status.WA]:
         msg_txt = f'{res.passed}/{res.testcases}'
 
       return SubmissionResult(
           id=str(res.submit_id),
           cur_status=cur_status,
-          time_note=str(res.ms),
-          mem_note=str(res.mem),
-          url=f'/contest/{res.contest_id}/submission/{res.submit_id}',
+          time_note=str(res.ms) + ' ms',
+          mem_note=str(int(res.mem)/1000) + ' kb',
+          url=f'https://codeforces.com/contest/{res.contest_id}/submission/{res.submit_id}',
           msg_txt=msg_txt,
       )
 
     # TODO visit page without ws first
-    results = await async_fetch_submission_page(http=self.http, problem_url=problem_url)
+    results = await async_fetch_submission_page(http=self.http, problem_url=problem_url,logger=self.api_sub_logger)
+    fix_submit_id = ''
     if len(results) > 0:
       result = page_result_transform(results[0])
+      fix_submit_id = result.id
+      self.logger.debug(f"fix submit_id = {fix_submit_id}");
       yield result
       if result.cur_status not in [SubmissionResult.Status.PENDING, SubmissionResult.Status.RUNNING]:
         return
 
+    self.logger.debug('after page result, enter ws result')
+
     # TODO add timeout for ws
-    async for wsresult in create_contest_ws_task_yield(http=self.http, contest_id=contest_id, ws_handler=custom_handler):
+    # TODO 可能有别人的? pc/cc?
+    async for wsresult in create_contest_ws_task_yield(http=self.http, contest_id=contest_id, ws_handler=custom_handler,logger=self.api_sub_logger):
+      self.logger.debug('ws res:'+str(wsresult))
+      if fix_submit_id and wsresult.submit_id != fix_submit_id:
+        self.logger.debug('[skip]fixed id not match! continue')
+        continue
       data = ws_result_transform(wsresult)
       yield data
       if data.cur_status not in [SubmissionResult.Status.PENDING, SubmissionResult.Status.RUNNING]:
         return
 
     results = await async_fetch_submission_page(http=self.http, problem_url=problem_url)
     assert len(results) > 0
```

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/custom/Codeforces/contestList.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/custom/Codeforces/contestList.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/custom/Codeforces/standing.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/custom/Codeforces/standing.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/Account.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/Account.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/Analyze.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/Analyze.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/BaseOj.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/BaseOj.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/Contest.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/Contest.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/FolderState.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/FolderState.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# TODO dataclasses, for better debug
+
 class FolderState:
   oj: str
   id: str  # string id
   cid: str  # contest id
   pid: str  # problem id
   problem_url: str
   up_lang: str
```

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/ParseProblemResult.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/ParseProblemResult.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/Problem.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/Problem.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/ProblemMeta.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/ProblemMeta.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/Result.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/Result.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     PENDING, RUNNING, AC, RE, CE, WA, TLE, MLE, IDLE, UNKNOWN = range(10)
 
   id: str = '0'
   cur_status: Status = Status.PENDING
   url: str = ''  # print for user
   quick_key: str = ''  # for refetch result
   state_note: str = '0'
-  time_note: str = '0/0'
-  mem_note: str = '0/0'
+  time_note: str = ''
+  mem_note: str = ''
   msg_txt: str = ''
 
 
 def status_string(result: SubmissionResult) -> str:
   return {
       SubmissionResult.Status.PENDING: YELLOW + 'Pending...' + DEFAULT,
       SubmissionResult.Status.RUNNING: GREEN + 'Running...' + DEFAULT,
```

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/model/Template.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/model/Template.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/FileUtil.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/FileUtil.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/HtmlTag.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/HtmlTag.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/HttpUtil.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/HttpUtil.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/HttpUtilCookiesHelper.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/HttpUtilCookiesHelper.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/Logger.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/Logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import os
 import traceback
 
 from oi_cli2.utils.Singleton import Singleton
 
+from oi_cli2.cli.constant import APP_NAME
+
 
 @Singleton
 class LogConfig:
 
   def __init__(self):
     self.env = os.getenv('OITERMINAL_ENV')
     if self.env is None:
@@ -25,23 +27,24 @@
     os.makedirs(os.path.dirname(logger_path))
   except FileExistsError:
     pass
   except Exception as e:
     print(e)
     traceback.print_exc()
 
-  logger = logging.getLogger(__name__)
+  # 调用库的 logging 名是 {APP_NAME}.xxx
+  logger = logging.getLogger(APP_NAME)
   # basic level shoud not larger than handler
   logger.setLevel(logging.DEBUG)
   # remove default handler
   logging.getLogger().handlers.clear()
 
   # file
   fh = logging.FileHandler(logger_path)
-  fileformatter = logging.Formatter('[%(asctime)s %(levelname)s %(filename)s %(funcName)s %(lineno)d]: %(message)s')
+  fileformatter = logging.Formatter('[%(asctime)s %(name)s %(levelname)s %(filename)s %(funcName)s %(lineno)d]: %(message)s')
   fh.setFormatter(fileformatter)
   fh.setLevel(logging.DEBUG)
   logger.addHandler(fh)
 
   # stream warning
   sh = logging.StreamHandler()
   streamformatter = logging.Formatter('[%(levelname)s]: %(message)s')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/OJUtil.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/OJUtil.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/Provider2.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/Provider2.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/account.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/account.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/analyze.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/analyze.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/async2sync.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/async2sync.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/configFolder.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/configFolder.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/db.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/db.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/diffTool.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/diffTool.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/enc.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/enc.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/template.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/template.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/oi_cli2/utils/wsTool.py` & `yxr_oi_cli-0.2.2.3/oi_cli2/utils/wsTool.py`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/.gitignore` & `yxr_oi_cli-0.2.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/LICENSE` & `yxr_oi_cli-0.2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yxr_oi_cli-0.2.2.2/pyproject.toml` & `yxr_oi_cli-0.2.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "requests >= 2",
   "beautifulsoup4 >= 4",
   "lxml >= 4",
   "pycryptodome >= 3.13.0",
   "click >= 8.1.3",
   "rich >= 11.0.0",
   "yxr-atcoder-core == 0.0.3.3",
-  "yxr-codeforces-core == 0.0.2.1",
+  "yxr-codeforces-core == 0.0.2.2",
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
 ]
```

### Comparing `yxr_oi_cli-0.2.2.2/PKG-INFO` & `yxr_oi_cli-0.2.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yxr-oi-cli
-Version: 0.2.2.2
+Version: 0.2.2.3
 Summary: Simple Online Judge Cli Tool
 Project-URL: Homepage, https://github.com/CroMarmot/oiTerminal
 Project-URL: Bug Tracker, https://github.com/CroMarmot/oiTerminal/issues
 Author-email: YeXiaoRain <yexiaorain@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 陈鼫RWHTYFZ
@@ -34,15 +34,15 @@
 Requires-Dist: beautifulsoup4>=4
 Requires-Dist: click>=8.1.3
 Requires-Dist: lxml>=4
 Requires-Dist: pycryptodome>=3.13.0
 Requires-Dist: requests>=2
 Requires-Dist: rich>=11.0.0
 Requires-Dist: yxr-atcoder-core==0.0.3.3
-Requires-Dist: yxr-codeforces-core==0.0.2.1
+Requires-Dist: yxr-codeforces-core==0.0.2.2
 Provides-Extra: tests
 Requires-Dist: build; extra == 'tests'
 Requires-Dist: coverage>=6; extra == 'tests'
 Requires-Dist: pytest>=7; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # oiTerminal
```

