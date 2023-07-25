# Comparing `tmp/pulumi_gitlab-6.2.0a1689690121.tar.gz` & `tmp/pulumi_gitlab-6.2.0a1690301864.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_gitlab-6.2.0a1689690121.tar", last modified: Tue Jul 18 14:27:05 2023, max compression
+gzip compressed data, was "pulumi_gitlab-6.2.0a1690301864.tar", last modified: Tue Jul 25 16:22:16 2023, max compression
```

## Comparing `pulumi_gitlab-6.2.0a1689690121.tar` & `pulumi_gitlab-6.2.0a1690301864.tar`

### file list

```diff
@@ -1,140 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:05.459537 pulumi_gitlab-6.2.0a1689690121/
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-18 14:27:05.459537 pulumi_gitlab-6.2.0a1689690121/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:05.459537 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45582 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/application.py
--rw-r--r--   0 runner    (1001) docker     (123)   690759 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30857 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    21349 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/cluster_agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:05.459537 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/deploy_key_enable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/deploy_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_cluster_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_current_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_instance_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_instance_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    44465 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24930 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    31009 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_milestones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_protected_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_protected_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_release_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_release_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_repository_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    17432 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_user_sshkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    68245 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_badge.py
--rw-r--r--   0 runner    (1001) docker     (123)    33679 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    46605 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    24408 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_ldap_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_project_file_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_saml_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_share_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    34419 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/instance_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    17060 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_custom_issue_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26646 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_emails_on_push.py
--rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_external_wiki.py
--rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    45241 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_microsoft_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_pipelines_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    60436 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/label.py
--rw-r--r--   0 runner    (1001) docker     (123)   168744 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/pages_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    20010 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/personal_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/pipeline_schedule_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/pipeline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)   262332 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24082 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_approval_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_badge.py
--rw-r--r--   0 runner    (1001) docker     (123)    36176 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_freeze_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    73619 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_issue_board.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    24086 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_level_mr_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_protected_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_runner_enablement.py
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_share_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/release_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    36358 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_custom_issue_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26698 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_emails_on_push.py
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_external_wiki.py
--rw-r--r--   0 runner    (1001) docker     (123)    19121 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    45261 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)    38116 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_microsoft_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_pipelines_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    60458 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)    21890 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/system_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    32444 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/user_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:05.459537 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:27:05.459537 pulumi_gitlab-6.2.0a1689690121/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-18 14:27:05.000000 pulumi_gitlab-6.2.0a1689690121/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:16.919537 pulumi_gitlab-6.2.0a1690301864/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-25 16:22:16.919537 pulumi_gitlab-6.2.0a1690301864/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:16.915537 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    18511 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45582 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)   690647 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30920 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21349 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/cluster_agent_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21841 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/compliance_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:16.919537 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/deploy_key_enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/deploy_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_cluster_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_current_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_instance_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_instance_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44465 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24930 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31009 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_milestones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_protected_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_protected_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25810 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_release_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_release_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_repository_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17432 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_user_sshkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68245 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33679 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46605 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24408 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_ldap_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_project_file_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_saml_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34419 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/instance_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17060 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_custom_issue_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26646 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_emails_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45241 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60436 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168744 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/pages_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20010 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/personal_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/pipeline_schedule_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/pipeline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)   262332 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24082 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_approval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36176 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_compliance_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_freeze_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73619 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_issue_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24086 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_level_mr_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_protected_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_runner_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/release_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34937 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_custom_issue_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26698 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_emails_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19121 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45261 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38116 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60458 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21890 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/system_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32444 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/user_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:16.919537 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:22:16.919537 pulumi_gitlab-6.2.0a1690301864/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-25 16:22:16.000000 pulumi_gitlab-6.2.0a1690301864/setup.py
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/PKG-INFO` & `pulumi_gitlab-6.2.0a1690301864/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_gitlab
-Version: 6.2.0a1689690121
+Version: 6.2.0a1690301864
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/README.md` & `pulumi_gitlab-6.2.0a1690301864/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/__init__.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Export this package's modules as members:
 from .application import *
 from .application_settings import *
 from .branch import *
 from .branch_protection import *
 from .cluster_agent import *
 from .cluster_agent_token import *
+from .compliance_framework import *
 from .deploy_key import *
 from .deploy_key_enable import *
 from .deploy_token import *
 from .get_application import *
 from .get_branch import *
 from .get_cluster_agent import *
 from .get_cluster_agents import *
@@ -84,14 +85,15 @@
 from .pipeline_schedule_variable import *
 from .pipeline_trigger import *
 from .project import *
 from .project_access_token import *
 from .project_approval_rule import *
 from .project_badge import *
 from .project_cluster import *
+from .project_compliance_framework import *
 from .project_custom_attribute import *
 from .project_environment import *
 from .project_freeze_period import *
 from .project_hook import *
 from .project_issue import *
 from .project_issue_board import *
 from .project_label import *
@@ -182,14 +184,22 @@
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/clusterAgentToken:ClusterAgentToken": "ClusterAgentToken"
   }
  },
  {
   "pkg": "gitlab",
+  "mod": "index/complianceFramework",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/complianceFramework:ComplianceFramework": "ComplianceFramework"
+  }
+ },
+ {
+  "pkg": "gitlab",
   "mod": "index/deployKey",
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/deployKey:DeployKey": "DeployKey"
   }
  },
  {
@@ -478,14 +488,22 @@
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/projectCluster:ProjectCluster": "ProjectCluster"
   }
  },
  {
   "pkg": "gitlab",
+  "mod": "index/projectComplianceFramework",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/projectComplianceFramework:ProjectComplianceFramework": "ProjectComplianceFramework"
+  }
+ },
+ {
+  "pkg": "gitlab",
   "mod": "index/projectCustomAttribute",
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/projectCustomAttribute:ProjectCustomAttribute": "ProjectCustomAttribute"
   }
  },
  {
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/_inputs.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/_utilities.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/application.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/application_settings.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/application_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
         :param pulumi.Input[bool] hide_third_party_offers: Do not display offers from third parties in GitLab.
         :param pulumi.Input[str] home_page_url: Redirect to this URL when not logged in.
         :param pulumi.Input[bool] housekeeping_enabled: (If enabled, requires: housekeeping*bitmaps*enabled, housekeeping*full*repack*period, housekeeping*gc*period, and housekeeping*incremental*repack*period) Enable or disable Git housekeeping.
         :param pulumi.Input[int] housekeeping_full_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[int] housekeeping_gc_period: Number of Git pushes after which git gc is run.
         :param pulumi.Input[int] housekeeping_incremental_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[bool] html_emails_enabled: Enable HTML emails.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from. Valid values are: `github`, `bitbucket`, `bitbucket_server`, `fogbugz`, `git`, `Project`, `gitea`, `manifest`
         :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails.
         :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up.
         :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user.
         :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
@@ -2366,15 +2366,15 @@
     def html_emails_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "html_emails_enabled", value)
 
     @property
     @pulumi.getter(name="importSources")
     def import_sources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
+        Sources to allow project import from. Valid values are: `github`, `bitbucket`, `bitbucket_server`, `fogbugz`, `git`, `Project`, `gitea`, `manifest`
         """
         return pulumi.get(self, "import_sources")
 
     @import_sources.setter
     def import_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "import_sources", value)
 
@@ -4249,15 +4249,15 @@
         :param pulumi.Input[bool] hide_third_party_offers: Do not display offers from third parties in GitLab.
         :param pulumi.Input[str] home_page_url: Redirect to this URL when not logged in.
         :param pulumi.Input[bool] housekeeping_enabled: (If enabled, requires: housekeeping*bitmaps*enabled, housekeeping*full*repack*period, housekeeping*gc*period, and housekeeping*incremental*repack*period) Enable or disable Git housekeeping.
         :param pulumi.Input[int] housekeeping_full_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[int] housekeeping_gc_period: Number of Git pushes after which git gc is run.
         :param pulumi.Input[int] housekeeping_incremental_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[bool] html_emails_enabled: Enable HTML emails.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from. Valid values are: `github`, `bitbucket`, `bitbucket_server`, `fogbugz`, `git`, `Project`, `gitea`, `manifest`
         :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails.
         :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up.
         :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user.
         :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
@@ -6246,15 +6246,15 @@
     def html_emails_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "html_emails_enabled", value)
 
     @property
     @pulumi.getter(name="importSources")
     def import_sources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
+        Sources to allow project import from. Valid values are: `github`, `bitbucket`, `bitbucket_server`, `fogbugz`, `git`, `Project`, `gitea`, `manifest`
         """
         return pulumi.get(self, "import_sources")
 
     @import_sources.setter
     def import_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "import_sources", value)
 
@@ -8145,15 +8145,15 @@
         :param pulumi.Input[bool] hide_third_party_offers: Do not display offers from third parties in GitLab.
         :param pulumi.Input[str] home_page_url: Redirect to this URL when not logged in.
         :param pulumi.Input[bool] housekeeping_enabled: (If enabled, requires: housekeeping*bitmaps*enabled, housekeeping*full*repack*period, housekeeping*gc*period, and housekeeping*incremental*repack*period) Enable or disable Git housekeeping.
         :param pulumi.Input[int] housekeeping_full_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[int] housekeeping_gc_period: Number of Git pushes after which git gc is run.
         :param pulumi.Input[int] housekeeping_incremental_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[bool] html_emails_enabled: Enable HTML emails.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from. Valid values are: `github`, `bitbucket`, `bitbucket_server`, `fogbugz`, `git`, `Project`, `gitea`, `manifest`
         :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails.
         :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up.
         :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user.
         :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
@@ -9176,15 +9176,15 @@
         :param pulumi.Input[bool] hide_third_party_offers: Do not display offers from third parties in GitLab.
         :param pulumi.Input[str] home_page_url: Redirect to this URL when not logged in.
         :param pulumi.Input[bool] housekeeping_enabled: (If enabled, requires: housekeeping*bitmaps*enabled, housekeeping*full*repack*period, housekeeping*gc*period, and housekeeping*incremental*repack*period) Enable or disable Git housekeeping.
         :param pulumi.Input[int] housekeeping_full_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[int] housekeeping_gc_period: Number of Git pushes after which git gc is run.
         :param pulumi.Input[int] housekeeping_incremental_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[bool] html_emails_enabled: Enable HTML emails.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from. Valid values are: `github`, `bitbucket`, `bitbucket_server`, `fogbugz`, `git`, `Project`, `gitea`, `manifest`
         :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails.
         :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up.
         :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user.
         :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
@@ -10476,15 +10476,15 @@
         """
         return pulumi.get(self, "html_emails_enabled")
 
     @property
     @pulumi.getter(name="importSources")
     def import_sources(self) -> pulumi.Output[Sequence[str]]:
         """
