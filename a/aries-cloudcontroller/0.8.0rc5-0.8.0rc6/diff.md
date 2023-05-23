# Comparing `tmp/aries_cloudcontroller-0.8.0rc5.tar.gz` & `tmp/aries_cloudcontroller-0.8.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aries_cloudcontroller-0.8.0rc5.tar", last modified: Tue Apr  4 09:31:55 2023, max compression
+gzip compressed data, was "aries_cloudcontroller-0.8.0rc6.tar", last modified: Tue May 23 08:57:29 2023, max compression
```

## Comparing `aries_cloudcontroller-0.8.0rc5.tar` & `aries_cloudcontroller-0.8.0rc6.tar`

### file list

```diff
@@ -1,329 +1,326 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:55.714633 aries_cloudcontroller-0.8.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-04-04 09:31:55.714633 aries_cloudcontroller-0.8.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:55.674632 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/acapy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:55.682633 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/action_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/basicmessage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/did_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/discover_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/discover_features_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/endorse_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/introduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/issue_credential_v1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/issue_credential_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/jsonld.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/ledger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/mediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/multitenancy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/out_of_band.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/present_proof_v1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/present_proof_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/trustping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:55.710633 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/
--rw-r--r--   0 runner    (1001) docker     (123)    29643 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/action_menu_fetch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_api_message_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_status_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_status_readiness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/aml_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator_data1_jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator_data_jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator_data_jws_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attachment_def.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attribute_mime_types_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/claim_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/clear_pending_revocations_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/conn_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_metadata_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_static_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_static_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_wallet_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_wallet_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_def_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_def_value_primary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_def_value_revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_info_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_rev_indy_records_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_rev_record_details_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_rev_record_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_revoked_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definition_get_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definition_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definitions_created_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_status_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_endpoint_with_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/didx_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_proof_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/disclose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/disclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/endorser_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/endpoints_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/generated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/get_did_endpoint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/get_did_verkey_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/get_nym_role_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_attr_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_cred_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_cred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_cred_precis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_eq_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_ge_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_ge_proof_pred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_key_correctness_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_non_revoc_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_non_revocation_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_pres_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_pres_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_pres_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_primary_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_req_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_req_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_request_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_requested_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_def_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_entry_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/input_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/invitation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/invitation_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/invitation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/invitation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/issuer_cred_rev_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/issuer_rev_reg_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_query_filter_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_query_paginate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_update_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ld_proof_vc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ld_proof_vc_detail_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ledger_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ledger_config_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/linked_data_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu_form_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/model_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/oob_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/perform_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ping_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ping_request_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/presentation_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/presentation_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/presentation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/protocol_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/publish_revocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/query_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/raw_encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/receive_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/register_ledger_nym_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/remove_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/resolution_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_issued_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_regs_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/revoke_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/route_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schema_get_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schema_input_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schema_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schemas_created_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schemas_input_descriptor_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/send_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/service_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/sign_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/sign_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/signature_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/signed_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/submission_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_accept.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/transaction_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/transaction_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/transaction_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_publish_revocations_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/update_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_store_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_discovery_exchange_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_exchange_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_indy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_filter_indy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_request_free.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_store_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_discovery_exchange_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_issue_cred_schema_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_ex_record_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_proposal_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_request_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/vc_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/vc_record_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/verify_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/verify_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/w3_c_credentials_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/wallet_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/write_ledger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/uplink_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:55.710633 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/util/pydantic_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:55.674632 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-04-04 09:31:55.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-04-04 09:31:55.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 09:31:55.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-04 09:31:55.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-04 09:31:55.000000 aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 09:31:55.714633 aries_cloudcontroller-0.8.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:55.714633 aries_cloudcontroller-0.8.0rc5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:55.714633 aries_cloudcontroller-0.8.0rc5/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/tests/model/test_presentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-04 09:31:44.000000 aries_cloudcontroller-0.8.0rc5/tests/test_acapy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:29.146462 aries_cloudcontroller-0.8.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-23 08:57:29.146462 aries_cloudcontroller-0.8.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:29.118461 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/acapy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:29.122461 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/action_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/basicmessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/did_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/discover_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/discover_features_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/endorse_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/issue_credential_v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/issue_credential_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/ledger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/mediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/multitenancy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/out_of_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/present_proof_v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/present_proof_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/trustping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:29.146462 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    29725 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/action_menu_fetch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_status_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_status_readiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/aml_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator_data1_jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator_data_jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator_data_jws_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attachment_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attribute_mime_types_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/claim_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/clear_pending_revocations_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/conn_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_metadata_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_static_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_static_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_wallet_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_wallet_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_def_value_primary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_def_value_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_info_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_rev_indy_records_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_rev_record_details_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_rev_record_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_revoked_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definition_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definition_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definitions_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_status_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_endpoint_with_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/didx_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_proof_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/disclose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/disclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/endorser_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/endpoints_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/get_did_endpoint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/get_did_verkey_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/get_nym_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_attr_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_cred_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_cred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_cred_precis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_eq_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_ge_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_ge_proof_pred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_key_correctness_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_non_revoc_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_non_revocation_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_pres_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_pres_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_pres_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_primary_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_req_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_req_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_request_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_requested_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_entry_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/input_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/invitation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/invitation_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/invitation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/invitation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/issuer_cred_rev_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/issuer_rev_reg_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_query_filter_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_query_paginate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_update_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ld_proof_vc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ld_proof_vc_detail_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ledger_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ledger_config_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/linked_data_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_id_match_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu_form_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/model_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/oob_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/perform_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ping_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ping_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/presentation_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/presentation_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/presentation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/protocol_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/publish_revocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/query_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/raw_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/receive_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/remove_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/resolution_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_issued_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_regs_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/revoke_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/route_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schema_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schema_input_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schema_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schemas_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schemas_input_descriptor_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/send_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/service_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/sign_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/sign_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/signature_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/signed_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/submission_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_accept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/tails_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/transaction_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/transaction_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/transaction_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_publish_revocations_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/update_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_exchange_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_indy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_filter_indy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_request_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_discovery_exchange_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_issue_cred_schema_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_ex_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_proposal_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_request_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/vc_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/vc_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/verify_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/verify_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/w3_c_credentials_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/wallet_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/write_ledger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/uplink_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:29.146462 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/util/pydantic_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:29.118461 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-23 08:57:29.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-05-23 08:57:29.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:57:29.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 08:57:29.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 08:57:29.000000 aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:57:29.146462 aries_cloudcontroller-0.8.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:29.146462 aries_cloudcontroller-0.8.0rc6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:29.146462 aries_cloudcontroller-0.8.0rc6/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/tests/model/test_presentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-23 08:57:18.000000 aries_cloudcontroller-0.8.0rc6/tests/test_acapy_client.py
```

### Comparing `aries_cloudcontroller-0.8.0rc5/LICENSE` & `aries_cloudcontroller-0.8.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/PKG-INFO` & `aries_cloudcontroller-0.8.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aries_cloudcontroller
-Version: 0.8.0rc5
+Version: 0.8.0rc6
 Summary: A simple python package for controlling an aries agent through the admin-api interface
 Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.8.0rc5 Summary: A
+Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.8.0rc6 Summary: A
 simple python package for controlling an aries agent through the admin-api
 interface Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/
 tree/main/aries_cloudcontroller Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `aries_cloudcontroller-0.8.0rc5/README.md` & `aries_cloudcontroller-0.8.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/__init__.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,15 @@
     LDProofVCDetailOptions,
     LedgerConfigInstance,
     LedgerConfigList,
     LinkedDataProof,
     MediationCreateRequest,
     MediationDeny,
     MediationGrant,
+    MediationIdMatchInfo,
     MediationList,
     MediationRecord,
     Menu,
     MenuForm,
     MenuFormParam,
     MenuJson,
     MenuOption,
@@ -213,14 +214,15 @@
     SignedDoc,
     SubmissionRequirements,
     TAAAccept,
     TAAAcceptance,
     TAAInfo,
     TAARecord,
     TAAResult,
+    TailsDeleteResponse,
     TransactionJobs,
     TransactionList,
     TransactionRecord,
     TxnOrCredentialDefinitionSendResult,
     TxnOrPublishRevocationsResult,
     TxnOrRegisterLedgerNymResponse,
     TxnOrRevRegResult,
@@ -234,15 +236,14 @@
     V10CredentialFreeOfferRequest,
     V10CredentialIssueRequest,
     V10CredentialProblemReportRequest,
     V10CredentialProposalRequestMand,
     V10CredentialProposalRequestOpt,
     V10CredentialStoreRequest,
     V10DiscoveryExchangeListResult,
-    V10DiscoveryExchangeResult,
     V10DiscoveryRecord,
     V10PresentationCreateRequestRequest,
     V10PresentationExchange,
     V10PresentationExchangeList,
     V10PresentationProblemReportRequest,
     V10PresentationProposalRequest,
     V10PresentationSendRequestRequest,
@@ -435,14 +436,15 @@
     "LDProofVCDetailOptions",
     "LedgerConfigInstance",
     "LedgerConfigList",
     "LinkedDataProof",
     "MediationCreateRequest",
     "MediationDeny",
     "MediationGrant",
+    "MediationIdMatchInfo",
     "MediationList",
     "MediationRecord",
     "Menu",
     "MenuForm",
     "MenuFormParam",
     "MenuJson",
     "MenuOption",
@@ -486,14 +488,15 @@
     "SignedDoc",
     "SubmissionRequirements",
     "TAAAccept",
     "TAAAcceptance",
     "TAAInfo",
     "TAARecord",
     "TAAResult",
+    "TailsDeleteResponse",
     "TransactionJobs",
     "TransactionList",
     "TransactionRecord",
     "TxnOrCredentialDefinitionSendResult",
     "TxnOrPublishRevocationsResult",
     "TxnOrRegisterLedgerNymResponse",
     "TxnOrRevRegResult",
@@ -507,15 +510,14 @@
     "V10CredentialFreeOfferRequest",
     "V10CredentialIssueRequest",
     "V10CredentialProblemReportRequest",
     "V10CredentialProposalRequestMand",
     "V10CredentialProposalRequestOpt",
     "V10CredentialStoreRequest",
     "V10DiscoveryExchangeListResult",
-    "V10DiscoveryExchangeResult",
     "V10DiscoveryRecord",
     "V10PresentationCreateRequestRequest",
     "V10PresentationExchange",
     "V10PresentationExchangeList",
     "V10PresentationProblemReportRequest",
     "V10PresentationProposalRequest",
     "V10PresentationSendRequestRequest",
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/acapy_client.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/acapy_client.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/__init__.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/action_menu.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/action_menu.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/basicmessage.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/basicmessage.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/connection.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/connection.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/credential_definition.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/credential_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 
 from aries_cloudcontroller.model.credential_definition_get_result import (
     CredentialDefinitionGetResult,
 )
 from aries_cloudcontroller.model.credential_definition_send_request import (
     CredentialDefinitionSendRequest,
 )
-from aries_cloudcontroller.model.credential_definition_send_result import (
-    CredentialDefinitionSendResult,
-)
 from aries_cloudcontroller.model.credential_definitions_created_result import (
     CredentialDefinitionsCreatedResult,
 )
 from aries_cloudcontroller.model.txn_or_credential_definition_send_result import (
     TxnOrCredentialDefinitionSendResult,
 )
 
@@ -71,15 +68,15 @@
 
     async def publish_cred_def(
         self,
         *,
         conn_id: Optional[str] = None,
         create_transaction_for_endorser: Optional[bool] = None,
         body: Optional[CredentialDefinitionSendRequest] = None
-    ) -> Union[CredentialDefinitionSendResult, TxnOrCredentialDefinitionSendResult]:
+    ) -> TxnOrCredentialDefinitionSendResult:
         """Sends a credential definition to the ledger"""
         return await self.__publish_cred_def(
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
             body=body,
         )
 
@@ -114,9 +111,9 @@
     @post("/credential-definitions")
     def __publish_cred_def(
         self,
         *,
         conn_id: Query = None,
         create_transaction_for_endorser: Query = None,
         body: Body(type=CredentialDefinitionSendRequest) = {}
-    ) -> Union[CredentialDefinitionSendResult, TxnOrCredentialDefinitionSendResult]:
+    ) -> TxnOrCredentialDefinitionSendResult:
         """Internal uplink method for publish_cred_def"""
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/credentials.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/credentials.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/did_exchange.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/did_exchange.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/discover_features.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/discover_features.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,27 +16,25 @@
 from typing import Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.v10_discovery_exchange_list_result import (
     V10DiscoveryExchangeListResult,
 )
-from aries_cloudcontroller.model.v10_discovery_exchange_result import (
-    V10DiscoveryExchangeResult,
-)
+from aries_cloudcontroller.model.v10_discovery_record import V10DiscoveryRecord
 
 
 class DiscoverFeaturesApi(Consumer):
     async def discover_features_query_get(
         self,
         *,
         comment: Optional[str] = None,
         connection_id: Optional[str] = None,
         query: Optional[str] = None
-    ) -> V10DiscoveryExchangeResult:
+    ) -> V10DiscoveryRecord:
         """Query supported features"""
         return await self.__discover_features_query_get(
             comment=comment,
             connection_id=connection_id,
             query=query,
         )
 
@@ -48,15 +46,15 @@
             connection_id=connection_id,
         )
 
     @returns.json
     @get("/discover-features/query")
     def __discover_features_query_get(
         self, *, comment: Query = None, connection_id: Query = None, query: Query = None
-    ) -> V10DiscoveryExchangeResult:
+    ) -> V10DiscoveryRecord:
         """Internal uplink method for discover_features_query_get"""
 
     @returns.json
     @get("/discover-features/records")
     def __discover_features_records_get(
         self, *, connection_id: Query = None
     ) -> V10DiscoveryExchangeListResult:
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/discover_features_v2_0.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/discover_features_v2_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/endorse_transaction.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/endorse_transaction.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/introduction.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/introduction.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/issue_credential_v1_0.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/issue_credential_v1_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 )
 
 
 class IssueCredentialV10Api(Consumer):
     async def create_credential(
         self, *, body: Optional[V10CredentialCreate] = None
     ) -> V10CredentialExchange:
-        """Send holder a credential, automating entire flow"""
+        """Create a credential record without sending (generally for use with Out-Of-Band)"""
         return await self.__create_credential(
             body=body,
         )
 
     async def create_offer(
         self, *, body: Optional[V10CredentialConnFreeOfferRequest] = None
     ) -> V10CredentialExchange:
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/issue_credential_v2_0.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/issue_credential_v2_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 )
 
 
 class IssueCredentialV20Api(Consumer):
     async def create_credential(
         self, *, body: Optional[V20IssueCredSchemaCore] = None
     ) -> V20CredExRecord:
-        """Create credential from attribute values"""
+        """Create a credential record without sending (generally for use with Out-Of-Band)"""
         return await self.__create_credential(
             body=body,
         )
 
     async def delete_record(self, *, cred_ex_id: str) -> Dict:
         """Remove an existing credential exchange record"""
         return await self.__delete_record(
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/jsonld.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/jsonld.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/ledger.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/ledger.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/mediation.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/mediation.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     KeylistQueryFilterRequest,
 )
 from aries_cloudcontroller.model.keylist_update import KeylistUpdate
 from aries_cloudcontroller.model.keylist_update_request import KeylistUpdateRequest
 from aries_cloudcontroller.model.mediation_create_request import MediationCreateRequest
 from aries_cloudcontroller.model.mediation_deny import MediationDeny
 from aries_cloudcontroller.model.mediation_grant import MediationGrant
+from aries_cloudcontroller.model.mediation_id_match_info import MediationIdMatchInfo
 from aries_cloudcontroller.model.mediation_list import MediationList
 from aries_cloudcontroller.model.mediation_record import MediationRecord
 
 
 class MediationApi(Consumer):
     async def clear_default_mediator(self) -> MediationRecord:
         """Clear default mediator"""
@@ -80,14 +81,23 @@
 
     async def grant_mediation_request(self, *, mediation_id: str) -> MediationGrant:
         """Grant received mediation"""
         return await self.__grant_mediation_request(
             mediation_id=mediation_id,
         )
 
+    async def mediation_update_keylist_conn_id_post(
+        self, *, conn_id: str, body: Optional[MediationIdMatchInfo] = None
+    ) -> KeylistUpdate:
+        """Update keylist for a connection"""
+        return await self.__mediation_update_keylist_conn_id_post(
+            conn_id=conn_id,
+            body=body,
+        )
+
     async def request_mediation(
         self, *, conn_id: str, body: Optional[MediationCreateRequest] = None
     ) -> MediationRecord:
         """Request mediation from connection"""
         return await self.__request_mediation(
             conn_id=conn_id,
             body=body,
@@ -176,14 +186,22 @@
     @returns.json
     @post("/mediation/requests/{mediation_id}/grant")
     def __grant_mediation_request(self, *, mediation_id: str) -> MediationGrant:
         """Internal uplink method for grant_mediation_request"""
 
     @returns.json
     @json
+    @post("/mediation/update-keylist/{conn_id}")
+    def __mediation_update_keylist_conn_id_post(
+        self, *, conn_id: str, body: Body(type=MediationIdMatchInfo) = {}
+    ) -> KeylistUpdate:
+        """Internal uplink method for mediation_update_keylist_conn_id_post"""
+
+    @returns.json
+    @json
     @post("/mediation/request/{conn_id}")
     def __request_mediation(
         self, *, conn_id: str, body: Body(type=MediationCreateRequest) = {}
     ) -> MediationRecord:
         """Internal uplink method for request_mediation"""
 
     @returns.json
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/multitenancy.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/multitenancy.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/out_of_band.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/out_of_band.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/present_proof_v1_0.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/present_proof_v1_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/present_proof_v2_0.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/present_proof_v2_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/resolver.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/resolver.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/revocation.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/revocation.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     RevRegUpdateTailsFileUri,
 )
 from aries_cloudcontroller.model.rev_reg_wallet_updated_result import (
     RevRegWalletUpdatedResult,
 )
 from aries_cloudcontroller.model.rev_regs_created import RevRegsCreated
 from aries_cloudcontroller.model.revoke_request import RevokeRequest
+from aries_cloudcontroller.model.tails_delete_response import TailsDeleteResponse
 from aries_cloudcontroller.model.txn_or_publish_revocations_result import (
     TxnOrPublishRevocationsResult,
 )
 from aries_cloudcontroller.model.txn_or_rev_reg_result import TxnOrRevRegResult
 
 
 class RevocationApi(Consumer):
@@ -115,15 +116,15 @@
 
     async def publish_rev_reg_def(
         self,
         *,
         rev_reg_id: str,
         conn_id: Optional[str] = None,
         create_transaction_for_endorser: Optional[bool] = None
-    ) -> Union[RevRegResult, TxnOrRevRegResult]:
+    ) -> TxnOrRevRegResult:
         """Send revocation registry definition to ledger"""
         return await self.__publish_rev_reg_def(
             rev_reg_id=rev_reg_id,
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
         )
 
@@ -139,20 +140,29 @@
             rev_reg_id=rev_reg_id,
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
         )
 
     async def publish_revocations(
         self, *, body: Optional[PublishRevocations] = None
-    ) -> Union[PublishRevocations, TxnOrPublishRevocationsResult]:
+    ) -> TxnOrPublishRevocationsResult:
         """Publish pending revocations to ledger"""
         return await self.__publish_revocations(
             body=body,
         )
 
+    async def revocation_registry_delete_tails_file_delete(
+        self, *, cred_def_id: Optional[str] = None, rev_reg_id: Optional[str] = None
+    ) -> TailsDeleteResponse:
+        """Delete the tail files"""
+        return await self.__revocation_registry_delete_tails_file_delete(
+            cred_def_id=cred_def_id,
+            rev_reg_id=rev_reg_id,
+        )
+
     async def revocation_registry_rev_reg_id_fix_revocation_entry_state_put(
         self, *, rev_reg_id: str, apply_ledger_update: bool
     ) -> RevRegWalletUpdatedResult:
         """Fix revocation state in wallet and return number of updated entries"""
         return (
             await self.__revocation_registry_rev_reg_id_fix_revocation_entry_state_put(
                 rev_reg_id=rev_reg_id,
@@ -263,15 +273,15 @@
     @post("/revocation/registry/{rev_reg_id}/definition")
     def __publish_rev_reg_def(
         self,
         *,
         rev_reg_id: str,
         conn_id: Query = None,
         create_transaction_for_endorser: Query = None
-    ) -> Union[RevRegResult, TxnOrRevRegResult]:
+    ) -> TxnOrRevRegResult:
         """Internal uplink method for publish_rev_reg_def"""
 
     @returns.json
     @post("/revocation/registry/{rev_reg_id}/entry")
     def __publish_rev_reg_entry(
         self,
         *,
@@ -282,18 +292,25 @@
         """Internal uplink method for publish_rev_reg_entry"""
 
     @returns.json
     @json
     @post("/revocation/publish-revocations")
     def __publish_revocations(
         self, *, body: Body(type=PublishRevocations) = {}
-    ) -> Union[PublishRevocations, TxnOrPublishRevocationsResult]:
+    ) -> TxnOrPublishRevocationsResult:
         """Internal uplink method for publish_revocations"""
 
     @returns.json
+    @delete("/revocation/registry/delete-tails-file")
+    def __revocation_registry_delete_tails_file_delete(
+        self, *, cred_def_id: Query = None, rev_reg_id: Query = None
+    ) -> TailsDeleteResponse:
+        """Internal uplink method for revocation_registry_delete_tails_file_delete"""
+
+    @returns.json
     @put("/revocation/registry/{rev_reg_id}/fix-revocation-entry-state")
     def __revocation_registry_rev_reg_id_fix_revocation_entry_state_put(
         self, *, rev_reg_id: str, apply_ledger_update: Query
     ) -> RevRegWalletUpdatedResult:
         """Internal uplink method for revocation_registry_rev_reg_id_fix_revocation_entry_state_put"""
 
     @returns.json
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/schema.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 from typing import Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.schema_get_result import SchemaGetResult
 from aries_cloudcontroller.model.schema_send_request import SchemaSendRequest
-from aries_cloudcontroller.model.schema_send_result import SchemaSendResult
 from aries_cloudcontroller.model.schemas_created_result import SchemasCreatedResult
 from aries_cloudcontroller.model.txn_or_schema_send_result import TxnOrSchemaSendResult
 
 
 class SchemaApi(Consumer):
     async def get_created_schemas(
         self,
@@ -49,15 +48,15 @@
 
     async def publish_schema(
         self,
         *,
         conn_id: Optional[str] = None,
         create_transaction_for_endorser: Optional[bool] = None,
         body: Optional[SchemaSendRequest] = None
-    ) -> Union[SchemaSendResult, TxnOrSchemaSendResult]:
+    ) -> TxnOrSchemaSendResult:
         """Sends a schema to the ledger"""
         return await self.__publish_schema(
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
             body=body,
         )
 
@@ -89,14 +88,14 @@
     @post("/schemas")
     def __publish_schema(
         self,
         *,
         conn_id: Query = None,
         create_transaction_for_endorser: Query = None,
         body: Body(type=SchemaSendRequest) = {}
-    ) -> Union[SchemaSendResult, TxnOrSchemaSendResult]:
+    ) -> TxnOrSchemaSendResult:
         """Internal uplink method for publish_schema"""
 
     @returns.json
     @post("/schemas/{schema_id}/write_record")
     def __write_record(self, *, schema_id: str) -> SchemaGetResult:
         """Internal uplink method for write_record"""
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/server.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/server.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/trustping.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/trustping.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/api/wallet.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/api/wallet.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,21 +80,23 @@
         )
 
     async def set_public_did(
         self,
         *,
         did: str,
         conn_id: Optional[str] = None,
-        create_transaction_for_endorser: Optional[bool] = None
+        create_transaction_for_endorser: Optional[bool] = None,
+        mediation_id: Optional[str] = None
     ) -> DIDResult:
         """Assign the current public DID"""
         return await self.__set_public_did(
             did=did,
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
+            mediation_id=mediation_id,
         )
 
     @returns.json
     @json
     @post("/wallet/did/create")
     def __create_did(self, *, body: Body(type=DIDCreate) = {}) -> DIDResult:
         """Internal uplink method for create_did"""
@@ -142,10 +144,11 @@
     @returns.json
     @post("/wallet/did/public")
     def __set_public_did(
         self,
         *,
         did: Query,
         conn_id: Query = None,
-        create_transaction_for_endorser: Query = None
+        create_transaction_for_endorser: Query = None,
+        mediation_id: Query = None
     ) -> DIDResult:
         """Internal uplink method for set_public_did"""
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/client.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/client.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/__init__.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,15 @@
 )
 from aries_cloudcontroller.model.ledger_config_instance import LedgerConfigInstance
 from aries_cloudcontroller.model.ledger_config_list import LedgerConfigList
 from aries_cloudcontroller.model.linked_data_proof import LinkedDataProof
 from aries_cloudcontroller.model.mediation_create_request import MediationCreateRequest
 from aries_cloudcontroller.model.mediation_deny import MediationDeny
 from aries_cloudcontroller.model.mediation_grant import MediationGrant
+from aries_cloudcontroller.model.mediation_id_match_info import MediationIdMatchInfo
 from aries_cloudcontroller.model.mediation_list import MediationList
 from aries_cloudcontroller.model.mediation_record import MediationRecord
 from aries_cloudcontroller.model.menu import Menu
 from aries_cloudcontroller.model.menu_form import MenuForm
 from aries_cloudcontroller.model.menu_form_param import MenuFormParam
 from aries_cloudcontroller.model.menu_json import MenuJson
 from aries_cloudcontroller.model.menu_option import MenuOption
@@ -259,14 +260,15 @@
 from aries_cloudcontroller.model.signed_doc import SignedDoc
 from aries_cloudcontroller.model.submission_requirements import SubmissionRequirements
 from aries_cloudcontroller.model.taa_accept import TAAAccept
 from aries_cloudcontroller.model.taa_acceptance import TAAAcceptance
 from aries_cloudcontroller.model.taa_info import TAAInfo
 from aries_cloudcontroller.model.taa_record import TAARecord
 from aries_cloudcontroller.model.taa_result import TAAResult
+from aries_cloudcontroller.model.tails_delete_response import TailsDeleteResponse
 from aries_cloudcontroller.model.transaction_jobs import TransactionJobs
 from aries_cloudcontroller.model.transaction_list import TransactionList
 from aries_cloudcontroller.model.transaction_record import TransactionRecord
 from aries_cloudcontroller.model.txn_or_credential_definition_send_result import (
     TxnOrCredentialDefinitionSendResult,
 )
 from aries_cloudcontroller.model.txn_or_publish_revocations_result import (
@@ -306,17 +308,14 @@
 )
 from aries_cloudcontroller.model.v10_credential_store_request import (
     V10CredentialStoreRequest,
 )
 from aries_cloudcontroller.model.v10_discovery_exchange_list_result import (
     V10DiscoveryExchangeListResult,
 )
-from aries_cloudcontroller.model.v10_discovery_exchange_result import (
-    V10DiscoveryExchangeResult,
-)
 from aries_cloudcontroller.model.v10_discovery_record import V10DiscoveryRecord
 from aries_cloudcontroller.model.v10_presentation_create_request_request import (
     V10PresentationCreateRequestRequest,
 )
 from aries_cloudcontroller.model.v10_presentation_exchange import (
     V10PresentationExchange,
 )
@@ -557,14 +556,15 @@
     "LDProofVCDetailOptions",
     "LedgerConfigInstance",
     "LedgerConfigList",
     "LinkedDataProof",
     "MediationCreateRequest",
     "MediationDeny",
     "MediationGrant",
+    "MediationIdMatchInfo",
     "MediationList",
     "MediationRecord",
     "Menu",
     "MenuForm",
     "MenuFormParam",
     "MenuJson",
     "MenuOption",
@@ -608,14 +608,15 @@
     "SignedDoc",
     "SubmissionRequirements",
     "TAAAccept",
     "TAAAcceptance",
     "TAAInfo",
     "TAARecord",
     "TAAResult",
+    "TailsDeleteResponse",
     "TransactionJobs",
     "TransactionList",
     "TransactionRecord",
     "TxnOrCredentialDefinitionSendResult",
     "TxnOrPublishRevocationsResult",
     "TxnOrRegisterLedgerNymResponse",
     "TxnOrRevRegResult",
@@ -629,15 +630,14 @@
     "V10CredentialFreeOfferRequest",
     "V10CredentialIssueRequest",
     "V10CredentialProblemReportRequest",
     "V10CredentialProposalRequestMand",
     "V10CredentialProposalRequestOpt",
     "V10CredentialStoreRequest",
     "V10DiscoveryExchangeListResult",
-    "V10DiscoveryExchangeResult",
     "V10DiscoveryRecord",
     "V10PresentationCreateRequestRequest",
     "V10PresentationExchange",
     "V10PresentationExchangeList",
     "V10PresentationProblemReportRequest",
     "V10PresentationProposalRequest",
     "V10PresentationSendRequestRequest",
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/action_menu_fetch_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/action_menu_fetch_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_api_message_tracing.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schema_get_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,36 +4,37 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.model_schema import ModelSchema
 
 
-class AdminAPIMessageTracing(BaseModel):
+class SchemaGetResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    AdminAPIMessageTracing - a model defined in OpenAPI
-        trace: Record trace information, based on agent configuration [Optional].
+    SchemaGetResult - a model defined in OpenAPI
+        schema_: The schema_ of this SchemaGetResult [Optional].
     """
 
-    trace: Optional[bool] = None
+    schema_: Optional[ModelSchema] = Field(None, alias="schema")
 
     def __init__(
         self,
         *,
-        trace: Optional[bool] = None,
+        schema_: Optional[ModelSchema] = None,
         **kwargs,
     ):
         super().__init__(
-            trace=trace,
+            schema_=schema_,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-AdminAPIMessageTracing.update_forward_refs()
+SchemaGetResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_config.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_config.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_mediation_deny.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_mediation_deny.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_modules.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_modules.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_status.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_status.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_status_liveliness.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_status_liveliness.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/admin_status_readiness.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/admin_status_readiness.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/aml_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/aml_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator_data.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator_data.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator_data1_jws.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator_data1_jws.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator_data_jws.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator_data_jws.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attach_decorator_data_jws_header.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attach_decorator_data_jws_header.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attachment_def.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attachment_def.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/attribute_mime_types_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/attribute_mime_types_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/claim_format.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/claim_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/clear_pending_revocations_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/clear_pending_revocations_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/conn_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/conn_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_invitation.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_invitation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_list.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_metadata.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_metadata.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_metadata_set_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_metadata_set_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_static_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_static_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/connection_static_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/connection_static_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/constraints.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/constraints.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_invitation_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_invitation_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_wallet_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_wallet_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_wallet_response.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_wallet_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_wallet_token_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_wallet_token_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/create_wallet_token_response.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/create_wallet_token_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_attr_spec.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_def_value.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_def_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_def_value_primary.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_def_value_primary.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_def_value_revocation.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_def_value_revocation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_info_list.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_info_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_rev_indy_records_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_rev_indy_records_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_rev_record_details_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_rev_record_details_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_rev_record_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_rev_record_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/cred_revoked_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/cred_revoked_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definition.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definition.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definition_get_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definition_get_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definition_send_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definition_send_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definition_send_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definition_send_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,32 +12,36 @@
 
 class CredentialDefinitionSendResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
     CredentialDefinitionSendResult - a model defined in OpenAPI
-        credential_definition_id: Credential definition identifier.
+        credential_definition_id: Credential definition identifier [Optional].
     """
 
-    credential_definition_id: str
+    credential_definition_id: Optional[str] = None
 
     def __init__(
         self,
         *,
-        credential_definition_id: str = None,
+        credential_definition_id: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
             credential_definition_id=credential_definition_id,
             **kwargs,
         )
 
     @validator("credential_definition_id")
     def credential_definition_id_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of credential_definition_id does not match regex pattern ('{pattern}')"
             )
         return value
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_definitions_created_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_definitions_created_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_offer.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_offer.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_preview.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_preview.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_proposal.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/credential_status_options.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/credential_status_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/date.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/date.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     @validator("did")
     def did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^did:key:z[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]+$|^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$|^did:([a-zA-Z0-9_]+):([a-zA-Z0-9_.%-]+(:[a-zA-Z0-9_.%-]+)*)((;[a-zA-Z0-9_.:%-]+=[a-zA-Z0-9_.:%-]*)*)(\\/[^#?]*)?([?][^#]*)?(\#.*)?$$"
         if not re.match(pattern, value):
             raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
         return value
 
     @validator("verkey")
     def verkey_pattern(cls, value):
         # Property is optional
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_create.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_update.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,41 +4,45 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.did_create_options import DIDCreateOptions
+from aries_cloudcontroller.model.keylist_update_rule import KeylistUpdateRule
 
 
-class DIDCreate(BaseModel):
+class KeylistUpdate(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    DIDCreate - a model defined in OpenAPI
-        method: The method of this DIDCreate [Optional].
-        options: To define a key type for a did:key [Optional].
+    KeylistUpdate - a model defined in OpenAPI
+        id: Message identifier [Optional].
+        type: Message type [Optional].
+        updates: List of update rules [Optional].
     """
 
-    method: Optional[Literal["key", "sov"]] = None
-    options: Optional[DIDCreateOptions] = None
+    id: Optional[str] = Field(None, alias="@id")
+    type: Optional[str] = Field(None, alias="@type")
+    updates: Optional[List[KeylistUpdateRule]] = None
 
     def __init__(
         self,
         *,
-        method: Optional[Literal["key", "sov"]] = None,
-        options: Optional[DIDCreateOptions] = None,
+        id: Optional[str] = None,
+        type: Optional[str] = None,
+        updates: Optional[List[KeylistUpdateRule]] = None,
         **kwargs,
     ):
         super().__init__(
-            method=method,
-            options=options,
+            id=id,
+            type=type,
+            updates=updates,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-DIDCreate.update_forward_refs()
+KeylistUpdate.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_create_options.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/perform_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,34 +6,38 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class DIDCreateOptions(BaseModel):
+class PerformRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    DIDCreateOptions - a model defined in OpenAPI
-        key_type: The key_type of this DIDCreateOptions.
+    PerformRequest - a model defined in OpenAPI
+        name: Menu option name [Optional].
+        params: Input parameter values [Optional].
     """
 
-    key_type: Literal["ed25519", "bls12381g2"]
+    name: Optional[str] = None
+    params: Optional[Dict[str, str]] = None
 
     def __init__(
         self,
         *,
-        key_type: Literal["ed25519", "bls12381g2"] = None,
+        name: Optional[str] = None,
+        params: Optional[Dict[str, str]] = None,
         **kwargs,
     ):
         super().__init__(
-            key_type=key_type,
+            name=name,
+            params=params,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-DIDCreateOptions.update_forward_refs()
+PerformRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_endpoint.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_endpoint.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_endpoint_with_type.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_endpoint_with_type.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_list.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/did_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/didx_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/didx_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_field.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_field.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_holder.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_holder.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_options.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_pres_spec.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_pres_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_proof_proposal.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_proof_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/dif_proof_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/dif_proof_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/disclose.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/disclose.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/disclosures.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/disclosures.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/doc.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/doc.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/endorser_info.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/endorser_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/endpoints_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/endpoints_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/filter.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/filter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/generated.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/generated.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/get_did_endpoint_response.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/get_did_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/get_did_verkey_response.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/get_did_verkey_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/get_nym_role_response.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/get_nym_role_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_attr_value.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_attr_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_cred_abstract.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_cred_abstract.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_cred_info.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_cred_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_cred_precis.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_cred_precis.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_cred_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_cred_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,31 +16,31 @@
     Do not edit the class manually.
 
     IndyCredRequest - a model defined in OpenAPI
         blinded_ms: Blinded master secret.
         blinded_ms_correctness_proof: Blinded master secret correctness proof.
         cred_def_id: Credential definition identifier.
         nonce: Nonce in credential request.
-        prover_did: Prover DID [Optional].
+        prover_did: Prover DID.
     """
 
     blinded_ms: Dict[str, Any]
     blinded_ms_correctness_proof: Dict[str, Any]
     cred_def_id: str
     nonce: str
-    prover_did: Optional[str] = None
+    prover_did: str
 
     def __init__(
         self,
         *,
         blinded_ms: Dict[str, Any] = None,
         blinded_ms_correctness_proof: Dict[str, Any] = None,
         cred_def_id: str = None,
         nonce: str = None,
-        prover_did: Optional[str] = None,
+        prover_did: str = None,
         **kwargs,
     ):
         super().__init__(
             blinded_ms=blinded_ms,
             blinded_ms_correctness_proof=blinded_ms_correctness_proof,
             cred_def_id=cred_def_id,
             nonce=nonce,
@@ -64,18 +64,14 @@
             raise ValueError(
                 f"Value of nonce does not match regex pattern ('{pattern}')"
             )
         return value
 
     @validator("prover_did")
     def prover_did_pattern(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
         pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of prover_did does not match regex pattern ('{pattern}')"
             )
         return value
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_credential.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_credential.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_eq_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_eq_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_ge_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_ge_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_ge_proof_pred.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_ge_proof_pred.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_key_correctness_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_key_correctness_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_non_revoc_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_non_revoc_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_non_revocation_interval.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_non_revocation_interval.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,24 +33,44 @@
         super().__init__(
             from_=from_,
             to=to,
             **kwargs,
         )
 
     @validator("from_")
+    def from__max(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value > -1:
+            raise ValueError(f"from_ must be less than -1, currently {value}")
+        return value
+
+    @validator("from_")
     def from__min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
             raise ValueError(f"from_ must be greater than 0, currently {value}")
         return value
 
     @validator("to")
+    def to_max(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value > -1:
+            raise ValueError(f"to must be less than -1, currently {value}")
+        return value
+
+    @validator("to")
     def to_min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
             raise ValueError(f"to must be greater than 0, currently {value}")
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_pres_attr_spec.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_pres_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_pres_pred_spec.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_pres_pred_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_pres_preview.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_pres_preview.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_pres_spec.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_pres_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_primary_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_primary_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_identifier.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_identifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,24 @@
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of schema_id does not match regex pattern ('{pattern}')"
             )
         return value
 
     @validator("timestamp")
+    def timestamp_max(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value > -1:
+            raise ValueError(f"timestamp must be less than -1, currently {value}")
+        return value
+
+    @validator("timestamp")
     def timestamp_min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
             raise ValueError(f"timestamp must be greater than 0, currently {value}")
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_req_attr_spec.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_req_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_request_non_revoked.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class IndyProofReqAttrSpecNonRevoked(BaseModel):
+class IndyProofRequestNonRevoked(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyProofReqAttrSpecNonRevoked - a model defined in OpenAPI
+    IndyProofRequestNonRevoked - a model defined in OpenAPI
         from_: Earliest time of interest in non-revocation interval [Optional].
         to: Latest time of interest in non-revocation interval [Optional].
     """
 
     from_: Optional[int] = Field(None, alias="from")
     to: Optional[int] = None
 
@@ -33,31 +33,51 @@
         super().__init__(
             from_=from_,
             to=to,
             **kwargs,
         )
 
     @validator("from_")
+    def from__max(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value > -1:
+            raise ValueError(f"from_ must be less than -1, currently {value}")
+        return value
+
+    @validator("from_")
     def from__min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
             raise ValueError(f"from_ must be greater than 0, currently {value}")
         return value
 
     @validator("to")
+    def to_max(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value > -1:
+            raise ValueError(f"to must be less than -1, currently {value}")
+        return value
+
+    @validator("to")
     def to_min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
             raise ValueError(f"to must be greater than 0, currently {value}")
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyProofReqAttrSpecNonRevoked.update_forward_refs()
+IndyProofRequestNonRevoked.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_req_pred_spec.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_req_pred_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class IndyProofReqPredSpecNonRevoked(BaseModel):
+class IndyProofReqAttrSpecNonRevoked(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyProofReqPredSpecNonRevoked - a model defined in OpenAPI
+    IndyProofReqAttrSpecNonRevoked - a model defined in OpenAPI
         from_: Earliest time of interest in non-revocation interval [Optional].
         to: Latest time of interest in non-revocation interval [Optional].
     """
 
     from_: Optional[int] = Field(None, alias="from")
     to: Optional[int] = None
 
@@ -33,31 +33,51 @@
         super().__init__(
             from_=from_,
             to=to,
             **kwargs,
         )
 
     @validator("from_")
+    def from__max(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value > -1:
+            raise ValueError(f"from_ must be less than -1, currently {value}")
+        return value
+
+    @validator("from_")
     def from__min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
             raise ValueError(f"from_ must be greater than 0, currently {value}")
         return value
 
     @validator("to")
+    def to_max(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value > -1:
+            raise ValueError(f"to must be less than -1, currently {value}")
+        return value
+
+    @validator("to")
     def to_min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
             raise ValueError(f"to must be greater than 0, currently {value}")
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyProofReqPredSpecNonRevoked.update_forward_refs()
+IndyProofReqAttrSpecNonRevoked.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_request_non_revoked.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_bound_offer_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,60 +4,42 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.v20_cred_filter import V20CredFilter
+from aries_cloudcontroller.model.v20_cred_preview import V20CredPreview
 
 
-class IndyProofRequestNonRevoked(BaseModel):
+class V20CredBoundOfferRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyProofRequestNonRevoked - a model defined in OpenAPI
-        from_: Earliest time of interest in non-revocation interval [Optional].
-        to: Latest time of interest in non-revocation interval [Optional].
+    V20CredBoundOfferRequest - a model defined in OpenAPI
+        counter_preview: Optional content for counter-proposal [Optional].
+        filter: Credential specification criteria by format [Optional].
     """
 
-    from_: Optional[int] = Field(None, alias="from")
-    to: Optional[int] = None
+    counter_preview: Optional[V20CredPreview] = None
+    filter: Optional[V20CredFilter] = None
 
     def __init__(
         self,
         *,
-        from_: Optional[int] = None,
-        to: Optional[int] = None,
+        counter_preview: Optional[V20CredPreview] = None,
+        filter: Optional[V20CredFilter] = None,
         **kwargs,
     ):
         super().__init__(
-            from_=from_,
-            to=to,
+            counter_preview=counter_preview,
+            filter=filter,
             **kwargs,
         )
 
-    @validator("from_")
-    def from__min(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        if value < 0:
-            raise ValueError(f"from_ must be greater than 0, currently {value}")
-        return value
-
-    @validator("to")
-    def to_min(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        if value < 0:
-            raise ValueError(f"to must be greater than 0, currently {value}")
-        return value
-
     class Config:
         allow_population_by_field_name = True
 
 
-IndyProofRequestNonRevoked.update_forward_refs()
+V20CredBoundOfferRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_requested_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_requested_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,24 @@
         super().__init__(
             cred_id=cred_id,
             timestamp=timestamp,
             **kwargs,
         )
 
     @validator("timestamp")
+    def timestamp_max(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value > -1:
+            raise ValueError(f"timestamp must be less than -1, currently {value}")
+        return value
+
+    @validator("timestamp")
     def timestamp_min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
             raise ValueError(f"timestamp must be greater than 0, currently {value}")
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_def.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_def.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_def_value.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_def_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_entry.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_entry.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/indy_rev_reg_entry_value.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/indy_rev_reg_entry_value.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/input_descriptors.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/input_descriptors.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/invitation_create_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/invitation_create_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/invitation_message.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_proposal.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,62 +5,58 @@
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 from aries_cloudcontroller.model.attach_decorator import AttachDecorator
+from aries_cloudcontroller.model.v20_cred_format import V20CredFormat
+from aries_cloudcontroller.model.v20_cred_preview import V20CredPreview
 
 
-class InvitationMessage(BaseModel):
+class V20CredProposal(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    InvitationMessage - a model defined in OpenAPI
+    V20CredProposal - a model defined in OpenAPI
+        filtersattach: Credential filter per acceptable format on corresponding identifier.
+        formats: Attachment formats.
         id: Message identifier [Optional].
         type: Message type [Optional].
-        accept: List of mime type in order of preference [Optional].
-        handshake_protocols: The handshake_protocols of this InvitationMessage [Optional].
-        label: Optional label [Optional].
-        requestsattach: Optional request attachment [Optional].
-        services: The services of this InvitationMessage [Optional].
+        comment: Human-readable comment [Optional].
+        credential_preview: Credential preview [Optional].
     """
 
+    filtersattach: List[AttachDecorator] = Field(..., alias="filters~attach")
+    formats: List[V20CredFormat]
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
-    accept: Optional[List[str]] = None
-    handshake_protocols: Optional[List[str]] = None
-    label: Optional[str] = None
-    requestsattach: Optional[List[AttachDecorator]] = Field(
-        None, alias="requests~attach"
-    )
-    services: Optional[List[Union[Dict, str]]] = None
+    comment: Optional[str] = None
+    credential_preview: Optional[V20CredPreview] = None
 
     def __init__(
         self,
         *,
+        filtersattach: List[AttachDecorator] = None,
+        formats: List[V20CredFormat] = None,
         id: Optional[str] = None,
         type: Optional[str] = None,
-        accept: Optional[List[str]] = None,
-        handshake_protocols: Optional[List[str]] = None,
-        label: Optional[str] = None,
-        requestsattach: Optional[List[AttachDecorator]] = None,
-        services: Optional[List[Union[Dict, str]]] = None,
+        comment: Optional[str] = None,
+        credential_preview: Optional[V20CredPreview] = None,
         **kwargs,
     ):
         super().__init__(
             id=id,
             type=type,
-            accept=accept,
-            handshake_protocols=handshake_protocols,
-            label=label,
-            requestsattach=requestsattach,
-            services=services,
+            comment=comment,
+            credential_preview=credential_preview,
+            filtersattach=filtersattach,
+            formats=formats,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-InvitationMessage.update_forward_refs()
+V20CredProposal.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/invitation_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/invitation_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/invitation_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/invitation_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/issuer_cred_rev_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/issuer_cred_rev_record.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,47 +15,51 @@
 
     Do not edit the class manually.
 
     IssuerCredRevRecord - a model defined in OpenAPI
         created_at: Time of record creation [Optional].
         cred_def_id: Credential definition identifier [Optional].
         cred_ex_id: Credential exchange record identifier at credential issue [Optional].
+        cred_ex_version: Credential exchange version [Optional].
         cred_rev_id: Credential revocation identifier [Optional].
         record_id: Issuer credential revocation record identifier [Optional].
         rev_reg_id: Revocation registry identifier [Optional].
         state: Issue credential revocation record state [Optional].
         updated_at: Time of last record update [Optional].
     """
 
     created_at: Optional[str] = None
     cred_def_id: Optional[str] = None
     cred_ex_id: Optional[str] = None
+    cred_ex_version: Optional[str] = None
     cred_rev_id: Optional[str] = None
     record_id: Optional[str] = None
     rev_reg_id: Optional[str] = None
     state: Optional[str] = None
     updated_at: Optional[str] = None
 
     def __init__(
         self,
         *,
         created_at: Optional[str] = None,
         cred_def_id: Optional[str] = None,
         cred_ex_id: Optional[str] = None,
+        cred_ex_version: Optional[str] = None,
         cred_rev_id: Optional[str] = None,
         record_id: Optional[str] = None,
         rev_reg_id: Optional[str] = None,
         state: Optional[str] = None,
         updated_at: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
             created_at=created_at,
             cred_def_id=cred_def_id,
             cred_ex_id=cred_ex_id,
+            cred_ex_version=cred_ex_version,
             cred_rev_id=cred_rev_id,
             record_id=record_id,
             rev_reg_id=rev_reg_id,
             state=state,
             updated_at=updated_at,
             **kwargs,
         )
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/issuer_rev_reg_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/issuer_rev_reg_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_query.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_query.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_query_filter_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_query_filter_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_query_paginate.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_query_paginate.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_update.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ping_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,45 +4,36 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.keylist_update_rule import KeylistUpdateRule
 
 
-class KeylistUpdate(BaseModel):
+class PingRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    KeylistUpdate - a model defined in OpenAPI
-        id: Message identifier [Optional].
-        type: Message type [Optional].
-        updates: List of update rules [Optional].
+    PingRequest - a model defined in OpenAPI
+        comment: Comment for the ping message [Optional].
     """
 
-    id: Optional[str] = Field(None, alias="@id")
-    type: Optional[str] = Field(None, alias="@type")
-    updates: Optional[List[KeylistUpdateRule]] = None
+    comment: Optional[str] = None
 
     def __init__(
         self,
         *,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        updates: Optional[List[KeylistUpdateRule]] = None,
+        comment: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
-            id=id,
-            type=type,
-            updates=updates,
+            comment=comment,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-KeylistUpdate.update_forward_refs()
+PingRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_update_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_update_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/keylist_update_rule.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/keylist_update_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,15 @@
             action=action,
             recipient_key=recipient_key,
             **kwargs,
         )
 
     @validator("recipient_key")
     def recipient_key_pattern(cls, value):
-        pattern = (
-            r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{43,44}$"
-        )
+        pattern = r"^did:key:z[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]+$|^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{43,44}$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of recipient_key does not match regex pattern ('{pattern}')"
             )
         return value
 
     class Config:
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ld_proof_vc_detail.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ld_proof_vc_detail.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ld_proof_vc_detail_options.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ld_proof_vc_detail_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ledger_config_instance.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ledger_config_instance.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ledger_config_list.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ledger_config_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/linked_data_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/linked_data_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_create_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_create_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_deny.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_deny.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_grant.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_grant.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_list.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/mediation_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/mediation_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu_form.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu_form.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu_form_param.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu_form_param.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu_json.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu_json.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/menu_option.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/menu_option.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/model_schema.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/model_schema.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/oob_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_discovery_record.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,79 +4,67 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.invitation_message import InvitationMessage
-from aries_cloudcontroller.model.service_decorator import ServiceDecorator
+from aries_cloudcontroller.model.disclose import Disclose
+from aries_cloudcontroller.model.query import Query
 
 
-class OobRecord(BaseModel):
+class V10DiscoveryRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    OobRecord - a model defined in OpenAPI
-        invi_msg_id: Invitation message identifier.
-        invitation: Out of band invitation message.
-        oob_id: Oob record identifier.
-        state: Out of band message exchange state.
-        attach_thread_id: Connection record identifier [Optional].
-        connection_id: Connection record identifier [Optional].
+    V10DiscoveryRecord - a model defined in OpenAPI
+        connection_id: Connection identifier [Optional].
         created_at: Time of record creation [Optional].
-        our_recipient_key: Recipient key used for oob invitation [Optional].
-        role: OOB Role [Optional].
-        their_service: The their_service of this OobRecord [Optional].
+        disclose: Disclose message [Optional].
+        discovery_exchange_id: Credential exchange identifier [Optional].
+        query_msg: Query message [Optional].
+        state: Current record state [Optional].
+        thread_id: Thread identifier [Optional].
         trace: Record trace information, based on agent configuration [Optional].
         updated_at: Time of last record update [Optional].
     """
 
-    invi_msg_id: str
-    invitation: InvitationMessage
-    oob_id: str
-    state: str
-    attach_thread_id: Optional[str] = None
     connection_id: Optional[str] = None
     created_at: Optional[str] = None
-    our_recipient_key: Optional[str] = None
-    role: Optional[str] = None
-    their_service: Optional[ServiceDecorator] = None
+    disclose: Optional[Disclose] = None
+    discovery_exchange_id: Optional[str] = None
+    query_msg: Optional[Query] = None
+    state: Optional[str] = None
+    thread_id: Optional[str] = None
     trace: Optional[bool] = None
     updated_at: Optional[str] = None
 
     def __init__(
         self,
         *,
-        invi_msg_id: str = None,
-        invitation: InvitationMessage = None,
-        oob_id: str = None,
-        state: str = None,
-        attach_thread_id: Optional[str] = None,
         connection_id: Optional[str] = None,
         created_at: Optional[str] = None,
-        our_recipient_key: Optional[str] = None,
-        role: Optional[str] = None,
-        their_service: Optional[ServiceDecorator] = None,
+        disclose: Optional[Disclose] = None,
+        discovery_exchange_id: Optional[str] = None,
+        query_msg: Optional[Query] = None,
+        state: Optional[str] = None,
+        thread_id: Optional[str] = None,
         trace: Optional[bool] = None,
         updated_at: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
-            attach_thread_id=attach_thread_id,
             connection_id=connection_id,
             created_at=created_at,
-            invi_msg_id=invi_msg_id,
-            invitation=invitation,
-            oob_id=oob_id,
-            our_recipient_key=our_recipient_key,
-            role=role,
+            disclose=disclose,
+            discovery_exchange_id=discovery_exchange_id,
+            query_msg=query_msg,
             state=state,
-            their_service=their_service,
+            thread_id=thread_id,
             trace=trace,
             updated_at=updated_at,
             **kwargs,
         )
 
     @validator("created_at")
     def created_at_pattern(cls, value):
@@ -104,8 +92,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-OobRecord.update_forward_refs()
+V10DiscoveryRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/perform_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schema_input_descriptor.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,38 +6,38 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class PerformRequest(BaseModel):
+class SchemaInputDescriptor(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    PerformRequest - a model defined in OpenAPI
-        name: Menu option name [Optional].
-        params: Input parameter values [Optional].
+    SchemaInputDescriptor - a model defined in OpenAPI
+        required: Required [Optional].
+        uri: URI [Optional].
     """
 
-    name: Optional[str] = None
-    params: Optional[Dict[str, str]] = None
+    required: Optional[bool] = None
+    uri: Optional[str] = None
 
     def __init__(
         self,
         *,
-        name: Optional[str] = None,
-        params: Optional[Dict[str, str]] = None,
+        required: Optional[bool] = None,
+        uri: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
-            name=name,
-            params=params,
+            required=required,
+            uri=uri,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-PerformRequest.update_forward_refs()
+SchemaInputDescriptor.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ping_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_issue_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class PingRequest(BaseModel):
+class V20CredIssueRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    PingRequest - a model defined in OpenAPI
-        comment: Comment for the ping message [Optional].
+    V20CredIssueRequest - a model defined in OpenAPI
+        comment: Human-readable comment [Optional].
     """
 
     comment: Optional[str] = None
 
     def __init__(
         self,
         *,
@@ -32,8 +32,8 @@
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-PingRequest.update_forward_refs()
+V20CredIssueRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/ping_request_response.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/ping_request_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/presentation_definition.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/presentation_definition.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/presentation_proposal.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/presentation_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/presentation_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/presentation_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/protocol_descriptor.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/publish_revocations.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/publish_revocations.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/queries.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/queries.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/query.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/query.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/query_item.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/query_item.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/query_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/vc_record_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,36 +4,37 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.vc_record import VCRecord
 
 
-class QueryResult(BaseModel):
+class VCRecordList(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    QueryResult - a model defined in OpenAPI
-        results: Query results keyed by protocol [Optional].
+    VCRecordList - a model defined in OpenAPI
+        results: The results of this VCRecordList [Optional].
     """
 
-    results: Optional[Dict[str, Any]] = None
+    results: Optional[List[VCRecord]] = None
 
     def __init__(
         self,
         *,
-        results: Optional[Dict[str, Any]] = None,
+        results: Optional[List[VCRecord]] = None,
         **kwargs,
     ):
         super().__init__(
             results=results,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-QueryResult.update_forward_refs()
+VCRecordList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/raw_encoded.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/raw_encoded.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/receive_invitation_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/receive_invitation_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/register_ledger_nym_response.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,36 +4,41 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.transaction_record import TransactionRecord
 
 
-class RegisterLedgerNymResponse(BaseModel):
+class TxnOrRegisterLedgerNymResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    RegisterLedgerNymResponse - a model defined in OpenAPI
+    TxnOrRegisterLedgerNymResponse - a model defined in OpenAPI
         success: Success of nym registration operation [Optional].
+        txn: DID transaction to endorse [Optional].
     """
 
     success: Optional[bool] = None
+    txn: Optional[TransactionRecord] = None
 
     def __init__(
         self,
         *,
         success: Optional[bool] = None,
+        txn: Optional[TransactionRecord] = None,
         **kwargs,
     ):
         super().__init__(
             success=success,
+            txn=txn,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-RegisterLedgerNymResponse.update_forward_refs()
+TxnOrRegisterLedgerNymResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/remove_wallet_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/remove_wallet_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/resolution_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/resolution_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 class ResolutionResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
     ResolutionResult - a model defined in OpenAPI
-        did_doc: DID Document.
+        did_document: DID Document.
         metadata: Resolution metadata.
     """
 
-    did_doc: Dict[str, Any]
+    did_document: Dict[str, Any]
     metadata: Dict[str, Any]
 
     def __init__(
         self,
         *,
-        did_doc: Dict[str, Any] = None,
+        did_document: Dict[str, Any] = None,
         metadata: Dict[str, Any] = None,
         **kwargs,
     ):
         super().__init__(
-            did_doc=did_doc,
+            did_document=did_document,
             metadata=metadata,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_create_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_create_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_issued_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_issued_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 class RevRegResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
     RevRegResult - a model defined in OpenAPI
-        result: The result of this RevRegResult.
+        result: The result of this RevRegResult [Optional].
     """
 
-    result: IssuerRevRegRecord
+    result: Optional[IssuerRevRegRecord] = None
 
     def __init__(
         self,
         *,
-        result: IssuerRevRegRecord = None,
+        result: Optional[IssuerRevRegRecord] = None,
         **kwargs,
     ):
         super().__init__(
             result=result,
             **kwargs,
         )
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/rev_regs_created.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/rev_regs_created.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/revoke_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/revoke_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/route_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/route_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schema_get_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_problem_report_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,37 +4,36 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.model_schema import ModelSchema
 
 
-class SchemaGetResult(BaseModel):
+class V20PresProblemReportRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    SchemaGetResult - a model defined in OpenAPI
-        schema_: The schema_ of this SchemaGetResult [Optional].
+    V20PresProblemReportRequest - a model defined in OpenAPI
+        description: The description of this V20PresProblemReportRequest.
     """
 
-    schema_: Optional[ModelSchema] = Field(None, alias="schema")
+    description: str
 
     def __init__(
         self,
         *,
-        schema_: Optional[ModelSchema] = None,
+        description: str = None,
         **kwargs,
     ):
         super().__init__(
-            schema_=schema_,
+            description=description,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-SchemaGetResult.update_forward_refs()
+V20PresProblemReportRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schema_input_descriptor.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,40 +4,37 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.taa_info import TAAInfo
 
 
-class SchemaInputDescriptor(BaseModel):
+class TAAResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    SchemaInputDescriptor - a model defined in OpenAPI
-        required: Required [Optional].
-        uri: URI [Optional].
+    TAAResult - a model defined in OpenAPI
+        result: The result of this TAAResult [Optional].
     """
 
-    required: Optional[bool] = None
-    uri: Optional[str] = None
+    result: Optional[TAAInfo] = None
 
     def __init__(
         self,
         *,
-        required: Optional[bool] = None,
-        uri: Optional[str] = None,
+        result: Optional[TAAInfo] = None,
         **kwargs,
     ):
         super().__init__(
-            required=required,
-            uri=uri,
+            result=result,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-SchemaInputDescriptor.update_forward_refs()
+TAAResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schema_send_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schema_send_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schema_send_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schema_send_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 class SchemaSendResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
     SchemaSendResult - a model defined in OpenAPI
-        schema_: Schema definition.
         schema_id: Schema identifier.
+        schema_: Schema definition [Optional].
     """
 
-    schema_: ModelSchema = Field(..., alias="schema")
     schema_id: str
+    schema_: Optional[ModelSchema] = Field(None, alias="schema")
 
     def __init__(
         self,
         *,
-        schema_: ModelSchema = None,
         schema_id: str = None,
+        schema_: Optional[ModelSchema] = None,
         **kwargs,
     ):
         super().__init__(
             schema_=schema_,
             schema_id=schema_id,
             **kwargs,
         )
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schemas_created_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schemas_created_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/schemas_input_descriptor_filter.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/schemas_input_descriptor_filter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/send_menu.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/send_menu.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/send_message.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/send_message.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/service_decorator.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/service_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
 class ServiceDecorator(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
     ServiceDecorator - a model defined in OpenAPI
-        recipient_keys: List of recipient keys [Optional].
-        service_endpoint: Service endpoint at which to reach this agent [Optional].
+        recipient_keys: List of recipient keys.
+        service_endpoint: Service endpoint at which to reach this agent.
         routing_keys: List of routing keys [Optional].
     """
 
-    recipient_keys: Optional[List[str]] = Field(None, alias="recipientKeys")
-    service_endpoint: Optional[str] = Field(None, alias="serviceEndpoint")
+    recipient_keys: List[str] = Field(..., alias="recipientKeys")
+    service_endpoint: str = Field(..., alias="serviceEndpoint")
     routing_keys: Optional[List[str]] = Field(None, alias="routingKeys")
 
     def __init__(
         self,
         *,
-        recipient_keys: Optional[List[str]] = None,
-        service_endpoint: Optional[str] = None,
+        recipient_keys: List[str] = None,
+        service_endpoint: str = None,
         routing_keys: Optional[List[str]] = None,
         **kwargs,
     ):
         super().__init__(
             recipient_keys=recipient_keys,
             routing_keys=routing_keys,
             service_endpoint=service_endpoint,
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/sign_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/sign_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/sign_response.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/sign_response.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/signature_options.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/signature_options.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/signed_doc.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/signed_doc.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/submission_requirements.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/submission_requirements.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_accept.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_accept.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_acceptance.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_acceptance.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,18 +38,16 @@
 
     @validator("time")
     def time_max(cls, value):
         # Property is optional
         if value is None:
             return
 
-        if value > 18446744073709552000:
-            raise ValueError(
-                f"time must be less than 18446744073709552000, currently {value}"
-            )
+        if value > -1:
+            raise ValueError(f"time must be less than -1, currently {value}")
         return value
 
     @validator("time")
     def time_min(cls, value):
         # Property is optional
         if value is None:
             return
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_info.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_info.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/taa_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/taa_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/wallet_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.taa_info import TAAInfo
+from aries_cloudcontroller.model.wallet_record import WalletRecord
 
 
-class TAAResult(BaseModel):
+class WalletList(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    TAAResult - a model defined in OpenAPI
-        result: The result of this TAAResult [Optional].
+    WalletList - a model defined in OpenAPI
+        results: List of wallet records [Optional].
     """
 
-    result: Optional[TAAInfo] = None
+    results: Optional[List[WalletRecord]] = None
 
     def __init__(
         self,
         *,
-        result: Optional[TAAInfo] = None,
+        results: Optional[List[WalletRecord]] = None,
         **kwargs,
     ):
         super().__init__(
-            result=result,
+            results=results,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-TAAResult.update_forward_refs()
+WalletList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/transaction_jobs.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/transaction_jobs.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/transaction_list.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/transaction_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/transaction_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/transaction_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_publish_revocations_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_publish_revocations_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_ex_record_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,41 +4,37 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.transaction_record import TransactionRecord
+from aries_cloudcontroller.model.v20_pres_ex_record import V20PresExRecord
 
 
-class TxnOrRegisterLedgerNymResponse(BaseModel):
+class V20PresExRecordList(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    TxnOrRegisterLedgerNymResponse - a model defined in OpenAPI
-        success: Success of nym registration operation [Optional].
-        txn: DID transaction to endorse [Optional].
+    V20PresExRecordList - a model defined in OpenAPI
+        results: Presentation exchange records [Optional].
     """
 
-    success: Optional[bool] = None
-    txn: Optional[TransactionRecord] = None
+    results: Optional[List[V20PresExRecord]] = None
 
     def __init__(
         self,
         *,
-        success: Optional[bool] = None,
-        txn: Optional[TransactionRecord] = None,
+        results: Optional[List[V20PresExRecord]] = None,
         **kwargs,
     ):
         super().__init__(
-            success=success,
-            txn=txn,
+            results=results,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-TxnOrRegisterLedgerNymResponse.update_forward_refs()
+V20PresExRecordList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_rev_reg_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_rev_reg_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/txn_or_schema_send_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/txn_or_schema_send_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/update_wallet_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/update_wallet_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_bound_offer_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_bound_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_create.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_create.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_exchange.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_exchange.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_exchange_list_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_exchange_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_free_offer_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_free_offer_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_issue_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_issue_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_problem_report_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_credential_store_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_credential_store_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_discovery_exchange_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_discovery_exchange_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.v10_discovery_record import V10DiscoveryRecord
+from aries_cloudcontroller.model.v20_discovery_record import V20DiscoveryRecord
 
 
-class V10DiscoveryExchangeResult(BaseModel):
+class V20DiscoveryExchangeResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V10DiscoveryExchangeResult - a model defined in OpenAPI
-        results: Discover Features v1.0 exchange record [Optional].
+    V20DiscoveryExchangeResult - a model defined in OpenAPI
+        results: Discover Features v2.0 exchange record [Optional].
     """
 
-    results: Optional[V10DiscoveryRecord] = None
+    results: Optional[V20DiscoveryRecord] = None
 
     def __init__(
         self,
         *,
-        results: Optional[V10DiscoveryRecord] = None,
+        results: Optional[V20DiscoveryRecord] = None,
         **kwargs,
     ):
         super().__init__(
             results=results,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V10DiscoveryExchangeResult.update_forward_refs()
+V20DiscoveryExchangeResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_discovery_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_discovery_record.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,65 +4,65 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.disclose import Disclose
-from aries_cloudcontroller.model.query import Query
+from aries_cloudcontroller.model.disclosures import Disclosures
+from aries_cloudcontroller.model.queries import Queries
 
 
-class V10DiscoveryRecord(BaseModel):
+class V20DiscoveryRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V10DiscoveryRecord - a model defined in OpenAPI
+    V20DiscoveryRecord - a model defined in OpenAPI
         connection_id: Connection identifier [Optional].
         created_at: Time of record creation [Optional].
-        disclose: Disclose message [Optional].
+        disclosures: Disclosures message [Optional].
         discovery_exchange_id: Credential exchange identifier [Optional].
-        query_msg: Query message [Optional].
+        queries_msg: Queries message [Optional].
         state: Current record state [Optional].
         thread_id: Thread identifier [Optional].
         trace: Record trace information, based on agent configuration [Optional].
         updated_at: Time of last record update [Optional].
     """
 
     connection_id: Optional[str] = None
     created_at: Optional[str] = None
-    disclose: Optional[Disclose] = None
+    disclosures: Optional[Disclosures] = None
     discovery_exchange_id: Optional[str] = None
-    query_msg: Optional[Query] = None
+    queries_msg: Optional[Queries] = None
     state: Optional[str] = None
     thread_id: Optional[str] = None
     trace: Optional[bool] = None
     updated_at: Optional[str] = None
 
     def __init__(
         self,
         *,
         connection_id: Optional[str] = None,
         created_at: Optional[str] = None,
-        disclose: Optional[Disclose] = None,
+        disclosures: Optional[Disclosures] = None,
         discovery_exchange_id: Optional[str] = None,
-        query_msg: Optional[Query] = None,
+        queries_msg: Optional[Queries] = None,
         state: Optional[str] = None,
         thread_id: Optional[str] = None,
         trace: Optional[bool] = None,
         updated_at: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
             connection_id=connection_id,
             created_at=created_at,
-            disclose=disclose,
+            disclosures=disclosures,
             discovery_exchange_id=discovery_exchange_id,
-            query_msg=query_msg,
+            queries_msg=queries_msg,
             state=state,
             thread_id=thread_id,
             trace=trace,
             updated_at=updated_at,
             **kwargs,
         )
 
@@ -92,8 +92,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-V10DiscoveryRecord.update_forward_refs()
+V20DiscoveryRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_create_request_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_create_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_exchange.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_exchange.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_exchange_list.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_exchange_list.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_problem_report_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_proposal_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_proposal_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_send_request_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_send_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_attr_spec.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_attr_spec.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_bound_offer_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.v20_cred_filter import V20CredFilter
-from aries_cloudcontroller.model.v20_cred_preview import V20CredPreview
+from aries_cloudcontroller.model.ld_proof_vc_detail import LDProofVCDetail
+from aries_cloudcontroller.model.v20_cred_filter_indy import V20CredFilterIndy
 
 
-class V20CredBoundOfferRequest(BaseModel):
+class V20CredFilter(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredBoundOfferRequest - a model defined in OpenAPI
-        counter_preview: Optional content for counter-proposal [Optional].
-        filter: Credential specification criteria by format [Optional].
+    V20CredFilter - a model defined in OpenAPI
+        indy: Credential filter for indy [Optional].
+        ld_proof: Credential filter for linked data proof [Optional].
     """
 
-    counter_preview: Optional[V20CredPreview] = None
-    filter: Optional[V20CredFilter] = None
+    indy: Optional[V20CredFilterIndy] = None
+    ld_proof: Optional[LDProofVCDetail] = None
 
     def __init__(
         self,
         *,
-        counter_preview: Optional[V20CredPreview] = None,
-        filter: Optional[V20CredFilter] = None,
+        indy: Optional[V20CredFilterIndy] = None,
+        ld_proof: Optional[LDProofVCDetail] = None,
         **kwargs,
     ):
         super().__init__(
-            counter_preview=counter_preview,
-            filter=filter,
+            indy=indy,
+            ld_proof=ld_proof,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredBoundOfferRequest.update_forward_refs()
+V20CredFilter.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_free.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_offer_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,54 +8,58 @@
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 from aries_cloudcontroller.model.v20_cred_filter import V20CredFilter
 from aries_cloudcontroller.model.v20_cred_preview import V20CredPreview
 
 
-class V20CredExFree(BaseModel):
+class V20CredOfferRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredExFree - a model defined in OpenAPI
+    V20CredOfferRequest - a model defined in OpenAPI
         connection_id: Connection identifier.
         filter: Credential specification criteria by format.
+        auto_issue: Whether to respond automatically to credential requests, creating and issuing requested credentials [Optional].
         auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
         comment: Human-readable comment [Optional].
-        credential_preview: The credential_preview of this V20CredExFree [Optional].
+        credential_preview: The credential_preview of this V20CredOfferRequest [Optional].
         trace: Record trace information, based on agent configuration [Optional].
     """
 
     connection_id: str
     filter: V20CredFilter
+    auto_issue: Optional[bool] = None
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
     trace: Optional[bool] = None
 
     def __init__(
         self,
         *,
         connection_id: str = None,
         filter: V20CredFilter = None,
+        auto_issue: Optional[bool] = None,
         auto_remove: Optional[bool] = None,
         comment: Optional[str] = None,
         credential_preview: Optional[V20CredPreview] = None,
         trace: Optional[bool] = None,
         **kwargs,
     ):
         super().__init__(
+            auto_issue=auto_issue,
             auto_remove=auto_remove,
             comment=comment,
             connection_id=connection_id,
             credential_preview=credential_preview,
             filter=filter,
             trace=trace,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredExFree.update_forward_refs()
+V20CredOfferRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
             "request-sent",
             "request-received",
             "credential-issued",
             "credential-received",
             "done",
             "credential-revoked",
             "abandoned",
+            "deleted",
         ]
     ] = None
     thread_id: Optional[str] = None
     trace: Optional[bool] = None
     updated_at: Optional[str] = None
 
     def __init__(
@@ -109,14 +110,15 @@
                 "request-sent",
                 "request-received",
                 "credential-issued",
                 "credential-received",
                 "done",
                 "credential-revoked",
                 "abandoned",
+                "deleted",
             ]
         ] = None,
         thread_id: Optional[str] = None,
         trace: Optional[bool] = None,
         updated_at: Optional[str] = None,
         **kwargs,
     ):
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_detail.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_detail.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_indy.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_indy.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_filter_indy.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_filter_indy.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_format.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_issue.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_issue.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_issue_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_request_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class V20CredIssueRequest(BaseModel):
+class V20CredRequestRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredIssueRequest - a model defined in OpenAPI
-        comment: Human-readable comment [Optional].
+    V20CredRequestRequest - a model defined in OpenAPI
+        holder_did: Holder DID to substitute for the credentialSubject.id [Optional].
     """
 
-    comment: Optional[str] = None
+    holder_did: Optional[str] = None
 
     def __init__(
         self,
         *,
-        comment: Optional[str] = None,
+        holder_did: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
-            comment=comment,
+            holder_did=holder_did,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredIssueRequest.update_forward_refs()
+V20CredRequestRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_offer.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_offer.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_offer_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_ex_free.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,58 +8,58 @@
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 from aries_cloudcontroller.model.v20_cred_filter import V20CredFilter
 from aries_cloudcontroller.model.v20_cred_preview import V20CredPreview
 
 
-class V20CredOfferRequest(BaseModel):
+class V20CredExFree(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredOfferRequest - a model defined in OpenAPI
+    V20CredExFree - a model defined in OpenAPI
         connection_id: Connection identifier.
         filter: Credential specification criteria by format.
-        auto_issue: Whether to respond automatically to credential requests, creating and issuing requested credentials [Optional].
         auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
         comment: Human-readable comment [Optional].
-        credential_preview: The credential_preview of this V20CredOfferRequest [Optional].
+        credential_preview: The credential_preview of this V20CredExFree [Optional].
         trace: Record trace information, based on agent configuration [Optional].
+        verification_method: For ld-proofs. Verification method for signing. [Optional].
     """
 
     connection_id: str
     filter: V20CredFilter
-    auto_issue: Optional[bool] = None
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
     trace: Optional[bool] = None
+    verification_method: Optional[str] = None
 
     def __init__(
         self,
         *,
         connection_id: str = None,
         filter: V20CredFilter = None,
-        auto_issue: Optional[bool] = None,
         auto_remove: Optional[bool] = None,
         comment: Optional[str] = None,
         credential_preview: Optional[V20CredPreview] = None,
         trace: Optional[bool] = None,
+        verification_method: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
-            auto_issue=auto_issue,
             auto_remove=auto_remove,
             comment=comment,
             connection_id=connection_id,
             credential_preview=credential_preview,
             filter=filter,
             trace=trace,
+            verification_method=verification_method,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredOfferRequest.update_forward_refs()
+V20CredExFree.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_preview.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_preview.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_proposal.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,57 +6,52 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 from aries_cloudcontroller.model.attach_decorator import AttachDecorator
 from aries_cloudcontroller.model.v20_cred_format import V20CredFormat
-from aries_cloudcontroller.model.v20_cred_preview import V20CredPreview
 
 
-class V20CredProposal(BaseModel):
+class V20CredRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredProposal - a model defined in OpenAPI
-        filtersattach: Credential filter per acceptable format on corresponding identifier.
-        formats: Attachment formats.
+    V20CredRequest - a model defined in OpenAPI
+        formats: Acceptable attachment formats.
+        requestsattach: Request attachments.
         id: Message identifier [Optional].
         type: Message type [Optional].
         comment: Human-readable comment [Optional].
-        credential_preview: Credential preview [Optional].
     """
 
-    filtersattach: List[AttachDecorator] = Field(..., alias="filters~attach")
     formats: List[V20CredFormat]
+    requestsattach: List[AttachDecorator] = Field(..., alias="requests~attach")
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     comment: Optional[str] = None
-    credential_preview: Optional[V20CredPreview] = None
 
     def __init__(
         self,
         *,
-        filtersattach: List[AttachDecorator] = None,
         formats: List[V20CredFormat] = None,
+        requestsattach: List[AttachDecorator] = None,
         id: Optional[str] = None,
         type: Optional[str] = None,
         comment: Optional[str] = None,
-        credential_preview: Optional[V20CredPreview] = None,
         **kwargs,
     ):
         super().__init__(
             id=id,
             type=type,
             comment=comment,
-            credential_preview=credential_preview,
-            filtersattach=filtersattach,
             formats=formats,
+            requestsattach=requestsattach,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredProposal.update_forward_refs()
+V20CredRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_proposal.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,53 +5,53 @@
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 from aries_cloudcontroller.model.attach_decorator import AttachDecorator
-from aries_cloudcontroller.model.v20_cred_format import V20CredFormat
+from aries_cloudcontroller.model.v20_pres_format import V20PresFormat
 
 
-class V20CredRequest(BaseModel):
+class V20PresProposal(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredRequest - a model defined in OpenAPI
-        formats: Acceptable attachment formats.
-        requestsattach: Request attachments.
+    V20PresProposal - a model defined in OpenAPI
+        formats: The formats of this V20PresProposal.
+        proposalsattach: Attachment per acceptable format on corresponding identifier.
         id: Message identifier [Optional].
         type: Message type [Optional].
         comment: Human-readable comment [Optional].
     """
 
-    formats: List[V20CredFormat]
-    requestsattach: List[AttachDecorator] = Field(..., alias="requests~attach")
+    formats: List[V20PresFormat]
+    proposalsattach: List[AttachDecorator] = Field(..., alias="proposals~attach")
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     comment: Optional[str] = None
 
     def __init__(
         self,
         *,
-        formats: List[V20CredFormat] = None,
-        requestsattach: List[AttachDecorator] = None,
+        formats: List[V20PresFormat] = None,
+        proposalsattach: List[AttachDecorator] = None,
         id: Optional[str] = None,
         type: Optional[str] = None,
         comment: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
             id=id,
             type=type,
             comment=comment,
             formats=formats,
-            requestsattach=requestsattach,
+            proposalsattach=proposalsattach,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredRequest.update_forward_refs()
+V20PresProposal.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_request_free.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_request_free.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_request_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/verify_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,34 +6,38 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class V20CredRequestRequest(BaseModel):
+class VerifyResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredRequestRequest - a model defined in OpenAPI
-        holder_did: Holder DID to substitute for the credentialSubject.id [Optional].
+    VerifyResponse - a model defined in OpenAPI
+        valid: The valid of this VerifyResponse.
+        error: Error text [Optional].
     """
 
-    holder_did: Optional[str] = None
+    valid: bool
+    error: Optional[str] = None
 
     def __init__(
         self,
         *,
-        holder_did: Optional[str] = None,
+        valid: bool = None,
+        error: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
-            holder_did=holder_did,
+            error=error,
+            valid=valid,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredRequestRequest.update_forward_refs()
+VerifyResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_send_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/invitation_message.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,58 +4,67 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.v20_cred_filter import V20CredFilter
-from aries_cloudcontroller.model.v20_cred_preview import V20CredPreview
+from aries_cloudcontroller.model.attach_decorator import AttachDecorator
 
 
-class V20CredSendRequest(BaseModel):
+class InvitationMessage(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredSendRequest - a model defined in OpenAPI
-        connection_id: Connection identifier.
-        filter: Credential specification criteria by format.
-        auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
-        comment: Human-readable comment [Optional].
-        credential_preview: The credential_preview of this V20CredSendRequest [Optional].
-        trace: Record trace information, based on agent configuration [Optional].
+    InvitationMessage - a model defined in OpenAPI
+        id: Message identifier [Optional].
+        type: Message type [Optional].
+        accept: List of mime type in order of preference [Optional].
+        handshake_protocols: The handshake_protocols of this InvitationMessage [Optional].
+        image_url: Optional image URL for out-of-band invitation [Optional].
+        label: Optional label [Optional].
+        requestsattach: Optional request attachment [Optional].
+        services: The services of this InvitationMessage [Optional].
     """
 
-    connection_id: str
-    filter: V20CredFilter
-    auto_remove: Optional[bool] = None
-    comment: Optional[str] = None
-    credential_preview: Optional[V20CredPreview] = None
-    trace: Optional[bool] = None
+    id: Optional[str] = Field(None, alias="@id")
+    type: Optional[str] = Field(None, alias="@type")
+    accept: Optional[List[str]] = None
+    handshake_protocols: Optional[List[str]] = None
+    image_url: Optional[str] = Field(None, alias="imageUrl")
+    label: Optional[str] = None
+    requestsattach: Optional[List[AttachDecorator]] = Field(
+        None, alias="requests~attach"
+    )
+    services: Optional[List[Dict]] = None
 
     def __init__(
         self,
         *,
-        connection_id: str = None,
-        filter: V20CredFilter = None,
-        auto_remove: Optional[bool] = None,
-        comment: Optional[str] = None,
-        credential_preview: Optional[V20CredPreview] = None,
-        trace: Optional[bool] = None,
+        id: Optional[str] = None,
+        type: Optional[str] = None,
+        accept: Optional[List[str]] = None,
+        handshake_protocols: Optional[List[str]] = None,
+        image_url: Optional[str] = None,
+        label: Optional[str] = None,
+        requestsattach: Optional[List[AttachDecorator]] = None,
+        services: Optional[List[Dict]] = None,
         **kwargs,
     ):
         super().__init__(
-            auto_remove=auto_remove,
-            comment=comment,
-            connection_id=connection_id,
-            credential_preview=credential_preview,
-            filter=filter,
-            trace=trace,
+            id=id,
+            type=type,
+            accept=accept,
+            handshake_protocols=handshake_protocols,
+            image_url=image_url,
+            label=label,
+            requestsattach=requestsattach,
+            services=services,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredSendRequest.update_forward_refs()
+InvitationMessage.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_cred_store_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_cred_store_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_discovery_exchange_result.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/verify_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,37 +4,41 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.v20_discovery_record import V20DiscoveryRecord
+from aries_cloudcontroller.model.signed_doc import SignedDoc
 
 
-class V20DiscoveryExchangeResult(BaseModel):
+class VerifyRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20DiscoveryExchangeResult - a model defined in OpenAPI
-        results: Discover Features v2.0 exchange record [Optional].
+    VerifyRequest - a model defined in OpenAPI
+        doc: Signed document.
+        verkey: Verkey to use for doc verification [Optional].
     """
 
-    results: Optional[V20DiscoveryRecord] = None
+    doc: SignedDoc
+    verkey: Optional[str] = None
 
     def __init__(
         self,
         *,
-        results: Optional[V20DiscoveryRecord] = None,
+        doc: SignedDoc = None,
+        verkey: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
-            results=results,
+            doc=doc,
+            verkey=verkey,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20DiscoveryExchangeResult.update_forward_refs()
+VerifyRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_issue_cred_schema_core.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_issue_cred_schema_core.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_create_request_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_create_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_ex_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_ex_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_ex_record_list.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,37 +4,40 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.v20_pres_ex_record import V20PresExRecord
 
 
-class V20PresExRecordList(BaseModel):
+class V20PresentationSendRequestToProposal(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20PresExRecordList - a model defined in OpenAPI
-        results: Presentation exchange records [Optional].
+    V20PresentationSendRequestToProposal - a model defined in OpenAPI
+        auto_verify: Verifier choice to auto-verify proof presentation [Optional].
+        trace: Whether to trace event (default false) [Optional].
     """
 
-    results: Optional[List[V20PresExRecord]] = None
+    auto_verify: Optional[bool] = None
+    trace: Optional[bool] = None
 
     def __init__(
         self,
         *,
-        results: Optional[List[V20PresExRecord]] = None,
+        auto_verify: Optional[bool] = None,
+        trace: Optional[bool] = None,
         **kwargs,
     ):
         super().__init__(
-            results=results,
+            auto_verify=auto_verify,
+            trace=trace,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20PresExRecordList.update_forward_refs()
+V20PresentationSendRequestToProposal.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_format.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_proposal.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_request_by_format.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,54 +4,42 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.attach_decorator import AttachDecorator
-from aries_cloudcontroller.model.v20_pres_format import V20PresFormat
+from aries_cloudcontroller.model.dif_proof_request import DIFProofRequest
+from aries_cloudcontroller.model.indy_proof_request import IndyProofRequest
 
 
-class V20PresProposal(BaseModel):
+class V20PresRequestByFormat(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20PresProposal - a model defined in OpenAPI
-        formats: The formats of this V20PresProposal.
-        proposalsattach: Attachment per acceptable format on corresponding identifier.
-        id: Message identifier [Optional].
-        type: Message type [Optional].
-        comment: Human-readable comment [Optional].
+    V20PresRequestByFormat - a model defined in OpenAPI
+        dif: Presentation request for DIF [Optional].
+        indy: Presentation request for indy [Optional].
     """
 
-    formats: List[V20PresFormat]
-    proposalsattach: List[AttachDecorator] = Field(..., alias="proposals~attach")
-    id: Optional[str] = Field(None, alias="@id")
-    type: Optional[str] = Field(None, alias="@type")
-    comment: Optional[str] = None
+    dif: Optional[DIFProofRequest] = None
+    indy: Optional[IndyProofRequest] = None
 
     def __init__(
         self,
         *,
-        formats: List[V20PresFormat] = None,
-        proposalsattach: List[AttachDecorator] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
+        dif: Optional[DIFProofRequest] = None,
+        indy: Optional[IndyProofRequest] = None,
         **kwargs,
     ):
         super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            formats=formats,
-            proposalsattach=proposalsattach,
+            dif=dif,
+            indy=indy,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20PresProposal.update_forward_refs()
+V20PresRequestByFormat.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_proposal_by_format.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_proposal_by_format.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_proposal_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_proposal_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_request_by_format.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,42 +4,46 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.dif_proof_request import DIFProofRequest
-from aries_cloudcontroller.model.indy_proof_request import IndyProofRequest
+from aries_cloudcontroller.model.dif_pres_spec import DIFPresSpec
+from aries_cloudcontroller.model.indy_pres_spec import IndyPresSpec
 
 
-class V20PresRequestByFormat(BaseModel):
+class V20PresSpecByFormatRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20PresRequestByFormat - a model defined in OpenAPI
-        dif: Presentation request for DIF [Optional].
-        indy: Presentation request for indy [Optional].
+    V20PresSpecByFormatRequest - a model defined in OpenAPI
+        dif: Optional Presentation specification for DIF, overrides the PresentionExchange record&#39;s PresRequest [Optional].
+        indy: Presentation specification for indy [Optional].
+        trace: Record trace information, based on agent configuration [Optional].
     """
 
-    dif: Optional[DIFProofRequest] = None
-    indy: Optional[IndyProofRequest] = None
+    dif: Optional[DIFPresSpec] = None
+    indy: Optional[IndyPresSpec] = None
+    trace: Optional[bool] = None
 
     def __init__(
         self,
         *,
-        dif: Optional[DIFProofRequest] = None,
-        indy: Optional[IndyProofRequest] = None,
+        dif: Optional[DIFPresSpec] = None,
+        indy: Optional[IndyPresSpec] = None,
+        trace: Optional[bool] = None,
         **kwargs,
     ):
         super().__init__(
             dif=dif,
             indy=indy,
+            trace=trace,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20PresRequestByFormat.update_forward_refs()
+V20PresSpecByFormatRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_send_request_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/v20_pres_send_request_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/did_create_options.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,46 +4,51 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.dif_pres_spec import DIFPresSpec
-from aries_cloudcontroller.model.indy_pres_spec import IndyPresSpec
 
 
-class V20PresSpecByFormatRequest(BaseModel):
+class DIDCreateOptions(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20PresSpecByFormatRequest - a model defined in OpenAPI
-        dif: Optional Presentation specification for DIF, overrides the PresentionExchange record&#39;s PresRequest [Optional].
-        indy: Presentation specification for indy [Optional].
-        trace: Record trace information, based on agent configuration [Optional].
+    DIDCreateOptions - a model defined in OpenAPI
+        key_type: Key type to use for the DID keypair. Validated with the chosen DID method's supported key types..
+        did: Specify final value of the did (including did:&lt;method&gt;: prefix)if the method supports or requires so. [Optional].
     """
 
-    dif: Optional[DIFPresSpec] = None
-    indy: Optional[IndyPresSpec] = None
-    trace: Optional[bool] = None
+    key_type: Literal["ed25519", "bls12381g2"]
+    did: Optional[str] = None
 
     def __init__(
         self,
         *,
-        dif: Optional[DIFPresSpec] = None,
-        indy: Optional[IndyPresSpec] = None,
-        trace: Optional[bool] = None,
+        key_type: Literal["ed25519", "bls12381g2"] = None,
+        did: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
-            dif=dif,
-            indy=indy,
-            trace=trace,
+            did=did,
+            key_type=key_type,
             **kwargs,
         )
 
+    @validator("did")
+    def did_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$|^did:([a-zA-Z0-9_]+):([a-zA-Z0-9_.%-]+(:[a-zA-Z0-9_.%-]+)*)((;[a-zA-Z0-9_.:%-]+=[a-zA-Z0-9_.:%-]*)*)(\\/[^#?]*)?([?][^#]*)?(\#.*)?$$"
+        if not re.match(pattern, value):
+            raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
+        return value
+
     class Config:
         allow_population_by_field_name = True
 
 
-V20PresSpecByFormatRequest.update_forward_refs()
+DIDCreateOptions.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/vc_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/vc_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/vc_record_list.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/tails_delete_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,37 +4,36 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.vc_record import VCRecord
 
 
-class VCRecordList(BaseModel):
+class TailsDeleteResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    VCRecordList - a model defined in OpenAPI
-        results: The results of this VCRecordList [Optional].
+    TailsDeleteResponse - a model defined in OpenAPI
+        message: The message of this TailsDeleteResponse [Optional].
     """
 
-    results: Optional[List[VCRecord]] = None
+    message: Optional[str] = None
 
     def __init__(
         self,
         *,
-        results: Optional[List[VCRecord]] = None,
+        message: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(
-            results=results,
+            message=message,
             **kwargs,
         )
 
     class Config:
         allow_population_by_field_name = True
 
 
-VCRecordList.update_forward_refs()
+TailsDeleteResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/w3_c_credentials_list_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/w3_c_credentials_list_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/wallet_record.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/wallet_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/model/write_ledger_request.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/model/write_ledger_request.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller/util/pydantic_converter.py` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller/util/pydantic_converter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller.egg-info/PKG-INFO` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aries-cloudcontroller
-Version: 0.8.0rc5
+Version: 0.8.0rc6
 Summary: A simple python package for controlling an aries agent through the admin-api interface
 Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.8.0rc5 Summary: A
+Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.8.0rc6 Summary: A
 simple python package for controlling an aries agent through the admin-api
 interface Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/
 tree/main/aries_cloudcontroller Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `aries_cloudcontroller-0.8.0rc5/aries_cloudcontroller.egg-info/SOURCES.txt` & `aries_cloudcontroller-0.8.0rc6/aries_cloudcontroller.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 aries_cloudcontroller/api/revocation.py
 aries_cloudcontroller/api/schema.py
 aries_cloudcontroller/api/server.py
 aries_cloudcontroller/api/trustping.py
 aries_cloudcontroller/api/wallet.py
 aries_cloudcontroller/model/__init__.py
 aries_cloudcontroller/model/action_menu_fetch_result.py
