# Comparing `tmp/faradaysec-5.2.0.tar.gz` & `tmp/faradaysec-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faradaysec-5.2.0.tar", last modified: Thu Mar 14 18:17:34 2024, max compression
+gzip compressed data, was "faradaysec-5.2.1.tar", last modified: Wed Mar 20 20:45:10 2024, max compression
```

## Comparing `faradaysec-5.2.0.tar` & `faradaysec-5.2.1.tar`

### file list

```diff
@@ -1,377 +1,377 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.078438 faradaysec-5.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1261 2024-03-14 18:17:08.000000 faradaysec-5.2.0/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    32681 2024-03-14 18:17:08.000000 faradaysec-5.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      333 2024-03-14 18:17:08.000000 faradaysec-5.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7835 2024-03-14 18:17:34.078438 faradaysec-5.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6553 2024-03-14 18:17:08.000000 faradaysec-5.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.003440 faradaysec-5.2.0/faraday/
--rw-rw-rw-   0 root         (0) root         (0)      208 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/alembic.ini
--rwxrwxrwx   0 root         (0) root         (0)    12753 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.003440 faradaysec-5.2.0/faraday/migrations/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/README
--rw-rw-rw-   0 root         (0) root         (0)     2555 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/env.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.018439 faradaysec-5.2.0/faraday/migrations/versions/
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      650 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/0409e696eeec_workspace_important_flag_and_risk_.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/06c48492f587_reformat_jira_issue_fields_value.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/077b7c925ded_add_last_run_to_executors.py
--rw-rw-rw-   0 root         (0) root         (0)     5283 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/085188e0a016_create_rules_tables.py
--rw-rw-rw-   0 root         (0) root         (0)      534 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/08d02214aedc_add_advanced_filter_to_executive_report_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1922 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/0d216660da28_add_notification_table.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/0ed0dab44def_add_tags_arguments_for_agent_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/1145efa88414_add_warnings_to_command_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/1574fbcf72f5_disable_several_notifications_and_add_event_enabled_flag.py
--rw-rw-rw-   0 root         (0) root         (0)     3406 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/15d70093d262_severities_histogram_model.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/182832ed9733_add_socket_agent_sid.py
--rw-rw-rw-   0 root         (0) root         (0)     2735 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/18891ca61db6_add_cascade_delete_from_workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     2794 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/1b2533cc16fe_fix_custom_fields_display_name_was_used_.py
--rw-rw-rw-   0 root         (0) root         (0)     4346 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/1d328f7bf643_planner_model.py
--rw-rw-rw-   0 root         (0) root         (0)      838 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/1dbe9e8e4247_add_rule_execution_start_and_end_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/1e95dde5b9c8_cascade_on_kb.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/20f3d0c2f71f_alter_table_executive_report_add_.py
--rw-rw-rw-   0 root         (0) root         (0)     1553 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/247a90b029f2_fix_severities_ordering.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/257f6d0ad43f_add_fields_to_kb.py
--rw-rw-rw-   0 root         (0) root         (0)     2152 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/282ac9b6569f_add_agent_as_import_source_to_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/2a0de6132377_add_searchfilter_table.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/2ca03a8feef5_workspace_readonly.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/2db31733fb78_unique_field_name_in_customfield.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/33094e577642_add__tmp_id_for_on_conflict_inserts.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/384784872dc1_add_weight_column_in_role.py
--rw-rw-rw-   0 root         (0) root         (0)     7804 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/38bb251889e6_bulks.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/3eb96406e88d_rename_important_with_importance_and_remove_check_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/3f771124f0a2_add_metadata_to_cf_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/443a136bb5f2_severities_histogram_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/47e53ddc0308_add_cwe.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/4bb882a7f9b5_enable_notifications_for_v3.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/4d7a8fdd94e4_rename_not_active_users.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/51e533d41312_add_host_stats_static_columns.py
--rw-rw-rw-   0 root         (0) root         (0)     3706 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/526aa91cac98_vulnerability_merge_model.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/5272b3f5a820_add_markdown_column_to_exectuive_reports.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/5658775e113f_add_command_id_to_agent_execution.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/581121b181d8_add_owasp_model.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/59bed5515407_vuln_external_id.py
--rw-rw-rw-   0 root         (0) root         (0)     1910 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/5cf9660bba80_policyviolationvulnerabilityassociation_.py
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/5d7a930c439e_cve_many_to_many.py
--rw-rw-rw-   0 root         (0) root         (0)     7152 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/61ded0c8fbf6_notification_center.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/6471033046cb_added_delete_on_cascade_to_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/699402156cf4_update_risk_value.py
--rw-rw-rw-   0 root         (0) root         (0)     1896 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/73854f804a8d_cascade_kb_2.py
--rw-rw-rw-   0 root         (0) root         (0)     3030 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/7dea3a6caf51_cascade_in_vuls_relation.py
--rw-rw-rw-   0 root         (0) root         (0)      928 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/84f266a05be3_add_tool_column_to_vuln.py
--rw-rw-rw-   0 root         (0) root         (0)    13765 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/85aeb4185f98_refactor_cvss.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/877dd088c8cb_comment_ws_not_mandatory.py
--rw-rw-rw-   0 root         (0) root         (0)     4212 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/89115e133f0a_add_hosts_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/8a10ff3926a5_2fa_columns.py
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/901344f297fb_change_object_type_of_custom_logos_to_.py
--rw-rw-rw-   0 root         (0) root         (0)     3400 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/904a517a2f0c_create_executor_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/905261860ad0_user_types_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/97a9348d0406_add_fields_to_report.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/99a740945c44_add_index_into_vulnerability.py
--rw-rw-rw-   0 root         (0) root         (0)     2280 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/9c4091d1a09b_create_agent_table.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/9c678c44aa61_add_enabled_field_to_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/a39a3a6e3f99_create_user_preferences_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/a4def820a5bb_alter_otp_secret_length_in_user.py
--rw-rw-rw-   0 root         (0) root         (0)    15209 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/a9fcf8444c79_add_notification_event_and_subscription_.py
--rw-rw-rw-   0 root         (0) root         (0)     3297 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/aa56852fa76d_update_rule_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     8670 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/abb7ed8c56b4_add_workflow_models.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/b1d15a55556d_remove_ticketing_tools_credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     3532 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/b31fa447f00c_add_analytics_monthly_graphs_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/b49d8efbd0c2_add_configuration_table.py
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/b5065f401599_report_template_object_type.py
--rw-rw-rw-   0 root         (0) root         (0)     8514 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/b87b1de2f348_add_delete_workspace_missing_cascades.py
--rw-rw-rw-   0 root         (0) root         (0)     1883 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/be1f942eba28_add_analytics_saved_graphics_model.py
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/be89aa03e35e_add_severities_column_to_executive_.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/cb25cf42bda7_remove_knowledge_base_aka_pasta_base.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/d0a6105fdef1_modify_analytics_type_enum.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/d3afdb4e0b11_add_enum_to_comment_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4134 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/d8f0b32a5c0e_cvss_model.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/dd3181b9b3e9_severity_and_service_id_index_in_.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/e03a13c41a67_check_important_host.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/e61afb450465_add_custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2585 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/ed403da439d4_agents_with_multiple_workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f00247a92a14_add_agent_execution_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3494 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f0439bf6688a_updating_to_a_role_model_to_use_faraday_.py
--rw-rw-rw-   0 root         (0) root         (0)     2035 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f0a32e2753f6_new_one_to_one_reference_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f0a507afabd4_adding_fs_uniquifier_to_user_model.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f20aa8756612_change_executivereport_field_to_text.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f28eae25416b_fix_constraint_in_cve_association.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f6edb9a16479_add_type_to_reference_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4194 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f7ca45632cce_add_advanced_notifs_to_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2380 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f82a9136c408_remove_ws_from_agents_and_make_schedule_.py
--rw-rw-rw-   0 root         (0) root         (0)     2198 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/f8a44acd0e41_add_new_user_role.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/fa12b8322112_update_workflow_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/migrations/versions/fa73865dc11c_add_cvss3_scope_field.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.018439 faradaysec-5.2.0/faraday/openapi/
--rw-rw-rw-   0 root         (0) root         (0)   196938 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/openapi/faraday_swagger.json
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.021439 faradaysec-5.2.0/faraday/server/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.021439 faradaysec-5.2.0/faraday/server/api/
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    79248 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.026439 faradaysec-5.2.0/faraday/server/api/modules/
--rw-rw-rw-   0 root         (0) root         (0)      156 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4359 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/activity_feed.py
--rw-rw-rw-   0 root         (0) root         (0)    11433 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/agent_auth_token.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)    43506 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/bulk_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4911 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/commandsrun.py
--rw-rw-rw-   0 root         (0) root         (0)     3171 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/comments.py
--rw-rw-rw-   0 root         (0) root         (0)     5215 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     9913 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/export_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/get_exploits.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/global_commands.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)    19811 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/hosts.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/info.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/licenses.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/preferences.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/search_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     6174 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/services.py
--rw-rw-rw-   0 root         (0) root         (0)     1174 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/session.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      728 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/settings_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/settings_reports.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/swagger.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)     6583 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/upload_reports.py
--rw-rw-rw-   0 root         (0) root         (0)    14831 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/vulnerability_template.py
--rw-rw-rw-   0 root         (0) root         (0)    61729 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/vulns.py
--rw-rw-rw-   0 root         (0) root         (0)     3349 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/websocket_auth.py
--rw-rw-rw-   0 root         (0) root         (0)    23049 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/api/modules/workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)    28607 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/app.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/celery_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/celery_worker_gevent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.028439 faradaysec-5.2.0/faraday/server/commands/
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3139 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/app_urls.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/change_password.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/change_username.py
--rw-rw-rw-   0 root         (0) root         (0)     3449 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2975 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/faraday_schema_display.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/import_vulnerability_template.py
--rw-rw-rw-   0 root         (0) root         (0)    20708 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/initdb.py
--rw-rw-rw-   0 root         (0) root         (0)     4139 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/manage_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/move_references.py
--rw-rw-rw-   0 root         (0) root         (0)     1588 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/nginx_config.py
--rwxrwxrwx   0 root         (0) root         (0)     1235 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/reset_db.py
--rw-rw-rw-   0 root         (0) root         (0)     1233 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/sync_hosts_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.028439 faradaysec-5.2.0/faraday/server/commands/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1392 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/commands/templates/nginx_config.j2
--rw-rw-rw-   0 root         (0) root         (0)     5229 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/config.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/default.ini
--rw-rw-rw-   0 root         (0) root         (0)    15572 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/events.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/extensions.py
--rw-rw-rw-   0 root         (0) root         (0)     4615 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/gunicorn_app.py
--rw-rw-rw-   0 root         (0) root         (0)   133820 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/models.py
--rw-rw-rw-   0 root         (0) root         (0)    13586 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     7114 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.029439 faradaysec-5.2.0/faraday/server/threads/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/threads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.032439 faradaysec-5.2.0/faraday/server/utils/
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/agents.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/bulk_create.py
--rw-rw-rw-   0 root         (0) root         (0)     1064 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/command.py
--rw-rw-rw-   0 root         (0) root         (0)     2505 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/cvss.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/cwe.py
--rw-rw-rw-   0 root         (0) root         (0)     8853 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/daemonize.py
--rw-rw-rw-   0 root         (0) root         (0)    12231 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     8465 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/export.py
--rw-rw-rw-   0 root         (0) root         (0)    13160 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/invalid_chars.py
--rw-rw-rw-   0 root         (0) root         (0)     2673 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/ping.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     5769 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/reports_processor.py
--rw-rw-rw-   0 root         (0) root         (0)    34555 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/search.py
--rw-rw-rw-   0 root         (0) root         (0)    11697 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/vulns.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/utils/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.032439 faradaysec-5.2.0/faraday/server/websockets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/websockets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4381 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/websockets/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/websockets_worker.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/server/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.033439 faradaysec-5.2.0/faraday/server/www/
--rw-r--r--   0 root         (0) root         (0)    12005 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/asset-manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1150 2024-03-13 21:04:51.000000 faradaysec-5.2.0/faraday/server/www/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     1918 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/index.html
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-03-13 21:04:51.000000 faradaysec-5.2.0/faraday/server/www/manifest.json
--rw-r--r--   0 root         (0) root         (0)    15619 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/precache-manifest.d07621b882e4ff866b395d7787977d42.js
--rw-r--r--   0 root         (0) root         (0)     1181 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.001440 faradaysec-5.2.0/faraday/server/www/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.035439 faradaysec-5.2.0/faraday/server/www/static/css/
--rw-r--r--   0 root         (0) root         (0)   183537 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/css/2.b43efbd6.chunk.css
--rw-r--r--   0 root         (0) root         (0)   317573 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/css/2.b43efbd6.chunk.css.map
--rw-r--r--   0 root         (0) root         (0)   622877 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/css/main.3023afbd.chunk.css
--rw-r--r--   0 root         (0) root         (0)   507650 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/css/main.3023afbd.chunk.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.052439 faradaysec-5.2.0/faraday/server/www/static/js/
--rw-r--r--   0 root         (0) root         (0)  3063896 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/js/2.3d6f7f6b.chunk.js
--rw-r--r--   0 root         (0) root         (0)     5668 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/js/2.3d6f7f6b.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0) 17092343 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/js/2.3d6f7f6b.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)  1368432 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/js/main.afa469ce.chunk.js
--rw-r--r--   0 root         (0) root         (0)      149 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/js/main.afa469ce.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  2711933 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/js/main.afa469ce.chunk.js.map
--rw-r--r--   0 root         (0) root         (0)     1573 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/js/runtime-main.ea9693b3.js
--rw-r--r--   0 root         (0) root         (0)     8286 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/js/runtime-main.ea9693b3.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.075439 faradaysec-5.2.0/faraday/server/www/static/media/
--rw-r--r--   0 root         (0) root         (0)    79144 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/CentraNo2-Book.386f0594.otf
--rw-r--r--   0 root         (0) root         (0)    81720 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/CentraNo2-Medium.63911e85.otf
--rw-r--r--   0 root         (0) root         (0)     1117 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/Checkbox.b83098ac.svg
--rw-r--r--   0 root         (0) root         (0)      177 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/Checkbox_empty.195b4c92.svg
--rw-r--r--   0 root         (0) root         (0)     1263 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/Checkbox_ok.52c5a6cc.svg
--rw-r--r--   0 root         (0) root         (0)    76768 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_Bold.89985cf2.woff
--rw-r--r--   0 root         (0) root         (0)    82720 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_Book.b99ba59e.woff
--rw-r--r--   0 root         (0) root         (0)    78520 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_Medium.db87ffc9.woff
--rw-r--r--   0 root         (0) root         (0)    79728 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_Roman.db35328c.woff
--rw-r--r--   0 root         (0) root         (0)    77184 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_SemiBold.48873506.woff
--rw-r--r--   0 root         (0) root         (0)      713 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/activity-dashboard.b37176e7.svg
--rw-r--r--   0 root         (0) root         (0)     1569 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/agent_small.d1a2c9fe.svg
--rw-r--r--   0 root         (0) root         (0)      629 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/analytics.b5f3011a.svg
--rw-r--r--   0 root         (0) root         (0)     1313 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/api_link.dcbdf06d.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/arrow-down.d8661d88.svg
--rw-r--r--   0 root         (0) root         (0)      294 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/arrow-right.ec48cf40.svg
--rw-r--r--   0 root         (0) root         (0)     1123 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/assets.581bf13b.svg
--rw-r--r--   0 root         (0) root         (0)     1555 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/automation.a512d67b.svg
--rw-r--r--   0 root         (0) root         (0)     1150 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/clear.26371e5f.svg
--rw-r--r--   0 root         (0) root         (0)     1438 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/cog.6f2e860c.svg
--rw-r--r--   0 root         (0) root         (0)     3586 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/command.4ada7185.svg
--rw-r--r--   0 root         (0) root         (0)      387 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/copy.7e1b1006.svg
--rw-r--r--   0 root         (0) root         (0)      650 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/copy_link.852fb400.svg
--rw-r--r--   0 root         (0) root         (0)     2233 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/customAttributes.c7457305.svg
--rw-r--r--   0 root         (0) root         (0)      627 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/download-icon.eadbcf9c.svg
--rw-r--r--   0 root         (0) root         (0)      403 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/drag.b17c0ec9.svg
--rw-r--r--   0 root         (0) root         (0)    24438 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/empty-feed.3ebce7f3.png
--rw-r--r--   0 root         (0) root         (0)    18252 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/empty-vulns.1b2994f2.png
--rw-r--r--   0 root         (0) root         (0)      416 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/error-mark.364d0169.svg
--rw-r--r--   0 root         (0) root         (0)     1576 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/evidence-default.2dcc3b35.svg
--rw-r--r--   0 root         (0) root         (0)      215 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/exclamation_error.73360ffd.svg
--rw-r--r--   0 root         (0) root         (0)     1513 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/faraday-logo-nav.8385ead1.svg
--rw-r--r--   0 root         (0) root         (0)      241 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/faraday-logo.6f6c122b.svg
--rw-r--r--   0 root         (0) root         (0)    22547 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/faraday_loadingbar.13bdbd54.gif
--rw-r--r--   0 root         (0) root         (0)     5739 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/faraday_logo.3af44fcb.svg
--rw-r--r--   0 root         (0) root         (0)     4303 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/faraday_logo_product.57beba14.svg
--rw-r--r--   0 root         (0) root         (0)    29976 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_2fa.efd0850b.png
--rw-r--r--   0 root         (0) root         (0)    58320 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_analytics.b39bc4e5.png
--rw-r--r--   0 root         (0) root         (0)    80103 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_duplicates.46352b01.png
--rw-r--r--   0 root         (0) root         (0)    14262 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_ldap.e96f786d.png
--rw-r--r--   0 root         (0) root         (0)   137773 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_pipelines.165eec78.png
--rw-r--r--   0 root         (0) root         (0)    53910 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_planner.7afb07e6.png
--rw-r--r--   0 root         (0) root         (0)    87874 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_reporting.a9a7890d.png
--rw-r--r--   0 root         (0) root         (0)    67214 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_saml.119fe76f.png
--rw-r--r--   0 root         (0) root         (0)    63209 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_scheduler.b29ac5ec.png
--rw-r--r--   0 root         (0) root         (0)   171169 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_tags.ccc5427b.png
--rw-r--r--   0 root         (0) root         (0)   183858 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ff_users.ea35eac5.png
--rw-r--r--   0 root         (0) root         (0)     1454 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/generic_file.f9988671.svg
--rw-r--r--   0 root         (0) root         (0)      725 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/grid_view.580f3d12.svg
--rw-r--r--   0 root         (0) root         (0)      931 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/help-sysreq.5680b8ff.svg
--rw-r--r--   0 root         (0) root         (0)     1175 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/help.61ace590.svg
--rw-r--r--   0 root         (0) root         (0)     1027 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ico-web-shell.fc841a37.svg
--rw-r--r--   0 root         (0) root         (0)     1092 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-column.efe44a0e.svg
--rw-r--r--   0 root         (0) root         (0)      855 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-edit.a362c51d.svg
--rw-r--r--   0 root         (0) root         (0)      718 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-more.fd9db67e.svg
--rw-r--r--   0 root         (0) root         (0)      144 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-plus.8879f3f6.svg
--rw-r--r--   0 root         (0) root         (0)     1642 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-tags.c0f5d2b3.svg
--rw-r--r--   0 root         (0) root         (0)     1883 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-token.d7973c77.svg
--rw-r--r--   0 root         (0) root         (0)     1193 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-trash.b1589206.svg
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-trigger-disabled.af2d2680.svg
--rw-r--r--   0 root         (0) root         (0)      922 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-trigger.f9c88d81.svg
--rw-r--r--   0 root         (0) root         (0)      489 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-clipboard.c53f2936.svg
--rw-r--r--   0 root         (0) root         (0)      685 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-close-without-background.9b3b0c89.svg
--rw-r--r--   0 root         (0) root         (0)      744 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-close.9a5cad5c.svg
--rw-r--r--   0 root         (0) root         (0)      605 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-edit-enabled.a68d0409.svg
--rw-r--r--   0 root         (0) root         (0)      837 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-evidence.fdee90dd.svg
--rw-r--r--   0 root         (0) root         (0)      591 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-show-duplicates.79a1569d.svg
--rw-r--r--   0 root         (0) root         (0)      563 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-toolbar-confirmed-on.6c7a2996.svg
--rw-r--r--   0 root         (0) root         (0)     1037 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon-trash-red.1ebe0df4.svg
--rw-r--r--   0 root         (0) root         (0)      694 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_clearsearch.e7b18936.svg
--rw-r--r--   0 root         (0) root         (0)      717 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_close_error.459e6ef9.svg
--rw-r--r--   0 root         (0) root         (0)      956 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_drag.d52758c1.svg
--rw-r--r--   0 root         (0) root         (0)      870 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_edit.97c1ea04.svg
--rw-r--r--   0 root         (0) root         (0)      429 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_filter_off.c7a0db30.svg
--rw-r--r--   0 root         (0) root         (0)      568 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_filter_on.6de198fd.svg
--rw-r--r--   0 root         (0) root         (0)     1603 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_help.1b34b217.svg
--rw-r--r--   0 root         (0) root         (0)     1074 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_loupe.663ddfdd.svg
--rw-r--r--   0 root         (0) root         (0)      362 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_modal_asset.f360b291.svg
--rw-r--r--   0 root         (0) root         (0)      822 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_severity.b2244c26.svg
--rw-r--r--   0 root         (0) root         (0)      707 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_upload.cd99484a.svg
--rw-r--r--   0 root         (0) root         (0)     1754 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/icon_users.0781ec97.svg
--rw-r--r--   0 root         (0) root         (0)      969 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/laptop_icon.21863406.svg
--rw-r--r--   0 root         (0) root         (0)      493 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/laquo.d5f6e3f8.svg
--rw-r--r--   0 root         (0) root         (0)     1455 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/list_view.cacc94c7.svg
--rw-r--r--   0 root         (0) root         (0)      649 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/mini-terminal.f5a8e1d0.svg
--rw-r--r--   0 root         (0) root         (0)     1374 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/moveVuln.ba569948.svg
--rw-r--r--   0 root         (0) root         (0)     3222 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/new_vuln_modal_icon.033159cd.svg
--rw-r--r--   0 root         (0) root         (0)      393 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/next.0e62ddad.svg
--rw-r--r--   0 root         (0) root         (0)      283 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/next_arrow.407b029f.svg
--rw-r--r--   0 root         (0) root         (0)      837 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/noun-help.a93b0458.svg
--rw-r--r--   0 root         (0) root         (0)     1210 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/preferences_icons_Account.e0a4aa09.svg
--rw-r--r--   0 root         (0) root         (0)      757 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/preferences_icons_Authentication.1b59fc92.svg
--rw-r--r--   0 root         (0) root         (0)      390 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/prev.ecd34f23.svg
--rw-r--r--   0 root         (0) root         (0)      352 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/queue.b922c0be.svg
--rw-r--r--   0 root         (0) root         (0)      851 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/reload.0d7f0f5c.svg
--rw-r--r--   0 root         (0) root         (0)     1260 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/report_small.e8a3d444.svg
--rw-r--r--   0 root         (0) root         (0)     1195 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/reports.f38dca7f.svg
--rw-r--r--   0 root         (0) root         (0)      327 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/resize_bottom_right.eced93cf.svg
--rw-r--r--   0 root         (0) root         (0)     1483 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/save_template.d74f944a.svg
--rw-r--r--   0 root         (0) root         (0)     3621 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/services.0f83c980.svg
--rw-r--r--   0 root         (0) root         (0)      399 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/shape.9ea9d3d6.svg
--rw-r--r--   0 root         (0) root         (0)      482 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/sort.062a68ce.svg
--rw-r--r--   0 root         (0) root         (0)      836 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/star.33d47a05.svg
--rw-r--r--   0 root         (0) root         (0)      674 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/status.660ac4e6.svg
--rw-r--r--   0 root         (0) root         (0)     1126 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tasks_icon.ba912fa5.svg
--rw-r--r--   0 root         (0) root         (0)      842 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/template.bc90870d.svg
--rw-r--r--   0 root         (0) root         (0)   164554 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_appscan.9b037d8b.png
--rw-r--r--   0 root         (0) root         (0)    16275 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_arachni.ac5b15cb.png
--rw-r--r--   0 root         (0) root         (0)    34524 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_insightVM.f0295560.png
--rw-r--r--   0 root         (0) root         (0)    11697 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_nessus.8ed3098d.png
--rw-r--r--   0 root         (0) root         (0)    18860 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_nikto.9acc1459.png
--rw-r--r--   0 root         (0) root         (0)    21908 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_nmap.9a81da35.png
--rw-r--r--   0 root         (0) root         (0)    19674 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_openvas.88898507.png
--rw-r--r--   0 root         (0) root         (0)    38433 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_qualys.8f7b2a7f.png
--rw-r--r--   0 root         (0) root         (0)    14816 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_sonarQube.3af1625a.jpeg
--rw-r--r--   0 root         (0) root         (0)    22535 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_tenable.05c390dc.png
--rw-r--r--   0 root         (0) root         (0)    19425 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_w3af.221ef0f2.png
--rw-r--r--   0 root         (0) root         (0)    14366 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_wpscan.92adc6c5.png
--rw-r--r--   0 root         (0) root         (0)   185420 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_zap.62021c39.png
--rw-r--r--   0 root         (0) root         (0)     1490 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_trash.e6d04612.svg
--rw-r--r--   0 root         (0) root         (0)     2256 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/tool_wheel.1b4bc890.svg
--rw-r--r--   0 root         (0) root         (0)     1501 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/unknown_filetype.f6b0014d.svg
--rw-r--r--   0 root         (0) root         (0)     1670 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/vulnerabilities.bc957e73.svg
--rw-r--r--   0 root         (0) root         (0)     2873 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/warning-delete.33357364.svg
--rw-r--r--   0 root         (0) root         (0)      813 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/wf_arrow_collapsed.51829f9b.svg
--rw-r--r--   0 root         (0) root         (0)      905 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/wf_arrow_expand.06e6e9bd.svg
--rw-r--r--   0 root         (0) root         (0)     1261 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ws-lock.5d1e24be.svg
--rw-r--r--   0 root         (0) root         (0)     1233 2024-03-13 21:09:48.000000 faradaysec-5.2.0/faraday/server/www/static/media/ws-unlock.b7653513.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.076439 faradaysec-5.2.0/faraday/settings/
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3457 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/settings/base.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/settings/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/settings/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/settings/reports.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/settings/smtp.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/start_all.py
--rw-rw-rw-   0 root         (0) root         (0)     8175 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/start_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.077438 faradaysec-5.2.0/faraday/utils/
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1205 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/utils/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5964 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/utils/faraday_openapi_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2024-03-14 18:17:08.000000 faradaysec-5.2.0/faraday/utils/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 18:17:34.078438 faradaysec-5.2.0/faradaysec.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7835 2024-03-14 18:17:33.000000 faradaysec-5.2.0/faradaysec.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18864 2024-03-14 18:17:33.000000 faradaysec-5.2.0/faradaysec.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 18:17:33.000000 faradaysec-5.2.0/faradaysec.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      256 2024-03-14 18:17:33.000000 faradaysec-5.2.0/faradaysec.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1101 2024-03-14 18:17:33.000000 faradaysec-5.2.0/faradaysec.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-14 18:17:33.000000 faradaysec-5.2.0/faradaysec.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-14 18:17:08.000000 faradaysec-5.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      192 2024-03-14 18:17:08.000000 faradaysec-5.2.0/requirements_dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      294 2024-03-14 18:17:34.079439 faradaysec-5.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    10659 2024-03-14 18:17:08.000000 faradaysec-5.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:10.043897 faradaysec-5.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2024-03-20 20:44:43.000000 faradaysec-5.2.1/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    32681 2024-03-20 20:44:43.000000 faradaysec-5.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      333 2024-03-20 20:44:43.000000 faradaysec-5.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7835 2024-03-20 20:45:10.043897 faradaysec-5.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6553 2024-03-20 20:44:43.000000 faradaysec-5.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.955897 faradaysec-5.2.1/faraday/
+-rw-rw-rw-   0 root         (0) root         (0)      208 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/alembic.ini
+-rwxrwxrwx   0 root         (0) root         (0)    12753 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.955897 faradaysec-5.2.1/faraday/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/README
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.972897 faradaysec-5.2.1/faraday/migrations/versions/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      650 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/0409e696eeec_workspace_important_flag_and_risk_.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/06c48492f587_reformat_jira_issue_fields_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/077b7c925ded_add_last_run_to_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5283 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/085188e0a016_create_rules_tables.py
+-rw-rw-rw-   0 root         (0) root         (0)      534 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/08d02214aedc_add_advanced_filter_to_executive_report_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/0d216660da28_add_notification_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/0ed0dab44def_add_tags_arguments_for_agent_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/1145efa88414_add_warnings_to_command_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/1574fbcf72f5_disable_several_notifications_and_add_event_enabled_flag.py
+-rw-rw-rw-   0 root         (0) root         (0)     3406 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/15d70093d262_severities_histogram_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/182832ed9733_add_socket_agent_sid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/18891ca61db6_add_cascade_delete_from_workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2794 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/1b2533cc16fe_fix_custom_fields_display_name_was_used_.py
+-rw-rw-rw-   0 root         (0) root         (0)     4346 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/1d328f7bf643_planner_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      838 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/1dbe9e8e4247_add_rule_execution_start_and_end_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/1e95dde5b9c8_cascade_on_kb.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/20f3d0c2f71f_alter_table_executive_report_add_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1553 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/247a90b029f2_fix_severities_ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/257f6d0ad43f_add_fields_to_kb.py
+-rw-rw-rw-   0 root         (0) root         (0)     2152 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/282ac9b6569f_add_agent_as_import_source_to_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/2a0de6132377_add_searchfilter_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/2ca03a8feef5_workspace_readonly.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/2db31733fb78_unique_field_name_in_customfield.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/33094e577642_add__tmp_id_for_on_conflict_inserts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/384784872dc1_add_weight_column_in_role.py
+-rw-rw-rw-   0 root         (0) root         (0)     7804 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/38bb251889e6_bulks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/3eb96406e88d_rename_important_with_importance_and_remove_check_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/3f771124f0a2_add_metadata_to_cf_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/443a136bb5f2_severities_histogram_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/47e53ddc0308_add_cwe.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/4bb882a7f9b5_enable_notifications_for_v3.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/4d7a8fdd94e4_rename_not_active_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/51e533d41312_add_host_stats_static_columns.py
+-rw-rw-rw-   0 root         (0) root         (0)     3706 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/526aa91cac98_vulnerability_merge_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/5272b3f5a820_add_markdown_column_to_exectuive_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/5658775e113f_add_command_id_to_agent_execution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/581121b181d8_add_owasp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/59bed5515407_vuln_external_id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/5cf9660bba80_policyviolationvulnerabilityassociation_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/5d7a930c439e_cve_many_to_many.py
+-rw-rw-rw-   0 root         (0) root         (0)     7152 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/61ded0c8fbf6_notification_center.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/6471033046cb_added_delete_on_cascade_to_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/699402156cf4_update_risk_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/73854f804a8d_cascade_kb_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/7dea3a6caf51_cascade_in_vuls_relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/84f266a05be3_add_tool_column_to_vuln.py
+-rw-rw-rw-   0 root         (0) root         (0)    13765 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/85aeb4185f98_refactor_cvss.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/877dd088c8cb_comment_ws_not_mandatory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4212 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/89115e133f0a_add_hosts_notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/8a10ff3926a5_2fa_columns.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/901344f297fb_change_object_type_of_custom_logos_to_.py
+-rw-rw-rw-   0 root         (0) root         (0)     3400 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/904a517a2f0c_create_executor_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/905261860ad0_user_types_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/97a9348d0406_add_fields_to_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/99a740945c44_add_index_into_vulnerability.py
+-rw-rw-rw-   0 root         (0) root         (0)     2280 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/9c4091d1a09b_create_agent_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/9c678c44aa61_add_enabled_field_to_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/a39a3a6e3f99_create_user_preferences_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/a4def820a5bb_alter_otp_secret_length_in_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    15209 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/a9fcf8444c79_add_notification_event_and_subscription_.py
+-rw-rw-rw-   0 root         (0) root         (0)     3297 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/aa56852fa76d_update_rule_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/abb7ed8c56b4_add_workflow_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/b1d15a55556d_remove_ticketing_tools_credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)     3532 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/b31fa447f00c_add_analytics_monthly_graphs_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/b49d8efbd0c2_add_configuration_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/b5065f401599_report_template_object_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     8514 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/b87b1de2f348_add_delete_workspace_missing_cascades.py
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/be1f942eba28_add_analytics_saved_graphics_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/be89aa03e35e_add_severities_column_to_executive_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/cb25cf42bda7_remove_knowledge_base_aka_pasta_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/d0a6105fdef1_modify_analytics_type_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/d3afdb4e0b11_add_enum_to_comment_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4134 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/d8f0b32a5c0e_cvss_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/dd3181b9b3e9_severity_and_service_id_index_in_.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/e03a13c41a67_check_important_host.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/e61afb450465_add_custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2585 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/ed403da439d4_agents_with_multiple_workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f00247a92a14_add_agent_execution_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f0439bf6688a_updating_to_a_role_model_to_use_faraday_.py
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f0a32e2753f6_new_one_to_one_reference_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f0a507afabd4_adding_fs_uniquifier_to_user_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      746 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f20aa8756612_change_executivereport_field_to_text.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f28eae25416b_fix_constraint_in_cve_association.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f6edb9a16479_add_type_to_reference_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4194 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f7ca45632cce_add_advanced_notifs_to_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2380 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f82a9136c408_remove_ws_from_agents_and_make_schedule_.py
+-rw-rw-rw-   0 root         (0) root         (0)     2198 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/f8a44acd0e41_add_new_user_role.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/fa12b8322112_update_workflow_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/migrations/versions/fa73865dc11c_add_cvss3_scope_field.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.973897 faradaysec-5.2.1/faraday/openapi/
+-rw-rw-rw-   0 root         (0) root         (0)   196938 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/openapi/faraday_swagger.json
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.977897 faradaysec-5.2.1/faraday/server/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.977897 faradaysec-5.2.1/faraday/server/api/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    79248 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.985897 faradaysec-5.2.1/faraday/server/api/modules/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4359 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/activity_feed.py
+-rw-rw-rw-   0 root         (0) root         (0)    11433 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/agent_auth_token.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)    43506 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/bulk_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/commandsrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     3171 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/comments.py
+-rw-rw-rw-   0 root         (0) root         (0)     5215 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     9913 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/export_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/get_exploits.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/global_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)    19811 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/hosts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/licenses.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/preferences.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/search_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      728 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/settings_dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/settings_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/swagger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     6583 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/upload_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)    14831 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/vulnerability_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    61729 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/vulns.py
+-rw-rw-rw-   0 root         (0) root         (0)     3349 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/websocket_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    23049 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/api/modules/workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    28607 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/app.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/celery_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/celery_worker_gevent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.988897 faradaysec-5.2.1/faraday/server/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3139 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/app_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/change_password.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/change_username.py
+-rw-rw-rw-   0 root         (0) root         (0)     3449 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2975 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/faraday_schema_display.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/import_vulnerability_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    20708 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/initdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     4139 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/manage_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/move_references.py
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/nginx_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     1235 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/reset_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/sync_hosts_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.988897 faradaysec-5.2.1/faraday/server/commands/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1392 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/commands/templates/nginx_config.j2
+-rw-rw-rw-   0 root         (0) root         (0)     5229 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/default.ini
+-rw-rw-rw-   0 root         (0) root         (0)    15572 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/extensions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4615 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/gunicorn_app.py
+-rw-rw-rw-   0 root         (0) root         (0)   133820 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    13586 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.988897 faradaysec-5.2.1/faraday/server/threads/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/threads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.993897 faradaysec-5.2.1/faraday/server/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/agents.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/bulk_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2505 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/cvss.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/cwe.py
+-rw-rw-rw-   0 root         (0) root         (0)     8853 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/daemonize.py
+-rw-rw-rw-   0 root         (0) root         (0)    12231 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     8465 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/export.py
+-rw-rw-rw-   0 root         (0) root         (0)    13160 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/invalid_chars.py
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/ping.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     5769 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/reports_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)    34555 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/search.py
+-rw-rw-rw-   0 root         (0) root         (0)    11697 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/vulns.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/utils/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.993897 faradaysec-5.2.1/faraday/server/websockets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/websockets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/websockets/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/websockets_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/server/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.995897 faradaysec-5.2.1/faraday/server/www/
+-rw-r--r--   0 root         (0) root         (0)    12005 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/asset-manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2024-03-13 21:04:51.000000 faradaysec-5.2.1/faraday/server/www/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/index.html
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-03-13 21:04:51.000000 faradaysec-5.2.1/faraday/server/www/manifest.json
+-rw-r--r--   0 root         (0) root         (0)    15619 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/precache-manifest.d07621b882e4ff866b395d7787977d42.js
+-rw-r--r--   0 root         (0) root         (0)     1181 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.951897 faradaysec-5.2.1/faraday/server/www/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:09.996897 faradaysec-5.2.1/faraday/server/www/static/css/
+-rw-r--r--   0 root         (0) root         (0)   183537 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/css/2.b43efbd6.chunk.css
+-rw-r--r--   0 root         (0) root         (0)   317573 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/css/2.b43efbd6.chunk.css.map
+-rw-r--r--   0 root         (0) root         (0)   622877 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/css/main.3023afbd.chunk.css
+-rw-r--r--   0 root         (0) root         (0)   507650 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/css/main.3023afbd.chunk.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:10.014897 faradaysec-5.2.1/faraday/server/www/static/js/
+-rw-r--r--   0 root         (0) root         (0)  3063896 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/js/2.3d6f7f6b.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     5668 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/js/2.3d6f7f6b.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0) 17092343 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/js/2.3d6f7f6b.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)  1368432 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/js/main.afa469ce.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      149 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/js/main.afa469ce.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  2711933 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/js/main.afa469ce.chunk.js.map
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/js/runtime-main.ea9693b3.js
+-rw-r--r--   0 root         (0) root         (0)     8286 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/js/runtime-main.ea9693b3.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:10.040897 faradaysec-5.2.1/faraday/server/www/static/media/
+-rw-r--r--   0 root         (0) root         (0)    79144 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/CentraNo2-Book.386f0594.otf
+-rw-r--r--   0 root         (0) root         (0)    81720 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/CentraNo2-Medium.63911e85.otf
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/Checkbox.b83098ac.svg
+-rw-r--r--   0 root         (0) root         (0)      177 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/Checkbox_empty.195b4c92.svg
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/Checkbox_ok.52c5a6cc.svg
+-rw-r--r--   0 root         (0) root         (0)    76768 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_Bold.89985cf2.woff
+-rw-r--r--   0 root         (0) root         (0)    82720 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_Book.b99ba59e.woff
+-rw-r--r--   0 root         (0) root         (0)    78520 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_Medium.db87ffc9.woff
+-rw-r--r--   0 root         (0) root         (0)    79728 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_Roman.db35328c.woff
+-rw-r--r--   0 root         (0) root         (0)    77184 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_SemiBold.48873506.woff
+-rw-r--r--   0 root         (0) root         (0)      713 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/activity-dashboard.b37176e7.svg
+-rw-r--r--   0 root         (0) root         (0)     1569 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/agent_small.d1a2c9fe.svg
+-rw-r--r--   0 root         (0) root         (0)      629 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/analytics.b5f3011a.svg
+-rw-r--r--   0 root         (0) root         (0)     1313 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/api_link.dcbdf06d.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/arrow-down.d8661d88.svg
+-rw-r--r--   0 root         (0) root         (0)      294 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/arrow-right.ec48cf40.svg
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/assets.581bf13b.svg
+-rw-r--r--   0 root         (0) root         (0)     1555 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/automation.a512d67b.svg
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/clear.26371e5f.svg
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/cog.6f2e860c.svg
+-rw-r--r--   0 root         (0) root         (0)     3586 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/command.4ada7185.svg
+-rw-r--r--   0 root         (0) root         (0)      387 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/copy.7e1b1006.svg
+-rw-r--r--   0 root         (0) root         (0)      650 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/copy_link.852fb400.svg
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/customAttributes.c7457305.svg
+-rw-r--r--   0 root         (0) root         (0)      627 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/download-icon.eadbcf9c.svg
+-rw-r--r--   0 root         (0) root         (0)      403 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/drag.b17c0ec9.svg
+-rw-r--r--   0 root         (0) root         (0)    24438 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/empty-feed.3ebce7f3.png
+-rw-r--r--   0 root         (0) root         (0)    18252 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/empty-vulns.1b2994f2.png
+-rw-r--r--   0 root         (0) root         (0)      416 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/error-mark.364d0169.svg
+-rw-r--r--   0 root         (0) root         (0)     1576 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/evidence-default.2dcc3b35.svg
+-rw-r--r--   0 root         (0) root         (0)      215 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/exclamation_error.73360ffd.svg
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/faraday-logo-nav.8385ead1.svg
+-rw-r--r--   0 root         (0) root         (0)      241 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/faraday-logo.6f6c122b.svg
+-rw-r--r--   0 root         (0) root         (0)    22547 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/faraday_loadingbar.13bdbd54.gif
+-rw-r--r--   0 root         (0) root         (0)     5739 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/faraday_logo.3af44fcb.svg
+-rw-r--r--   0 root         (0) root         (0)     4303 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/faraday_logo_product.57beba14.svg
+-rw-r--r--   0 root         (0) root         (0)    29976 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_2fa.efd0850b.png
+-rw-r--r--   0 root         (0) root         (0)    58320 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_analytics.b39bc4e5.png
+-rw-r--r--   0 root         (0) root         (0)    80103 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_duplicates.46352b01.png
+-rw-r--r--   0 root         (0) root         (0)    14262 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_ldap.e96f786d.png
+-rw-r--r--   0 root         (0) root         (0)   137773 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_pipelines.165eec78.png
+-rw-r--r--   0 root         (0) root         (0)    53910 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_planner.7afb07e6.png
+-rw-r--r--   0 root         (0) root         (0)    87874 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_reporting.a9a7890d.png
+-rw-r--r--   0 root         (0) root         (0)    67214 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_saml.119fe76f.png
+-rw-r--r--   0 root         (0) root         (0)    63209 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_scheduler.b29ac5ec.png
+-rw-r--r--   0 root         (0) root         (0)   171169 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_tags.ccc5427b.png
+-rw-r--r--   0 root         (0) root         (0)   183858 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ff_users.ea35eac5.png
+-rw-r--r--   0 root         (0) root         (0)     1454 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/generic_file.f9988671.svg
+-rw-r--r--   0 root         (0) root         (0)      725 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/grid_view.580f3d12.svg
+-rw-r--r--   0 root         (0) root         (0)      931 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/help-sysreq.5680b8ff.svg
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/help.61ace590.svg
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ico-web-shell.fc841a37.svg
+-rw-r--r--   0 root         (0) root         (0)     1092 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-column.efe44a0e.svg
+-rw-r--r--   0 root         (0) root         (0)      855 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-edit.a362c51d.svg
+-rw-r--r--   0 root         (0) root         (0)      718 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-more.fd9db67e.svg
+-rw-r--r--   0 root         (0) root         (0)      144 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-plus.8879f3f6.svg
+-rw-r--r--   0 root         (0) root         (0)     1642 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-tags.c0f5d2b3.svg
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-token.d7973c77.svg
+-rw-r--r--   0 root         (0) root         (0)     1193 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-trash.b1589206.svg
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-trigger-disabled.af2d2680.svg
+-rw-r--r--   0 root         (0) root         (0)      922 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-trigger.f9c88d81.svg
+-rw-r--r--   0 root         (0) root         (0)      489 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-clipboard.c53f2936.svg
+-rw-r--r--   0 root         (0) root         (0)      685 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-close-without-background.9b3b0c89.svg
+-rw-r--r--   0 root         (0) root         (0)      744 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-close.9a5cad5c.svg
+-rw-r--r--   0 root         (0) root         (0)      605 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-edit-enabled.a68d0409.svg
+-rw-r--r--   0 root         (0) root         (0)      837 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-evidence.fdee90dd.svg
+-rw-r--r--   0 root         (0) root         (0)      591 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-show-duplicates.79a1569d.svg
+-rw-r--r--   0 root         (0) root         (0)      563 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-toolbar-confirmed-on.6c7a2996.svg
+-rw-r--r--   0 root         (0) root         (0)     1037 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon-trash-red.1ebe0df4.svg
+-rw-r--r--   0 root         (0) root         (0)      694 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_clearsearch.e7b18936.svg
+-rw-r--r--   0 root         (0) root         (0)      717 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_close_error.459e6ef9.svg
+-rw-r--r--   0 root         (0) root         (0)      956 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_drag.d52758c1.svg
+-rw-r--r--   0 root         (0) root         (0)      870 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_edit.97c1ea04.svg
+-rw-r--r--   0 root         (0) root         (0)      429 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_filter_off.c7a0db30.svg
+-rw-r--r--   0 root         (0) root         (0)      568 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_filter_on.6de198fd.svg
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_help.1b34b217.svg
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_loupe.663ddfdd.svg
+-rw-r--r--   0 root         (0) root         (0)      362 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_modal_asset.f360b291.svg
+-rw-r--r--   0 root         (0) root         (0)      822 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_severity.b2244c26.svg
+-rw-r--r--   0 root         (0) root         (0)      707 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_upload.cd99484a.svg
+-rw-r--r--   0 root         (0) root         (0)     1754 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/icon_users.0781ec97.svg
+-rw-r--r--   0 root         (0) root         (0)      969 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/laptop_icon.21863406.svg
+-rw-r--r--   0 root         (0) root         (0)      493 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/laquo.d5f6e3f8.svg
+-rw-r--r--   0 root         (0) root         (0)     1455 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/list_view.cacc94c7.svg
+-rw-r--r--   0 root         (0) root         (0)      649 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/mini-terminal.f5a8e1d0.svg
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/moveVuln.ba569948.svg
+-rw-r--r--   0 root         (0) root         (0)     3222 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/new_vuln_modal_icon.033159cd.svg
+-rw-r--r--   0 root         (0) root         (0)      393 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/next.0e62ddad.svg
+-rw-r--r--   0 root         (0) root         (0)      283 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/next_arrow.407b029f.svg
+-rw-r--r--   0 root         (0) root         (0)      837 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/noun-help.a93b0458.svg
+-rw-r--r--   0 root         (0) root         (0)     1210 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/preferences_icons_Account.e0a4aa09.svg
+-rw-r--r--   0 root         (0) root         (0)      757 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/preferences_icons_Authentication.1b59fc92.svg
+-rw-r--r--   0 root         (0) root         (0)      390 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/prev.ecd34f23.svg
+-rw-r--r--   0 root         (0) root         (0)      352 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/queue.b922c0be.svg
+-rw-r--r--   0 root         (0) root         (0)      851 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/reload.0d7f0f5c.svg
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/report_small.e8a3d444.svg
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/reports.f38dca7f.svg
+-rw-r--r--   0 root         (0) root         (0)      327 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/resize_bottom_right.eced93cf.svg
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/save_template.d74f944a.svg
+-rw-r--r--   0 root         (0) root         (0)     3621 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/services.0f83c980.svg
+-rw-r--r--   0 root         (0) root         (0)      399 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/shape.9ea9d3d6.svg
+-rw-r--r--   0 root         (0) root         (0)      482 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/sort.062a68ce.svg
+-rw-r--r--   0 root         (0) root         (0)      836 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/star.33d47a05.svg
+-rw-r--r--   0 root         (0) root         (0)      674 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/status.660ac4e6.svg
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tasks_icon.ba912fa5.svg
+-rw-r--r--   0 root         (0) root         (0)      842 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/template.bc90870d.svg
+-rw-r--r--   0 root         (0) root         (0)   164554 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_appscan.9b037d8b.png
+-rw-r--r--   0 root         (0) root         (0)    16275 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_arachni.ac5b15cb.png
+-rw-r--r--   0 root         (0) root         (0)    34524 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_insightVM.f0295560.png
+-rw-r--r--   0 root         (0) root         (0)    11697 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_nessus.8ed3098d.png
+-rw-r--r--   0 root         (0) root         (0)    18860 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_nikto.9acc1459.png
+-rw-r--r--   0 root         (0) root         (0)    21908 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_nmap.9a81da35.png
+-rw-r--r--   0 root         (0) root         (0)    19674 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_openvas.88898507.png
+-rw-r--r--   0 root         (0) root         (0)    38433 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_qualys.8f7b2a7f.png
+-rw-r--r--   0 root         (0) root         (0)    14816 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_sonarQube.3af1625a.jpeg
+-rw-r--r--   0 root         (0) root         (0)    22535 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_tenable.05c390dc.png
+-rw-r--r--   0 root         (0) root         (0)    19425 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_w3af.221ef0f2.png
+-rw-r--r--   0 root         (0) root         (0)    14366 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_wpscan.92adc6c5.png
+-rw-r--r--   0 root         (0) root         (0)   185420 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_zap.62021c39.png
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_trash.e6d04612.svg
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/tool_wheel.1b4bc890.svg
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/unknown_filetype.f6b0014d.svg
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/vulnerabilities.bc957e73.svg
+-rw-r--r--   0 root         (0) root         (0)     2873 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/warning-delete.33357364.svg
+-rw-r--r--   0 root         (0) root         (0)      813 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/wf_arrow_collapsed.51829f9b.svg
+-rw-r--r--   0 root         (0) root         (0)      905 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/wf_arrow_expand.06e6e9bd.svg
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ws-lock.5d1e24be.svg
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-03-13 21:09:48.000000 faradaysec-5.2.1/faraday/server/www/static/media/ws-unlock.b7653513.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:10.041897 faradaysec-5.2.1/faraday/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/settings/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/settings/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/settings/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/settings/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/settings/smtp.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/start_all.py
+-rw-rw-rw-   0 root         (0) root         (0)     8175 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/start_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:10.042898 faradaysec-5.2.1/faraday/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/utils/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5964 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/utils/faraday_openapi_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2024-03-20 20:44:43.000000 faradaysec-5.2.1/faraday/utils/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 20:45:10.043897 faradaysec-5.2.1/faradaysec.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7835 2024-03-20 20:45:09.000000 faradaysec-5.2.1/faradaysec.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18864 2024-03-20 20:45:09.000000 faradaysec-5.2.1/faradaysec.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 20:45:09.000000 faradaysec-5.2.1/faradaysec.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2024-03-20 20:45:09.000000 faradaysec-5.2.1/faradaysec.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1101 2024-03-20 20:45:09.000000 faradaysec-5.2.1/faradaysec.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-03-20 20:45:09.000000 faradaysec-5.2.1/faradaysec.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-20 20:44:43.000000 faradaysec-5.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-03-20 20:44:43.000000 faradaysec-5.2.1/requirements_dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-03-20 20:45:10.044898 faradaysec-5.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    10659 2024-03-20 20:44:43.000000 faradaysec-5.2.1/setup.py
```

### Comparing `faradaysec-5.2.0/AUTHORS` & `faradaysec-5.2.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/LICENSE` & `faradaysec-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/PKG-INFO` & `faradaysec-5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faradaysec
-Version: 5.2.0
+Version: 5.2.1
 Summary: Open Source Collaborative Penetration Test and Vulnerability Management Platform https://www.faradaysec.com
 Home-page: https://github.com/infobyte/faraday
 Author: Faradaysec
 Author-email: devel@faradaysec.com
 Project-URL: Bug Reports, https://github.com/infobyte/faraday/issues
 Project-URL: Say Thanks!, http://saythanks.io/to/faradaysec
 Project-URL: Source, https://github.com/infobyte/faraday/