-        Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
+        Sources to allow project import from. Valid values are: `github`, `bitbucket`, `bitbucket_server`, `fogbugz`, `git`, `Project`, `gitea`, `manifest`
         """
         return pulumi.get(self, "import_sources")
 
     @property
     @pulumi.getter(name="inProductMarketingEmailsEnabled")
     def in_product_marketing_emails_enabled(self) -> pulumi.Output[bool]:
         """
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/branch.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/branch_protection.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/branch_protection.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         :param pulumi.Input[bool] allow_force_push: Can be set to true to allow users with push access to force push.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToMergeArgs']]] allowed_to_merges: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToPushArgs']]] allowed_to_pushes: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToUnprotectArgs']]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`, `admin`.
         """
         pulumi.set(__self__, "branch", branch)
         pulumi.set(__self__, "project", project)
         if allow_force_push is not None:
             pulumi.set(__self__, "allow_force_push", allow_force_push)
         if allowed_to_merges is not None:
             pulumi.set(__self__, "allowed_to_merges", allowed_to_merges)
@@ -166,15 +166,15 @@
     def push_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "push_access_level", value)
 
     @property
     @pulumi.getter(name="unprotectAccessLevel")
     def unprotect_access_level(self) -> Optional[pulumi.Input[str]]:
         """
-        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`, `admin`.
         """
         return pulumi.get(self, "unprotect_access_level")
 
     @unprotect_access_level.setter
     def unprotect_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "unprotect_access_level", value)
 
@@ -201,15 +201,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToUnprotectArgs']]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[str] branch: Name of the branch.
         :param pulumi.Input[int] branch_protection_id: The ID of the branch protection (not the branch name).
         :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`, `admin`.
         """
         if allow_force_push is not None:
             pulumi.set(__self__, "allow_force_push", allow_force_push)
         if allowed_to_merges is not None:
             pulumi.set(__self__, "allowed_to_merges", allowed_to_merges)
         if allowed_to_pushes is not None:
             pulumi.set(__self__, "allowed_to_pushes", allowed_to_pushes)
@@ -350,15 +350,15 @@
     def push_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "push_access_level", value)
 
     @property
     @pulumi.getter(name="unprotectAccessLevel")
     def unprotect_access_level(self) -> Optional[pulumi.Input[str]]:
         """
-        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`, `admin`.
         """
         return pulumi.get(self, "unprotect_access_level")
 
     @unprotect_access_level.setter
     def unprotect_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "unprotect_access_level", value)
 
@@ -395,15 +395,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToPushArgs']]]] allowed_to_pushes: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToUnprotectArgs']]]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[str] branch: Name of the branch.
         :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`, `admin`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: BranchProtectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -499,15 +499,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToUnprotectArgs']]]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[str] branch: Name of the branch.
         :param pulumi.Input[int] branch_protection_id: The ID of the branch protection (not the branch name).
         :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`, `admin`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _BranchProtectionState.__new__(_BranchProtectionState)
 
         __props__.__dict__["allow_force_push"] = allow_force_push
         __props__.__dict__["allowed_to_merges"] = allowed_to_merges
@@ -602,11 +602,11 @@
         """
         return pulumi.get(self, "push_access_level")
 
     @property
     @pulumi.getter(name="unprotectAccessLevel")
     def unprotect_access_level(self) -> pulumi.Output[Optional[str]]:
         """
-        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`, `admin`.
         """
         return pulumi.get(self, "unprotect_access_level")
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/cluster_agent.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/cluster_agent_token.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/cluster_agent_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/config/vars.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/deploy_key.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/deploy_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/deploy_key_enable.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/deploy_key_enable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/deploy_token.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/deploy_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_application.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_branch.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_cluster_agent.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_cluster_agents.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_cluster_agents.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_current_user.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_current_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_hook.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_hooks.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_membership.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_subgroups.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_subgroups.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_variable.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_group_variables.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_group_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_groups.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_groups.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetGroupsResult:
     """
     A collection of values returned by getGroups.
     """
-    def __init__(__self__, groups=None, id=None, order_by=None, search=None, sort=None):
+    def __init__(__self__, groups=None, id=None, order_by=None, search=None, sort=None, top_level_only=None):
         if groups and not isinstance(groups, list):
             raise TypeError("Expected argument 'groups' to be a list")
         pulumi.set(__self__, "groups", groups)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if order_by and not isinstance(order_by, str):
@@ -34,14 +34,17 @@
         pulumi.set(__self__, "order_by", order_by)
         if search and not isinstance(search, str):
             raise TypeError("Expected argument 'search' to be a str")
         pulumi.set(__self__, "search", search)
         if sort and not isinstance(sort, str):
             raise TypeError("Expected argument 'sort' to be a str")
         pulumi.set(__self__, "sort", sort)
+        if top_level_only and not isinstance(top_level_only, bool):
+            raise TypeError("Expected argument 'top_level_only' to be a bool")
+        pulumi.set(__self__, "top_level_only", top_level_only)
 
     @property
     @pulumi.getter
     def groups(self) -> Sequence['outputs.GetGroupsGroupResult']:
         """
         The list of groups.
         """
@@ -75,31 +78,41 @@
     @pulumi.getter
     def sort(self) -> Optional[str]:
         """
         Sort groups' list in asc or desc order. (Requires administrator privileges)
         """
         return pulumi.get(self, "sort")
 
+    @property
+    @pulumi.getter(name="topLevelOnly")
+    def top_level_only(self) -> Optional[bool]:
+        """
+        Limit to top level groups, excluding all subgroups.
+        """
+        return pulumi.get(self, "top_level_only")
+
 
 class AwaitableGetGroupsResult(GetGroupsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetGroupsResult(
             groups=self.groups,
             id=self.id,
             order_by=self.order_by,
             search=self.search,
-            sort=self.sort)
+            sort=self.sort,
+            top_level_only=self.top_level_only)
 
 
 def get_groups(order_by: Optional[str] = None,
                search: Optional[str] = None,
                sort: Optional[str] = None,
+               top_level_only: Optional[bool] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupsResult:
     """
     The `get_groups` data source allows details of multiple groups to be retrieved given some optional filter criteria.
 
     > Some attributes might not be returned depending on if you're an admin or not.
 
     > Some available options require administrator privileges.
@@ -117,34 +130,38 @@
     example_two = gitlab.get_groups(search="GitLab")
     ```
 
 
     :param str order_by: Order the groups' list by `id`, `name`, `path`, or `similarity`. (Requires administrator privileges)
     :param str search: Search groups by name or path.
     :param str sort: Sort groups' list in asc or desc order. (Requires administrator privileges)
+    :param bool top_level_only: Limit to top level groups, excluding all subgroups.
     """
     __args__ = dict()
     __args__['orderBy'] = order_by
     __args__['search'] = search
     __args__['sort'] = sort
+    __args__['topLevelOnly'] = top_level_only
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroups:getGroups', __args__, opts=opts, typ=GetGroupsResult).value
 
     return AwaitableGetGroupsResult(
         groups=pulumi.get(__ret__, 'groups'),
         id=pulumi.get(__ret__, 'id'),
         order_by=pulumi.get(__ret__, 'order_by'),
         search=pulumi.get(__ret__, 'search'),
-        sort=pulumi.get(__ret__, 'sort'))
+        sort=pulumi.get(__ret__, 'sort'),
+        top_level_only=pulumi.get(__ret__, 'top_level_only'))
 
 
 @_utilities.lift_output_func(get_groups)
 def get_groups_output(order_by: Optional[pulumi.Input[Optional[str]]] = None,
                       search: Optional[pulumi.Input[Optional[str]]] = None,
                       sort: Optional[pulumi.Input[Optional[str]]] = None,
+                      top_level_only: Optional[pulumi.Input[Optional[bool]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupsResult]:
     """
     The `get_groups` data source allows details of multiple groups to be retrieved given some optional filter criteria.
 
     > Some attributes might not be returned depending on if you're an admin or not.
 
     > Some available options require administrator privileges.
@@ -162,9 +179,10 @@
     example_two = gitlab.get_groups(search="GitLab")
     ```
 
 
     :param str order_by: Order the groups' list by `id`, `name`, `path`, or `similarity`. (Requires administrator privileges)
     :param str search: Search groups by name or path.
     :param str sort: Sort groups' list in asc or desc order. (Requires administrator privileges)
+    :param bool top_level_only: Limit to top level groups, excluding all subgroups.
     """
     ...
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_instance_deploy_keys.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_instance_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_instance_variable.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_instance_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_instance_variables.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_instance_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_metadata.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_branches.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_hook.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_hooks.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_issue.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_issues.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_issues.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_membership.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_milestone.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_milestones.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_milestones.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_protected_branch.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_protected_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_protected_branches.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_protected_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_tag.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_tags.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_variable.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_project_variables.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_project_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_projects.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetProjectsResult:
     """
     A collection of values returned by getProjects.
     """
-    def __init__(__self__, archived=None, group_id=None, id=None, include_subgroups=None, max_queryable_pages=None, membership=None, min_access_level=None, order_by=None, owned=None, page=None, per_page=None, projects=None, search=None, simple=None, sort=None, starred=None, statistics=None, visibility=None, with_custom_attributes=None, with_issues_enabled=None, with_merge_requests_enabled=None, with_programming_language=None, with_shared=None):
+    def __init__(__self__, archived=None, group_id=None, id=None, include_subgroups=None, max_queryable_pages=None, membership=None, min_access_level=None, order_by=None, owned=None, page=None, per_page=None, projects=None, search=None, simple=None, sort=None, starred=None, statistics=None, topics=None, visibility=None, with_custom_attributes=None, with_issues_enabled=None, with_merge_requests_enabled=None, with_programming_language=None, with_shared=None):
         if archived and not isinstance(archived, bool):
             raise TypeError("Expected argument 'archived' to be a bool")
         pulumi.set(__self__, "archived", archived)
         if group_id and not isinstance(group_id, int):
             raise TypeError("Expected argument 'group_id' to be a int")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
@@ -70,14 +70,17 @@
         pulumi.set(__self__, "sort", sort)
         if starred and not isinstance(starred, bool):
             raise TypeError("Expected argument 'starred' to be a bool")
         pulumi.set(__self__, "starred", starred)
         if statistics and not isinstance(statistics, bool):
             raise TypeError("Expected argument 'statistics' to be a bool")
         pulumi.set(__self__, "statistics", statistics)
+        if topics and not isinstance(topics, list):
+            raise TypeError("Expected argument 'topics' to be a list")
+        pulumi.set(__self__, "topics", topics)
         if visibility and not isinstance(visibility, str):
             raise TypeError("Expected argument 'visibility' to be a str")
         pulumi.set(__self__, "visibility", visibility)
         if with_custom_attributes and not isinstance(with_custom_attributes, bool):
             raise TypeError("Expected argument 'with_custom_attributes' to be a bool")
         pulumi.set(__self__, "with_custom_attributes", with_custom_attributes)
         if with_issues_enabled and not isinstance(with_issues_enabled, bool):
@@ -227,14 +230,22 @@
         """
         Include project statistics. Cannot be used with `group_id`.
         """
         return pulumi.get(self, "statistics")
 
     @property
     @pulumi.getter
+    def topics(self) -> Optional[Sequence[str]]:
+        """
+        Limit by projects that have all of the given topics.
+        """
+        return pulumi.get(self, "topics")
+
+    @property
+    @pulumi.getter
     def visibility(self) -> Optional[str]:
         """
         Limit by visibility `public`, `internal`, or `private`.
         """
         return pulumi.get(self, "visibility")
 
     @property
@@ -297,14 +308,15 @@
             per_page=self.per_page,
             projects=self.projects,
             search=self.search,
             simple=self.simple,
             sort=self.sort,
             starred=self.starred,
             statistics=self.statistics,
+            topics=self.topics,
             visibility=self.visibility,
             with_custom_attributes=self.with_custom_attributes,
             with_issues_enabled=self.with_issues_enabled,
             with_merge_requests_enabled=self.with_merge_requests_enabled,
             with_programming_language=self.with_programming_language,
             with_shared=self.with_shared)
 
@@ -320,14 +332,15 @@
                  page: Optional[int] = None,
                  per_page: Optional[int] = None,
                  search: Optional[str] = None,
                  simple: Optional[bool] = None,
                  sort: Optional[str] = None,
                  starred: Optional[bool] = None,
                  statistics: Optional[bool] = None,
+                 topics: Optional[Sequence[str]] = None,
                  visibility: Optional[str] = None,
                  with_custom_attributes: Optional[bool] = None,
                  with_issues_enabled: Optional[bool] = None,
                  with_merge_requests_enabled: Optional[bool] = None,
                  with_programming_language: Optional[str] = None,
                  with_shared: Optional[bool] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectsResult:
@@ -367,14 +380,15 @@
     :param int page: The first page to begin the query on.
     :param int per_page: The number of results to return per page.
     :param str search: Return list of authorized projects matching the search criteria.
     :param bool simple: Return only the ID, URL, name, and path of each project.
     :param str sort: Return projects sorted in `asc` or `desc` order. Default is `desc`.
     :param bool starred: Limit by projects starred by the current user.
     :param bool statistics: Include project statistics. Cannot be used with `group_id`.
+    :param Sequence[str] topics: Limit by projects that have all of the given topics.
     :param str visibility: Limit by visibility `public`, `internal`, or `private`.
     :param bool with_custom_attributes: Include custom attributes in response *(admins only)*.
     :param bool with_issues_enabled: Limit by projects with issues feature enabled. Default is `false`.
     :param bool with_merge_requests_enabled: Limit by projects with merge requests feature enabled. Default is `false`.
     :param str with_programming_language: Limit by projects which use the given programming language. Cannot be used with `group_id`.
     :param bool with_shared: Include projects shared to this group. Default is `true`. Needs `group_id`.
     """