-aries_cloudcontroller/model/admin_api_message_tracing.py
 aries_cloudcontroller/model/admin_config.py
 aries_cloudcontroller/model/admin_mediation_deny.py
 aries_cloudcontroller/model/admin_modules.py
 aries_cloudcontroller/model/admin_status.py
 aries_cloudcontroller/model/admin_status_liveliness.py
 aries_cloudcontroller/model/admin_status_readiness.py
 aries_cloudcontroller/model/aml_record.py
@@ -171,14 +170,15 @@
 aries_cloudcontroller/model/ld_proof_vc_detail_options.py
 aries_cloudcontroller/model/ledger_config_instance.py
 aries_cloudcontroller/model/ledger_config_list.py
 aries_cloudcontroller/model/linked_data_proof.py
 aries_cloudcontroller/model/mediation_create_request.py
 aries_cloudcontroller/model/mediation_deny.py
 aries_cloudcontroller/model/mediation_grant.py
+aries_cloudcontroller/model/mediation_id_match_info.py
 aries_cloudcontroller/model/mediation_list.py
 aries_cloudcontroller/model/mediation_record.py
 aries_cloudcontroller/model/menu.py
 aries_cloudcontroller/model/menu_form.py
 aries_cloudcontroller/model/menu_form_param.py
 aries_cloudcontroller/model/menu_json.py
 aries_cloudcontroller/model/menu_option.py
