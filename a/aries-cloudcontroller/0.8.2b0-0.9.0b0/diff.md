# Comparing `tmp/aries_cloudcontroller-0.8.2b0.tar.gz` & `tmp/aries_cloudcontroller-0.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aries_cloudcontroller-0.8.2b0.tar", last modified: Mon Jul 24 10:05:56 2023, max compression
+gzip compressed data, was "aries_cloudcontroller-0.9.0b0.tar", last modified: Tue Jul 25 10:13:36 2023, max compression
```

## Comparing `aries_cloudcontroller-0.8.2b0.tar` & `aries_cloudcontroller-0.9.0b0.tar`

### file list

```diff
@@ -1,341 +1,344 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.390951 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/acapy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.394952 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/action_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/basicmessage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/did_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/discover_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/discover_features_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/endorse_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/introduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/issue_credential_v1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/issue_credential_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/jsonld.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/ledger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/mediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/multitenancy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/out_of_band.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/present_proof_v1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/present_proof_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/trustping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/action_menu_fetch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status_readiness.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/aml_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data1_jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data_jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data_jws_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attachment_def.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attribute_mime_types_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/claim_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/clear_pending_revocations_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/conn_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_metadata_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_static_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_static_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value_primary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value_revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_info_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_indy_records_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_record_details_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_record_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_revoked_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_get_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definitions_created_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_status_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_endpoint_with_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/didx_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_proof_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/disclose.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/disclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/endorser_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/endpoints_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/generated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_did_endpoint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_did_verkey_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_nym_role_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_attr_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_precis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_eq_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_ge_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_ge_proof_pred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_key_correctness_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_non_revoc_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_non_revocation_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_primary_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_request_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_entry_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/input_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/issuer_cred_rev_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/issuer_rev_reg_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query_filter_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query_paginate.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ld_proof_vc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ld_proof_vc_detail_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ledger_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ledger_config_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/linked_data_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_id_match_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_form_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/model_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/oob_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/perform_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ping_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ping_request_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/profile_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/protocol_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/publish_revocations.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/query_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/raw_encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/receive_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/remove_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/resolution_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_issued_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_regs_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/revoke_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/route_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_get_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_input_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schemas_created_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schemas_input_descriptor_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/send_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/service_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/sign_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/sign_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/signature_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/signed_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/submission_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_accept.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/tails_delete_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_publish_revocations_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/update_profile_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/update_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_store_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_exchange_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_indy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter_indy.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request_free.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_store_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_exchange_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_issue_cred_schema_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_request_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/vc_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/vc_record_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/verify_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/verify_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/w3_c_credentials_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/wallet_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/write_ledger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/uplink_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/acapy_client_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/pydantic_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.390951 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 10:05:56.000000 aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/tests/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/client/test_acapy_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/client/test_pydantic_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_credential_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_presentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_v20_cred_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/model/test_v20_pres_ex_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:56.422952 aries_cloudcontroller-0.8.2b0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-24 10:05:45.000000 aries_cloudcontroller-0.8.2b0/tests/util/compare_dicts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.955165 aries_cloudcontroller-0.9.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-25 10:13:36.951166 aries_cloudcontroller-0.9.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.911166 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/acapy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.911166 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/action_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/basicmessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/did_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/discover_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/discover_features_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/endorse_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/issue_credential_v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/issue_credential_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/ledger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/mediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/multitenancy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/out_of_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/present_proof_v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/present_proof_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/trustping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.947166 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    30195 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/action_menu_fetch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_status_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_status_readiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/aml_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator_data1_jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator_data_jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator_data_jws_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attachment_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attribute_mime_types_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/claim_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/clear_pending_revocations_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/conn_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_metadata_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_static_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_static_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_wallet_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_wallet_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_def_value_primary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_def_value_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_info_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_rev_indy_records_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_rev_record_details_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_rev_record_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_revoked_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definition_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definition_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definitions_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_status_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_endpoint_with_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/didx_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_proof_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/disclose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/disclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/endorser_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/endpoints_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/get_did_endpoint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/get_did_verkey_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/get_nym_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_attr_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_cred_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_cred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_cred_precis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_eq_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_ge_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_ge_proof_pred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_key_correctness_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_non_revoc_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_non_revocation_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_pres_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_pres_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_pres_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_primary_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_req_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_req_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_request_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_requested_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_entry_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/input_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/invitation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/invitation_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/invitation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/invitation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/issuer_cred_rev_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/issuer_rev_reg_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/jws_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/jws_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/jws_verify_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_query_filter_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_query_paginate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_update_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ld_proof_vc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ld_proof_vc_detail_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ledger_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ledger_config_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/linked_data_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_id_match_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu_form_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/model_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/oob_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/perform_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ping_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ping_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/presentation_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/presentation_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/presentation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/profile_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/protocol_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/publish_revocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/query_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/raw_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/receive_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/remove_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/resolution_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_issued_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_regs_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/revoke_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/route_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schema_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schema_input_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schema_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schemas_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schemas_input_descriptor_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/send_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/service_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/sign_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/sign_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/signature_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/signed_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/submission_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_accept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/tails_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/transaction_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/transaction_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/transaction_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_publish_revocations_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/update_profile_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/update_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_exchange_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_indy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_filter_indy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_request_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_discovery_exchange_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_issue_cred_schema_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_ex_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_proposal_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_request_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/vc_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/vc_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/verify_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/verify_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/w3_c_credentials_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/wallet_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/write_ledger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/uplink_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.951166 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/util/acapy_client_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/util/pydantic_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.911166 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-25 10:13:36.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-07-25 10:13:36.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:13:36.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 10:13:36.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 10:13:36.000000 aries_cloudcontroller-0.9.0b0/aries_cloudcontroller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:13:36.955165 aries_cloudcontroller-0.9.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.951166 aries_cloudcontroller-0.9.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.951166 aries_cloudcontroller-0.9.0b0/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/client/test_acapy_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/client/test_pydantic_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.951166 aries_cloudcontroller-0.9.0b0/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/model/test_credential_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/model/test_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/model/test_presentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/model/test_v20_cred_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/model/test_v20_pres_ex_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:36.951166 aries_cloudcontroller-0.9.0b0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-25 10:13:15.000000 aries_cloudcontroller-0.9.0b0/tests/util/compare_dicts.py
```

### Comparing `aries_cloudcontroller-0.8.2b0/LICENSE` & `aries_cloudcontroller-0.9.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/PKG-INFO` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: aries_cloudcontroller
-Version: 0.8.2b0
+Name: aries-cloudcontroller
+Version: 0.9.0b0
 Summary: A simple python package for controlling an aries agent through the admin-api interface
 Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <br />
   <img
     alt="Hyperledger Aries logo"
@@ -56,21 +56,23 @@
 | Aries Cloud Controller Version | Aries Cloud Agent Python Version |
 | ------------------------------ | -------------------------------- |
 | 0.5.1-0.5.2                    | 0.7.3                            |
 | 0.6.0-0.6.3                    | 0.7.4                            |
 | 0.7.0                          | 0.7.5                            |
 | 0.8.0                          | 0.8.0                            |
 | 0.8.1                          | 0.8.1                            |
+| 0.8.2                          | 0.8.2                            |
+| 0.9.0                          | 0.9.0                            |
 
 ## Features
 
 Aries Cloud Controller Python is a fully featured client for interacting with ACA-Py.
 
 - Fully Typed wrapper around Aries Cloud Agent Python
-- Supports latest ACA-Py version (0.8.1)
+- Supports latest ACA-Py version (0.9.0)
 - Client is auto generated based on OpenAPI definitions, allowing us to keep up to date with new releases.
 - Supports multi-tenant APIs and authentication
 - Async API
 
 ## Usage
 
 Aries Cloud Controller Python is published to PyPi and can be installed using pip:
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.8.2b0 Summary: A
+Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.9.0b0 Summary: A
 simple python package for controlling an aries agent through the admin-api
 interface Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/
 tree/main/aries_cloudcontroller Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
+Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE
 
                            [Hyperledger Aries logo]
                   ****** Aries Cloud Controller Python ******
      [Pipeline Status] [aries-cloudcontroller_version] [License] [Python]
 
       Features  |  Usage  |  Available_APIs  |  Contributing  |  License
@@ -17,30 +17,30 @@
 definition provided by ACA-Py, giving a fully-typed rich API for interacting
 the cloud agent. Each Cloud Controller version maps to a specific ACA-Py
 version, which is outlined in the table below. Although not strictly adhered to
 in the past, a new ACA-Py version will result in a new Minor version bump for
 the Cloud Controller, as there are often times breaking changes. | Aries Cloud
 Controller Version | Aries Cloud Agent Python Version | | ---------------------
 --------- | -------------------------------- | | 0.5.1-0.5.2 | 0.7.3 | | 0.6.0-
-0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | | 0.8.1 | 0.8.1 | ##
-Features Aries Cloud Controller Python is a fully featured client for
-interacting with ACA-Py. - Fully Typed wrapper around Aries Cloud Agent Python
-- Supports latest ACA-Py version (0.8.1) - Client is auto generated based on
-OpenAPI definitions, allowing us to keep up to date with new releases. -
-Supports multi-tenant APIs and authentication - Async API ## Usage Aries Cloud
-Controller Python is published to PyPi and can be installed using pip: ```sh
-pip install aries-cloudcontroller ``` ### Creating a client ```python from
-aries_cloudcontroller import AcaPyClient client = AcaPyClient( base_url="http:/
-/localhost:8000", api_key="myApiKey" ) ``` **Admin insecure mode** If you are
-running ACA-Py with the admin insecure flag and don't have the API key, you
-must set the `admin_insecure` property: ```python client = AcaPyClient
-( base_url="http://localhost:8000", # Explicitly mark that no api key is used
-admin_insecure=True ) ``` **Multitenancy** To provision the agent in the
-context of specific tenant of the agent, the `tenant_jwt` property must be set:
-```python client = AcaPyClient( base_url="http://localhost:8000",
+0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | | 0.8.1 | 0.8.1 | | 0.8.2 |
+0.8.2 | | 0.9.0 | 0.9.0 | ## Features Aries Cloud Controller Python is a fully
+featured client for interacting with ACA-Py. - Fully Typed wrapper around Aries
+Cloud Agent Python - Supports latest ACA-Py version (0.9.0) - Client is auto
+generated based on OpenAPI definitions, allowing us to keep up to date with new
+releases. - Supports multi-tenant APIs and authentication - Async API ## Usage
+Aries Cloud Controller Python is published to PyPi and can be installed using
+pip: ```sh pip install aries-cloudcontroller ``` ### Creating a client
+```python from aries_cloudcontroller import AcaPyClient client = AcaPyClient
+( base_url="http://localhost:8000", api_key="myApiKey" ) ``` **Admin insecure
+mode** If you are running ACA-Py with the admin insecure flag and don't have
+the API key, you must set the `admin_insecure` property: ```python client =
+AcaPyClient( base_url="http://localhost:8000", # Explicitly mark that no api
+key is used admin_insecure=True ) ``` **Multitenancy** To provision the agent
+in the context of specific tenant of the agent, the `tenant_jwt` property must
+be set: ```python client = AcaPyClient( base_url="http://localhost:8000",
 tenant_jwt="eyXXX" ) ``` ### Interacting with the client Once you have the
 client set up, you're ready to interact with it. Because the API is fully
 typed, the best way to know what is available is by looking at the ACA-Py
 swagger UI, and the available properties on the client. For example to create
 and receive an invitation the following methods can be called: ```python
 invitation = await client.connection.create_invitation
 ( body=CreateInvitationRequest(my_label="Cloud Controller") ) connection =
```

### Comparing `aries_cloudcontroller-0.8.2b0/README.md` & `aries_cloudcontroller-0.9.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,21 +44,23 @@
 | Aries Cloud Controller Version | Aries Cloud Agent Python Version |
 | ------------------------------ | -------------------------------- |
 | 0.5.1-0.5.2                    | 0.7.3                            |
 | 0.6.0-0.6.3                    | 0.7.4                            |
 | 0.7.0                          | 0.7.5                            |
 | 0.8.0                          | 0.8.0                            |
 | 0.8.1                          | 0.8.1                            |
+| 0.8.2                          | 0.8.2                            |
+| 0.9.0                          | 0.9.0                            |
 
 ## Features
 
 Aries Cloud Controller Python is a fully featured client for interacting with ACA-Py.
 
 - Fully Typed wrapper around Aries Cloud Agent Python
-- Supports latest ACA-Py version (0.8.1)
+- Supports latest ACA-Py version (0.9.0)
 - Client is auto generated based on OpenAPI definitions, allowing us to keep up to date with new releases.
 - Supports multi-tenant APIs and authentication
 - Async API
 
 ## Usage
 
 Aries Cloud Controller Python is published to PyPi and can be installed using pip:
```

#### html2text {}

```diff
@@ -10,30 +10,30 @@
 definition provided by ACA-Py, giving a fully-typed rich API for interacting
 the cloud agent. Each Cloud Controller version maps to a specific ACA-Py
 version, which is outlined in the table below. Although not strictly adhered to
 in the past, a new ACA-Py version will result in a new Minor version bump for
 the Cloud Controller, as there are often times breaking changes. | Aries Cloud
 Controller Version | Aries Cloud Agent Python Version | | ---------------------
 --------- | -------------------------------- | | 0.5.1-0.5.2 | 0.7.3 | | 0.6.0-
-0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | | 0.8.1 | 0.8.1 | ##
-Features Aries Cloud Controller Python is a fully featured client for
-interacting with ACA-Py. - Fully Typed wrapper around Aries Cloud Agent Python
-- Supports latest ACA-Py version (0.8.1) - Client is auto generated based on
-OpenAPI definitions, allowing us to keep up to date with new releases. -
-Supports multi-tenant APIs and authentication - Async API ## Usage Aries Cloud
-Controller Python is published to PyPi and can be installed using pip: ```sh
-pip install aries-cloudcontroller ``` ### Creating a client ```python from
-aries_cloudcontroller import AcaPyClient client = AcaPyClient( base_url="http:/
-/localhost:8000", api_key="myApiKey" ) ``` **Admin insecure mode** If you are
-running ACA-Py with the admin insecure flag and don't have the API key, you
-must set the `admin_insecure` property: ```python client = AcaPyClient
-( base_url="http://localhost:8000", # Explicitly mark that no api key is used
-admin_insecure=True ) ``` **Multitenancy** To provision the agent in the
-context of specific tenant of the agent, the `tenant_jwt` property must be set:
-```python client = AcaPyClient( base_url="http://localhost:8000",
+0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | | 0.8.1 | 0.8.1 | | 0.8.2 |
+0.8.2 | | 0.9.0 | 0.9.0 | ## Features Aries Cloud Controller Python is a fully
+featured client for interacting with ACA-Py. - Fully Typed wrapper around Aries
+Cloud Agent Python - Supports latest ACA-Py version (0.9.0) - Client is auto
+generated based on OpenAPI definitions, allowing us to keep up to date with new
+releases. - Supports multi-tenant APIs and authentication - Async API ## Usage
+Aries Cloud Controller Python is published to PyPi and can be installed using
+pip: ```sh pip install aries-cloudcontroller ``` ### Creating a client
+```python from aries_cloudcontroller import AcaPyClient client = AcaPyClient
+( base_url="http://localhost:8000", api_key="myApiKey" ) ``` **Admin insecure
+mode** If you are running ACA-Py with the admin insecure flag and don't have
+the API key, you must set the `admin_insecure` property: ```python client =
+AcaPyClient( base_url="http://localhost:8000", # Explicitly mark that no api
+key is used admin_insecure=True ) ``` **Multitenancy** To provision the agent
+in the context of specific tenant of the agent, the `tenant_jwt` property must
+be set: ```python client = AcaPyClient( base_url="http://localhost:8000",
 tenant_jwt="eyXXX" ) ``` ### Interacting with the client Once you have the
 client set up, you're ready to interact with it. Because the API is fully
 typed, the best way to know what is available is by looking at the ACA-Py
 swagger UI, and the available properties on the client. For example to create
 and receive an invitation the following methods can be called: ```python
 invitation = await client.connection.create_invitation
 ( body=CreateInvitationRequest(my_label="Cloud Controller") ) connection =
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/__init__.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,17 @@
     InputDescriptors,
     InvitationCreateRequest,
     InvitationMessage,
     InvitationRecord,
     InvitationResult,
     IssuerCredRevRecord,
     IssuerRevRegRecord,
+    JWSCreate,
+    JWSVerify,
+    JWSVerifyResponse,
     Keylist,
     KeylistQuery,
     KeylistQueryFilterRequest,
     KeylistQueryPaginate,
     KeylistUpdate,
     KeylistUpdateRequest,
     KeylistUpdateRule,
@@ -424,14 +427,17 @@
     "InputDescriptors",
     "InvitationCreateRequest",
     "InvitationMessage",
     "InvitationRecord",
     "InvitationResult",
     "IssuerCredRevRecord",
     "IssuerRevRegRecord",
+    "JWSCreate",
+    "JWSVerify",
+    "JWSVerifyResponse",
     "Keylist",
     "KeylistQuery",
     "KeylistQueryFilterRequest",
     "KeylistQueryPaginate",
     "KeylistUpdate",
     "KeylistUpdateRequest",
     "KeylistUpdateRule",
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/acapy_client.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/acapy_client.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/__init__.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/action_menu.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/action_menu.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/basicmessage.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/basicmessage.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/connection.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/connection.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/credential_definition.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/credential_definition.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/credentials.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/credentials.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/did_exchange.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/did_exchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,23 +51,27 @@
         )
 
     async def create_request(
         self,
         *,
         their_public_did: str,
         alias: Optional[str] = None,
+        goal: Optional[str] = None,
+        goal_code: Optional[str] = None,
         mediation_id: Optional[str] = None,
         my_endpoint: Optional[str] = None,
         my_label: Optional[str] = None,
         use_public_did: Optional[bool] = None
     ) -> ConnRecord:
         """Create and send a request against public DID's implicit invitation"""
         return await self.__create_request(
             their_public_did=their_public_did,
             alias=alias,
+            goal=goal,
+            goal_code=goal_code,
             mediation_id=mediation_id,
             my_endpoint=my_endpoint,
             my_label=my_label,
             use_public_did=bool_query(use_public_did),
         )
 
     async def receive_request(
@@ -107,14 +111,16 @@
     @returns.json
     @post("/didexchange/create-request")
     def __create_request(
         self,
         *,
         their_public_did: Query,
         alias: Query = None,
+        goal: Query = None,
+        goal_code: Query = None,
         mediation_id: Query = None,
         my_endpoint: Query = None,
         my_label: Query = None,
         use_public_did: Query = None
     ) -> ConnRecord:
         """Internal uplink method for create_request"""
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/discover_features.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/discover_features.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/discover_features_v2_0.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/discover_features_v2_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/endorse_transaction.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/endorse_transaction.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/introduction.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/introduction.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/issue_credential_v1_0.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/issue_credential_v1_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/issue_credential_v2_0.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/issue_credential_v2_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/jsonld.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/jsonld.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/ledger.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/ledger.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/mediation.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/mediation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/multitenancy.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/multitenancy.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/out_of_band.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/out_of_band.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/present_proof_v1_0.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/present_proof_v1_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/present_proof_v2_0.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/present_proof_v2_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/resolver.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/resolver.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/revocation.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/revocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,22 @@
         """Publish pending revocations to ledger"""
         if not body:
             body = PublishRevocations()
         return await self.__publish_revocations(
             body=body,
         )
 
+    async def revocation_active_registry_cred_def_id_rotate_post(
+        self, *, cred_def_id: str
+    ) -> RevRegsCreated:
+        """Rotate revocation registry"""
+        return await self.__revocation_active_registry_cred_def_id_rotate_post(
+            cred_def_id=cred_def_id,
+        )
+
     async def revocation_registry_delete_tails_file_delete(
         self, *, cred_def_id: Optional[str] = None, rev_reg_id: Optional[str] = None
     ) -> TailsDeleteResponse:
         """Delete the tail files"""
         return await self.__revocation_registry_delete_tails_file_delete(
             cred_def_id=cred_def_id,
             rev_reg_id=rev_reg_id,
@@ -308,14 +316,21 @@
     @post("/revocation/publish-revocations")
     def __publish_revocations(
         self, *, body: Body(type=PublishRevocations) = {}
     ) -> TxnOrPublishRevocationsResult:
         """Internal uplink method for publish_revocations"""
 
     @returns.json
+    @post("/revocation/active-registry/{cred_def_id}/rotate")
+    def __revocation_active_registry_cred_def_id_rotate_post(
+        self, *, cred_def_id: str
+    ) -> RevRegsCreated:
+        """Internal uplink method for revocation_active_registry_cred_def_id_rotate_post"""
+
+    @returns.json
     @delete("/revocation/registry/delete-tails-file")
     def __revocation_registry_delete_tails_file_delete(
         self, *, cred_def_id: Query = None, rev_reg_id: Query = None
     ) -> TailsDeleteResponse:
         """Internal uplink method for revocation_registry_delete_tails_file_delete"""
 
     @returns.json
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/schema.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/schema.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/server.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/server.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/settings.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/settings.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/trustping.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/trustping.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/api/wallet.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/api/wallet.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.did_create import DIDCreate
 from aries_cloudcontroller.model.did_endpoint import DIDEndpoint
 from aries_cloudcontroller.model.did_endpoint_with_type import DIDEndpointWithType
 from aries_cloudcontroller.model.did_list import DIDList
 from aries_cloudcontroller.model.did_result import DIDResult
+from aries_cloudcontroller.model.jws_create import JWSCreate
+from aries_cloudcontroller.model.jws_verify import JWSVerify
+from aries_cloudcontroller.model.jws_verify_response import JWSVerifyResponse
 
 
 class WalletApi(Consumer):
     async def create_did(self, *, body: Optional[DIDCreate] = None) -> DIDResult:
         """Create a local DID"""
         if not body:
             body = DIDCreate()
@@ -95,14 +98,34 @@
         return await self.__set_public_did(
             did=did,
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
             mediation_id=mediation_id,
         )
 
+    async def wallet_jwt_sign_post(
+        self, *, body: Optional[JWSCreate] = None
+    ) -> Dict[str, Any]:
+        """Create a EdDSA jws using did keys with a given payload"""
+        if not body:
+            body = JWSCreate()
+        return await self.__wallet_jwt_sign_post(
+            body=body,
+        )
+
+    async def wallet_jwt_verify_post(
+        self, *, body: Optional[JWSVerify] = None
+    ) -> JWSVerifyResponse:
+        """Verify a EdDSA jws using did keys with a given JWS"""
+        if not body:
+            body = JWSVerify()
+        return await self.__wallet_jwt_verify_post(
+            body=body,
+        )
+
     @returns.json
     @json
     @post("/wallet/did/create")
     def __create_did(self, *, body: Body(type=DIDCreate) = {}) -> DIDResult:
         """Internal uplink method for create_did"""
 
     @returns.json
@@ -152,7 +175,23 @@
         *,
         did: Query,
         conn_id: Query = None,
         create_transaction_for_endorser: Query = None,
         mediation_id: Query = None
     ) -> DIDResult:
         """Internal uplink method for set_public_did"""
+
+    @returns.json
+    @json
+    @post("/wallet/jwt/sign")
+    def __wallet_jwt_sign_post(
+        self, *, body: Body(type=JWSCreate) = {}
+    ) -> Dict[str, Any]:
+        """Internal uplink method for wallet_jwt_sign_post"""
+
+    @returns.json
+    @json
+    @post("/wallet/jwt/verify")
+    def __wallet_jwt_verify_post(
+        self, *, body: Body(type=JWSVerify) = {}
+    ) -> JWSVerifyResponse:
+        """Internal uplink method for wallet_jwt_verify_post"""
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/client.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/client.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/__init__.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,17 @@
     InvitationCreateRequest,
 )
 from aries_cloudcontroller.model.invitation_message import InvitationMessage
 from aries_cloudcontroller.model.invitation_record import InvitationRecord
 from aries_cloudcontroller.model.invitation_result import InvitationResult
 from aries_cloudcontroller.model.issuer_cred_rev_record import IssuerCredRevRecord
 from aries_cloudcontroller.model.issuer_rev_reg_record import IssuerRevRegRecord
+from aries_cloudcontroller.model.jws_create import JWSCreate
+from aries_cloudcontroller.model.jws_verify import JWSVerify
+from aries_cloudcontroller.model.jws_verify_response import JWSVerifyResponse
 from aries_cloudcontroller.model.keylist import Keylist
 from aries_cloudcontroller.model.keylist_query import KeylistQuery
 from aries_cloudcontroller.model.keylist_query_filter_request import (
     KeylistQueryFilterRequest,
 )
 from aries_cloudcontroller.model.keylist_query_paginate import KeylistQueryPaginate
 from aries_cloudcontroller.model.keylist_update import KeylistUpdate
@@ -543,14 +546,17 @@
     "InputDescriptors",
     "InvitationCreateRequest",
     "InvitationMessage",
     "InvitationRecord",
     "InvitationResult",
     "IssuerCredRevRecord",
     "IssuerRevRegRecord",
+    "JWSCreate",
+    "JWSVerify",
+    "JWSVerifyResponse",
     "Keylist",
     "KeylistQuery",
     "KeylistQueryFilterRequest",
     "KeylistQueryPaginate",
     "KeylistUpdate",
     "KeylistUpdateRequest",
     "KeylistUpdateRule",
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/action_menu_fetch_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/action_menu_fetch_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_config.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_config.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_mediation_deny.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_mediation_deny.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_modules.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_modules.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_status.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status_liveliness.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_status_liveliness.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/admin_status_readiness.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/admin_status_readiness.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/aml_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/aml_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator_data.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data1_jws.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator_data1_jws.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data_jws.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator_data_jws.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attach_decorator_data_jws_header.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attach_decorator_data_jws_header.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attachment_def.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attachment_def.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/attribute_mime_types_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/attribute_mime_types_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/claim_format.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/claim_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/clear_pending_revocations_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/clear_pending_revocations_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/conn_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/conn_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_invitation.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/receive_invitation_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class ConnectionInvitation(BaseModel):
+class ReceiveInvitationRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    ConnectionInvitation - a model defined in OpenAPI
+    ReceiveInvitationRequest - a model defined in OpenAPI
         id: Message identifier [Optional].
         type: Message type [Optional].
         did: DID for connection invitation [Optional].
         image_url: Optional image URL for connection invitation [Optional].
         label: Optional label for connection invitation [Optional].
         recipient_keys: List of recipient keys [Optional].
         routing_keys: List of routing keys [Optional].
@@ -37,17 +37,17 @@
 
     @validator("did")
     def did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$|^did:([a-zA-Z0-9_]+):([a-zA-Z0-9_.%-]+(:[a-zA-Z0-9_.%-]+)*)((;[a-zA-Z0-9_.:%-]+=[a-zA-Z0-9_.:%-]*)*)(\\/[^#?]*)?([?][^#]*)?(\#.*)?$$"
         if not re.match(pattern, value):
             raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-ConnectionInvitation.update_forward_refs()
+ReceiveInvitationRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_metadata.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_metadata.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_metadata_set_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_metadata_set_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_static_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_static_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/connection_static_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_static_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/constraints.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/constraints.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_invitation_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_invitation_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_wallet_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_wallet_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_token_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_wallet_token_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/create_wallet_token_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/create_wallet_token_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_attr_spec.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_def_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value_primary.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_def_value_primary.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_def_value_revocation.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_def_value_revocation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_info_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_info_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_indy_records_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_rev_indy_records_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_record_details_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_rev_record_details_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_rev_record_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_rev_record_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/cred_revoked_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/cred_revoked_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definition.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_get_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definition_get_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_send_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definition_send_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definition_send_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definition_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_definitions_created_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_definitions_created_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_offer.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_offer.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_preview.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_preview.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_proposal.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/credential_status_options.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/credential_status_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/date.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/date.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_create.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     DIDCreate - a model defined in OpenAPI
         method: Method for the requested DID.Supported methods are &#39;key&#39;, &#39;sov&#39;, and any other registered method. [Optional].
         options: To define a key type and/or a did depending on chosen DID method. [Optional].
         seed: Optional seed to use for DID, Must beenabled in configuration before use. [Optional].
     """
 
-    method: Optional[Literal["key", "sov"]] = None
+    method: Optional[str] = None
     options: Optional[DIDCreateOptions] = None
     seed: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_create_options.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_create_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_endpoint.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_endpoint.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_endpoint_with_type.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_endpoint_with_type.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/did_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/did_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/didx_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/didx_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,21 +18,25 @@
 
     DIDXRequest - a model defined in OpenAPI
         label: Label for DID exchange request.
         id: Message identifier [Optional].
         type: Message type [Optional].
         did: DID of exchange [Optional].
         did_docattach: As signed attachment, DID Doc associated with DID [Optional].
+        goal: A self-attested string that the receiver may want to display to the user about the context-specific goal of the out-of-band message [Optional].
+        goal_code: A self-attested code the receiver may want to display to the user or use in automatically deciding what to do with the out-of-band message [Optional].
     """
 
     label: str
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     did: Optional[str] = None
     did_docattach: Optional[AttachDecorator] = Field(None, alias="did_doc~attach")
+    goal: Optional[str] = None
+    goal_code: Optional[str] = None
 
     @validator("did")
     def did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_field.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_field.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_holder.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_holder.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_options.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_pres_spec.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_pres_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_proof_proposal.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_proof_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/dif_proof_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/dif_proof_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/disclose.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/disclose.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/disclosures.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/disclosures.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/doc.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/doc.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/endorser_info.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/endorser_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/endpoints_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/endpoints_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/filter.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/filter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/generated.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/generated.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_did_endpoint_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/get_did_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_did_verkey_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/get_did_verkey_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/get_nym_role_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/get_nym_role_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_attr_value.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_attr_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_abstract.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_cred_abstract.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_info.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_cred_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_precis.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_cred_precis.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_cred_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_cred_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_credential.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_credential.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_eq_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_eq_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_ge_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_ge_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_ge_proof_pred.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_ge_proof_pred.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_key_correctness_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_key_correctness_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_non_revoc_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_non_revoc_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_non_revocation_interval.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_non_revocation_interval.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_attr_spec.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_pres_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_pred_spec.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_pres_pred_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_preview.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_pres_preview.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_pres_spec.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_pres_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_primary_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_primary_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_identifier.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_identifier.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_attr_spec.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_req_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_pred_spec.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_req_pred_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_request_non_revoked.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_request_non_revoked.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_requested_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_def.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_def_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_entry.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_entry.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/indy_rev_reg_entry_value.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/indy_rev_reg_entry_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/input_descriptors.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/input_descriptors.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_create_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/invitation_create_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,25 +16,29 @@
 
     Do not edit the class manually.
 
     InvitationCreateRequest - a model defined in OpenAPI
         accept: List of mime type in order of preference that should be use in responding to the message [Optional].
         alias: Alias for connection [Optional].
         attachments: Optional invitation attachments [Optional].
+        goal: A self-attested string that the receiver may want to display to the user about the context-specific goal of the out-of-band message [Optional].
+        goal_code: A self-attested code the receiver may want to display to the user or use in automatically deciding what to do with the out-of-band message [Optional].
         handshake_protocols: The handshake_protocols of this InvitationCreateRequest [Optional].
         mediation_id: Identifier for active mediation record to be used [Optional].
         metadata: Optional metadata to attach to the connection created with the invitation [Optional].
         my_label: Label for connection invitation [Optional].
         protocol_version: OOB protocol version [Optional].
         use_public_did: Whether to use public DID in invitation [Optional].
     """
 
     accept: Optional[List[str]] = None
     alias: Optional[str] = None
     attachments: Optional[List[AttachmentDef]] = None
+    goal: Optional[str] = None
+    goal_code: Optional[str] = None
     handshake_protocols: Optional[List[str]] = None
     mediation_id: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
     my_label: Optional[str] = None
     protocol_version: Optional[str] = None
     use_public_did: Optional[bool] = None
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_message.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/invitation_message.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,24 +16,28 @@
 
     Do not edit the class manually.
 
     InvitationMessage - a model defined in OpenAPI
         id: Message identifier [Optional].
         type: Message type [Optional].
         accept: List of mime type in order of preference [Optional].
+        goal: A self-attested string that the receiver may want to display to the user about the context-specific goal of the out-of-band message [Optional].
+        goal_code: A self-attested code the receiver may want to display to the user or use in automatically deciding what to do with the out-of-band message [Optional].
         handshake_protocols: The handshake_protocols of this InvitationMessage [Optional].
         image_url: Optional image URL for out-of-band invitation [Optional].
         label: Optional label [Optional].
         requestsattach: Optional request attachment [Optional].
         services: The services of this InvitationMessage [Optional].
     """
 
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     accept: Optional[List[str]] = None
+    goal: Optional[str] = None
+    goal_code: Optional[str] = None
     handshake_protocols: Optional[List[str]] = None
     image_url: Optional[str] = Field(None, alias="imageUrl")
     label: Optional[str] = None
     requestsattach: Optional[List[AttachDecorator]] = Field(
         None, alias="requests~attach"
     )
     services: Optional[List[Union[Dict, str]]] = None
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/invitation_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/invitation_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/invitation_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/issuer_cred_rev_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/issuer_cred_rev_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/issuer_rev_reg_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/issuer_rev_reg_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_query.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query_filter_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_query_filter_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_query_paginate.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_query_paginate.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_update.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_update_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/keylist_update_rule.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/keylist_update_rule.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ld_proof_vc_detail.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ld_proof_vc_detail.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ld_proof_vc_detail_options.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ld_proof_vc_detail_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ledger_config_instance.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ledger_config_instance.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ledger_config_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ledger_config_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/linked_data_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/linked_data_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_create_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_create_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_deny.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_deny.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_grant.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_grant.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_id_match_info.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_id_match_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/mediation_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/mediation_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_form.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu_form.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_form_param.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu_form_param.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_json.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu_json.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/menu_option.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/menu_option.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/model_schema.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/model_schema.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/oob_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/oob_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/perform_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/perform_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ping_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ping_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/ping_request_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/ping_request_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_definition.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/presentation_definition.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_proposal.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/presentation_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/presentation_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/presentation_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/profile_settings.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/profile_settings.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/protocol_descriptor.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/publish_revocations.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/publish_revocations.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/queries.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/queries.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/query.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/query.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/query_item.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/query_item.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/raw_encoded.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/raw_encoded.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/receive_invitation_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/connection_invitation.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class ReceiveInvitationRequest(BaseModel):
+class ConnectionInvitation(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    ReceiveInvitationRequest - a model defined in OpenAPI
+    ConnectionInvitation - a model defined in OpenAPI
         id: Message identifier [Optional].
         type: Message type [Optional].
         did: DID for connection invitation [Optional].
         image_url: Optional image URL for connection invitation [Optional].
         label: Optional label for connection invitation [Optional].
         recipient_keys: List of recipient keys [Optional].
         routing_keys: List of routing keys [Optional].
@@ -37,17 +37,17 @@
 
     @validator("did")
     def did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$|^did:([a-zA-Z0-9_]+):([a-zA-Z0-9_.%-]+(:[a-zA-Z0-9_.%-]+)*)((;[a-zA-Z0-9_.:%-]+=[a-zA-Z0-9_.:%-]*)*)(\\/[^#?]*)?([?][^#]*)?(\#.*)?$$"
         if not re.match(pattern, value):
             raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-ReceiveInvitationRequest.update_forward_refs()
+ConnectionInvitation.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/remove_wallet_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/remove_wallet_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/resolution_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/resolution_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_create_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_create_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_issued_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_issued_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/rev_regs_created.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/rev_regs_created.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/revoke_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/revoke_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/route_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/route_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_get_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schema_get_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_input_descriptor.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schema_input_descriptor.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_send_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schema_send_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schema_send_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schema_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schemas_created_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schemas_created_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/schemas_input_descriptor_filter.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/schemas_input_descriptor_filter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/send_menu.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/send_menu.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/send_message.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/send_message.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/service_decorator.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/service_decorator.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/sign_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/sign_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/sign_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/sign_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/signature_options.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/signature_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/signed_doc.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/signed_doc.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/submission_requirements.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/submission_requirements.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_accept.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_accept.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_acceptance.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_acceptance.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_info.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/taa_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/taa_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/tails_delete_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/tails_delete_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_jobs.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/transaction_jobs.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/transaction_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/transaction_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/transaction_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_publish_revocations_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_publish_revocations_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_rev_reg_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_rev_reg_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/txn_or_schema_send_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/txn_or_schema_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/update_profile_settings.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/update_profile_settings.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/update_wallet_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/update_wallet_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_bound_offer_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_bound_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_create.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_create.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_exchange.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_exchange.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_exchange_list_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_exchange_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_free_offer_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_free_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_issue_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_issue_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_problem_report_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_credential_store_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_credential_store_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_discovery_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_discovery_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_create_request_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_create_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_exchange.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_exchange.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_exchange_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_exchange_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_problem_report_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_proposal_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_proposal_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_send_request_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_send_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_attr_spec.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_bound_offer_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_bound_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_free.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_free.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 
     V20CredExFree - a model defined in OpenAPI
         connection_id: Connection identifier.
         filter: Credential specification criteria by format.
         auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
         comment: Human-readable comment [Optional].
         credential_preview: The credential_preview of this V20CredExFree [Optional].
+        replacement_id: Optional identifier used to manage credential replacement [Optional].
         trace: Record trace information, based on agent configuration [Optional].
         verification_method: For ld-proofs. Verification method for signing. [Optional].
     """
 
     connection_id: str
     filter: V20CredFilter
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
+    replacement_id: Optional[str] = None
     trace: Optional[bool] = None
     verification_method: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_detail.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_detail.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_indy.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_indy.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_filter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter_indy.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_filter_indy.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_format.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_issue.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_issue_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_issue_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_offer.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 
     V20CredOfferConnFreeRequest - a model defined in OpenAPI
         filter: Credential specification criteria by format.
         auto_issue: Whether to respond automatically to credential requests, creating and issuing requested credentials [Optional].
         auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
         comment: Human-readable comment [Optional].
         credential_preview: The credential_preview of this V20CredOfferConnFreeRequest [Optional].
+        replacement_id: Optional identifier used to manage credential replacement [Optional].
         trace: Record trace information, based on agent configuration [Optional].
     """
 
     filter: V20CredFilter
     auto_issue: Optional[bool] = None
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
+    replacement_id: Optional[str] = None
     trace: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredOfferConnFreeRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_offer_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_offer_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,23 +20,25 @@
     V20CredOfferRequest - a model defined in OpenAPI
         connection_id: Connection identifier.
         filter: Credential specification criteria by format.
         auto_issue: Whether to respond automatically to credential requests, creating and issuing requested credentials [Optional].
         auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
         comment: Human-readable comment [Optional].
         credential_preview: The credential_preview of this V20CredOfferRequest [Optional].
+        replacement_id: Optional identifier used to manage credential replacement [Optional].
         trace: Record trace information, based on agent configuration [Optional].
     """
 
     connection_id: str
     filter: V20CredFilter
     auto_issue: Optional[bool] = None
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
+    replacement_id: Optional[str] = None
     trace: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredOfferRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_preview.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_preview.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_proposal.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request_free.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_request_free.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_request_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_cred_store_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_cred_store_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_exchange_result.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_discovery_exchange_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_discovery_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_discovery_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_issue_cred_schema_core.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_issue_cred_schema_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,21 +18,23 @@
     Do not edit the class manually.
 
     V20IssueCredSchemaCore - a model defined in OpenAPI
         filter: Credential specification criteria by format.
         auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
         comment: Human-readable comment [Optional].
         credential_preview: The credential_preview of this V20IssueCredSchemaCore [Optional].
+        replacement_id: Optional identifier used to manage credential replacement [Optional].
         trace: Record trace information, based on agent configuration [Optional].
     """
 
     filter: V20CredFilter
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
+    replacement_id: Optional[str] = None
     trace: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
 V20IssueCredSchemaCore.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_create_request_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_create_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_ex_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_ex_record_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_ex_record_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_format.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_problem_report_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal_by_format.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_proposal_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_proposal_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_proposal_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_request_by_format.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_request_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_send_request_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_send_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/vc_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/vc_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/vc_record_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/vc_record_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/verify_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/verify_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/verify_response.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/verify_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/w3_c_credentials_list_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/w3_c_credentials_list_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/wallet_list.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/wallet_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/wallet_record.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/wallet_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/model/write_ledger_request.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/model/write_ledger_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/acapy_client_session.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/util/acapy_client_session.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller/util/pydantic_converter.py` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller/util/pydantic_converter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/PKG-INFO` & `aries_cloudcontroller-0.9.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: aries-cloudcontroller
-Version: 0.8.2b0
+Name: aries_cloudcontroller
+Version: 0.9.0b0
 Summary: A simple python package for controlling an aries agent through the admin-api interface
 Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <br />
   <img
     alt="Hyperledger Aries logo"
@@ -56,21 +56,23 @@
 | Aries Cloud Controller Version | Aries Cloud Agent Python Version |
 | ------------------------------ | -------------------------------- |
 | 0.5.1-0.5.2                    | 0.7.3                            |
 | 0.6.0-0.6.3                    | 0.7.4                            |
 | 0.7.0                          | 0.7.5                            |
 | 0.8.0                          | 0.8.0                            |
 | 0.8.1                          | 0.8.1                            |
+| 0.8.2                          | 0.8.2                            |
+| 0.9.0                          | 0.9.0                            |
 
 ## Features
 
 Aries Cloud Controller Python is a fully featured client for interacting with ACA-Py.
 
 - Fully Typed wrapper around Aries Cloud Agent Python
-- Supports latest ACA-Py version (0.8.1)
+- Supports latest ACA-Py version (0.9.0)
 - Client is auto generated based on OpenAPI definitions, allowing us to keep up to date with new releases.
 - Supports multi-tenant APIs and authentication
 - Async API
 
 ## Usage
 
 Aries Cloud Controller Python is published to PyPi and can be installed using pip:
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.8.2b0 Summary: A
+Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.9.0b0 Summary: A
 simple python package for controlling an aries agent through the admin-api
 interface Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/
 tree/main/aries_cloudcontroller Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
+Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE
 
                            [Hyperledger Aries logo]
                   ****** Aries Cloud Controller Python ******
      [Pipeline Status] [aries-cloudcontroller_version] [License] [Python]
 
       Features  |  Usage  |  Available_APIs  |  Contributing  |  License
@@ -17,30 +17,30 @@
 definition provided by ACA-Py, giving a fully-typed rich API for interacting
 the cloud agent. Each Cloud Controller version maps to a specific ACA-Py
 version, which is outlined in the table below. Although not strictly adhered to
 in the past, a new ACA-Py version will result in a new Minor version bump for
 the Cloud Controller, as there are often times breaking changes. | Aries Cloud
 Controller Version | Aries Cloud Agent Python Version | | ---------------------
 --------- | -------------------------------- | | 0.5.1-0.5.2 | 0.7.3 | | 0.6.0-
-0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | | 0.8.1 | 0.8.1 | ##
-Features Aries Cloud Controller Python is a fully featured client for
-interacting with ACA-Py. - Fully Typed wrapper around Aries Cloud Agent Python
-- Supports latest ACA-Py version (0.8.1) - Client is auto generated based on
-OpenAPI definitions, allowing us to keep up to date with new releases. -
-Supports multi-tenant APIs and authentication - Async API ## Usage Aries Cloud
-Controller Python is published to PyPi and can be installed using pip: ```sh
-pip install aries-cloudcontroller ``` ### Creating a client ```python from
-aries_cloudcontroller import AcaPyClient client = AcaPyClient( base_url="http:/
-/localhost:8000", api_key="myApiKey" ) ``` **Admin insecure mode** If you are
-running ACA-Py with the admin insecure flag and don't have the API key, you
-must set the `admin_insecure` property: ```python client = AcaPyClient
-( base_url="http://localhost:8000", # Explicitly mark that no api key is used
-admin_insecure=True ) ``` **Multitenancy** To provision the agent in the
-context of specific tenant of the agent, the `tenant_jwt` property must be set:
-```python client = AcaPyClient( base_url="http://localhost:8000",
+0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | | 0.8.1 | 0.8.1 | | 0.8.2 |
+0.8.2 | | 0.9.0 | 0.9.0 | ## Features Aries Cloud Controller Python is a fully
+featured client for interacting with ACA-Py. - Fully Typed wrapper around Aries
+Cloud Agent Python - Supports latest ACA-Py version (0.9.0) - Client is auto
+generated based on OpenAPI definitions, allowing us to keep up to date with new
+releases. - Supports multi-tenant APIs and authentication - Async API ## Usage
+Aries Cloud Controller Python is published to PyPi and can be installed using
+pip: ```sh pip install aries-cloudcontroller ``` ### Creating a client
+```python from aries_cloudcontroller import AcaPyClient client = AcaPyClient
+( base_url="http://localhost:8000", api_key="myApiKey" ) ``` **Admin insecure
+mode** If you are running ACA-Py with the admin insecure flag and don't have
+the API key, you must set the `admin_insecure` property: ```python client =
+AcaPyClient( base_url="http://localhost:8000", # Explicitly mark that no api
+key is used admin_insecure=True ) ``` **Multitenancy** To provision the agent
+in the context of specific tenant of the agent, the `tenant_jwt` property must
+be set: ```python client = AcaPyClient( base_url="http://localhost:8000",
 tenant_jwt="eyXXX" ) ``` ### Interacting with the client Once you have the
 client set up, you're ready to interact with it. Because the API is fully
 typed, the best way to know what is available is by looking at the ACA-Py
 swagger UI, and the available properties on the client. For example to create
 and receive an invitation the following methods can be called: ```python
 invitation = await client.connection.create_invitation
 ( body=CreateInvitationRequest(my_label="Cloud Controller") ) connection =
```

### Comparing `aries_cloudcontroller-0.8.2b0/aries_cloudcontroller.egg-info/SOURCES.txt` & `aries_cloudcontroller-0.9.0b0/aries_cloudcontroller.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,17 @@
 aries_cloudcontroller/model/input_descriptors.py
 aries_cloudcontroller/model/invitation_create_request.py
 aries_cloudcontroller/model/invitation_message.py
 aries_cloudcontroller/model/invitation_record.py
 aries_cloudcontroller/model/invitation_result.py
 aries_cloudcontroller/model/issuer_cred_rev_record.py
 aries_cloudcontroller/model/issuer_rev_reg_record.py
+aries_cloudcontroller/model/jws_create.py
+aries_cloudcontroller/model/jws_verify.py
+aries_cloudcontroller/model/jws_verify_response.py
 aries_cloudcontroller/model/keylist.py
 aries_cloudcontroller/model/keylist_query.py
 aries_cloudcontroller/model/keylist_query_filter_request.py
 aries_cloudcontroller/model/keylist_query_paginate.py
 aries_cloudcontroller/model/keylist_update.py
 aries_cloudcontroller/model/keylist_update_request.py
 aries_cloudcontroller/model/keylist_update_rule.py
```

### Comparing `aries_cloudcontroller-0.8.2b0/setup.py` & `aries_cloudcontroller-0.9.0b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,28 @@
     lineiter = (line.strip() for line in open(filename))
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 if __name__ == "__main__":
     setup(
         name=PACKAGE_NAME,
-        version="0.8.2-beta0",
+        version="0.9.0-beta0",
         description="A simple python package for controlling an aries agent through the admin-api interface",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller",
         packages=find_packages(),
         include_package_data=True,
         package_data={
             "aries_cloudcontroller": [
                 "requirements.txt",
             ]
         },
         tests_require=parse_requirements("requirements.dev.txt"),
         install_requires=parse_requirements("requirements.txt"),
-        python_requires=">=3.8",
+        python_requires=">=3.9",
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
     )
```

### Comparing `aries_cloudcontroller-0.8.2b0/tests/client/test_acapy_client.py` & `aries_cloudcontroller-0.9.0b0/tests/client/test_acapy_client.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/tests/client/test_pydantic_converter.py` & `aries_cloudcontroller-0.9.0b0/tests/client/test_pydantic_converter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/tests/model/test_credential_offer.py` & `aries_cloudcontroller-0.9.0b0/tests/model/test_credential_offer.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/tests/model/test_invitation.py` & `aries_cloudcontroller-0.9.0b0/tests/model/test_invitation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/tests/model/test_presentation.py` & `aries_cloudcontroller-0.9.0b0/tests/model/test_presentation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/tests/model/test_v20_cred_ex_record.py` & `aries_cloudcontroller-0.9.0b0/tests/model/test_v20_cred_ex_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/tests/model/test_v20_pres_ex_record.py` & `aries_cloudcontroller-0.9.0b0/tests/model/test_v20_pres_ex_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.2b0/tests/util/compare_dicts.py` & `aries_cloudcontroller-0.9.0b0/tests/util/compare_dicts.py`

 * *Files identical despite different names*