@@ -390,14 +404,15 @@
     __args__['page'] = page
     __args__['perPage'] = per_page
     __args__['search'] = search
     __args__['simple'] = simple
     __args__['sort'] = sort
     __args__['starred'] = starred
     __args__['statistics'] = statistics
+    __args__['topics'] = topics
     __args__['visibility'] = visibility
     __args__['withCustomAttributes'] = with_custom_attributes
     __args__['withIssuesEnabled'] = with_issues_enabled
     __args__['withMergeRequestsEnabled'] = with_merge_requests_enabled
     __args__['withProgrammingLanguage'] = with_programming_language
     __args__['withShared'] = with_shared
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -417,14 +432,15 @@
         per_page=pulumi.get(__ret__, 'per_page'),
         projects=pulumi.get(__ret__, 'projects'),
         search=pulumi.get(__ret__, 'search'),
         simple=pulumi.get(__ret__, 'simple'),
         sort=pulumi.get(__ret__, 'sort'),
         starred=pulumi.get(__ret__, 'starred'),
         statistics=pulumi.get(__ret__, 'statistics'),
+        topics=pulumi.get(__ret__, 'topics'),
         visibility=pulumi.get(__ret__, 'visibility'),
         with_custom_attributes=pulumi.get(__ret__, 'with_custom_attributes'),
         with_issues_enabled=pulumi.get(__ret__, 'with_issues_enabled'),
         with_merge_requests_enabled=pulumi.get(__ret__, 'with_merge_requests_enabled'),
         with_programming_language=pulumi.get(__ret__, 'with_programming_language'),
         with_shared=pulumi.get(__ret__, 'with_shared'))
 
@@ -441,14 +457,15 @@
                         page: Optional[pulumi.Input[Optional[int]]] = None,
                         per_page: Optional[pulumi.Input[Optional[int]]] = None,
                         search: Optional[pulumi.Input[Optional[str]]] = None,
                         simple: Optional[pulumi.Input[Optional[bool]]] = None,
                         sort: Optional[pulumi.Input[Optional[str]]] = None,
                         starred: Optional[pulumi.Input[Optional[bool]]] = None,
                         statistics: Optional[pulumi.Input[Optional[bool]]] = None,
+                        topics: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                         visibility: Optional[pulumi.Input[Optional[str]]] = None,
                         with_custom_attributes: Optional[pulumi.Input[Optional[bool]]] = None,
                         with_issues_enabled: Optional[pulumi.Input[Optional[bool]]] = None,
                         with_merge_requests_enabled: Optional[pulumi.Input[Optional[bool]]] = None,
                         with_programming_language: Optional[pulumi.Input[Optional[str]]] = None,
                         with_shared: Optional[pulumi.Input[Optional[bool]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectsResult]:
@@ -488,14 +505,15 @@
     :param int page: The first page to begin the query on.
     :param int per_page: The number of results to return per page.
     :param str search: Return list of authorized projects matching the search criteria.
     :param bool simple: Return only the ID, URL, name, and path of each project.
     :param str sort: Return projects sorted in `asc` or `desc` order. Default is `desc`.
     :param bool starred: Limit by projects starred by the current user.
     :param bool statistics: Include project statistics. Cannot be used with `group_id`.
+    :param Sequence[str] topics: Limit by projects that have all of the given topics.
     :param str visibility: Limit by visibility `public`, `internal`, or `private`.
     :param bool with_custom_attributes: Include custom attributes in response *(admins only)*.
     :param bool with_issues_enabled: Limit by projects with issues feature enabled. Default is `false`.
     :param bool with_merge_requests_enabled: Limit by projects with merge requests feature enabled. Default is `false`.
     :param str with_programming_language: Limit by projects which use the given programming language. Cannot be used with `group_id`.
     :param bool with_shared: Include projects shared to this group. Default is `true`. Needs `group_id`.
     """
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_release_link.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_release_links.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_release_links.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_repository_file.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_repository_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         """
         return pulumi.get(self, "commit_id")
 
     @property
     @pulumi.getter
     def content(self) -> str:
         """
-        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        File content.
         """
         return pulumi.get(self, "content")
 
     @property
     @pulumi.getter(name="contentSha256")
     def content_sha256(self) -> str:
         """
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_repository_tree.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_repository_tree.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_user.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_user_sshkeys.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_user_sshkeys.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/get_users.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_access_token.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_badge.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_badge.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,49 +5,41 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['GroupBadgeArgs', 'GroupBadge']
+__all__ = ['ProjectBadgeArgs', 'ProjectBadge']
 
 @pulumi.input_type
-class GroupBadgeArgs:
+class ProjectBadgeArgs:
     def __init__(__self__, *,
-                 group: pulumi.Input[str],
                  image_url: pulumi.Input[str],
-                 link_url: pulumi.Input[str]):
+                 link_url: pulumi.Input[str],
+                 project: pulumi.Input[str],
+                 name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a GroupBadge resource.
-        :param pulumi.Input[str] group: The id of the group to add the badge to.
-        :param pulumi.Input[str] image_url: The image url which will be presented on group overview.
+        The set of arguments for constructing a ProjectBadge resource.
+        :param pulumi.Input[str] image_url: The image url which will be presented on project overview.
         :param pulumi.Input[str] link_url: The url linked with the badge.
+        :param pulumi.Input[str] project: The id of the project to add the badge to.
+        :param pulumi.Input[str] name: The name of the badge.
         """
-        pulumi.set(__self__, "group", group)
         pulumi.set(__self__, "image_url", image_url)
         pulumi.set(__self__, "link_url", link_url)
-
-    @property
-    @pulumi.getter
-    def group(self) -> pulumi.Input[str]:
-        """
-        The id of the group to add the badge to.
-        """
-        return pulumi.get(self, "group")
-
-    @group.setter
-    def group(self, value: pulumi.Input[str]):
-        pulumi.set(self, "group", value)
+        pulumi.set(__self__, "project", project)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="imageUrl")
     def image_url(self) -> pulumi.Input[str]:
         """
-        The image url which will be presented on group overview.
+        The image url which will be presented on project overview.
         """
         return pulumi.get(self, "image_url")
 
     @image_url.setter
     def image_url(self, value: pulumi.Input[str]):
         pulumi.set(self, "image_url", value)
 
@@ -59,59 +51,75 @@
         """
         return pulumi.get(self, "link_url")
 
     @link_url.setter
     def link_url(self, value: pulumi.Input[str]):
         pulumi.set(self, "link_url", value)
 
+    @property
+    @pulumi.getter
+    def project(self) -> pulumi.Input[str]:
+        """
+        The id of the project to add the badge to.
+        """
+        return pulumi.get(self, "project")
+
+    @project.setter
+    def project(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The name of the badge.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
 
 @pulumi.input_type
-class _GroupBadgeState:
+class _ProjectBadgeState:
     def __init__(__self__, *,
-                 group: Optional[pulumi.Input[str]] = None,
                  image_url: Optional[pulumi.Input[str]] = None,
                  link_url: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  rendered_image_url: Optional[pulumi.Input[str]] = None,
                  rendered_link_url: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering GroupBadge resources.
-        :param pulumi.Input[str] group: The id of the group to add the badge to.
-        :param pulumi.Input[str] image_url: The image url which will be presented on group overview.
+        Input properties used for looking up and filtering ProjectBadge resources.
+        :param pulumi.Input[str] image_url: The image url which will be presented on project overview.
         :param pulumi.Input[str] link_url: The url linked with the badge.
+        :param pulumi.Input[str] name: The name of the badge.
+        :param pulumi.Input[str] project: The id of the project to add the badge to.
         :param pulumi.Input[str] rendered_image_url: The image_url argument rendered (in case of use of placeholders).
         :param pulumi.Input[str] rendered_link_url: The link_url argument rendered (in case of use of placeholders).
         """
-        if group is not None:
-            pulumi.set(__self__, "group", group)
         if image_url is not None:
             pulumi.set(__self__, "image_url", image_url)
         if link_url is not None:
             pulumi.set(__self__, "link_url", link_url)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if project is not None:
+            pulumi.set(__self__, "project", project)
         if rendered_image_url is not None:
             pulumi.set(__self__, "rendered_image_url", rendered_image_url)
         if rendered_link_url is not None:
             pulumi.set(__self__, "rendered_link_url", rendered_link_url)
 
     @property
-    @pulumi.getter
-    def group(self) -> Optional[pulumi.Input[str]]:
-        """
-        The id of the group to add the badge to.
-        """
-        return pulumi.get(self, "group")
-
-    @group.setter
-    def group(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "group", value)
-
-    @property
     @pulumi.getter(name="imageUrl")
     def image_url(self) -> Optional[pulumi.Input[str]]:
         """
-        The image url which will be presented on group overview.
+        The image url which will be presented on project overview.
         """
         return pulumi.get(self, "image_url")
 
     @image_url.setter
     def image_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image_url", value)
 