@@ -191,18 +191,16 @@
 aries_cloudcontroller/model/presentation_proposal.py
 aries_cloudcontroller/model/presentation_request.py
 aries_cloudcontroller/model/protocol_descriptor.py
 aries_cloudcontroller/model/publish_revocations.py
 aries_cloudcontroller/model/queries.py
 aries_cloudcontroller/model/query.py
 aries_cloudcontroller/model/query_item.py
-aries_cloudcontroller/model/query_result.py
 aries_cloudcontroller/model/raw_encoded.py
 aries_cloudcontroller/model/receive_invitation_request.py
-aries_cloudcontroller/model/register_ledger_nym_response.py
 aries_cloudcontroller/model/remove_wallet_request.py
 aries_cloudcontroller/model/resolution_result.py
 aries_cloudcontroller/model/rev_reg_create_request.py
 aries_cloudcontroller/model/rev_reg_issued_result.py
 aries_cloudcontroller/model/rev_reg_result.py
 aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py
 aries_cloudcontroller/model/rev_reg_wallet_updated_result.py
@@ -224,14 +222,15 @@
 aries_cloudcontroller/model/signed_doc.py
 aries_cloudcontroller/model/submission_requirements.py
 aries_cloudcontroller/model/taa_accept.py
 aries_cloudcontroller/model/taa_acceptance.py
 aries_cloudcontroller/model/taa_info.py
 aries_cloudcontroller/model/taa_record.py
 aries_cloudcontroller/model/taa_result.py