```

### Comparing `faradaysec-5.2.0/README.md` & `faradaysec-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/alembic.ini` & `faradaysec-5.2.1/faraday/alembic.ini`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/manage.py` & `faradaysec-5.2.1/faraday/manage.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/env.py` & `faradaysec-5.2.1/faraday/migrations/env.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/0409e696eeec_workspace_important_flag_and_risk_.py` & `faradaysec-5.2.1/faraday/migrations/versions/0409e696eeec_workspace_important_flag_and_risk_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/06c48492f587_reformat_jira_issue_fields_value.py` & `faradaysec-5.2.1/faraday/migrations/versions/06c48492f587_reformat_jira_issue_fields_value.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/085188e0a016_create_rules_tables.py` & `faradaysec-5.2.1/faraday/migrations/versions/085188e0a016_create_rules_tables.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/08d02214aedc_add_advanced_filter_to_executive_report_table.py` & `faradaysec-5.2.1/faraday/migrations/versions/08d02214aedc_add_advanced_filter_to_executive_report_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/0d216660da28_add_notification_table.py` & `faradaysec-5.2.1/faraday/migrations/versions/0d216660da28_add_notification_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/0ed0dab44def_add_tags_arguments_for_agent_schedule.py` & `faradaysec-5.2.1/faraday/migrations/versions/0ed0dab44def_add_tags_arguments_for_agent_schedule.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/1145efa88414_add_warnings_to_command_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/1145efa88414_add_warnings_to_command_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/1574fbcf72f5_disable_several_notifications_and_add_event_enabled_flag.py` & `faradaysec-5.2.1/faraday/migrations/versions/1574fbcf72f5_disable_several_notifications_and_add_event_enabled_flag.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/15d70093d262_severities_histogram_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/15d70093d262_severities_histogram_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/182832ed9733_add_socket_agent_sid.py` & `faradaysec-5.2.1/faraday/migrations/versions/182832ed9733_add_socket_agent_sid.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/18891ca61db6_add_cascade_delete_from_workspace.py` & `faradaysec-5.2.1/faraday/migrations/versions/18891ca61db6_add_cascade_delete_from_workspace.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/1b2533cc16fe_fix_custom_fields_display_name_was_used_.py` & `faradaysec-5.2.1/faraday/migrations/versions/1b2533cc16fe_fix_custom_fields_display_name_was_used_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/1d328f7bf643_planner_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/1d328f7bf643_planner_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/1dbe9e8e4247_add_rule_execution_start_and_end_fields.py` & `faradaysec-5.2.1/faraday/migrations/versions/1dbe9e8e4247_add_rule_execution_start_and_end_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/1e95dde5b9c8_cascade_on_kb.py` & `faradaysec-5.2.1/faraday/migrations/versions/1e95dde5b9c8_cascade_on_kb.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/20f3d0c2f71f_alter_table_executive_report_add_.py` & `faradaysec-5.2.1/faraday/migrations/versions/20f3d0c2f71f_alter_table_executive_report_add_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/247a90b029f2_fix_severities_ordering.py` & `faradaysec-5.2.1/faraday/migrations/versions/247a90b029f2_fix_severities_ordering.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/257f6d0ad43f_add_fields_to_kb.py` & `faradaysec-5.2.1/faraday/migrations/versions/257f6d0ad43f_add_fields_to_kb.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/282ac9b6569f_add_agent_as_import_source_to_command.py` & `faradaysec-5.2.1/faraday/migrations/versions/282ac9b6569f_add_agent_as_import_source_to_command.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/2a0de6132377_add_searchfilter_table.py` & `faradaysec-5.2.1/faraday/migrations/versions/2a0de6132377_add_searchfilter_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/2db31733fb78_unique_field_name_in_customfield.py` & `faradaysec-5.2.1/faraday/migrations/versions/2db31733fb78_unique_field_name_in_customfield.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/33094e577642_add__tmp_id_for_on_conflict_inserts.py` & `faradaysec-5.2.1/faraday/migrations/versions/33094e577642_add__tmp_id_for_on_conflict_inserts.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/384784872dc1_add_weight_column_in_role.py` & `faradaysec-5.2.1/faraday/migrations/versions/384784872dc1_add_weight_column_in_role.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/38bb251889e6_bulks.py` & `faradaysec-5.2.1/faraday/migrations/versions/38bb251889e6_bulks.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/3eb96406e88d_rename_important_with_importance_and_remove_check_constraint.py` & `faradaysec-5.2.1/faraday/migrations/versions/3eb96406e88d_rename_important_with_importance_and_remove_check_constraint.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/443a136bb5f2_severities_histogram_constraint.py` & `faradaysec-5.2.1/faraday/migrations/versions/443a136bb5f2_severities_histogram_constraint.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/47e53ddc0308_add_cwe.py` & `faradaysec-5.2.1/faraday/migrations/versions/47e53ddc0308_add_cwe.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/4d7a8fdd94e4_rename_not_active_users.py` & `faradaysec-5.2.1/faraday/migrations/versions/4d7a8fdd94e4_rename_not_active_users.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/51e533d41312_add_host_stats_static_columns.py` & `faradaysec-5.2.1/faraday/migrations/versions/51e533d41312_add_host_stats_static_columns.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/526aa91cac98_vulnerability_merge_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/526aa91cac98_vulnerability_merge_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/5272b3f5a820_add_markdown_column_to_exectuive_reports.py` & `faradaysec-5.2.1/faraday/migrations/versions/5272b3f5a820_add_markdown_column_to_exectuive_reports.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/5658775e113f_add_command_id_to_agent_execution.py` & `faradaysec-5.2.1/faraday/migrations/versions/5658775e113f_add_command_id_to_agent_execution.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/581121b181d8_add_owasp_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/581121b181d8_add_owasp_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/59bed5515407_vuln_external_id.py` & `faradaysec-5.2.1/faraday/migrations/versions/59bed5515407_vuln_external_id.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/5cf9660bba80_policyviolationvulnerabilityassociation_.py` & `faradaysec-5.2.1/faraday/migrations/versions/5cf9660bba80_policyviolationvulnerabilityassociation_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/5d7a930c439e_cve_many_to_many.py` & `faradaysec-5.2.1/faraday/migrations/versions/5d7a930c439e_cve_many_to_many.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/61ded0c8fbf6_notification_center.py` & `faradaysec-5.2.1/faraday/migrations/versions/61ded0c8fbf6_notification_center.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/6471033046cb_added_delete_on_cascade_to_schedule.py` & `faradaysec-5.2.1/faraday/migrations/versions/6471033046cb_added_delete_on_cascade_to_schedule.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/699402156cf4_update_risk_value.py` & `faradaysec-5.2.1/faraday/migrations/versions/699402156cf4_update_risk_value.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/73854f804a8d_cascade_kb_2.py` & `faradaysec-5.2.1/faraday/migrations/versions/73854f804a8d_cascade_kb_2.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/7dea3a6caf51_cascade_in_vuls_relation.py` & `faradaysec-5.2.1/faraday/migrations/versions/7dea3a6caf51_cascade_in_vuls_relation.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/84f266a05be3_add_tool_column_to_vuln.py` & `faradaysec-5.2.1/faraday/migrations/versions/84f266a05be3_add_tool_column_to_vuln.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/85aeb4185f98_refactor_cvss.py` & `faradaysec-5.2.1/faraday/migrations/versions/85aeb4185f98_refactor_cvss.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/877dd088c8cb_comment_ws_not_mandatory.py` & `faradaysec-5.2.1/faraday/migrations/versions/877dd088c8cb_comment_ws_not_mandatory.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/89115e133f0a_add_hosts_notifications.py` & `faradaysec-5.2.1/faraday/migrations/versions/89115e133f0a_add_hosts_notifications.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/8a10ff3926a5_2fa_columns.py` & `faradaysec-5.2.1/faraday/migrations/versions/8a10ff3926a5_2fa_columns.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/901344f297fb_change_object_type_of_custom_logos_to_.py` & `faradaysec-5.2.1/faraday/migrations/versions/901344f297fb_change_object_type_of_custom_logos_to_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/904a517a2f0c_create_executor_table.py` & `faradaysec-5.2.1/faraday/migrations/versions/904a517a2f0c_create_executor_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/905261860ad0_user_types_enum.py` & `faradaysec-5.2.1/faraday/migrations/versions/905261860ad0_user_types_enum.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/97a9348d0406_add_fields_to_report.py` & `faradaysec-5.2.1/faraday/migrations/versions/97a9348d0406_add_fields_to_report.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/99a740945c44_add_index_into_vulnerability.py` & `faradaysec-5.2.1/faraday/migrations/versions/99a740945c44_add_index_into_vulnerability.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/9c4091d1a09b_create_agent_table.py` & `faradaysec-5.2.1/faraday/migrations/versions/9c4091d1a09b_create_agent_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/a39a3a6e3f99_create_user_preferences_column.py` & `faradaysec-5.2.1/faraday/migrations/versions/a39a3a6e3f99_create_user_preferences_column.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/a4def820a5bb_alter_otp_secret_length_in_user.py` & `faradaysec-5.2.1/faraday/migrations/versions/a4def820a5bb_alter_otp_secret_length_in_user.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/a9fcf8444c79_add_notification_event_and_subscription_.py` & `faradaysec-5.2.1/faraday/migrations/versions/a9fcf8444c79_add_notification_event_and_subscription_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/aa56852fa76d_update_rule_fields.py` & `faradaysec-5.2.1/faraday/migrations/versions/aa56852fa76d_update_rule_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/abb7ed8c56b4_add_workflow_models.py` & `faradaysec-5.2.1/faraday/migrations/versions/abb7ed8c56b4_add_workflow_models.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/b1d15a55556d_remove_ticketing_tools_credentials.py` & `faradaysec-5.2.1/faraday/migrations/versions/b1d15a55556d_remove_ticketing_tools_credentials.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/b31fa447f00c_add_analytics_monthly_graphs_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/b31fa447f00c_add_analytics_monthly_graphs_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/b49d8efbd0c2_add_configuration_table.py` & `faradaysec-5.2.1/faraday/migrations/versions/b49d8efbd0c2_add_configuration_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/b5065f401599_report_template_object_type.py` & `faradaysec-5.2.1/faraday/migrations/versions/b5065f401599_report_template_object_type.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/b87b1de2f348_add_delete_workspace_missing_cascades.py` & `faradaysec-5.2.1/faraday/migrations/versions/b87b1de2f348_add_delete_workspace_missing_cascades.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/be1f942eba28_add_analytics_saved_graphics_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/be1f942eba28_add_analytics_saved_graphics_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/be89aa03e35e_add_severities_column_to_executive_.py` & `faradaysec-5.2.1/faraday/migrations/versions/be89aa03e35e_add_severities_column_to_executive_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/cb25cf42bda7_remove_knowledge_base_aka_pasta_base.py` & `faradaysec-5.2.1/faraday/migrations/versions/cb25cf42bda7_remove_knowledge_base_aka_pasta_base.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/d0a6105fdef1_modify_analytics_type_enum.py` & `faradaysec-5.2.1/faraday/migrations/versions/d0a6105fdef1_modify_analytics_type_enum.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/d3afdb4e0b11_add_enum_to_comment_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/d3afdb4e0b11_add_enum_to_comment_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/d8f0b32a5c0e_cvss_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/d8f0b32a5c0e_cvss_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/dd3181b9b3e9_severity_and_service_id_index_in_.py` & `faradaysec-5.2.1/faraday/migrations/versions/dd3181b9b3e9_severity_and_service_id_index_in_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/e61afb450465_add_custom_fields.py` & `faradaysec-5.2.1/faraday/migrations/versions/e61afb450465_add_custom_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/ed403da439d4_agents_with_multiple_workspaces.py` & `faradaysec-5.2.1/faraday/migrations/versions/ed403da439d4_agents_with_multiple_workspaces.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f00247a92a14_add_agent_execution_data.py` & `faradaysec-5.2.1/faraday/migrations/versions/f00247a92a14_add_agent_execution_data.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f0439bf6688a_updating_to_a_role_model_to_use_faraday_.py` & `faradaysec-5.2.1/faraday/migrations/versions/f0439bf6688a_updating_to_a_role_model_to_use_faraday_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f0a32e2753f6_new_one_to_one_reference_table.py` & `faradaysec-5.2.1/faraday/migrations/versions/f0a32e2753f6_new_one_to_one_reference_table.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f0a507afabd4_adding_fs_uniquifier_to_user_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/f0a507afabd4_adding_fs_uniquifier_to_user_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f20aa8756612_change_executivereport_field_to_text.py` & `faradaysec-5.2.1/faraday/migrations/versions/f20aa8756612_change_executivereport_field_to_text.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f28eae25416b_fix_constraint_in_cve_association.py` & `faradaysec-5.2.1/faraday/migrations/versions/f28eae25416b_fix_constraint_in_cve_association.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f6edb9a16479_add_type_to_reference_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/f6edb9a16479_add_type_to_reference_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f7ca45632cce_add_advanced_notifs_to_model.py` & `faradaysec-5.2.1/faraday/migrations/versions/f7ca45632cce_add_advanced_notifs_to_model.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f82a9136c408_remove_ws_from_agents_and_make_schedule_.py` & `faradaysec-5.2.1/faraday/migrations/versions/f82a9136c408_remove_ws_from_agents_and_make_schedule_.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/f8a44acd0e41_add_new_user_role.py` & `faradaysec-5.2.1/faraday/migrations/versions/f8a44acd0e41_add_new_user_role.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/fa12b8322112_update_workflow_modules.py` & `faradaysec-5.2.1/faraday/migrations/versions/fa12b8322112_update_workflow_modules.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/migrations/versions/fa73865dc11c_add_cvss3_scope_field.py` & `faradaysec-5.2.1/faraday/migrations/versions/fa73865dc11c_add_cvss3_scope_field.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/openapi/faraday_swagger.json` & `faradaysec-5.2.1/faraday/openapi/faraday_swagger.json`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/requirements.txt` & `faradaysec-5.2.1/faraday/requirements.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/base.py` & `faradaysec-5.2.1/faraday/server/api/base.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/activity_feed.py` & `faradaysec-5.2.1/faraday/server/api/modules/activity_feed.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/agent.py` & `faradaysec-5.2.1/faraday/server/api/modules/agent.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/agent_auth_token.py` & `faradaysec-5.2.1/faraday/server/api/modules/agent_auth_token.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/bulk_create.py` & `faradaysec-5.2.1/faraday/server/api/modules/bulk_create.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/commandsrun.py` & `faradaysec-5.2.1/faraday/server/api/modules/commandsrun.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/comments.py` & `faradaysec-5.2.1/faraday/server/api/modules/comments.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/credentials.py` & `faradaysec-5.2.1/faraday/server/api/modules/credentials.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/custom_fields.py` & `faradaysec-5.2.1/faraday/server/api/modules/custom_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/export_data.py` & `faradaysec-5.2.1/faraday/server/api/modules/export_data.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/get_exploits.py` & `faradaysec-5.2.1/faraday/server/api/modules/get_exploits.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/global_commands.py` & `faradaysec-5.2.1/faraday/server/api/modules/global_commands.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/hosts.py` & `faradaysec-5.2.1/faraday/server/api/modules/hosts.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/info.py` & `faradaysec-5.2.1/faraday/server/api/modules/info.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/licenses.py` & `faradaysec-5.2.1/faraday/server/api/modules/licenses.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/preferences.py` & `faradaysec-5.2.1/faraday/server/api/modules/preferences.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/search_filter.py` & `faradaysec-5.2.1/faraday/server/api/modules/search_filter.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/services.py` & `faradaysec-5.2.1/faraday/server/api/modules/services.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/session.py` & `faradaysec-5.2.1/faraday/server/api/modules/session.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/settings.py` & `faradaysec-5.2.1/faraday/server/api/modules/settings.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/settings_dashboard.py` & `faradaysec-5.2.1/faraday/server/api/modules/settings_dashboard.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/settings_reports.py` & `faradaysec-5.2.1/faraday/server/api/modules/settings_reports.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/swagger.py` & `faradaysec-5.2.1/faraday/server/api/modules/swagger.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/token.py` & `faradaysec-5.2.1/faraday/server/api/modules/token.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/upload_reports.py` & `faradaysec-5.2.1/faraday/server/api/modules/upload_reports.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/vulnerability_template.py` & `faradaysec-5.2.1/faraday/server/api/modules/vulnerability_template.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/vulns.py` & `faradaysec-5.2.1/faraday/server/api/modules/vulns.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/websocket_auth.py` & `faradaysec-5.2.1/faraday/server/api/modules/websocket_auth.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/api/modules/workspaces.py` & `faradaysec-5.2.1/faraday/server/api/modules/workspaces.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/app.py` & `faradaysec-5.2.1/faraday/server/app.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/celery_worker.py` & `faradaysec-5.2.1/faraday/server/celery_worker.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/celery_worker_gevent.py` & `faradaysec-5.2.1/faraday/server/celery_worker_gevent.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/app_urls.py` & `faradaysec-5.2.1/faraday/server/commands/app_urls.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/change_password.py` & `faradaysec-5.2.1/faraday/server/commands/change_password.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/change_username.py` & `faradaysec-5.2.1/faraday/server/commands/change_username.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/custom_fields.py` & `faradaysec-5.2.1/faraday/server/commands/custom_fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/faraday_schema_display.py` & `faradaysec-5.2.1/faraday/server/commands/faraday_schema_display.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/import_vulnerability_template.py` & `faradaysec-5.2.1/faraday/server/commands/import_vulnerability_template.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/initdb.py` & `faradaysec-5.2.1/faraday/server/commands/initdb.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/manage_settings.py` & `faradaysec-5.2.1/faraday/server/commands/manage_settings.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/move_references.py` & `faradaysec-5.2.1/faraday/server/commands/move_references.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/nginx_config.py` & `faradaysec-5.2.1/faraday/server/commands/nginx_config.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/reset_db.py` & `faradaysec-5.2.1/faraday/server/commands/reset_db.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/sync_hosts_stats.py` & `faradaysec-5.2.1/faraday/server/commands/sync_hosts_stats.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/commands/templates/nginx_config.j2` & `faradaysec-5.2.1/faraday/server/commands/templates/nginx_config.j2`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/config.py` & `faradaysec-5.2.1/faraday/server/config.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/events.py` & `faradaysec-5.2.1/faraday/server/events.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/fields.py` & `faradaysec-5.2.1/faraday/server/fields.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/gunicorn_app.py` & `faradaysec-5.2.1/faraday/server/gunicorn_app.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/models.py` & `faradaysec-5.2.1/faraday/server/models.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/schemas.py` & `faradaysec-5.2.1/faraday/server/schemas.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/tasks.py` & `faradaysec-5.2.1/faraday/server/tasks.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/agents.py` & `faradaysec-5.2.1/faraday/server/utils/agents.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/bulk_create.py` & `faradaysec-5.2.1/faraday/server/utils/bulk_create.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/command.py` & `faradaysec-5.2.1/faraday/server/utils/command.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/cvss.py` & `faradaysec-5.2.1/faraday/server/utils/cvss.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/cwe.py` & `faradaysec-5.2.1/faraday/server/utils/cwe.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/daemonize.py` & `faradaysec-5.2.1/faraday/server/utils/daemonize.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/database.py` & `faradaysec-5.2.1/faraday/server/utils/database.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/debug.py` & `faradaysec-5.2.1/faraday/server/utils/debug.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/export.py` & `faradaysec-5.2.1/faraday/server/utils/export.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/filters.py` & `faradaysec-5.2.1/faraday/server/utils/filters.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/logger.py` & `faradaysec-5.2.1/faraday/server/utils/logger.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/ping.py` & `faradaysec-5.2.1/faraday/server/utils/ping.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/reference.py` & `faradaysec-5.2.1/faraday/server/utils/reference.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/reports_processor.py` & `faradaysec-5.2.1/faraday/server/utils/reports_processor.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/search.py` & `faradaysec-5.2.1/faraday/server/utils/search.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/vulns.py` & `faradaysec-5.2.1/faraday/server/utils/vulns.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/utils/web.py` & `faradaysec-5.2.1/faraday/server/utils/web.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/websockets/dispatcher.py` & `faradaysec-5.2.1/faraday/server/websockets/dispatcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 See the file 'doc/LICENSE' for the license information
 """
 # Standard library imports
 import logging
 
 # Related third party imports
 import itsdangerous
-import sqlalchemy
 from flask import current_app, request
 
 from faraday.server.api.modules.websocket_auth import decode_agent_websocket_token
 from faraday.server.models import Workspace, db, Executor, Agent
 from flask_socketio import Namespace
 
 from faraday.server.utils.database import get_or_create
@@ -47,15 +46,15 @@
 
     return True
 
 
 def remove_sid():
     try:
         agents = Agent.query.filter(Agent.sid!=None).all()  # noqa E711
-    except sqlalchemy.exc.OperationalError as error:
+    except Exception as error:
         logger.warning("Could not update agents table. %s", error)
         return
     logger.debug(f"Found {len(agents)} agents connected")
     for agent in agents:
         agent.sid = None
     db.session.commit()
```