@@ -124,14 +132,38 @@
         return pulumi.get(self, "link_url")
 
     @link_url.setter
     def link_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "link_url", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The name of the badge.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def project(self) -> Optional[pulumi.Input[str]]:
+        """
+        The id of the project to add the badge to.
+        """
+        return pulumi.get(self, "project")
+
+    @project.setter
+    def project(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project", value)
+
+    @property
     @pulumi.getter(name="renderedImageUrl")
     def rendered_image_url(self) -> Optional[pulumi.Input[str]]:
         """
         The image_url argument rendered (in case of use of placeholders).
         """
         return pulumi.get(self, "rendered_image_url")
 
@@ -148,189 +180,234 @@
         return pulumi.get(self, "rendered_link_url")
 
     @rendered_link_url.setter
     def rendered_link_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rendered_link_url", value)
 
 
-class GroupBadge(pulumi.CustomResource):
+class ProjectBadge(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 group: Optional[pulumi.Input[str]] = None,
                  image_url: Optional[pulumi.Input[str]] = None,
                  link_url: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The `GroupBadge` resource allows to mange the lifecycle of group badges.
+        The `ProjectBadge` resource allows to manage the lifecycle of project badges.
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/user/project/badges.html#group-badges)
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/user/project/badges.html#project-badges)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        foo = gitlab.Group("foo")
-        example = gitlab.GroupBadge("example",
-            group=foo.id,
+        foo = gitlab.Project("foo")
+        example = gitlab.ProjectBadge("example",
+            project=foo.id,
             link_url="https://example.com/badge-123",
             image_url="https://example.com/badge-123.svg")
+        # Pipeline status badges with placeholders will be enabled
+        gitlab_pipeline = gitlab.ProjectBadge("gitlabPipeline",
+            project=foo.id,
+            link_url="https://gitlab.example.com/%{project_path}/-/pipelines?ref=%{default_branch}",
+            image_url="https://gitlab.example.com/%{project_path}/badges/%{default_branch}/pipeline.svg")
+        # Test coverage report badges with placeholders will be enabled
+        gitlab_coverage = gitlab.ProjectBadge("gitlabCoverage",
+            project=foo.id,
+            link_url="https://gitlab.example.com/%{project_path}/-/jobs",
+            image_url="https://gitlab.example.com/%{project_path}/badges/%{default_branch}/coverage.svg")
+        # Latest release badges with placeholders will be enabled
+        gitlab_release = gitlab.ProjectBadge("gitlabRelease",
+            project=foo.id,
+            link_url="https://gitlab.example.com/%{project_path}/-/releases",
+            image_url="https://gitlab.example.com/%{project_path}/-/badges/release.svg")
         ```
 
         ## Import
 
-        GitLab group badges can be imported using an id made up of `{group_id}:{badge_id}`, e.g.
+        GitLab project badges can be imported using an id made up of `{project_id}:{badge_id}`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/groupBadge:GroupBadge foo 1:3
+         $ pulumi import gitlab:index/projectBadge:ProjectBadge foo 1:3
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] group: The id of the group to add the badge to.
-        :param pulumi.Input[str] image_url: The image url which will be presented on group overview.
+        :param pulumi.Input[str] image_url: The image url which will be presented on project overview.
         :param pulumi.Input[str] link_url: The url linked with the badge.
+        :param pulumi.Input[str] name: The name of the badge.
+        :param pulumi.Input[str] project: The id of the project to add the badge to.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: GroupBadgeArgs,
+                 args: ProjectBadgeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `GroupBadge` resource allows to mange the lifecycle of group badges.
+        The `ProjectBadge` resource allows to manage the lifecycle of project badges.
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/user/project/badges.html#group-badges)
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/user/project/badges.html#project-badges)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        foo = gitlab.Group("foo")
-        example = gitlab.GroupBadge("example",
-            group=foo.id,
+        foo = gitlab.Project("foo")
+        example = gitlab.ProjectBadge("example",
+            project=foo.id,
             link_url="https://example.com/badge-123",
             image_url="https://example.com/badge-123.svg")
+        # Pipeline status badges with placeholders will be enabled
+        gitlab_pipeline = gitlab.ProjectBadge("gitlabPipeline",
+            project=foo.id,
+            link_url="https://gitlab.example.com/%{project_path}/-/pipelines?ref=%{default_branch}",
+            image_url="https://gitlab.example.com/%{project_path}/badges/%{default_branch}/pipeline.svg")
+        # Test coverage report badges with placeholders will be enabled
+        gitlab_coverage = gitlab.ProjectBadge("gitlabCoverage",
+            project=foo.id,
+            link_url="https://gitlab.example.com/%{project_path}/-/jobs",
+            image_url="https://gitlab.example.com/%{project_path}/badges/%{default_branch}/coverage.svg")
+        # Latest release badges with placeholders will be enabled
+        gitlab_release = gitlab.ProjectBadge("gitlabRelease",
+            project=foo.id,
+            link_url="https://gitlab.example.com/%{project_path}/-/releases",
+            image_url="https://gitlab.example.com/%{project_path}/-/badges/release.svg")
         ```
 
         ## Import
 
-        GitLab group badges can be imported using an id made up of `{group_id}:{badge_id}`, e.g.
+        GitLab project badges can be imported using an id made up of `{project_id}:{badge_id}`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/groupBadge:GroupBadge foo 1:3
+         $ pulumi import gitlab:index/projectBadge:ProjectBadge foo 1:3
         ```
 
         :param str resource_name: The name of the resource.
-        :param GroupBadgeArgs args: The arguments to use to populate this resource's properties.
+        :param ProjectBadgeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(GroupBadgeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProjectBadgeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 group: Optional[pulumi.Input[str]] = None,
                  image_url: Optional[pulumi.Input[str]] = None,
                  link_url: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = GroupBadgeArgs.__new__(GroupBadgeArgs)
+            __props__ = ProjectBadgeArgs.__new__(ProjectBadgeArgs)
 
-            if group is None and not opts.urn:
-                raise TypeError("Missing required property 'group'")
-            __props__.__dict__["group"] = group
             if image_url is None and not opts.urn:
                 raise TypeError("Missing required property 'image_url'")
             __props__.__dict__["image_url"] = image_url
             if link_url is None and not opts.urn:
                 raise TypeError("Missing required property 'link_url'")
             __props__.__dict__["link_url"] = link_url
+            __props__.__dict__["name"] = name
+            if project is None and not opts.urn:
+                raise TypeError("Missing required property 'project'")
+            __props__.__dict__["project"] = project
             __props__.__dict__["rendered_image_url"] = None
             __props__.__dict__["rendered_link_url"] = None
-        super(GroupBadge, __self__).__init__(
-            'gitlab:index/groupBadge:GroupBadge',
+        super(ProjectBadge, __self__).__init__(
+            'gitlab:index/projectBadge:ProjectBadge',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            group: Optional[pulumi.Input[str]] = None,
             image_url: Optional[pulumi.Input[str]] = None,
             link_url: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            project: Optional[pulumi.Input[str]] = None,
             rendered_image_url: Optional[pulumi.Input[str]] = None,
-            rendered_link_url: Optional[pulumi.Input[str]] = None) -> 'GroupBadge':
+            rendered_link_url: Optional[pulumi.Input[str]] = None) -> 'ProjectBadge':
         """
-        Get an existing GroupBadge resource's state with the given name, id, and optional extra
+        Get an existing ProjectBadge resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] group: The id of the group to add the badge to.
-        :param pulumi.Input[str] image_url: The image url which will be presented on group overview.
+        :param pulumi.Input[str] image_url: The image url which will be presented on project overview.
         :param pulumi.Input[str] link_url: The url linked with the badge.
+        :param pulumi.Input[str] name: The name of the badge.
+        :param pulumi.Input[str] project: The id of the project to add the badge to.
         :param pulumi.Input[str] rendered_image_url: The image_url argument rendered (in case of use of placeholders).
         :param pulumi.Input[str] rendered_link_url: The link_url argument rendered (in case of use of placeholders).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _GroupBadgeState.__new__(_GroupBadgeState)
+        __props__ = _ProjectBadgeState.__new__(_ProjectBadgeState)
 
-        __props__.__dict__["group"] = group
         __props__.__dict__["image_url"] = image_url
         __props__.__dict__["link_url"] = link_url
+        __props__.__dict__["name"] = name
+        __props__.__dict__["project"] = project
         __props__.__dict__["rendered_image_url"] = rendered_image_url
         __props__.__dict__["rendered_link_url"] = rendered_link_url
-        return GroupBadge(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter
-    def group(self) -> pulumi.Output[str]:
-        """
-        The id of the group to add the badge to.
-        """
-        return pulumi.get(self, "group")
+        return ProjectBadge(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="imageUrl")
     def image_url(self) -> pulumi.Output[str]:
         """
-        The image url which will be presented on group overview.
+        The image url which will be presented on project overview.
         """
         return pulumi.get(self, "image_url")
 
     @property
     @pulumi.getter(name="linkUrl")
     def link_url(self) -> pulumi.Output[str]:
         """
         The url linked with the badge.
         """
         return pulumi.get(self, "link_url")
 
     @property
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
+        """
+        The name of the badge.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def project(self) -> pulumi.Output[str]:
+        """
+        The id of the project to add the badge to.
+        """
+        return pulumi.get(self, "project")
+
+    @property
     @pulumi.getter(name="renderedImageUrl")
     def rendered_image_url(self) -> pulumi.Output[str]:
         """
         The image_url argument rendered (in case of use of placeholders).
         """
         return pulumi.get(self, "rendered_image_url")
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_cluster.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_custom_attribute.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_hook.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_label.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_ldap_link.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_ldap_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_membership.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_project_file_template.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_project_file_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_saml_link.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_saml_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_share_group.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/group_variable.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/group_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/instance_cluster.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/instance_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/instance_variable.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/instance_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_custom_issue_tracker.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_custom_issue_tracker.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_emails_on_push.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_emails_on_push.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_external_wiki.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_external_wiki.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_github.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_jira.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_jira.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_microsoft_teams.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_pipelines_email.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_pipelines_email.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/integration_slack.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/integration_slack.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/label.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/outputs.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/pages_domain.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/pages_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/personal_access_token.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/personal_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/pipeline_schedule.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/pipeline_schedule_variable.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/pipeline_schedule_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/pipeline_trigger.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/pipeline_trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_access_token.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_approval_rule.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_approval_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_badge.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_mirror.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,387 +5,417 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ProjectBadgeArgs', 'ProjectBadge']
+__all__ = ['ProjectMirrorArgs', 'ProjectMirror']
 
 @pulumi.input_type
-class ProjectBadgeArgs:
+class ProjectMirrorArgs:
     def __init__(__self__, *,
-                 image_url: pulumi.Input[str],
-                 link_url: pulumi.Input[str],
                  project: pulumi.Input[str],
-                 name: Optional[pulumi.Input[str]] = None):
+                 url: pulumi.Input[str],
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
+                 only_protected_branches: Optional[pulumi.Input[bool]] = None):
+        """
+        The set of arguments for constructing a ProjectMirror resource.
+        :param pulumi.Input[str] project: The id of the project.
+        :param pulumi.Input[str] url: The URL of the remote repository to be mirrored.
+        :param pulumi.Input[bool] enabled: Determines if the mirror is enabled.
+        :param pulumi.Input[bool] keep_divergent_refs: Determines if divergent refs are skipped.
+        :param pulumi.Input[bool] only_protected_branches: Determines if only protected branches are mirrored.
         """
-        The set of arguments for constructing a ProjectBadge resource.
-        :param pulumi.Input[str] image_url: The image url which will be presented on project overview.
-        :param pulumi.Input[str] link_url: The url linked with the badge.
-        :param pulumi.Input[str] project: The id of the project to add the badge to.
-        :param pulumi.Input[str] name: The name of the badge.
-        """
-        pulumi.set(__self__, "image_url", image_url)
-        pulumi.set(__self__, "link_url", link_url)
         pulumi.set(__self__, "project", project)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "url", url)
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if keep_divergent_refs is not None:
+            pulumi.set(__self__, "keep_divergent_refs", keep_divergent_refs)
+        if only_protected_branches is not None:
+            pulumi.set(__self__, "only_protected_branches", only_protected_branches)
 
     @property
-    @pulumi.getter(name="imageUrl")
-    def image_url(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def project(self) -> pulumi.Input[str]:
         """
-        The image url which will be presented on project overview.
+        The id of the project.
         """
-        return pulumi.get(self, "image_url")
+        return pulumi.get(self, "project")
 
-    @image_url.setter
-    def image_url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "image_url", value)
+    @project.setter
+    def project(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project", value)
 
     @property
-    @pulumi.getter(name="linkUrl")
-    def link_url(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def url(self) -> pulumi.Input[str]:
         """
-        The url linked with the badge.
+        The URL of the remote repository to be mirrored.
         """
-        return pulumi.get(self, "link_url")
+        return pulumi.get(self, "url")
 
-    @link_url.setter
-    def link_url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "link_url", value)
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
 
     @property
     @pulumi.getter
-    def project(self) -> pulumi.Input[str]:
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        The id of the project to add the badge to.
+        Determines if the mirror is enabled.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "enabled")
 
-    @project.setter
-    def project(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project", value)
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="keepDivergentRefs")
+    def keep_divergent_refs(self) -> Optional[pulumi.Input[bool]]:
         """
-        The name of the badge.
+        Determines if divergent refs are skipped.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "keep_divergent_refs")
+
+    @keep_divergent_refs.setter
+    def keep_divergent_refs(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "keep_divergent_refs", value)
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @property
+    @pulumi.getter(name="onlyProtectedBranches")
+    def only_protected_branches(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Determines if only protected branches are mirrored.
+        """
+        return pulumi.get(self, "only_protected_branches")
+
+    @only_protected_branches.setter
+    def only_protected_branches(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "only_protected_branches", value)
 
 
 @pulumi.input_type
-class _ProjectBadgeState:
+class _ProjectMirrorState:
     def __init__(__self__, *,
-                 image_url: Optional[pulumi.Input[str]] = None,
-                 link_url: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
+                 mirror_id: Optional[pulumi.Input[int]] = None,
+                 only_protected_branches: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
-                 rendered_image_url: Optional[pulumi.Input[str]] = None,
-                 rendered_link_url: Optional[pulumi.Input[str]] = None):
+                 url: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering ProjectBadge resources.
-        :param pulumi.Input[str] image_url: The image url which will be presented on project overview.
-        :param pulumi.Input[str] link_url: The url linked with the badge.
-        :param pulumi.Input[str] name: The name of the badge.
-        :param pulumi.Input[str] project: The id of the project to add the badge to.
-        :param pulumi.Input[str] rendered_image_url: The image_url argument rendered (in case of use of placeholders).
-        :param pulumi.Input[str] rendered_link_url: The link_url argument rendered (in case of use of placeholders).
-        """
-        if image_url is not None:
-            pulumi.set(__self__, "image_url", image_url)
-        if link_url is not None:
-            pulumi.set(__self__, "link_url", link_url)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
+        Input properties used for looking up and filtering ProjectMirror resources.
+        :param pulumi.Input[bool] enabled: Determines if the mirror is enabled.
+        :param pulumi.Input[bool] keep_divergent_refs: Determines if divergent refs are skipped.
+        :param pulumi.Input[int] mirror_id: Mirror ID.
+        :param pulumi.Input[bool] only_protected_branches: Determines if only protected branches are mirrored.
+        :param pulumi.Input[str] project: The id of the project.
+        :param pulumi.Input[str] url: The URL of the remote repository to be mirrored.
+        """
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if keep_divergent_refs is not None:
+            pulumi.set(__self__, "keep_divergent_refs", keep_divergent_refs)
+        if mirror_id is not None:
+            pulumi.set(__self__, "mirror_id", mirror_id)
+        if only_protected_branches is not None:
+            pulumi.set(__self__, "only_protected_branches", only_protected_branches)
         if project is not None:
             pulumi.set(__self__, "project", project)
-        if rendered_image_url is not None:
-            pulumi.set(__self__, "rendered_image_url", rendered_image_url)
-        if rendered_link_url is not None:
-            pulumi.set(__self__, "rendered_link_url", rendered_link_url)
+        if url is not None:
+            pulumi.set(__self__, "url", url)
 
     @property
-    @pulumi.getter(name="imageUrl")
-    def image_url(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        The image url which will be presented on project overview.
+        Determines if the mirror is enabled.
         """
-        return pulumi.get(self, "image_url")
+        return pulumi.get(self, "enabled")
 
-    @image_url.setter
-    def image_url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "image_url", value)
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
 
     @property
-    @pulumi.getter(name="linkUrl")
-    def link_url(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="keepDivergentRefs")
+    def keep_divergent_refs(self) -> Optional[pulumi.Input[bool]]:
         """
-        The url linked with the badge.
+        Determines if divergent refs are skipped.
         """
-        return pulumi.get(self, "link_url")
+        return pulumi.get(self, "keep_divergent_refs")
 
-    @link_url.setter
-    def link_url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "link_url", value)
+    @keep_divergent_refs.setter
+    def keep_divergent_refs(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "keep_divergent_refs", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="mirrorId")
+    def mirror_id(self) -> Optional[pulumi.Input[int]]:
         """
-        The name of the badge.
+        Mirror ID.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "mirror_id")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @mirror_id.setter
+    def mirror_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "mirror_id", value)
+
+    @property
+    @pulumi.getter(name="onlyProtectedBranches")
+    def only_protected_branches(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Determines if only protected branches are mirrored.
+        """
+        return pulumi.get(self, "only_protected_branches")
+
+    @only_protected_branches.setter
+    def only_protected_branches(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "only_protected_branches", value)
 
     @property
     @pulumi.getter
     def project(self) -> Optional[pulumi.Input[str]]:
         """
-        The id of the project to add the badge to.
+        The id of the project.
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project", value)
 
     @property
-    @pulumi.getter(name="renderedImageUrl")
-    def rendered_image_url(self) -> Optional[pulumi.Input[str]]:
-        """
-        The image_url argument rendered (in case of use of placeholders).
-        """
-        return pulumi.get(self, "rendered_image_url")
-
-    @rendered_image_url.setter
-    def rendered_image_url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "rendered_image_url", value)
-
-    @property
-    @pulumi.getter(name="renderedLinkUrl")
-    def rendered_link_url(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def url(self) -> Optional[pulumi.Input[str]]:
         """
-        The link_url argument rendered (in case of use of placeholders).
+        The URL of the remote repository to be mirrored.
         """
-        return pulumi.get(self, "rendered_link_url")
+        return pulumi.get(self, "url")
 
-    @rendered_link_url.setter
-    def rendered_link_url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "rendered_link_url", value)
+    @url.setter
+    def url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "url", value)
 
 
-class ProjectBadge(pulumi.CustomResource):
+class ProjectMirror(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 image_url: Optional[pulumi.Input[str]] = None,
-                 link_url: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
+                 only_protected_branches: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
+                 url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The `ProjectBadge` resource allows to mange the lifecycle of project badges.
+        The `ProjectMirror` resource allows to manage the lifecycle of a project mirror.
+
+        This is for *pushing* changes to a remote repository. *Pull Mirroring* can be configured using a combination of the
+        import_url, mirror, and mirror_trigger_builds properties on the Project resource.
+
+        > **Destroy Behavior** GitLab 14.10 introduced an API endpoint to delete a project mirror.
+           Therefore, for GitLab 14.10 and newer the project mirror will be destroyed when the resource is destroyed.
+           For older versions, the mirror will be disabled and the resource will be destroyed.
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/user/project/badges.html#project-badges)
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/remote_mirrors.html)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        foo = gitlab.Project("foo")
-        example = gitlab.ProjectBadge("example",
-            project=foo.id,
-            link_url="https://example.com/badge-123",
-            image_url="https://example.com/badge-123.svg")
+        foo = gitlab.ProjectMirror("foo",
+            project="1",
+            url="https://username:password@github.com/org/repository.git")
         ```
 
         ## Import
 
-        GitLab project badges can be imported using an id made up of `{project_id}:{badge_id}`, e.g.
+        GitLab project mirror can be imported using an id made up of `project_id:mirror_id`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/projectBadge:ProjectBadge foo 1:3
+         $ pulumi import gitlab:index/projectMirror:ProjectMirror foo "12345:1337"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] image_url: The image url which will be presented on project overview.
-        :param pulumi.Input[str] link_url: The url linked with the badge.
-        :param pulumi.Input[str] name: The name of the badge.
-        :param pulumi.Input[str] project: The id of the project to add the badge to.
+        :param pulumi.Input[bool] enabled: Determines if the mirror is enabled.
+        :param pulumi.Input[bool] keep_divergent_refs: Determines if divergent refs are skipped.
+        :param pulumi.Input[bool] only_protected_branches: Determines if only protected branches are mirrored.
+        :param pulumi.Input[str] project: The id of the project.
+        :param pulumi.Input[str] url: The URL of the remote repository to be mirrored.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProjectBadgeArgs,
+                 args: ProjectMirrorArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `ProjectBadge` resource allows to mange the lifecycle of project badges.
+        The `ProjectMirror` resource allows to manage the lifecycle of a project mirror.
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/user/project/badges.html#project-badges)
+        This is for *pushing* changes to a remote repository. *Pull Mirroring* can be configured using a combination of the
+        import_url, mirror, and mirror_trigger_builds properties on the Project resource.
+
+        > **Destroy Behavior** GitLab 14.10 introduced an API endpoint to delete a project mirror.
+           Therefore, for GitLab 14.10 and newer the project mirror will be destroyed when the resource is destroyed.
+           For older versions, the mirror will be disabled and the resource will be destroyed.
+
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/remote_mirrors.html)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        foo = gitlab.Project("foo")
-        example = gitlab.ProjectBadge("example",
-            project=foo.id,
-            link_url="https://example.com/badge-123",
-            image_url="https://example.com/badge-123.svg")
+        foo = gitlab.ProjectMirror("foo",
+            project="1",
+            url="https://username:password@github.com/org/repository.git")
         ```
 
         ## Import
 
-        GitLab project badges can be imported using an id made up of `{project_id}:{badge_id}`, e.g.
+        GitLab project mirror can be imported using an id made up of `project_id:mirror_id`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/projectBadge:ProjectBadge foo 1:3
+         $ pulumi import gitlab:index/projectMirror:ProjectMirror foo "12345:1337"
         ```
 
         :param str resource_name: The name of the resource.
-        :param ProjectBadgeArgs args: The arguments to use to populate this resource's properties.
+        :param ProjectMirrorArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ProjectBadgeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProjectMirrorArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 image_url: Optional[pulumi.Input[str]] = None,
-                 link_url: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
+                 only_protected_branches: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
+                 url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ProjectBadgeArgs.__new__(ProjectBadgeArgs)
+            __props__ = ProjectMirrorArgs.__new__(ProjectMirrorArgs)
 
-            if image_url is None and not opts.urn:
-                raise TypeError("Missing required property 'image_url'")
-            __props__.__dict__["image_url"] = image_url
-            if link_url is None and not opts.urn:
-                raise TypeError("Missing required property 'link_url'")
-            __props__.__dict__["link_url"] = link_url
-            __props__.__dict__["name"] = name
+            __props__.__dict__["enabled"] = enabled
+            __props__.__dict__["keep_divergent_refs"] = keep_divergent_refs
+            __props__.__dict__["only_protected_branches"] = only_protected_branches
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
-            __props__.__dict__["rendered_image_url"] = None
-            __props__.__dict__["rendered_link_url"] = None
-        super(ProjectBadge, __self__).__init__(
-            'gitlab:index/projectBadge:ProjectBadge',
+            if url is None and not opts.urn:
+                raise TypeError("Missing required property 'url'")
+            __props__.__dict__["url"] = None if url is None else pulumi.Output.secret(url)
+            __props__.__dict__["mirror_id"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["url"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+        super(ProjectMirror, __self__).__init__(
+            'gitlab:index/projectMirror:ProjectMirror',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            image_url: Optional[pulumi.Input[str]] = None,
-            link_url: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None,
+            enabled: Optional[pulumi.Input[bool]] = None,
+            keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
+            mirror_id: Optional[pulumi.Input[int]] = None,
+            only_protected_branches: Optional[pulumi.Input[bool]] = None,
             project: Optional[pulumi.Input[str]] = None,
-            rendered_image_url: Optional[pulumi.Input[str]] = None,
-            rendered_link_url: Optional[pulumi.Input[str]] = None) -> 'ProjectBadge':
+            url: Optional[pulumi.Input[str]] = None) -> 'ProjectMirror':
         """
-        Get an existing ProjectBadge resource's state with the given name, id, and optional extra
+        Get an existing ProjectMirror resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] image_url: The image url which will be presented on project overview.
-        :param pulumi.Input[str] link_url: The url linked with the badge.
-        :param pulumi.Input[str] name: The name of the badge.
-        :param pulumi.Input[str] project: The id of the project to add the badge to.
-        :param pulumi.Input[str] rendered_image_url: The image_url argument rendered (in case of use of placeholders).
-        :param pulumi.Input[str] rendered_link_url: The link_url argument rendered (in case of use of placeholders).
+        :param pulumi.Input[bool] enabled: Determines if the mirror is enabled.
+        :param pulumi.Input[bool] keep_divergent_refs: Determines if divergent refs are skipped.
+        :param pulumi.Input[int] mirror_id: Mirror ID.
+        :param pulumi.Input[bool] only_protected_branches: Determines if only protected branches are mirrored.
+        :param pulumi.Input[str] project: The id of the project.
+        :param pulumi.Input[str] url: The URL of the remote repository to be mirrored.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ProjectBadgeState.__new__(_ProjectBadgeState)
+        __props__ = _ProjectMirrorState.__new__(_ProjectMirrorState)
 
-        __props__.__dict__["image_url"] = image_url
-        __props__.__dict__["link_url"] = link_url
-        __props__.__dict__["name"] = name
+        __props__.__dict__["enabled"] = enabled
+        __props__.__dict__["keep_divergent_refs"] = keep_divergent_refs
+        __props__.__dict__["mirror_id"] = mirror_id
+        __props__.__dict__["only_protected_branches"] = only_protected_branches
         __props__.__dict__["project"] = project
-        __props__.__dict__["rendered_image_url"] = rendered_image_url
-        __props__.__dict__["rendered_link_url"] = rendered_link_url
-        return ProjectBadge(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["url"] = url
+        return ProjectMirror(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="imageUrl")
-    def image_url(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def enabled(self) -> pulumi.Output[Optional[bool]]:
         """
-        The image url which will be presented on project overview.
+        Determines if the mirror is enabled.
         """
-        return pulumi.get(self, "image_url")
+        return pulumi.get(self, "enabled")
 
     @property
-    @pulumi.getter(name="linkUrl")
-    def link_url(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="keepDivergentRefs")
+    def keep_divergent_refs(self) -> pulumi.Output[Optional[bool]]:
         """
-        The url linked with the badge.
+        Determines if divergent refs are skipped.
         """
-        return pulumi.get(self, "link_url")
+        return pulumi.get(self, "keep_divergent_refs")
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="mirrorId")
+    def mirror_id(self) -> pulumi.Output[int]:
         """
-        The name of the badge.
+        Mirror ID.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "mirror_id")
 
     @property
-    @pulumi.getter
-    def project(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="onlyProtectedBranches")
+    def only_protected_branches(self) -> pulumi.Output[Optional[bool]]:
         """
-        The id of the project to add the badge to.
+        Determines if only protected branches are mirrored.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "only_protected_branches")
 
     @property
-    @pulumi.getter(name="renderedImageUrl")
-    def rendered_image_url(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def project(self) -> pulumi.Output[str]:
         """
-        The image_url argument rendered (in case of use of placeholders).
+        The id of the project.
         """
-        return pulumi.get(self, "rendered_image_url")
+        return pulumi.get(self, "project")
 
     @property
-    @pulumi.getter(name="renderedLinkUrl")
-    def rendered_link_url(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def url(self) -> pulumi.Output[str]:
         """
-        The link_url argument rendered (in case of use of placeholders).
+        The URL of the remote repository to be mirrored.
         """
-        return pulumi.get(self, "rendered_link_url")
+        return pulumi.get(self, "url")
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_cluster.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_custom_attribute.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_environment.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_freeze_period.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_freeze_period.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_hook.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_issue.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_issue_board.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_issue_board.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_label.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_level_mr_approvals.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_level_mr_approvals.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_membership.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_milestone.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_mirror.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_tag.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,418 +4,453 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['ProjectMirrorArgs', 'ProjectMirror']
+__all__ = ['ProjectTagArgs', 'ProjectTag']
 
 @pulumi.input_type
-class ProjectMirrorArgs:
+class ProjectTagArgs:
     def __init__(__self__, *,
                  project: pulumi.Input[str],
-                 url: pulumi.Input[str],
-                 enabled: Optional[pulumi.Input[bool]] = None,
-                 keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
-                 only_protected_branches: Optional[pulumi.Input[bool]] = None):
-        """
-        The set of arguments for constructing a ProjectMirror resource.
-        :param pulumi.Input[str] project: The id of the project.
-        :param pulumi.Input[str] url: The URL of the remote repository to be mirrored.
-        :param pulumi.Input[bool] enabled: Determines if the mirror is enabled.
-        :param pulumi.Input[bool] keep_divergent_refs: Determines if divergent refs are skipped.
-        :param pulumi.Input[bool] only_protected_branches: Determines if only protected branches are mirrored.
+                 ref: pulumi.Input[str],
+                 message: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a ProjectTag resource.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
+        :param pulumi.Input[str] ref: Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
+        :param pulumi.Input[str] message: The message of the annotated tag.
+        :param pulumi.Input[str] name: The name of a tag.
         """
         pulumi.set(__self__, "project", project)
-        pulumi.set(__self__, "url", url)
-        if enabled is not None:
-            pulumi.set(__self__, "enabled", enabled)
-        if keep_divergent_refs is not None:
-            pulumi.set(__self__, "keep_divergent_refs", keep_divergent_refs)
-        if only_protected_branches is not None:
-            pulumi.set(__self__, "only_protected_branches", only_protected_branches)
+        pulumi.set(__self__, "ref", ref)
+        if message is not None:
+            pulumi.set(__self__, "message", message)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def project(self) -> pulumi.Input[str]:
         """
-        The id of the project.
+        The ID or URL-encoded path of the project owned by the authenticated user.
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
-    def url(self) -> pulumi.Input[str]:
+    def ref(self) -> pulumi.Input[str]:
         """
-        The URL of the remote repository to be mirrored.
+        Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
         """
-        return pulumi.get(self, "url")
+        return pulumi.get(self, "ref")
 
-    @url.setter
-    def url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "url", value)
+    @ref.setter
+    def ref(self, value: pulumi.Input[str]):
+        pulumi.set(self, "ref", value)
 
     @property
     @pulumi.getter
-    def enabled(self) -> Optional[pulumi.Input[bool]]:
+    def message(self) -> Optional[pulumi.Input[str]]:
         """
-        Determines if the mirror is enabled.
+        The message of the annotated tag.
         """
-        return pulumi.get(self, "enabled")
+        return pulumi.get(self, "message")
 
-    @enabled.setter
-    def enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enabled", value)
+    @message.setter
+    def message(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "message", value)
 
     @property
-    @pulumi.getter(name="keepDivergentRefs")
-    def keep_divergent_refs(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines if divergent refs are skipped.
-        """
-        return pulumi.get(self, "keep_divergent_refs")
-
-    @keep_divergent_refs.setter
-    def keep_divergent_refs(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "keep_divergent_refs", value)
-
-    @property
-    @pulumi.getter(name="onlyProtectedBranches")
-    def only_protected_branches(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Determines if only protected branches are mirrored.
+        The name of a tag.
         """
-        return pulumi.get(self, "only_protected_branches")
+        return pulumi.get(self, "name")
 
-    @only_protected_branches.setter
-    def only_protected_branches(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "only_protected_branches", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class _ProjectMirrorState:
+class _ProjectTagState:
     def __init__(__self__, *,
-                 enabled: Optional[pulumi.Input[bool]] = None,
-                 keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
-                 mirror_id: Optional[pulumi.Input[int]] = None,
-                 only_protected_branches: Optional[pulumi.Input[bool]] = None,
+                 commits: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagCommitArgs']]]] = None,
+                 message: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
-                 url: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering ProjectMirror resources.
-        :param pulumi.Input[bool] enabled: Determines if the mirror is enabled.
-        :param pulumi.Input[bool] keep_divergent_refs: Determines if divergent refs are skipped.
-        :param pulumi.Input[int] mirror_id: Mirror ID.
-        :param pulumi.Input[bool] only_protected_branches: Determines if only protected branches are mirrored.
-        :param pulumi.Input[str] project: The id of the project.
-        :param pulumi.Input[str] url: The URL of the remote repository to be mirrored.
-        """
-        if enabled is not None:
-            pulumi.set(__self__, "enabled", enabled)
-        if keep_divergent_refs is not None:
-            pulumi.set(__self__, "keep_divergent_refs", keep_divergent_refs)
-        if mirror_id is not None:
-            pulumi.set(__self__, "mirror_id", mirror_id)
-        if only_protected_branches is not None:
-            pulumi.set(__self__, "only_protected_branches", only_protected_branches)
+                 protected: Optional[pulumi.Input[bool]] = None,
+                 ref: Optional[pulumi.Input[str]] = None,
+                 releases: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagReleaseArgs']]]] = None,
+                 target: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering ProjectTag resources.
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectTagCommitArgs']]] commits: The commit associated with the tag.
+        :param pulumi.Input[str] message: The message of the annotated tag.
+        :param pulumi.Input[str] name: The name of a tag.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
+        :param pulumi.Input[bool] protected: Bool, true if tag has tag protection.
+        :param pulumi.Input[str] ref: Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectTagReleaseArgs']]] releases: The release associated with the tag.
+        :param pulumi.Input[str] target: The unique id assigned to the commit by Gitlab.
+        """
+        if commits is not None:
+            pulumi.set(__self__, "commits", commits)
+        if message is not None:
+            pulumi.set(__self__, "message", message)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if project is not None:
             pulumi.set(__self__, "project", project)
-        if url is not None:
-            pulumi.set(__self__, "url", url)
+        if protected is not None:
+            pulumi.set(__self__, "protected", protected)
+        if ref is not None:
+            pulumi.set(__self__, "ref", ref)
+        if releases is not None:
+            pulumi.set(__self__, "releases", releases)
+        if target is not None:
+            pulumi.set(__self__, "target", target)
 
     @property
     @pulumi.getter
-    def enabled(self) -> Optional[pulumi.Input[bool]]:
+    def commits(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagCommitArgs']]]]:
         """
-        Determines if the mirror is enabled.
+        The commit associated with the tag.
         """
-        return pulumi.get(self, "enabled")
+        return pulumi.get(self, "commits")
 
-    @enabled.setter
-    def enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "enabled", value)
+    @commits.setter
+    def commits(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagCommitArgs']]]]):
+        pulumi.set(self, "commits", value)
 
     @property
-    @pulumi.getter(name="keepDivergentRefs")
-    def keep_divergent_refs(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Determines if divergent refs are skipped.
-        """
-        return pulumi.get(self, "keep_divergent_refs")
-
-    @keep_divergent_refs.setter
-    def keep_divergent_refs(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "keep_divergent_refs", value)
-
-    @property
-    @pulumi.getter(name="mirrorId")
-    def mirror_id(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def message(self) -> Optional[pulumi.Input[str]]:
         """
-        Mirror ID.
+        The message of the annotated tag.
         """
-        return pulumi.get(self, "mirror_id")
+        return pulumi.get(self, "message")
 
-    @mirror_id.setter
-    def mirror_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "mirror_id", value)
+    @message.setter
+    def message(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "message", value)
 
     @property
-    @pulumi.getter(name="onlyProtectedBranches")
-    def only_protected_branches(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Determines if only protected branches are mirrored.
+        The name of a tag.
         """
-        return pulumi.get(self, "only_protected_branches")
+        return pulumi.get(self, "name")
 
-    @only_protected_branches.setter
-    def only_protected_branches(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "only_protected_branches", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def project(self) -> Optional[pulumi.Input[str]]:
         """
-        The id of the project.
+        The ID or URL-encoded path of the project owned by the authenticated user.
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
-    def url(self) -> Optional[pulumi.Input[str]]:
+    def protected(self) -> Optional[pulumi.Input[bool]]:
         """
-        The URL of the remote repository to be mirrored.
+        Bool, true if tag has tag protection.
         """
-        return pulumi.get(self, "url")
+        return pulumi.get(self, "protected")
 
-    @url.setter
-    def url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "url", value)
+    @protected.setter
+    def protected(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "protected", value)
 
+    @property
+    @pulumi.getter
+    def ref(self) -> Optional[pulumi.Input[str]]:
+        """
+        Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
+        """
+        return pulumi.get(self, "ref")
+
+    @ref.setter
+    def ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ref", value)
+
+    @property
+    @pulumi.getter
+    def releases(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagReleaseArgs']]]]:
+        """
+        The release associated with the tag.
+        """
+        return pulumi.get(self, "releases")
+
+    @releases.setter
+    def releases(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagReleaseArgs']]]]):
+        pulumi.set(self, "releases", value)
 
-class ProjectMirror(pulumi.CustomResource):
+    @property
+    @pulumi.getter
+    def target(self) -> Optional[pulumi.Input[str]]:
+        """
+        The unique id assigned to the commit by Gitlab.
+        """
+        return pulumi.get(self, "target")
+
+    @target.setter
+    def target(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "target", value)
+
+
+class ProjectTag(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 enabled: Optional[pulumi.Input[bool]] = None,
-                 keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
-                 only_protected_branches: Optional[pulumi.Input[bool]] = None,
+                 message: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
-                 url: Optional[pulumi.Input[str]] = None,
+                 ref: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The `ProjectMirror` resource allows to manage the lifecycle of a project mirror.
+        The `ProjectTag` resource allows to manage the lifecycle of a tag in a project.
 
-        This is for *pushing* changes to a remote repository. *Pull Mirroring* can be configured using a combination of the
-        import_url, mirror, and mirror_trigger_builds properties on the Project resource.
-
-        > **Destroy Behavior** GitLab 14.10 introduced an API endpoint to delete a project mirror.
-           Therefore, for GitLab 14.10 and newer the project mirror will be destroyed when the resource is destroyed.
-           For older versions, the mirror will be disabled and the resource will be destroyed.
-
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/remote_mirrors.html)
+        **Upstream API**: [GitLab API docs](https://docs.gitlab.com/ee/api/tags.html)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        foo = gitlab.ProjectMirror("foo",
-            project="1",
-            url="https://username:password@github.com/org/repository.git")
+        # Create a project for the tag to use
+        example_project = gitlab.Project("exampleProject",
+            description="An example project",
+            namespace_id=gitlab_group["example"]["id"])
+        example_project_tag = gitlab.ProjectTag("exampleProjectTag",
+            ref="main",
+            project=example_project.id)
         ```
 
         ## Import
 
-        GitLab project mirror can be imported using an id made up of `project_id:mirror_id`, e.g.
+        Gitlab project tags can be imported with a key composed of `<project_id>:<tag_name>`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/projectMirror:ProjectMirror foo "12345:1337"
+         $ pulumi import gitlab:index/projectTag:ProjectTag example "12345:develop"
         ```
 
+         NOTEthe `ref` attribute won't be available for imported `gitlab_project_tag` resources.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] enabled: Determines if the mirror is enabled.
-        :param pulumi.Input[bool] keep_divergent_refs: Determines if divergent refs are skipped.
-        :param pulumi.Input[bool] only_protected_branches: Determines if only protected branches are mirrored.
-        :param pulumi.Input[str] project: The id of the project.
-        :param pulumi.Input[str] url: The URL of the remote repository to be mirrored.
+        :param pulumi.Input[str] message: The message of the annotated tag.
+        :param pulumi.Input[str] name: The name of a tag.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
+        :param pulumi.Input[str] ref: Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProjectMirrorArgs,
+                 args: ProjectTagArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `ProjectMirror` resource allows to manage the lifecycle of a project mirror.
+        The `ProjectTag` resource allows to manage the lifecycle of a tag in a project.
 
-        This is for *pushing* changes to a remote repository. *Pull Mirroring* can be configured using a combination of the
-        import_url, mirror, and mirror_trigger_builds properties on the Project resource.
-
-        > **Destroy Behavior** GitLab 14.10 introduced an API endpoint to delete a project mirror.
-           Therefore, for GitLab 14.10 and newer the project mirror will be destroyed when the resource is destroyed.
-           For older versions, the mirror will be disabled and the resource will be destroyed.
-
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/remote_mirrors.html)
+        **Upstream API**: [GitLab API docs](https://docs.gitlab.com/ee/api/tags.html)
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
-        foo = gitlab.ProjectMirror("foo",
-            project="1",
-            url="https://username:password@github.com/org/repository.git")
+        # Create a project for the tag to use
+        example_project = gitlab.Project("exampleProject",
+            description="An example project",
+            namespace_id=gitlab_group["example"]["id"])
+        example_project_tag = gitlab.ProjectTag("exampleProjectTag",
+            ref="main",
+            project=example_project.id)
         ```
 
         ## Import
 
-        GitLab project mirror can be imported using an id made up of `project_id:mirror_id`, e.g.
+        Gitlab project tags can be imported with a key composed of `<project_id>:<tag_name>`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/projectMirror:ProjectMirror foo "12345:1337"
+         $ pulumi import gitlab:index/projectTag:ProjectTag example "12345:develop"
         ```
 
+         NOTEthe `ref` attribute won't be available for imported `gitlab_project_tag` resources.
+
         :param str resource_name: The name of the resource.
-        :param ProjectMirrorArgs args: The arguments to use to populate this resource's properties.
+        :param ProjectTagArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ProjectMirrorArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProjectTagArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 enabled: Optional[pulumi.Input[bool]] = None,
-                 keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
-                 only_protected_branches: Optional[pulumi.Input[bool]] = None,
+                 message: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
-                 url: Optional[pulumi.Input[str]] = None,
+                 ref: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ProjectMirrorArgs.__new__(ProjectMirrorArgs)
+            __props__ = ProjectTagArgs.__new__(ProjectTagArgs)
 
-            __props__.__dict__["enabled"] = enabled
-            __props__.__dict__["keep_divergent_refs"] = keep_divergent_refs
-            __props__.__dict__["only_protected_branches"] = only_protected_branches
+            __props__.__dict__["message"] = message
+            __props__.__dict__["name"] = name
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
-            if url is None and not opts.urn:
-                raise TypeError("Missing required property 'url'")
-            __props__.__dict__["url"] = None if url is None else pulumi.Output.secret(url)
-            __props__.__dict__["mirror_id"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["url"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(ProjectMirror, __self__).__init__(
-            'gitlab:index/projectMirror:ProjectMirror',
+            if ref is None and not opts.urn:
+                raise TypeError("Missing required property 'ref'")
+            __props__.__dict__["ref"] = ref
+            __props__.__dict__["commits"] = None
+            __props__.__dict__["protected"] = None
+            __props__.__dict__["releases"] = None
+            __props__.__dict__["target"] = None
+        super(ProjectTag, __self__).__init__(
+            'gitlab:index/projectTag:ProjectTag',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            enabled: Optional[pulumi.Input[bool]] = None,
-            keep_divergent_refs: Optional[pulumi.Input[bool]] = None,
-            mirror_id: Optional[pulumi.Input[int]] = None,
-            only_protected_branches: Optional[pulumi.Input[bool]] = None,
+            commits: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagCommitArgs']]]]] = None,
+            message: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
-            url: Optional[pulumi.Input[str]] = None) -> 'ProjectMirror':
+            protected: Optional[pulumi.Input[bool]] = None,
+            ref: Optional[pulumi.Input[str]] = None,
+            releases: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagReleaseArgs']]]]] = None,
+            target: Optional[pulumi.Input[str]] = None) -> 'ProjectTag':
         """
-        Get an existing ProjectMirror resource's state with the given name, id, and optional extra
+        Get an existing ProjectTag resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] enabled: Determines if the mirror is enabled.
-        :param pulumi.Input[bool] keep_divergent_refs: Determines if divergent refs are skipped.
-        :param pulumi.Input[int] mirror_id: Mirror ID.
-        :param pulumi.Input[bool] only_protected_branches: Determines if only protected branches are mirrored.
-        :param pulumi.Input[str] project: The id of the project.
-        :param pulumi.Input[str] url: The URL of the remote repository to be mirrored.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagCommitArgs']]]] commits: The commit associated with the tag.
+        :param pulumi.Input[str] message: The message of the annotated tag.
+        :param pulumi.Input[str] name: The name of a tag.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
+        :param pulumi.Input[bool] protected: Bool, true if tag has tag protection.
+        :param pulumi.Input[str] ref: Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagReleaseArgs']]]] releases: The release associated with the tag.
+        :param pulumi.Input[str] target: The unique id assigned to the commit by Gitlab.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ProjectMirrorState.__new__(_ProjectMirrorState)
+        __props__ = _ProjectTagState.__new__(_ProjectTagState)
 
-        __props__.__dict__["enabled"] = enabled
-        __props__.__dict__["keep_divergent_refs"] = keep_divergent_refs
-        __props__.__dict__["mirror_id"] = mirror_id
-        __props__.__dict__["only_protected_branches"] = only_protected_branches
+        __props__.__dict__["commits"] = commits
+        __props__.__dict__["message"] = message
+        __props__.__dict__["name"] = name
         __props__.__dict__["project"] = project
-        __props__.__dict__["url"] = url
-        return ProjectMirror(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["protected"] = protected
+        __props__.__dict__["ref"] = ref
+        __props__.__dict__["releases"] = releases
+        __props__.__dict__["target"] = target
+        return ProjectTag(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def enabled(self) -> pulumi.Output[Optional[bool]]:
+    def commits(self) -> pulumi.Output[Sequence['outputs.ProjectTagCommit']]:
         """
-        Determines if the mirror is enabled.
+        The commit associated with the tag.
         """
-        return pulumi.get(self, "enabled")
+        return pulumi.get(self, "commits")
 
     @property
-    @pulumi.getter(name="keepDivergentRefs")
-    def keep_divergent_refs(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def message(self) -> pulumi.Output[Optional[str]]:
         """
-        Determines if divergent refs are skipped.
+        The message of the annotated tag.
         """
-        return pulumi.get(self, "keep_divergent_refs")
+        return pulumi.get(self, "message")
 
     @property
-    @pulumi.getter(name="mirrorId")
-    def mirror_id(self) -> pulumi.Output[int]:
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
         """
-        Mirror ID.
+        The name of a tag.
         """
-        return pulumi.get(self, "mirror_id")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="onlyProtectedBranches")
-    def only_protected_branches(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def project(self) -> pulumi.Output[str]:
         """
-        Determines if only protected branches are mirrored.
+        The ID or URL-encoded path of the project owned by the authenticated user.
         """
-        return pulumi.get(self, "only_protected_branches")
+        return pulumi.get(self, "project")
 
     @property
     @pulumi.getter
-    def project(self) -> pulumi.Output[str]:
+    def protected(self) -> pulumi.Output[bool]:
         """
-        The id of the project.
+        Bool, true if tag has tag protection.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "protected")
+
+    @property
+    @pulumi.getter
+    def ref(self) -> pulumi.Output[str]:
+        """
+        Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
+        """
+        return pulumi.get(self, "ref")
+
+    @property
+    @pulumi.getter
+    def releases(self) -> pulumi.Output[Sequence['outputs.ProjectTagRelease']]:
+        """
+        The release associated with the tag.
+        """
+        return pulumi.get(self, "releases")
 
     @property
     @pulumi.getter
-    def url(self) -> pulumi.Output[str]:
+    def target(self) -> pulumi.Output[str]:
         """
-        The URL of the remote repository to be mirrored.
+        The unique id assigned to the commit by Gitlab.
         """
-        return pulumi.get(self, "url")
+        return pulumi.get(self, "target")
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_protected_environment.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_protected_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_runner_enablement.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_runner_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_share_group.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/project_variable.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/project_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/provider.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/release_link.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/repository_file.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/repository_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                  execute_filemode: Optional[pulumi.Input[bool]] = None,
                  overwrite_on_create: Optional[pulumi.Input[bool]] = None,
                  start_branch: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a RepositoryFile resource.
         :param pulumi.Input[str] branch: Name of the branch to which to commit to.
         :param pulumi.Input[str] commit_message: Commit message.
-        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        :param pulumi.Input[str] content: File content.
         :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
         :param pulumi.Input[str] project: The name or ID of the project.
         :param pulumi.Input[str] author_email: Email of the commit author.
         :param pulumi.Input[str] author_name: Name of the commit author.
         :param pulumi.Input[str] encoding: The file content encoding. Default value is `base64`. Valid values are: `base64`, `text`.
         :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
         :param pulumi.Input[bool] overwrite_on_create: Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
@@ -81,15 +81,15 @@
     def commit_message(self, value: pulumi.Input[str]):
         pulumi.set(self, "commit_message", value)
 
     @property
     @pulumi.getter
     def content(self) -> pulumi.Input[str]:
         """
-        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        File content.
         """
         return pulumi.get(self, "content")
 
     @content.setter
     def content(self, value: pulumi.Input[str]):
         pulumi.set(self, "content", value)
 
@@ -215,15 +215,15 @@
         Input properties used for looking up and filtering RepositoryFile resources.
         :param pulumi.Input[str] author_email: Email of the commit author.
         :param pulumi.Input[str] author_name: Name of the commit author.
         :param pulumi.Input[str] blob_id: The blob id.
         :param pulumi.Input[str] branch: Name of the branch to which to commit to.
         :param pulumi.Input[str] commit_id: The commit id.
         :param pulumi.Input[str] commit_message: Commit message.
-        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        :param pulumi.Input[str] content: File content.
         :param pulumi.Input[str] content_sha256: File content sha256 digest.
         :param pulumi.Input[str] encoding: The file content encoding. Default value is `base64`. Valid values are: `base64`, `text`.
         :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
         :param pulumi.Input[str] file_name: The filename.
         :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
         :param pulumi.Input[str] last_commit_id: The last known commit id.
         :param pulumi.Input[bool] overwrite_on_create: Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
@@ -341,15 +341,15 @@
     def commit_message(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "commit_message", value)
 
     @property
     @pulumi.getter
     def content(self) -> Optional[pulumi.Input[str]]:
         """
-        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        File content.
         """
         return pulumi.get(self, "content")
 
     @content.setter
     def content(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "content", value)
 
@@ -514,15 +514,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] author_email: Email of the commit author.
         :param pulumi.Input[str] author_name: Name of the commit author.
         :param pulumi.Input[str] branch: Name of the branch to which to commit to.
         :param pulumi.Input[str] commit_message: Commit message.
-        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        :param pulumi.Input[str] content: File content.
         :param pulumi.Input[str] encoding: The file content encoding. Default value is `base64`. Valid values are: `base64`, `text`.
         :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
         :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
         :param pulumi.Input[bool] overwrite_on_create: Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
         :param pulumi.Input[str] project: The name or ID of the project.
         :param pulumi.Input[str] start_branch: Name of the branch to start the new commit from.
         """
@@ -641,15 +641,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] author_email: Email of the commit author.
         :param pulumi.Input[str] author_name: Name of the commit author.
         :param pulumi.Input[str] blob_id: The blob id.
         :param pulumi.Input[str] branch: Name of the branch to which to commit to.
         :param pulumi.Input[str] commit_id: The commit id.
         :param pulumi.Input[str] commit_message: Commit message.
-        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        :param pulumi.Input[str] content: File content.
         :param pulumi.Input[str] content_sha256: File content sha256 digest.
         :param pulumi.Input[str] encoding: The file content encoding. Default value is `base64`. Valid values are: `base64`, `text`.
         :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
         :param pulumi.Input[str] file_name: The filename.
         :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
         :param pulumi.Input[str] last_commit_id: The last known commit id.
         :param pulumi.Input[bool] overwrite_on_create: Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
@@ -730,15 +730,15 @@
         """
         return pulumi.get(self, "commit_message")
 
     @property
     @pulumi.getter
     def content(self) -> pulumi.Output[str]:
         """
-        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        File content.
         """
         return pulumi.get(self, "content")
 
     @property
     @pulumi.getter(name="contentSha256")
     def content_sha256(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/runner.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_custom_issue_tracker.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_custom_issue_tracker.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_emails_on_push.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_emails_on_push.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_external_wiki.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_external_wiki.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_github.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_jira.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_jira.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_microsoft_teams.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_pipelines_email.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_pipelines_email.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/service_slack.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/service_slack.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/system_hook.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/system_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/tag_protection.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/tag_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/topic.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/user.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/user_custom_attribute.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/user_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/user_gpg_key.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/user_gpg_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab/user_ssh_key.py` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab.egg-info/PKG-INFO` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-gitlab
-Version: 6.2.0a1689690121
+Version: 6.2.0a1690301864
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/pulumi_gitlab.egg-info/SOURCES.txt` & `pulumi_gitlab-6.2.0a1690301864/pulumi_gitlab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 pulumi_gitlab/_utilities.py
 pulumi_gitlab/application.py
 pulumi_gitlab/application_settings.py
 pulumi_gitlab/branch.py
 pulumi_gitlab/branch_protection.py
 pulumi_gitlab/cluster_agent.py
 pulumi_gitlab/cluster_agent_token.py
+pulumi_gitlab/compliance_framework.py
 pulumi_gitlab/deploy_key.py
 pulumi_gitlab/deploy_key_enable.py
 pulumi_gitlab/deploy_token.py
 pulumi_gitlab/get_application.py
 pulumi_gitlab/get_branch.py
 pulumi_gitlab/get_cluster_agent.py
 pulumi_gitlab/get_cluster_agents.py
@@ -83,14 +84,15 @@
 pulumi_gitlab/pipeline_schedule_variable.py
 pulumi_gitlab/pipeline_trigger.py
 pulumi_gitlab/project.py
 pulumi_gitlab/project_access_token.py
 pulumi_gitlab/project_approval_rule.py
 pulumi_gitlab/project_badge.py
 pulumi_gitlab/project_cluster.py
+pulumi_gitlab/project_compliance_framework.py
 pulumi_gitlab/project_custom_attribute.py
 pulumi_gitlab/project_environment.py
 pulumi_gitlab/project_freeze_period.py
 pulumi_gitlab/project_hook.py
 pulumi_gitlab/project_issue.py
 pulumi_gitlab/project_issue_board.py
 pulumi_gitlab/project_label.py
```

### Comparing `pulumi_gitlab-6.2.0a1689690121/setup.py` & `pulumi_gitlab-6.2.0a1690301864/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.2.0a1689690121"
-PLUGIN_VERSION = "6.2.0-alpha.1689690121+7b7f7cf0"
+VERSION = "6.2.0a1690301864"
+PLUGIN_VERSION = "6.2.0-alpha.1690301864+a9613a6f"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'gitlab', PLUGIN_VERSION])
         except OSError as error:
```