+aries_cloudcontroller/model/tails_delete_response.py
 aries_cloudcontroller/model/transaction_jobs.py
 aries_cloudcontroller/model/transaction_list.py
 aries_cloudcontroller/model/transaction_record.py
 aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
 aries_cloudcontroller/model/txn_or_publish_revocations_result.py
 aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
 aries_cloudcontroller/model/txn_or_rev_reg_result.py
@@ -245,15 +244,14 @@
 aries_cloudcontroller/model/v10_credential_free_offer_request.py
 aries_cloudcontroller/model/v10_credential_issue_request.py
 aries_cloudcontroller/model/v10_credential_problem_report_request.py
 aries_cloudcontroller/model/v10_credential_proposal_request_mand.py
 aries_cloudcontroller/model/v10_credential_proposal_request_opt.py
 aries_cloudcontroller/model/v10_credential_store_request.py
 aries_cloudcontroller/model/v10_discovery_exchange_list_result.py
-aries_cloudcontroller/model/v10_discovery_exchange_result.py
 aries_cloudcontroller/model/v10_discovery_record.py
 aries_cloudcontroller/model/v10_presentation_create_request_request.py
 aries_cloudcontroller/model/v10_presentation_exchange.py
 aries_cloudcontroller/model/v10_presentation_exchange_list.py
 aries_cloudcontroller/model/v10_presentation_problem_report_request.py
 aries_cloudcontroller/model/v10_presentation_proposal_request.py
 aries_cloudcontroller/model/v10_presentation_send_request_request.py