### Comparing `faradaysec-5.2.0/faraday/server/www/asset-manifest.json` & `faradaysec-5.2.1/faraday/server/www/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/favicon.ico` & `faradaysec-5.2.1/faraday/server/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/index.html` & `faradaysec-5.2.1/faraday/server/www/index.html`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/precache-manifest.d07621b882e4ff866b395d7787977d42.js` & `faradaysec-5.2.1/faraday/server/www/precache-manifest.d07621b882e4ff866b395d7787977d42.js`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/service-worker.js` & `faradaysec-5.2.1/faraday/server/www/service-worker.js`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/css/2.b43efbd6.chunk.css` & `faradaysec-5.2.1/faraday/server/www/static/css/2.b43efbd6.chunk.css`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/css/2.b43efbd6.chunk.css.map` & `faradaysec-5.2.1/faraday/server/www/static/css/2.b43efbd6.chunk.css.map`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/css/main.3023afbd.chunk.css` & `faradaysec-5.2.1/faraday/server/www/static/css/main.3023afbd.chunk.css`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/css/main.3023afbd.chunk.css.map` & `faradaysec-5.2.1/faraday/server/www/static/css/main.3023afbd.chunk.css.map`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/js/2.3d6f7f6b.chunk.js` & `faradaysec-5.2.1/faraday/server/www/static/js/2.3d6f7f6b.chunk.js`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/js/2.3d6f7f6b.chunk.js.LICENSE.txt` & `faradaysec-5.2.1/faraday/server/www/static/js/2.3d6f7f6b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/js/2.3d6f7f6b.chunk.js.map` & `faradaysec-5.2.1/faraday/server/www/static/js/2.3d6f7f6b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/js/main.afa469ce.chunk.js` & `faradaysec-5.2.1/faraday/server/www/static/js/main.afa469ce.chunk.js`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/js/main.afa469ce.chunk.js.map` & `faradaysec-5.2.1/faraday/server/www/static/js/main.afa469ce.chunk.js.map`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/js/runtime-main.ea9693b3.js` & `faradaysec-5.2.1/faraday/server/www/static/js/runtime-main.ea9693b3.js`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/js/runtime-main.ea9693b3.js.map` & `faradaysec-5.2.1/faraday/server/www/static/js/runtime-main.ea9693b3.js.map`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/CentraNo2-Book.386f0594.otf` & `faradaysec-5.2.1/faraday/server/www/static/media/CentraNo2-Book.386f0594.otf`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/CentraNo2-Medium.63911e85.otf` & `faradaysec-5.2.1/faraday/server/www/static/media/CentraNo2-Medium.63911e85.otf`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/Checkbox.b83098ac.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/Checkbox.b83098ac.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/Checkbox_ok.52c5a6cc.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/Checkbox_ok.52c5a6cc.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_Bold.89985cf2.woff` & `faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_Bold.89985cf2.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_Book.b99ba59e.woff` & `faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_Book.b99ba59e.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_Medium.db87ffc9.woff` & `faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_Medium.db87ffc9.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_Roman.db35328c.woff` & `faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_Roman.db35328c.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/Sequel_Sans_Head_SemiBold.48873506.woff` & `faradaysec-5.2.1/faraday/server/www/static/media/Sequel_Sans_Head_SemiBold.48873506.woff`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/activity-dashboard.b37176e7.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/activity-dashboard.b37176e7.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/agent_small.d1a2c9fe.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/agent_small.d1a2c9fe.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/analytics.b5f3011a.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/analytics.b5f3011a.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/api_link.dcbdf06d.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/api_link.dcbdf06d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/assets.581bf13b.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/assets.581bf13b.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/automation.a512d67b.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/automation.a512d67b.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/clear.26371e5f.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/clear.26371e5f.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/cog.6f2e860c.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/cog.6f2e860c.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/command.4ada7185.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/command.4ada7185.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/copy_link.852fb400.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/copy_link.852fb400.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/customAttributes.c7457305.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/customAttributes.c7457305.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/download-icon.eadbcf9c.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/download-icon.eadbcf9c.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/empty-feed.3ebce7f3.png` & `faradaysec-5.2.1/faraday/server/www/static/media/empty-feed.3ebce7f3.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/empty-vulns.1b2994f2.png` & `faradaysec-5.2.1/faraday/server/www/static/media/empty-vulns.1b2994f2.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/evidence-default.2dcc3b35.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/evidence-default.2dcc3b35.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/faraday-logo-nav.8385ead1.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/faraday-logo-nav.8385ead1.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/faraday_loadingbar.13bdbd54.gif` & `faradaysec-5.2.1/faraday/server/www/static/media/faraday_loadingbar.13bdbd54.gif`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/faraday_logo.3af44fcb.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/faraday_logo.3af44fcb.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/faraday_logo_product.57beba14.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/faraday_logo_product.57beba14.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_2fa.efd0850b.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_2fa.efd0850b.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_analytics.b39bc4e5.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_analytics.b39bc4e5.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_duplicates.46352b01.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_duplicates.46352b01.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_ldap.e96f786d.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_ldap.e96f786d.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_pipelines.165eec78.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_pipelines.165eec78.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_planner.7afb07e6.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_planner.7afb07e6.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_reporting.a9a7890d.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_reporting.a9a7890d.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_saml.119fe76f.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_saml.119fe76f.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_scheduler.b29ac5ec.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_scheduler.b29ac5ec.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_tags.ccc5427b.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_tags.ccc5427b.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ff_users.ea35eac5.png` & `faradaysec-5.2.1/faraday/server/www/static/media/ff_users.ea35eac5.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/generic_file.f9988671.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/generic_file.f9988671.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/grid_view.580f3d12.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/grid_view.580f3d12.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/help-sysreq.5680b8ff.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/help-sysreq.5680b8ff.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/help.61ace590.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/help.61ace590.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ico-web-shell.fc841a37.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/ico-web-shell.fc841a37.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-column.efe44a0e.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-column.efe44a0e.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-edit.a362c51d.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-edit.a362c51d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-more.fd9db67e.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-more.fd9db67e.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-tags.c0f5d2b3.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-tags.c0f5d2b3.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-token.d7973c77.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-token.d7973c77.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-trash.b1589206.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-trash.b1589206.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-trigger-disabled.af2d2680.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-trigger-disabled.af2d2680.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-action-bar-trigger.f9c88d81.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-action-bar-trigger.f9c88d81.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-close-without-background.9b3b0c89.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-close-without-background.9b3b0c89.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-close.9a5cad5c.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-close.9a5cad5c.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-edit-enabled.a68d0409.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-edit-enabled.a68d0409.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-evidence.fdee90dd.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-evidence.fdee90dd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-show-duplicates.79a1569d.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-show-duplicates.79a1569d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-toolbar-confirmed-on.6c7a2996.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-toolbar-confirmed-on.6c7a2996.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon-trash-red.1ebe0df4.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon-trash-red.1ebe0df4.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_clearsearch.e7b18936.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_clearsearch.e7b18936.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_close_error.459e6ef9.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_close_error.459e6ef9.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_drag.d52758c1.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_drag.d52758c1.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_edit.97c1ea04.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_edit.97c1ea04.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_filter_on.6de198fd.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_filter_on.6de198fd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_help.1b34b217.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_help.1b34b217.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_loupe.663ddfdd.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_loupe.663ddfdd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_severity.b2244c26.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_severity.b2244c26.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_upload.cd99484a.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_upload.cd99484a.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/icon_users.0781ec97.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/icon_users.0781ec97.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/laptop_icon.21863406.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/laptop_icon.21863406.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/list_view.cacc94c7.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/list_view.cacc94c7.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/mini-terminal.f5a8e1d0.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/mini-terminal.f5a8e1d0.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/moveVuln.ba569948.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/moveVuln.ba569948.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/new_vuln_modal_icon.033159cd.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/new_vuln_modal_icon.033159cd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/noun-help.a93b0458.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/noun-help.a93b0458.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/preferences_icons_Account.e0a4aa09.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/preferences_icons_Account.e0a4aa09.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/preferences_icons_Authentication.1b59fc92.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/preferences_icons_Authentication.1b59fc92.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/reload.0d7f0f5c.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/reload.0d7f0f5c.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/report_small.e8a3d444.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/report_small.e8a3d444.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/reports.f38dca7f.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/reports.f38dca7f.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/save_template.d74f944a.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/save_template.d74f944a.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/services.0f83c980.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/services.0f83c980.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/star.33d47a05.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/star.33d47a05.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/status.660ac4e6.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/status.660ac4e6.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tasks_icon.ba912fa5.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/tasks_icon.ba912fa5.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/template.bc90870d.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/template.bc90870d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_appscan.9b037d8b.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_appscan.9b037d8b.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_arachni.ac5b15cb.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_arachni.ac5b15cb.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_insightVM.f0295560.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_insightVM.f0295560.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_nessus.8ed3098d.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_nessus.8ed3098d.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_nikto.9acc1459.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_nikto.9acc1459.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_nmap.9a81da35.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_nmap.9a81da35.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_openvas.88898507.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_openvas.88898507.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_qualys.8f7b2a7f.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_qualys.8f7b2a7f.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_sonarQube.3af1625a.jpeg` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_sonarQube.3af1625a.jpeg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_tenable.05c390dc.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_tenable.05c390dc.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_w3af.221ef0f2.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_w3af.221ef0f2.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_wpscan.92adc6c5.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_wpscan.92adc6c5.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_logo_zap.62021c39.png` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_logo_zap.62021c39.png`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_trash.e6d04612.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_trash.e6d04612.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/tool_wheel.1b4bc890.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/tool_wheel.1b4bc890.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/unknown_filetype.f6b0014d.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/unknown_filetype.f6b0014d.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/vulnerabilities.bc957e73.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/vulnerabilities.bc957e73.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/warning-delete.33357364.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/warning-delete.33357364.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/wf_arrow_collapsed.51829f9b.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/wf_arrow_collapsed.51829f9b.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/wf_arrow_expand.06e6e9bd.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/wf_arrow_expand.06e6e9bd.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ws-lock.5d1e24be.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/ws-lock.5d1e24be.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/server/www/static/media/ws-unlock.b7653513.svg` & `faradaysec-5.2.1/faraday/server/www/static/media/ws-unlock.b7653513.svg`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/settings/__init__.py` & `faradaysec-5.2.1/faraday/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/settings/base.py` & `faradaysec-5.2.1/faraday/settings/base.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/settings/dashboard.py` & `faradaysec-5.2.1/faraday/settings/dashboard.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/settings/reports.py` & `faradaysec-5.2.1/faraday/settings/reports.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/settings/smtp.py` & `faradaysec-5.2.1/faraday/settings/smtp.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/start_all.py` & `faradaysec-5.2.1/faraday/start_all.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/start_server.py` & `faradaysec-5.2.1/faraday/start_server.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/utils/decorators.py` & `faradaysec-5.2.1/faraday/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/utils/faraday_openapi_plugin.py` & `faradaysec-5.2.1/faraday/utils/faraday_openapi_plugin.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faraday/utils/smtp.py` & `faradaysec-5.2.1/faraday/utils/smtp.py`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faradaysec.egg-info/PKG-INFO` & `faradaysec-5.2.1/faradaysec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faradaysec
-Version: 5.2.0
+Version: 5.2.1
 Summary: Open Source Collaborative Penetration Test and Vulnerability Management Platform https://www.faradaysec.com
 Home-page: https://github.com/infobyte/faraday
 Author: Faradaysec
 Author-email: devel@faradaysec.com
 Project-URL: Bug Reports, https://github.com/infobyte/faraday/issues
 Project-URL: Say Thanks!, http://saythanks.io/to/faradaysec
 Project-URL: Source, https://github.com/infobyte/faraday/
```

### Comparing `faradaysec-5.2.0/faradaysec.egg-info/SOURCES.txt` & `faradaysec-5.2.1/faradaysec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/faradaysec.egg-info/requires.txt` & `faradaysec-5.2.1/faradaysec.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/requirements.txt` & `faradaysec-5.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `faradaysec-5.2.0/setup.py` & `faradaysec-5.2.1/setup.py`

 * *Files identical despite different names*