@@ -278,15 +276,14 @@
 aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py
 aries_cloudcontroller/model/v20_cred_offer_request.py
 aries_cloudcontroller/model/v20_cred_preview.py
 aries_cloudcontroller/model/v20_cred_proposal.py
 aries_cloudcontroller/model/v20_cred_request.py
 aries_cloudcontroller/model/v20_cred_request_free.py
 aries_cloudcontroller/model/v20_cred_request_request.py
-aries_cloudcontroller/model/v20_cred_send_request.py
 aries_cloudcontroller/model/v20_cred_store_request.py
 aries_cloudcontroller/model/v20_discovery_exchange_list_result.py
 aries_cloudcontroller/model/v20_discovery_exchange_result.py
 aries_cloudcontroller/model/v20_discovery_record.py
 aries_cloudcontroller/model/v20_issue_cred_schema_core.py
 aries_cloudcontroller/model/v20_pres.py
 aries_cloudcontroller/model/v20_pres_create_request_request.py
```

### Comparing `aries_cloudcontroller-0.8.0rc5/setup.py` & `aries_cloudcontroller-0.8.0rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     lineiter = (line.strip() for line in open(filename))
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 if __name__ == "__main__":
     setup(
         name=PACKAGE_NAME,
-        version="0.8.0-rc5",
+        version="0.8.0-rc6",
         description="A simple python package for controlling an aries agent through the admin-api interface",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller",
         packages=find_packages(),
         include_package_data=True,
         package_data={
```

### Comparing `aries_cloudcontroller-0.8.0rc5/tests/model/test_presentation.py` & `aries_cloudcontroller-0.8.0rc6/tests/model/test_presentation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc5/tests/test_acapy_client.py` & `aries_cloudcontroller-0.8.0rc6/tests/test_acapy_client.py`

 * *Files identical despite different names*

