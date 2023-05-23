# Comparing `tmp/vesselapi-3.23.0.tar.gz` & `tmp/vesselapi-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vesselapi-3.23.0.tar", last modified: Tue May 23 00:08:49 2023, max compression
+gzip compressed data, was "vesselapi-3.5.2.tar", last modified: Tue Mar  7 22:17:16 2023, max compression
```

## Comparing `vesselapi-3.23.0.tar` & `vesselapi-3.5.2.tar`

### file list

```diff
@@ -1,170 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:08:49.731182 vesselapi-3.23.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-23 00:08:49.731182 vesselapi-3.23.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6857 2023-05-23 00:08:37.000000 vesselapi-3.23.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 00:08:49.731182 vesselapi-3.23.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-05-23 00:08:37.000000 vesselapi-3.23.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:08:49.711181 vesselapi-3.23.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:08:49.715181 vesselapi-3.23.0/src/vesselapi/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9887 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9526 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/attendees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9753 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/calls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4381 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9849 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/contacts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9633 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/deals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9791 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/emails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9674 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1886 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9719 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/leads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2325 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/links.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:08:49.715181 vesselapi-3.23.0/src/vesselapi/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:08:49.723182 vesselapi-3.23.0/src/vesselapi/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10666 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/delete_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/delete_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2129 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2099 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_calls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2129 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_contacts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2099 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_deals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_emails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_event_attendees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2133 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1036 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2099 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_leads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2099 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2099 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_tasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2099 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2061 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2061 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2129 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1853 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1853 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2092 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1845 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1845 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1331 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1779 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2157 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1984 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1983 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1910 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1708 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1802 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1495 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/get_one_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1358 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1415 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1338 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1384 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3063 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_passthrough.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_link_exchange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_link_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/post_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1481 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6247 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_calls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4942 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_contacts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5432 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_deals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6278 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_emails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_event_attendees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5203 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5105 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_leads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4291 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4939 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_tasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4277 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:08:49.731182 vesselapi-3.23.0/src/vesselapi/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2244 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4703 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/accountcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2433 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/accountupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/address.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/booleanfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3328 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/callcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      706 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/callupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4138 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/contactcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1837 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/contactupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1701 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/datefilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4907 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/dealcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1920 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/dealupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5312 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5342 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/emailcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1397 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/emailupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4081 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2934 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/eventattendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/eventattendeecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      521 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/eventattendeeupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/eventcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/eventupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3205 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4311 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2149 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/leadcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2300 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/leadupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2541 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2252 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/notecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/noteupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/numberfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1848 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/stringfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/stringlistfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3459 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3193 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/taskcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2164 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/taskupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2901 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/webhookmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      599 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/models/shared/webhookmetadatacreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9711 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2265 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/passthrough.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7124 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9761 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/tasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2009 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/tokens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7021 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:08:49.731182 vesselapi-3.23.0/src/vesselapi/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4408 2023-05-23 00:08:37.000000 vesselapi-3.23.0/src/vesselapi/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:08:49.715181 vesselapi-3.23.0/src/vesselapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-23 00:08:49.000000 vesselapi-3.23.0/src/vesselapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-05-23 00:08:49.000000 vesselapi-3.23.0/src/vesselapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 00:08:49.000000 vesselapi-3.23.0/src/vesselapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-23 00:08:49.000000 vesselapi-3.23.0/src/vesselapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 00:08:49.000000 vesselapi-3.23.0/src/vesselapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.837517 vesselapi-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-07 22:17:16.837517 vesselapi-3.5.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3842 2023-03-07 22:17:08.000000 vesselapi-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 22:17:16.837517 vesselapi-3.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-03-07 22:17:08.000000 vesselapi-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.821517 vesselapi-3.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.825517 vesselapi-3.5.2/src/vesselapi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8486 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8065 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/attendees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3794 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8448 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/contacts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8247 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/deals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8400 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/emails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8283 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8333 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/leads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.825517 vesselapi-3.5.2/src/vesselapi/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.833517 vesselapi-3.5.2/src/vesselapi/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11828 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/delete_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/delete_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_contacts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_deals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1836 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_emails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1957 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_event_attendees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_leads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_tasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1685 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1685 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1840 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1474 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1644 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2608 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_passthrough.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2275 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_link_exchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1189 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_link_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1674 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5923 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4618 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_contacts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_deals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5950 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_emails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_event_attendees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4875 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4775 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_leads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3961 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4609 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_tasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3947 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.837517 vesselapi-3.5.2/src/vesselapi/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1979 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3714 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1915 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/accountcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1971 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/accountupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1129 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/address.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/booleanfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/contactcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1583 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/contactupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1620 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/datefilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3632 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/dealcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/dealupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4129 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4053 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/emailcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/emailupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2195 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventattendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventattendeecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventattendeeupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2518 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1918 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2634 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      971 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3485 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/leadcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/leadupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1599 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/notecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/noteupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/numberfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/stringfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/stringlistfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2949 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/taskcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1681 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/taskupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadatacreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8325 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2026 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/passthrough.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6878 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8375 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/tasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1761 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/tokens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5961 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.837517 vesselapi-3.5.2/src/vesselapi/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23642 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3878 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.825517 vesselapi-3.5.2/src/vesselapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/top_level.txt
```

### Comparing `vesselapi-3.23.0/src/vesselapi/accounts.py` & `vesselapi-3.5.2/src/vesselapi/accounts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Accounts:
     _client: requests_http.Session
@@ -17,55 +15,52 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def batch(self, request: operations.GetBatchCrmAccountRequest) -> operations.GetBatchCrmAccountResponse:
         r"""Get Batch Accounts
         Retrieve Accounts by a set of Id's
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/account/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmAccountRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBatchCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmAccountRequestBody) -> operations.PostCrmAccountResponse:
+    def create(self, request: operations.PostCrmAccountRequest) -> operations.PostCrmAccountResponse:
         r"""Create Account
         Create a new Account
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/account'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
@@ -73,113 +68,106 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmAccountRequest) -> operations.GetDetailsCrmAccountResponse:
         r"""Get Account Details
         Get details about all accounts. 
         Details include the type, possible values, and other meta data about the fields.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/account/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmAccountRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDetailsCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmAccountRequest) -> operations.GetOneCrmAccountResponse:
         r"""Get Account
         Retrieve a single Account by Id
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/account'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmAccountRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetOneCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmAccountsRequest) -> operations.GetAllCrmAccountsResponse:
         r"""Get All Accounts
         Retrieve all Accounts
         *CRM Caveats*:
         - Pipedrive: dealIds + contactIds not supported when querying for all accounts
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/accounts'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmAccountsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmAccountsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmAccountsRequest) -> operations.SearchCrmAccountsResponse:
         r"""Search Accounts
         Search all Accounts using filters
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/accounts/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmAccountsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchCrmAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
@@ -187,28 +175,27 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmAccountsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmAccountRequestBody) -> operations.PutCrmAccountResponse:
+    def update(self, request: operations.PutCrmAccountRequest) -> operations.PutCrmAccountResponse:
         r"""Update Account
         Update an existing Account
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/account'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PutCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/attendees.py` & `vesselapi-3.5.2/src/vesselapi/attendees.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Attendees:
     _client: requests_http.Session
@@ -17,164 +15,153 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def batch(self, request: operations.GetBatchCrmEventAttendeeRequest) -> operations.GetBatchCrmEventAttendeeResponse:
         r"""Get Batch Event Attendees
         Retrieve Event Attendees by a set of Id's
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event/attendee/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmEventAttendeeRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBatchCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmEventAttendeeResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def create(self) -> operations.PostCrmEventAttendeeResponse:
         r"""Create Event Attendee
         Add an Attendee to an Event
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event/attendee'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
         
         client = self._security_client
         
-        http_res = client.request('POST', url, headers=headers)
+        http_res = client.request('POST', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmEventAttendeeResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmEventAttendeeRequest) -> operations.GetDetailsCrmEventAttendeeResponse:
         r"""Get Event Attendee Details
         Get details about all event attendees. 
         Details include the type, possible values, and other meta data about the fields.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event/attendee/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmEventAttendeeRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDetailsCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmEventAttendeeResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmEventAttendeeRequest) -> operations.GetOneCrmEventAttendeeResponse:
         r"""Get Event Attendee
         Retrieve a single Event Attendee by Id
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event/attendee'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmEventAttendeeRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetOneCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmEventAttendeeResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmEventAttendeesRequest) -> operations.GetAllCrmEventAttendeesResponse:
         r"""Get All Event Attendees
         Retrieve all Attendees for all Events
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event/attendees'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmEventAttendeesRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmEventAttendeesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmEventAttendeesResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmEventAttendeesRequest) -> operations.SearchCrmEventAttendeesResponse:
         r"""Search Event Attendees
         Search all Event Attendees using filters
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event/attendees/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmEventAttendeesRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchCrmEventAttendeesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
@@ -182,29 +169,27 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmEventAttendeesResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def update(self) -> operations.PutCrmEventAttendeeResponse:
         r"""Update Event Attendee
         Update the status of an event attendee
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event/attendee'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
         
         client = self._security_client
         
-        http_res = client.request('PATCH', url, headers=headers)
+        http_res = client.request('PATCH', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PutCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmEventAttendeeResponseBody])
```

### Comparing `vesselapi-3.23.0/src/vesselapi/calls.py` & `vesselapi-3.5.2/src/vesselapi/emails.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Calls:
+class Emails:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -17,207 +15,199 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def batch(self, request: operations.GetBatchCrmCallRequestBody) -> operations.GetBatchCrmCallResponse:
-        r"""Batch Calls
-        Retrieve Call by a set of Id's
+    def batch(self, request: operations.GetBatchCrmEmailRequest) -> operations.GetBatchCrmEmailResponse:
+        r"""Get Batch Emails
+        Retrieve Email by a set of Id's
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/call/batch'
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/email/batch'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetBatchCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmEmailResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmCallRequestBody) -> operations.PostCrmCallResponse:
-        r"""Create Call
-        Create a new Call.
+    def create(self, request: operations.PostCrmEmailRequest) -> operations.PostCrmEmailResponse:
+        r"""Create Email
+        Create a new Email.
+        *CRM Caveats*:
+        
+        - Pipedrive: Not supported.
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/call'
+        url = base_url.removesuffix('/') + '/crm/email'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmEmailResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmCallRequest) -> operations.GetDetailsCrmCallResponse:
-        r"""Get Call Details
-        Get details about all Calls. 
+    def details(self, request: operations.GetDetailsCrmEmailRequest) -> operations.GetDetailsCrmEmailResponse:
+        r"""Get Email Details
+        Get details about all emails. 
         Details include the type, possible values, and other meta data about the fields.
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/call/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmCallRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/email/details'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetDetailsCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmEmailResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmCallRequest) -> operations.GetOneCrmCallResponse:
-        r"""Get Call
-        Retrieve a single Call by Id
+    def find(self, request: operations.GetOneCrmEmailRequest) -> operations.GetOneCrmEmailResponse:
+        r"""Get Email
+        Retrieve a single Task by Id
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/call'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmCallRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/email'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmEmailResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmCallsRequest) -> operations.GetAllCrmCallsResponse:
-        r"""Get All Calls
-        Retrieve all Calls
+    def list(self, request: operations.GetAllCrmEmailsRequest) -> operations.GetAllCrmEmailsResponse:
+        r"""Get All Emails
+        Retrieve all Emails
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/calls'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmCallsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/emails'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmCallsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAllCrmEmailsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmCallsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmEmailsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmCallsRequest) -> operations.SearchCrmCallsResponse:
-        r"""Search Calls
-        Search all Calls using filters
+    def search(self, request: operations.SearchCrmEmailsRequest) -> operations.SearchCrmEmailsResponse:
+        r"""Search Emails
+        Search all Emails using filters
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/calls/search'
+        url = base_url.removesuffix('/') + '/crm/emails/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmCallsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmCallsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.SearchCrmEmailsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmCallsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmEmailsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmCallRequestBody) -> operations.PutCrmCallResponse:
-        r"""Update Call
-        Update an Call by Id.
+    def update(self, request: operations.PutCrmEmailRequest) -> operations.PutCrmEmailResponse:
+        r"""Update Email
+        Update an Email by Id.
+        *CRM Caveats*:
+        - Pipedrive: Not supported.
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/call'
+        url = base_url.removesuffix('/') + '/crm/email'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PutCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmEmailResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.23.0/src/vesselapi/connections.py` & `vesselapi-3.5.2/src/vesselapi/webhooks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Connections:
+class Webhooks:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -17,86 +15,87 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def delete(self, request: operations.DeleteConnectionRequestBody, security: operations.DeleteConnectionSecurity) -> operations.DeleteConnectionResponse:
-        r"""Delete Connection
-        Remove a connection for a given `connectionId`. Removing a connection disconnects the user's CRM so they'll need to re-authenticate should they want to re-connect their CRM.
+    def create(self, request: operations.PostWebhookRequest) -> operations.PostWebhookResponse:
+        r"""Create Webhook
+        Create a new webhook for a given connection
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/connection/connection'
+        url = base_url.removesuffix('/') + '/connection/webhook'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = utils.configure_security_client(self._client, security)
+        client = self._security_client
         
-        http_res = client.request('DELETE', url, data=data, files=form, headers=headers)
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.DeleteConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostWebhookResponseBody])
+                res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneConnectionRequest) -> operations.GetOneConnectionResponse:
-        r"""Get Connection
-        Get info about a connection for a given accessToken.
+    def delete(self, request: operations.DeleteWebhookRequest) -> operations.DeleteWebhookResponse:
+        r"""Remove Webhook
+        Removes a webhook for a given connection and id
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/connection/connection'
+        url = base_url.removesuffix('/') + '/connection/webhook'
+        
         headers = {}
-        query_params = utils.get_query_params(operations.GetOneConnectionRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        req_content_type, data, form = utils.serialize_request_body(request)
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('DELETE', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneConnectionResponseBody])
-                res.response_body = out
+            pass
 
         return res
 
-    
-    def list(self) -> operations.GetAllCrmConnectionsResponse:
-        r"""Get All Connections
-        List all established connections for a workspace
+    def find(self, request: operations.GetOneWebhookRequest) -> operations.GetOneWebhookResponse:
+        r"""Get Webhook
+        Retrieve information about a webhook for a given connection and id
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/connection/connections'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/connection/webhook'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmConnectionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmConnectionsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneWebhookResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.23.0/src/vesselapi/contacts.py` & `vesselapi-3.5.2/src/vesselapi/contacts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Contacts:
     _client: requests_http.Session
@@ -17,55 +15,52 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def batch(self, request: operations.GetBatchCrmContactRequest) -> operations.GetBatchCrmContactResponse:
         r"""Get Batch Contacts
         Retrieve Contacts by a set of Id's
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/contact/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmContactRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBatchCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmContactRequestBody) -> operations.PostCrmContactResponse:
+    def create(self, request: operations.PostCrmContactRequest) -> operations.PostCrmContactResponse:
         r"""Create Contact
         Create a new contact.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/contact'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
@@ -73,111 +68,104 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmContactRequest) -> operations.GetDetailsCrmContactResponse:
         r"""Get Contact Details
         Get details about all contacts. 
         Details include the type, possible values, and other meta data about the fields.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/contact/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmContactRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDetailsCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmContactRequest) -> operations.GetOneCrmContactResponse:
         r"""Get Contact
         Retrieve a Contact by either Id or email. When both email and Id are included, Id will take priority.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/contact'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmContactRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetOneCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmContactsRequest) -> operations.GetAllCrmContactsResponse:
         r"""Get All Contacts
         Retrieve all Contacts
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/contacts'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmContactsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmContactsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmContactsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmContactsRequest) -> operations.SearchCrmContactsResponse:
         r"""Search Contacts
         Search all Contacts using filters
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/contacts/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmContactsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchCrmContactsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
@@ -185,28 +173,27 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmContactsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmContactRequestBody) -> operations.PutCrmContactResponse:
+    def update(self, request: operations.PutCrmContactRequest) -> operations.PutCrmContactResponse:
         r"""Update Contact
         Update an existing Contact.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/contact'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PutCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/deals.py` & `vesselapi-3.5.2/src/vesselapi/deals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Deals:
     _client: requests_http.Session
@@ -17,55 +15,52 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def batch(self, request: operations.GetBatchCrmDealRequest) -> operations.GetBatchCrmDealResponse:
         r"""Get Batch Deals
         Retrieve Deals by a set of Id's
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/deal/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmDealRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBatchCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmDealRequestBody) -> operations.PostCrmDealResponse:
+    def create(self, request: operations.PostCrmDealRequest) -> operations.PostCrmDealResponse:
         r"""Create Deal
         Create a new Deal
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/deal'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
@@ -73,111 +68,104 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmDealRequest) -> operations.GetDetailsCrmDealResponse:
         r"""Get Deal Details
         Get details about all deals or a particular deal. 
         Details include the type, possible values, and other meta data about the fields.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/deal/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmDealRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDetailsCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmDealRequest) -> operations.GetOneCrmDealResponse:
         r"""Get Deal
         Retrieve a single Deal by Id
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/deal'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmDealRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetOneCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmDealsRequest) -> operations.GetAllCrmDealsResponse:
         r"""Get All Deals
         Retrieve all Deals
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/deals'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmDealsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmDealsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmDealsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmDealsRequest) -> operations.SearchCrmDealsResponse:
         r"""Search Deals
         Search all Deals using filters
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/deals/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmDealsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchCrmDealsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
@@ -185,28 +173,27 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmDealsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmDealRequestBody) -> operations.PutCrmDealResponse:
+    def update(self, request: operations.PutCrmDealRequest) -> operations.PutCrmDealResponse:
         r"""Update Deal
         Update an existing Deal
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/deal'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PutCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/emails.py` & `vesselapi-3.5.2/src/vesselapi/leads.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Emails:
+class Leads:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -17,210 +15,196 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def batch(self, request: operations.GetBatchCrmEmailRequest) -> operations.GetBatchCrmEmailResponse:
-        r"""Get Batch Emails
-        Retrieve Email by a set of Id's
+    def batch(self, request: operations.GetBatchCrmLeadRequest) -> operations.GetBatchCrmLeadResponse:
+        r"""Get Batch Leads
+        Retrieve Leads by a set of Id's
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/email/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmEmailRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/lead/batch'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetBatchCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmEmailResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmEmailRequestBody) -> operations.PostCrmEmailResponse:
-        r"""Create Email
-        Create a new Email.
-        *CRM Caveats*:
-        
-        - Pipedrive: Not supported.
+    def create(self, request: operations.PostCrmLeadRequest) -> operations.PostCrmLeadResponse:
+        r"""Create Lead
+        Create a new Lead
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/email'
+        url = base_url.removesuffix('/') + '/crm/lead'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmEmailResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmEmailRequest) -> operations.GetDetailsCrmEmailResponse:
-        r"""Get Email Details
-        Get details about all emails. 
+    def details(self, request: operations.GetDetailsCrmLeadRequest) -> operations.GetDetailsCrmLeadResponse:
+        r"""Get Lead Details
+        Get details about all leads. 
         Details include the type, possible values, and other meta data about the fields.
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/email/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmEmailRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/lead/details'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetDetailsCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmEmailResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmEmailRequest) -> operations.GetOneCrmEmailResponse:
-        r"""Get Email
-        Retrieve a single Task by Id
+    def find(self, request: operations.GetOneCrmLeadRequest) -> operations.GetOneCrmLeadResponse:
+        r"""Get Lead
+        Retrieve a single Lead by Id
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/email'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmEmailRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/lead'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmEmailResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmEmailsRequest) -> operations.GetAllCrmEmailsResponse:
-        r"""Get All Emails
-        Retrieve all Emails
+    def list(self, request: operations.GetAllCrmLeadsRequest) -> operations.GetAllCrmLeadsResponse:
+        r"""Get All Leads
+        Retrieve all leads.
+        *CRM Caveats*:
+        - Pipedrive: Only `jobTitle` is returned when querying for all leads
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/emails'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmEmailsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/leads'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmEmailsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAllCrmLeadsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmEmailsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmLeadsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmEmailsRequest) -> operations.SearchCrmEmailsResponse:
-        r"""Search Emails
-        Search all Emails using filters
+    def search(self, request: operations.SearchCrmLeadsRequest) -> operations.SearchCrmLeadsResponse:
+        r"""Search Leads
+        Search all Leads using filters
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/emails/search'
+        url = base_url.removesuffix('/') + '/crm/leads/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmEmailsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmEmailsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.SearchCrmLeadsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmEmailsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmLeadsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmEmailRequestBody) -> operations.PutCrmEmailResponse:
-        r"""Update Email
-        Update an Email by Id.
-        *CRM Caveats*:
-        - Pipedrive: Not supported.
+    def update(self, request: operations.PutCrmLeadRequest) -> operations.PutCrmLeadResponse:
+        r"""Update Lead
+        Update an existing Lead by Id
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/email'
+        url = base_url.removesuffix('/') + '/crm/lead'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmEmailResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PutCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmEmailResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmLeadResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.23.0/src/vesselapi/events.py` & `vesselapi-3.5.2/src/vesselapi/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Events:
     _client: requests_http.Session
@@ -17,55 +15,52 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def batch(self, request: operations.GetBatchCrmEventRequest) -> operations.GetBatchCrmEventResponse:
         r"""Get Batch Events
         Retrieve Events by a set of Id's
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmEventRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBatchCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmEventRequestBody) -> operations.PostCrmEventResponse:
+    def create(self, request: operations.PostCrmEventRequest) -> operations.PostCrmEventResponse:
         r"""Create Event
         Create a new Event.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
@@ -73,111 +68,104 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmEventRequest) -> operations.GetDetailsCrmEventResponse:
         r"""Get Event Details
         Get details about all events. 
         Details include the type, possible values, and other meta data about the fields.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmEventRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDetailsCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmEventRequest) -> operations.GetOneCrmEventResponse:
         r"""Get Event
         Retrieve a single Event by Id
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmEventRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetOneCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmEventsRequest) -> operations.GetAllCrmEventsResponse:
         r"""Get All Events
         Retrieve all Events
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/events'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmEventsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmEventsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmEventsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmEventsRequest) -> operations.SearchCrmEventsResponse:
         r"""Search Events
         Search all Events using filters
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/events/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmEventsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchCrmEventsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
@@ -185,28 +173,27 @@
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmEventsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmEventRequestBody) -> operations.PutCrmEventResponse:
+    def update(self, request: operations.PutCrmEventRequest) -> operations.PutCrmEventResponse:
         r"""Update Event
         Update an existing Event by Id
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/event'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PutCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/integrations.py` & `vesselapi-3.5.2/src/vesselapi/integrations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Integrations:
     _client: requests_http.Session
@@ -17,29 +15,27 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def list(self) -> operations.GetAllCrmIntegrationsResponse:
         r"""Get CRM Integrations
         Return all of the CRM integrations supported by Vessel.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/connection/crm/integrations'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
         
         client = self._security_client
         
-        http_res = client.request('GET', url, headers=headers)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmIntegrationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmIntegrationsResponseBody])
```

### Comparing `vesselapi-3.23.0/src/vesselapi/leads.py` & `vesselapi-3.5.2/src/vesselapi/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Leads:
+class Tasks:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -17,207 +15,196 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def batch(self, request: operations.GetBatchCrmLeadRequest) -> operations.GetBatchCrmLeadResponse:
-        r"""Get Batch Leads
-        Retrieve Leads by a set of Id's
+    def batch(self, request: operations.GetBatchCrmTaskRequest) -> operations.GetBatchCrmTaskResponse:
+        r"""Get Batch Tasks
+        Retrieve Tasks by a set of Id's
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/lead/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmLeadRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/task/batch'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetBatchCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmLeadResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmLeadRequestBody) -> operations.PostCrmLeadResponse:
-        r"""Create Lead
-        Create a new Lead
+    def create(self, request: operations.PostCrmTaskRequest) -> operations.PostCrmTaskResponse:
+        r"""Create Task
+        Create a new Task.
+        *CRM Caveats*:
+        - Salesforce: You may only associate a Task with either a Lead or a Contact *and* either a Deal or an Account.
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/lead'
+        url = base_url.removesuffix('/') + '/crm/task'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmLeadResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmLeadRequest) -> operations.GetDetailsCrmLeadResponse:
-        r"""Get Lead Details
-        Get details about all leads. 
+    def details(self, request: operations.GetDetailsCrmTaskRequest) -> operations.GetDetailsCrmTaskResponse:
+        r"""Get Task Details
+        Get details about all tasks. 
         Details include the type, possible values, and other meta data about the fields.
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/lead/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmLeadRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/task/details'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetDetailsCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmLeadResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmLeadRequest) -> operations.GetOneCrmLeadResponse:
-        r"""Get Lead
-        Retrieve a single Lead by Id
+    def find(self, request: operations.GetOneCrmTaskRequest) -> operations.GetOneCrmTaskResponse:
+        r"""Get Task
+        Retrieve a single Task by Id
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/lead'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmLeadRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/task'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmLeadResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmLeadsRequest) -> operations.GetAllCrmLeadsResponse:
-        r"""Get All Leads
-        Retrieve all leads.
-        *CRM Caveats*:
-        - Pipedrive: Only `jobTitle` is returned when querying for all leads
+    def list(self, request: operations.GetAllCrmTasksRequest) -> operations.GetAllCrmTasksResponse:
+        r"""Get All Tasks
+        Retrieve all Tasks
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/leads'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmLeadsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        url = base_url.removesuffix('/') + '/crm/tasks'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmLeadsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAllCrmTasksResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmLeadsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmTasksResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmLeadsRequest) -> operations.SearchCrmLeadsResponse:
-        r"""Search Leads
-        Search all Leads using filters
+    def search(self, request: operations.SearchCrmTasksRequest) -> operations.SearchCrmTasksResponse:
+        r"""Search Tasks
+        Search all Tasks using filters
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/leads/search'
+        url = base_url.removesuffix('/') + '/crm/tasks/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmLeadsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmLeadsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.SearchCrmTasksResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmLeadsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmTasksResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmLeadRequestBody) -> operations.PutCrmLeadResponse:
-        r"""Update Lead
-        Update an existing Lead by Id
+    def update(self, request: operations.PutCrmTaskRequest) -> operations.PutCrmTaskResponse:
+        r"""Update Task
+        Update an existing Task by Id
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/crm/lead'
+        url = base_url.removesuffix('/') + '/crm/task'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PutCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmLeadResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmTaskResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.23.0/src/vesselapi/links.py` & `vesselapi-3.5.2/src/vesselapi/passthrough.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
-class Links:
+class Passthrough:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -17,37 +15,36 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def create(self, request: operations.PostLinkExchangeRequestBody, security: operations.PostLinkExchangeSecurity) -> operations.PostLinkExchangeResponse:
-        r"""Exchange Public Token for Access Token
-        Exchanges the public token for an access token used to interact with the account. Store the access token in a secure location.
+    def create(self, request: operations.PostCrmPassthroughRequest) -> operations.PostCrmPassthroughResponse:
+        r"""Passthrough Request
+        Send an authenticated passthrough request to the downstream CRM. This is useful for making requests to endpoints that are not yet supported by Vessel.
         """
+        
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/link/exchange'
+        url = base_url.removesuffix('/') + '/crm/passthrough'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = utils.configure_security_client(self._client, security)
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostLinkExchangeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmPassthroughResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostLinkExchangeResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmPassthroughResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/__init__.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,80 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from .delete_connection import *
 from .delete_webhook import *
 from .get_all_crm_accounts import *
-from .get_all_crm_calls import *
 from .get_all_crm_connections import *
 from .get_all_crm_contacts import *
 from .get_all_crm_deals import *
 from .get_all_crm_emails import *
 from .get_all_crm_event_attendees import *
 from .get_all_crm_events import *
 from .get_all_crm_integrations import *
 from .get_all_crm_leads import *
 from .get_all_crm_notes import *
 from .get_all_crm_tasks import *
 from .get_all_crm_users import *
 from .get_batch_crm_account import *
-from .get_batch_crm_call import *
 from .get_batch_crm_contact import *
 from .get_batch_crm_deal import *
 from .get_batch_crm_email import *
 from .get_batch_crm_event import *
 from .get_batch_crm_event_attendee import *
 from .get_batch_crm_lead import *
 from .get_batch_crm_note import *
 from .get_batch_crm_task import *
 from .get_batch_crm_user import *
 from .get_details_crm_account import *
-from .get_details_crm_call import *
 from .get_details_crm_contact import *
 from .get_details_crm_deal import *
 from .get_details_crm_email import *
 from .get_details_crm_event import *
 from .get_details_crm_event_attendee import *
 from .get_details_crm_lead import *
 from .get_details_crm_note import *
 from .get_details_crm_task import *
 from .get_details_crm_user import *
 from .get_one_connection import *
 from .get_one_crm_account import *
-from .get_one_crm_call import *
 from .get_one_crm_contact import *
 from .get_one_crm_deal import *
 from .get_one_crm_email import *
 from .get_one_crm_event import *
 from .get_one_crm_event_attendee import *
 from .get_one_crm_lead import *
 from .get_one_crm_note import *
 from .get_one_crm_task import *
 from .get_one_crm_user import *
 from .get_one_webhook import *
 from .post_crm_account import *
-from .post_crm_call import *
 from .post_crm_contact import *
 from .post_crm_deal import *
 from .post_crm_email import *
 from .post_crm_event import *
 from .post_crm_event_attendee import *
 from .post_crm_lead import *
 from .post_crm_note import *
 from .post_crm_passthrough import *
 from .post_crm_task import *
 from .post_link_exchange import *
 from .post_link_token import *
 from .post_webhook import *
 from .put_crm_account import *
-from .put_crm_call import *
 from .put_crm_contact import *
 from .put_crm_deal import *
 from .put_crm_email import *
 from .put_crm_event import *
 from .put_crm_event_attendee import *
 from .put_crm_lead import *
 from .put_crm_note import *
 from .put_crm_task import *
 from .search_crm_accounts import *
-from .search_crm_calls import *
 from .search_crm_contacts import *
 from .search_crm_deals import *
 from .search_crm_emails import *
 from .search_crm_event_attendees import *
 from .search_crm_events import *
 from .search_crm_leads import *
 from .search_crm_notes import *
 from .search_crm_tasks import *
 from .search_crm_users import *
 
-__all__ = ["DeleteConnectionRequestBody","DeleteConnectionResponse","DeleteConnectionSecurity","DeleteWebhookRequestBody","DeleteWebhookResponse","GetAllCrmAccountsRequest","GetAllCrmAccountsResponse","GetAllCrmAccountsResponseBody","GetAllCrmCallsRequest","GetAllCrmCallsResponse","GetAllCrmCallsResponseBody","GetAllCrmConnectionsResponse","GetAllCrmConnectionsResponseBody","GetAllCrmContactsRequest","GetAllCrmContactsResponse","GetAllCrmContactsResponseBody","GetAllCrmDealsRequest","GetAllCrmDealsResponse","GetAllCrmDealsResponseBody","GetAllCrmEmailsRequest","GetAllCrmEmailsResponse","GetAllCrmEmailsResponseBody","GetAllCrmEventAttendeesRequest","GetAllCrmEventAttendeesResponse","GetAllCrmEventAttendeesResponseBody","GetAllCrmEventsRequest","GetAllCrmEventsResponse","GetAllCrmEventsResponseBody","GetAllCrmIntegrationsResponse","GetAllCrmIntegrationsResponseBody","GetAllCrmLeadsRequest","GetAllCrmLeadsResponse","GetAllCrmLeadsResponseBody","GetAllCrmNotesRequest","GetAllCrmNotesResponse","GetAllCrmNotesResponseBody","GetAllCrmTasksRequest","GetAllCrmTasksResponse","GetAllCrmTasksResponseBody","GetAllCrmUsersRequest","GetAllCrmUsersResponse","GetAllCrmUsersResponseBody","GetBatchCrmAccountRequest","GetBatchCrmAccountResponse","GetBatchCrmAccountResponseBody","GetBatchCrmCallRequestBody","GetBatchCrmCallResponse","GetBatchCrmCallResponseBody","GetBatchCrmContactRequest","GetBatchCrmContactResponse","GetBatchCrmContactResponseBody","GetBatchCrmDealRequest","GetBatchCrmDealResponse","GetBatchCrmDealResponseBody","GetBatchCrmEmailRequest","GetBatchCrmEmailResponse","GetBatchCrmEmailResponseBody","GetBatchCrmEventAttendeeRequest","GetBatchCrmEventAttendeeResponse","GetBatchCrmEventAttendeeResponseBody","GetBatchCrmEventRequest","GetBatchCrmEventResponse","GetBatchCrmEventResponseBody","GetBatchCrmLeadRequest","GetBatchCrmLeadResponse","GetBatchCrmLeadResponseBody","GetBatchCrmNoteRequest","GetBatchCrmNoteResponse","GetBatchCrmNoteResponseBody","GetBatchCrmTaskRequest","GetBatchCrmTaskResponse","GetBatchCrmTaskResponseBody","GetBatchCrmUserRequest","GetBatchCrmUserResponse","GetBatchCrmUserResponseBody","GetDetailsCrmAccountRequest","GetDetailsCrmAccountResponse","GetDetailsCrmAccountResponseBody","GetDetailsCrmCallRequest","GetDetailsCrmCallResponse","GetDetailsCrmCallResponseBody","GetDetailsCrmContactRequest","GetDetailsCrmContactResponse","GetDetailsCrmContactResponseBody","GetDetailsCrmDealRequest","GetDetailsCrmDealResponse","GetDetailsCrmDealResponseBody","GetDetailsCrmEmailRequest","GetDetailsCrmEmailResponse","GetDetailsCrmEmailResponseBody","GetDetailsCrmEventAttendeeRequest","GetDetailsCrmEventAttendeeResponse","GetDetailsCrmEventAttendeeResponseBody","GetDetailsCrmEventRequest","GetDetailsCrmEventResponse","GetDetailsCrmEventResponseBody","GetDetailsCrmLeadRequest","GetDetailsCrmLeadResponse","GetDetailsCrmLeadResponseBody","GetDetailsCrmNoteRequest","GetDetailsCrmNoteResponse","GetDetailsCrmNoteResponseBody","GetDetailsCrmTaskRequest","GetDetailsCrmTaskResponse","GetDetailsCrmTaskResponseBody","GetDetailsCrmUserRequest","GetDetailsCrmUserResponse","GetDetailsCrmUserResponseBody","GetOneConnectionRequest","GetOneConnectionResponse","GetOneConnectionResponseBody","GetOneCrmAccountRequest","GetOneCrmAccountResponse","GetOneCrmAccountResponseBody","GetOneCrmCallRequest","GetOneCrmCallResponse","GetOneCrmCallResponseBody","GetOneCrmContactRequest","GetOneCrmContactResponse","GetOneCrmContactResponseBody","GetOneCrmDealRequest","GetOneCrmDealResponse","GetOneCrmDealResponseBody","GetOneCrmEmailRequest","GetOneCrmEmailResponse","GetOneCrmEmailResponseBody","GetOneCrmEventAttendeeRequest","GetOneCrmEventAttendeeResponse","GetOneCrmEventAttendeeResponseBody","GetOneCrmEventRequest","GetOneCrmEventResponse","GetOneCrmEventResponseBody","GetOneCrmLeadRequest","GetOneCrmLeadResponse","GetOneCrmLeadResponseBody","GetOneCrmNoteRequest","GetOneCrmNoteResponse","GetOneCrmNoteResponseBody","GetOneCrmTaskRequest","GetOneCrmTaskResponse","GetOneCrmTaskResponseBody","GetOneCrmUserRequest","GetOneCrmUserResponse","GetOneCrmUserResponseBody","GetOneWebhookRequest","GetOneWebhookResponse","GetOneWebhookResponseBody","PostCrmAccountRequestBody","PostCrmAccountResponse","PostCrmAccountResponseBody","PostCrmCallRequestBody","PostCrmCallResponse","PostCrmCallResponseBody","PostCrmContactRequestBody","PostCrmContactResponse","PostCrmContactResponseBody","PostCrmDealRequestBody","PostCrmDealResponse","PostCrmDealResponseBody","PostCrmEmailRequestBody","PostCrmEmailResponse","PostCrmEmailResponseBody","PostCrmEventAttendeeResponse","PostCrmEventAttendeeResponseBody","PostCrmEventRequestBody","PostCrmEventResponse","PostCrmEventResponseBody","PostCrmLeadRequestBody","PostCrmLeadResponse","PostCrmLeadResponseBody","PostCrmNoteRequestBody","PostCrmNoteResponse","PostCrmNoteResponseBody","PostCrmPassthroughRequestBody","PostCrmPassthroughRequestBodyMethod","PostCrmPassthroughResponse","PostCrmPassthroughResponseBody","PostCrmTaskRequestBody","PostCrmTaskResponse","PostCrmTaskResponseBody","PostLinkExchangeRequestBody","PostLinkExchangeResponse","PostLinkExchangeResponseBody","PostLinkExchangeResponseBodyIntegrationID","PostLinkExchangeSecurity","PostLinkTokenResponse","PostLinkTokenResponseBody","PostLinkTokenSecurity","PostWebhookRequestBody","PostWebhookResponse","PostWebhookResponseBody","PutCrmAccountRequestBody","PutCrmAccountResponse","PutCrmAccountResponseBody","PutCrmCallRequestBody","PutCrmCallResponse","PutCrmCallResponseBody","PutCrmContactRequestBody","PutCrmContactResponse","PutCrmContactResponseBody","PutCrmDealRequestBody","PutCrmDealResponse","PutCrmDealResponseBody","PutCrmEmailRequestBody","PutCrmEmailResponse","PutCrmEmailResponseBody","PutCrmEventAttendeeResponse","PutCrmEventAttendeeResponseBody","PutCrmEventRequestBody","PutCrmEventResponse","PutCrmEventResponseBody","PutCrmLeadRequestBody","PutCrmLeadResponse","PutCrmLeadResponseBody","PutCrmNoteRequestBody","PutCrmNoteResponse","PutCrmNoteResponseBody","PutCrmTaskRequestBody","PutCrmTaskResponse","PutCrmTaskResponseBody","SearchCrmAccountsRequest","SearchCrmAccountsRequestBody","SearchCrmAccountsRequestBodyFilters","SearchCrmAccountsResponse","SearchCrmAccountsResponseBody","SearchCrmCallsRequest","SearchCrmCallsRequestBody","SearchCrmCallsRequestBodyFilters","SearchCrmCallsResponse","SearchCrmCallsResponseBody","SearchCrmContactsRequest","SearchCrmContactsRequestBody","SearchCrmContactsRequestBodyFilters","SearchCrmContactsResponse","SearchCrmContactsResponseBody","SearchCrmDealsRequest","SearchCrmDealsRequestBody","SearchCrmDealsRequestBodyFilters","SearchCrmDealsResponse","SearchCrmDealsResponseBody","SearchCrmEmailsRequest","SearchCrmEmailsRequestBody","SearchCrmEmailsRequestBodyFilters","SearchCrmEmailsResponse","SearchCrmEmailsResponseBody","SearchCrmEventAttendeesRequest","SearchCrmEventAttendeesRequestBody","SearchCrmEventAttendeesRequestBodyFilters","SearchCrmEventAttendeesResponse","SearchCrmEventAttendeesResponseBody","SearchCrmEventsRequest","SearchCrmEventsRequestBody","SearchCrmEventsRequestBodyFilters","SearchCrmEventsResponse","SearchCrmEventsResponseBody","SearchCrmLeadsRequest","SearchCrmLeadsRequestBody","SearchCrmLeadsRequestBodyFilters","SearchCrmLeadsResponse","SearchCrmLeadsResponseBody","SearchCrmNotesRequest","SearchCrmNotesRequestBody","SearchCrmNotesRequestBodyFilters","SearchCrmNotesResponse","SearchCrmNotesResponseBody","SearchCrmTasksRequest","SearchCrmTasksRequestBody","SearchCrmTasksRequestBodyFilters","SearchCrmTasksResponse","SearchCrmTasksResponseBody","SearchCrmUsersRequest","SearchCrmUsersRequestBody","SearchCrmUsersRequestBodyFilters","SearchCrmUsersResponse","SearchCrmUsersResponseBody"]
+__all__ = ["DeleteConnectionRequest","DeleteConnectionRequestBody","DeleteConnectionResponse","DeleteConnectionSecurity","DeleteWebhookRequest","DeleteWebhookRequestBody","DeleteWebhookResponse","GetAllCrmAccountsQueryParams","GetAllCrmAccountsRequest","GetAllCrmAccountsResponse","GetAllCrmAccountsResponseBody","GetAllCrmConnectionsResponse","GetAllCrmConnectionsResponseBody","GetAllCrmContactsQueryParams","GetAllCrmContactsRequest","GetAllCrmContactsResponse","GetAllCrmContactsResponseBody","GetAllCrmDealsQueryParams","GetAllCrmDealsRequest","GetAllCrmDealsResponse","GetAllCrmDealsResponseBody","GetAllCrmEmailsQueryParams","GetAllCrmEmailsRequest","GetAllCrmEmailsResponse","GetAllCrmEmailsResponseBody","GetAllCrmEventAttendeesQueryParams","GetAllCrmEventAttendeesRequest","GetAllCrmEventAttendeesResponse","GetAllCrmEventAttendeesResponseBody","GetAllCrmEventsQueryParams","GetAllCrmEventsRequest","GetAllCrmEventsResponse","GetAllCrmEventsResponseBody","GetAllCrmIntegrationsResponse","GetAllCrmIntegrationsResponseBody","GetAllCrmLeadsQueryParams","GetAllCrmLeadsRequest","GetAllCrmLeadsResponse","GetAllCrmLeadsResponseBody","GetAllCrmNotesQueryParams","GetAllCrmNotesRequest","GetAllCrmNotesResponse","GetAllCrmNotesResponseBody","GetAllCrmTasksQueryParams","GetAllCrmTasksRequest","GetAllCrmTasksResponse","GetAllCrmTasksResponseBody","GetAllCrmUsersQueryParams","GetAllCrmUsersRequest","GetAllCrmUsersResponse","GetAllCrmUsersResponseBody","GetBatchCrmAccountQueryParams","GetBatchCrmAccountRequest","GetBatchCrmAccountResponse","GetBatchCrmAccountResponseBody","GetBatchCrmContactQueryParams","GetBatchCrmContactRequest","GetBatchCrmContactResponse","GetBatchCrmContactResponseBody","GetBatchCrmDealQueryParams","GetBatchCrmDealRequest","GetBatchCrmDealResponse","GetBatchCrmDealResponseBody","GetBatchCrmEmailQueryParams","GetBatchCrmEmailRequest","GetBatchCrmEmailResponse","GetBatchCrmEmailResponseBody","GetBatchCrmEventAttendeeQueryParams","GetBatchCrmEventAttendeeRequest","GetBatchCrmEventAttendeeResponse","GetBatchCrmEventAttendeeResponseBody","GetBatchCrmEventQueryParams","GetBatchCrmEventRequest","GetBatchCrmEventResponse","GetBatchCrmEventResponseBody","GetBatchCrmLeadQueryParams","GetBatchCrmLeadRequest","GetBatchCrmLeadResponse","GetBatchCrmLeadResponseBody","GetBatchCrmNoteQueryParams","GetBatchCrmNoteRequest","GetBatchCrmNoteResponse","GetBatchCrmNoteResponseBody","GetBatchCrmTaskQueryParams","GetBatchCrmTaskRequest","GetBatchCrmTaskResponse","GetBatchCrmTaskResponseBody","GetBatchCrmUserQueryParams","GetBatchCrmUserRequest","GetBatchCrmUserResponse","GetBatchCrmUserResponseBody","GetDetailsCrmAccountQueryParams","GetDetailsCrmAccountRequest","GetDetailsCrmAccountResponse","GetDetailsCrmAccountResponseBody","GetDetailsCrmContactQueryParams","GetDetailsCrmContactRequest","GetDetailsCrmContactResponse","GetDetailsCrmContactResponseBody","GetDetailsCrmDealQueryParams","GetDetailsCrmDealRequest","GetDetailsCrmDealResponse","GetDetailsCrmDealResponseBody","GetDetailsCrmEmailQueryParams","GetDetailsCrmEmailRequest","GetDetailsCrmEmailResponse","GetDetailsCrmEmailResponseBody","GetDetailsCrmEventAttendeeQueryParams","GetDetailsCrmEventAttendeeRequest","GetDetailsCrmEventAttendeeResponse","GetDetailsCrmEventAttendeeResponseBody","GetDetailsCrmEventQueryParams","GetDetailsCrmEventRequest","GetDetailsCrmEventResponse","GetDetailsCrmEventResponseBody","GetDetailsCrmLeadQueryParams","GetDetailsCrmLeadRequest","GetDetailsCrmLeadResponse","GetDetailsCrmLeadResponseBody","GetDetailsCrmNoteQueryParams","GetDetailsCrmNoteRequest","GetDetailsCrmNoteResponse","GetDetailsCrmNoteResponseBody","GetDetailsCrmTaskQueryParams","GetDetailsCrmTaskRequest","GetDetailsCrmTaskResponse","GetDetailsCrmTaskResponseBody","GetDetailsCrmUserQueryParams","GetDetailsCrmUserRequest","GetDetailsCrmUserResponse","GetDetailsCrmUserResponseBody","GetOneConnectionQueryParams","GetOneConnectionRequest","GetOneConnectionResponse","GetOneConnectionResponseBody","GetOneCrmAccountQueryParams","GetOneCrmAccountRequest","GetOneCrmAccountResponse","GetOneCrmAccountResponseBody","GetOneCrmContactQueryParams","GetOneCrmContactRequest","GetOneCrmContactResponse","GetOneCrmContactResponseBody","GetOneCrmDealQueryParams","GetOneCrmDealRequest","GetOneCrmDealResponse","GetOneCrmDealResponseBody","GetOneCrmEmailQueryParams","GetOneCrmEmailRequest","GetOneCrmEmailResponse","GetOneCrmEmailResponseBody","GetOneCrmEventAttendeeQueryParams","GetOneCrmEventAttendeeRequest","GetOneCrmEventAttendeeResponse","GetOneCrmEventAttendeeResponseBody","GetOneCrmEventQueryParams","GetOneCrmEventRequest","GetOneCrmEventResponse","GetOneCrmEventResponseBody","GetOneCrmLeadQueryParams","GetOneCrmLeadRequest","GetOneCrmLeadResponse","GetOneCrmLeadResponseBody","GetOneCrmNoteQueryParams","GetOneCrmNoteRequest","GetOneCrmNoteResponse","GetOneCrmNoteResponseBody","GetOneCrmTaskQueryParams","GetOneCrmTaskRequest","GetOneCrmTaskResponse","GetOneCrmTaskResponseBody","GetOneCrmUserQueryParams","GetOneCrmUserRequest","GetOneCrmUserResponse","GetOneCrmUserResponseBody","GetOneWebhookQueryParams","GetOneWebhookRequest","GetOneWebhookResponse","GetOneWebhookResponseBody","PostCrmAccountRequest","PostCrmAccountRequestBody","PostCrmAccountResponse","PostCrmAccountResponseBody","PostCrmContactRequest","PostCrmContactRequestBody","PostCrmContactResponse","PostCrmContactResponseBody","PostCrmDealRequest","PostCrmDealRequestBody","PostCrmDealResponse","PostCrmDealResponseBody","PostCrmEmailRequest","PostCrmEmailRequestBody","PostCrmEmailResponse","PostCrmEmailResponseBody","PostCrmEventAttendeeResponse","PostCrmEventAttendeeResponseBody","PostCrmEventRequest","PostCrmEventRequestBody","PostCrmEventResponse","PostCrmEventResponseBody","PostCrmLeadRequest","PostCrmLeadRequestBody","PostCrmLeadResponse","PostCrmLeadResponseBody","PostCrmNoteRequest","PostCrmNoteRequestBody","PostCrmNoteResponse","PostCrmNoteResponseBody","PostCrmPassthroughRequest","PostCrmPassthroughRequestBody","PostCrmPassthroughRequestBodyMethodEnum","PostCrmPassthroughResponse","PostCrmPassthroughResponseBody","PostCrmTaskRequest","PostCrmTaskRequestBody","PostCrmTaskResponse","PostCrmTaskResponseBody","PostLinkExchangeRequest","PostLinkExchangeRequestBody","PostLinkExchangeResponse","PostLinkExchangeResponseBody","PostLinkExchangeResponseBodyIntegrationIDEnum","PostLinkExchangeSecurity","PostLinkTokenRequest","PostLinkTokenResponse","PostLinkTokenResponseBody","PostLinkTokenSecurity","PostWebhookRequest","PostWebhookRequestBody","PostWebhookResponse","PostWebhookResponseBody","PutCrmAccountRequest","PutCrmAccountRequestBody","PutCrmAccountResponse","PutCrmAccountResponseBody","PutCrmContactRequest","PutCrmContactRequestBody","PutCrmContactResponse","PutCrmContactResponseBody","PutCrmDealRequest","PutCrmDealRequestBody","PutCrmDealResponse","PutCrmDealResponseBody","PutCrmEmailRequest","PutCrmEmailRequestBody","PutCrmEmailResponse","PutCrmEmailResponseBody","PutCrmEventAttendeeResponse","PutCrmEventAttendeeResponseBody","PutCrmEventRequest","PutCrmEventRequestBody","PutCrmEventResponse","PutCrmEventResponseBody","PutCrmLeadRequest","PutCrmLeadRequestBody","PutCrmLeadResponse","PutCrmLeadResponseBody","PutCrmNoteRequest","PutCrmNoteRequestBody","PutCrmNoteResponse","PutCrmNoteResponseBody","PutCrmTaskRequest","PutCrmTaskRequestBody","PutCrmTaskResponse","PutCrmTaskResponseBody","SearchCrmAccountsQueryParams","SearchCrmAccountsRequest","SearchCrmAccountsRequestBody","SearchCrmAccountsRequestBodyFilters","SearchCrmAccountsResponse","SearchCrmAccountsResponseBody","SearchCrmContactsQueryParams","SearchCrmContactsRequest","SearchCrmContactsRequestBody","SearchCrmContactsRequestBodyFilters","SearchCrmContactsResponse","SearchCrmContactsResponseBody","SearchCrmDealsQueryParams","SearchCrmDealsRequest","SearchCrmDealsRequestBody","SearchCrmDealsRequestBodyFilters","SearchCrmDealsResponse","SearchCrmDealsResponseBody","SearchCrmEmailsQueryParams","SearchCrmEmailsRequest","SearchCrmEmailsRequestBody","SearchCrmEmailsRequestBodyFilters","SearchCrmEmailsResponse","SearchCrmEmailsResponseBody","SearchCrmEventAttendeesQueryParams","SearchCrmEventAttendeesRequest","SearchCrmEventAttendeesRequestBody","SearchCrmEventAttendeesRequestBodyFilters","SearchCrmEventAttendeesResponse","SearchCrmEventAttendeesResponseBody","SearchCrmEventsQueryParams","SearchCrmEventsRequest","SearchCrmEventsRequestBody","SearchCrmEventsRequestBodyFilters","SearchCrmEventsResponse","SearchCrmEventsResponseBody","SearchCrmLeadsQueryParams","SearchCrmLeadsRequest","SearchCrmLeadsRequestBody","SearchCrmLeadsRequestBodyFilters","SearchCrmLeadsResponse","SearchCrmLeadsResponseBody","SearchCrmNotesQueryParams","SearchCrmNotesRequest","SearchCrmNotesRequestBody","SearchCrmNotesRequestBodyFilters","SearchCrmNotesResponse","SearchCrmNotesResponseBody","SearchCrmTasksQueryParams","SearchCrmTasksRequest","SearchCrmTasksRequestBody","SearchCrmTasksRequestBodyFilters","SearchCrmTasksResponse","SearchCrmTasksResponseBody","SearchCrmUsersQueryParams","SearchCrmUsersRequest","SearchCrmUsersRequestBody","SearchCrmUsersRequestBodyFilters","SearchCrmUsersResponse","SearchCrmUsersResponseBody"]
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/delete_connection.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_contact.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import contactcreate as shared_contactcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DeleteConnectionSecurity:
+class PostCrmContactRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    contact: shared_contactcreate.ContactCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
     
-    vessel_api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header', 'field_name': 'vessel-api-token' }})
+
+@dataclasses.dataclass
+class PostCrmContactRequest:
+    request: Optional[PostCrmContactRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DeleteConnectionRequestBody:
-    
-    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
+class PostCrmContactResponseBody:
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class DeleteConnectionResponse:
-    
+class PostCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmContactResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/delete_webhook.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event_attendee.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import eventattendeeupdate as shared_eventattendeeupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DeleteWebhookRequestBody:
-    
+class PutCrmEventAttendeeResponseBody:
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
-    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookId'), 'exclude': lambda f: f is None }})
+    event_attendee: Optional[shared_eventattendeeupdate.EventAttendeeUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class DeleteWebhookResponse:
-    
+class PutCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_accounts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_users.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import account as shared_account
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmAccountsRequest:
-    
+class GetAllCrmUsersQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmAccountsResponseBody:
-    r"""OK"""
+class GetAllCrmUsersRequest:
+    query_params: GetAllCrmUsersQueryParams = dataclasses.field()
     
-    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetAllCrmUsersResponseBody:
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmAccountsResponse:
-    
+class GetAllCrmUsersResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmAccountsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmUsersResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_calls.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_event_attendees.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import call as shared_call
+from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmCallsRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
+class GetAllCrmEventAttendeesQueryParams:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmCallsResponseBody:
-    r"""OK"""
+class GetAllCrmEventAttendeesRequest:
+    query_params: GetAllCrmEventAttendeesQueryParams = dataclasses.field()
     
-    calls: Optional[list[shared_call.Call]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('calls'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetAllCrmEventAttendeesResponseBody:
+    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmCallsResponse:
-    
+class GetAllCrmEventAttendeesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmCallsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmEventAttendeesResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_connections.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import connection as shared_connection
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmConnectionsResponseBody:
-    r"""OK"""
+class GetOneConnectionQueryParams:
+    connection_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'connectionId', 'style': 'form', 'explode': True }})
     
-    connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connections'), 'exclude': lambda f: f is None }})
+
+@dataclasses.dataclass
+class GetOneConnectionRequest:
+    query_params: GetOneConnectionQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmConnectionsResponse:
+class GetOneConnectionResponseBody:
+    connection: Optional[shared_connection.Connection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connection'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetOneConnectionResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmConnectionsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetOneConnectionResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_contacts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_tasks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import contact as shared_contact
+from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmContactsRequest:
-    
+class GetAllCrmTasksQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmContactsResponseBody:
-    r"""OK"""
+class GetAllCrmTasksRequest:
+    query_params: GetAllCrmTasksQueryParams = dataclasses.field()
     
-    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetAllCrmTasksResponseBody:
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmContactsResponse:
-    
+class GetAllCrmTasksResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmContactsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmTasksResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_deals.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_deals.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import deal as shared_deal
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmDealsRequest:
-    
+class GetAllCrmDealsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
+    
+
+@dataclasses.dataclass
+class GetAllCrmDealsRequest:
+    query_params: GetAllCrmDealsQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmDealsResponseBody:
-    r"""OK"""
-    
     deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmDealsResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmDealsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_emails.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import email as shared_email
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmEmailsRequest:
-    
+class GetDetailsCrmEventQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmEmailsResponseBody:
-    r"""OK"""
+class GetDetailsCrmEventRequest:
+    query_params: GetDetailsCrmEventQueryParams = dataclasses.field()
     
-    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmEventResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmEmailsResponse:
-    
+class GetDetailsCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmEmailsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmEventResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_event_attendees.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event_attendee.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventattendee as shared_eventattendee
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmEventAttendeesRequest:
-    
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
+class GetDetailsCrmEventAttendeeQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmEventAttendeesResponseBody:
-    r"""OK"""
+class GetDetailsCrmEventAttendeeRequest:
+    query_params: GetDetailsCrmEventAttendeeQueryParams = dataclasses.field()
     
-    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmEventAttendeeResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmEventAttendeesResponse:
-    
+class GetDetailsCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmEventAttendeesResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_events.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_note.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import event as shared_event
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmEventsRequest:
-    
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
+class GetDetailsCrmNoteQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmEventsResponseBody:
-    r"""OK"""
+class GetDetailsCrmNoteRequest:
+    query_params: GetDetailsCrmNoteQueryParams = dataclasses.field()
     
-    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmNoteResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmEventsResponse:
-    
+class GetDetailsCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmEventsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmNoteResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_integrations.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_integrations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import integration as shared_integration
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetAllCrmIntegrationsResponseBody:
-    r"""OK"""
-    
     integrations: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrations'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class GetAllCrmIntegrationsResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmIntegrationsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_leads.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_lead.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import lead as shared_lead
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmLeadsRequest:
-    
+class GetDetailsCrmLeadQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmLeadsResponseBody:
-    r"""OK"""
+class GetDetailsCrmLeadRequest:
+    query_params: GetDetailsCrmLeadQueryParams = dataclasses.field()
     
-    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmLeadResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmLeadsResponse:
-    
+class GetDetailsCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmLeadsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmLeadResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_notes.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_leads.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import note as shared_note
+from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmNotesRequest:
-    
+class GetAllCrmLeadsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmNotesResponseBody:
-    r"""OK"""
+class GetAllCrmLeadsRequest:
+    query_params: GetAllCrmLeadsQueryParams = dataclasses.field()
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetAllCrmLeadsResponseBody:
+    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmNotesResponse:
-    
+class GetAllCrmLeadsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmNotesResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmLeadsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_tasks.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_notes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import task as shared_task
+from ..shared import note as shared_note
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmTasksRequest:
-    
+class GetAllCrmNotesQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmTasksResponseBody:
-    r"""OK"""
+class GetAllCrmNotesRequest:
+    query_params: GetAllCrmNotesQueryParams = dataclasses.field()
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetAllCrmNotesResponseBody:
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
+    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmTasksResponse:
-    
+class GetAllCrmNotesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmTasksResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmNotesResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_all_crm_users.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import user as shared_user
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetAllCrmUsersRequest:
-    
+class GetDetailsCrmUserQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAllCrmUsersResponseBody:
-    r"""OK"""
+class GetDetailsCrmUserRequest:
+    query_params: GetDetailsCrmUserQueryParams = dataclasses.field()
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmUserResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetAllCrmUsersResponse:
-    
+class GetDetailsCrmUserResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmUsersResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmUserResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_contact.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import account as shared_account
+from ..shared import contact as shared_contact
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmAccountRequest:
-    
+class GetBatchCrmContactQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Account Id's."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmAccountResponseBody:
-    r"""OK"""
+class GetBatchCrmContactRequest:
+    query_params: GetBatchCrmContactQueryParams = dataclasses.field()
     
-    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetBatchCrmContactResponseBody:
+    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
     invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
     
 
 @dataclasses.dataclass
-class GetBatchCrmAccountResponse:
-    
+class GetBatchCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetBatchCrmContactResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_call.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/note.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import call as shared_call
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmCallRequestBody:
-    
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ids') }})
-    r"""List of call Ids."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allFields'), 'exclude': lambda f: f is None }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+class NoteAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmCallResponseBody:
-    r"""OK"""
-    
-    calls: Optional[list[shared_call.Call]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('calls'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    
-
-@dataclasses.dataclass
-class GetBatchCrmCallResponse:
+class Note:
+    r"""Note
+    A Note attached to some CRM Object. 
+    """
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmCallResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    associations: NoteAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_deal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import contact as shared_contact
+from ..shared import deal as shared_deal
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmContactRequest:
-    
+class GetBatchCrmDealQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Contact Id's."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmContactResponseBody:
-    r"""OK"""
+class GetBatchCrmDealRequest:
+    query_params: GetBatchCrmDealQueryParams = dataclasses.field()
     
-    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetBatchCrmDealResponseBody:
+    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
     invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
     
 
 @dataclasses.dataclass
-class GetBatchCrmContactResponse:
-    
+class GetBatchCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmContactResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetBatchCrmDealResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import deal as shared_deal
+from ..shared import taskupdate as shared_taskupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmDealRequest:
+class PutCrmTaskRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    task: Optional[shared_taskupdate.TaskUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Deal Id's."""
+
+@dataclasses.dataclass
+class PutCrmTaskRequest:
+    request: Optional[PutCrmTaskRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmDealResponseBody:
-    r"""OK"""
-    
-    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
+class PutCrmTaskResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmDealResponse:
-    
+class PutCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PutCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_emails.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import email as shared_email
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmEmailRequest:
-    
+class GetAllCrmEmailsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Email Id's."""
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmEmailResponseBody:
-    r"""OK"""
+class GetAllCrmEmailsRequest:
+    query_params: GetAllCrmEmailsQueryParams = dataclasses.field()
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetAllCrmEmailsResponseBody:
     emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmEmailResponse:
-    
+class GetAllCrmEmailsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmEmailResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmEmailsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_connections.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,22 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import event as shared_event
+from ..shared import connection as shared_connection
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclasses.dataclass
-class GetBatchCrmEventRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account"""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response."""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Event Id's."""
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmEventResponseBody:
-    r"""OK"""
-    
-    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
+class GetAllCrmConnectionsResponseBody:
+    connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connections'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetBatchCrmEventResponse:
-    
+class GetAllCrmConnectionsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmEventResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmConnectionsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event_attendee.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmEventAttendeeRequest:
-    
+class GetBatchCrmEventAttendeeQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Event Attendee Id's."""
+    
+
+@dataclasses.dataclass
+class GetBatchCrmEventAttendeeRequest:
+    query_params: GetBatchCrmEventAttendeeQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetBatchCrmEventAttendeeResponseBody:
-    r"""OK"""
-    
     event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
     invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
     
 
 @dataclasses.dataclass
 class GetBatchCrmEventAttendeeResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetBatchCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/datefilter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,19 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclasses.dataclass
-class GetBatchCrmLeadRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Lead Id's."""
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmLeadResponseBody:
-    r"""OK"""
-    
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class GetBatchCrmLeadResponse:
-    
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class DateFilter:
+    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    gt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gt'), 'exclude': lambda f: f is None }})
+    gte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gte'), 'exclude': lambda f: f is None }})
+    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
+    lt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lt'), 'exclude': lambda f: f is None }})
+    lte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lte'), 'exclude': lambda f: f is None }})
+    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
+    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/taskcreate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,23 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import note as shared_note
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-@dataclasses.dataclass
-class GetBatchCrmNoteRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Note Id's."""
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmNoteResponseBody:
-    r"""OK"""
-    
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class GetBatchCrmNoteResponse:
-    
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class TaskCreate:
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
+    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/eventupdate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,20 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-@dataclasses.dataclass
-class GetBatchCrmTaskRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Task Id's."""
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmTaskResponseBody:
-    r"""OK"""
-    
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class GetBatchCrmTaskResponse:
-    
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class EventUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
+    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_batch_crm_user.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_contacts.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import user as shared_user
+from ..shared import contact as shared_contact
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetBatchCrmUserRequest:
-    
+class GetAllCrmContactsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of User Id's."""
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmUserResponseBody:
-    r"""OK"""
-    
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
+class GetAllCrmContactsRequest:
+    query_params: GetAllCrmContactsQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmUserResponse:
+class GetAllCrmContactsResponseBody:
+    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetAllCrmContactsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmUserResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmContactsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmAccountRequest:
-    
+class GetDetailsCrmTaskQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmAccountResponseBody:
-    r"""OK"""
+class GetDetailsCrmTaskRequest:
+    query_params: GetDetailsCrmTaskQueryParams = dataclasses.field()
     
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmTaskResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmAccountResponse:
-    
+class GetDetailsCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_call.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_contact.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmCallRequest:
-    
+class GetDetailsCrmContactQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmCallResponseBody:
-    r"""OK"""
+class GetDetailsCrmContactRequest:
+    query_params: GetDetailsCrmContactQueryParams = dataclasses.field()
     
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmContactResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmCallResponse:
-    
+class GetDetailsCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmCallResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmContactResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmContactRequest:
-    
+class GetDetailsCrmEmailQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmContactResponseBody:
-    r"""OK"""
+class GetDetailsCrmEmailRequest:
+    query_params: GetDetailsCrmEmailQueryParams = dataclasses.field()
     
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmEmailResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmContactResponse:
-    
+class GetDetailsCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmContactResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmEmailResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_lead.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmDealRequest:
-    
+class GetOneCrmLeadQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    r"""If provided, get the details about a particular deal. If not provided, get details about all deals."""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmDealResponseBody:
-    r"""OK"""
-    
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetOneCrmLeadRequest:
+    query_params: GetOneCrmLeadQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmDealResponse:
+class GetOneCrmLeadResponseBody:
+    lead: Optional[shared_lead.Lead] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetOneCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetOneCrmLeadResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_task.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmEmailRequest:
-    
+class GetBatchCrmTaskQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmEmailResponseBody:
-    r"""OK"""
-    
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetBatchCrmTaskRequest:
+    query_params: GetBatchCrmTaskQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmEmailResponse:
+class GetBatchCrmTaskResponseBody:
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetBatchCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmEmailResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetBatchCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_account.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmEventRequest:
-    
+class GetDetailsCrmAccountQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmEventResponseBody:
-    r"""OK"""
+class GetDetailsCrmAccountRequest:
+    query_params: GetDetailsCrmAccountQueryParams = dataclasses.field()
     
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmAccountResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmEventResponse:
-    
+class GetDetailsCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmEventResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmAccountResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/leadupdate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,19 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-@dataclasses.dataclass
-class GetDetailsCrmEventAttendeeRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmEventAttendeeResponseBody:
-    r"""OK"""
-    
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class GetDetailsCrmEventAttendeeResponse:
-    
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class LeadUpdate:
+    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_deal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmLeadRequest:
-    
+class GetDetailsCrmDealQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmLeadResponseBody:
-    r"""OK"""
+class GetDetailsCrmDealRequest:
+    query_params: GetDetailsCrmDealQueryParams = dataclasses.field()
     
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetDetailsCrmDealResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetDetailsCrmLeadResponse:
-    
+class GetDetailsCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetDetailsCrmDealResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_email.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import email as shared_email
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmNoteRequest:
-    
+class GetBatchCrmEmailQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmNoteResponseBody:
-    r"""OK"""
-    
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetBatchCrmEmailRequest:
+    query_params: GetBatchCrmEmailQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmNoteResponse:
+class GetBatchCrmEmailResponseBody:
+    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetBatchCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetBatchCrmEmailResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import event as shared_event
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetDetailsCrmTaskRequest:
-    
+class GetBatchCrmEventQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmTaskResponseBody:
-    r"""OK"""
-    
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetBatchCrmEventRequest:
+    query_params: GetBatchCrmEventQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmTaskResponse:
+class GetBatchCrmEventResponseBody:
+    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetBatchCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetBatchCrmEventResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_details_crm_user.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/connection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,28 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from typing import Optional
 from vesselapi import utils
 
+class ConnectionIntegrationIDEnum(str, Enum):
+    SALESFORCE = "salesforce"
+    HUBSPOT = "hubspot"
+    PIPEDRIVE = "pipedrive"
 
-@dataclasses.dataclass
-class GetDetailsCrmUserRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    
+class ConnectionStatusEnum(str, Enum):
+    NEW_CONNECTION = "NEW_CONNECTION"
+    INITIAL_SYNC = "INITIAL_SYNC"
+    READY = "READY"
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetDetailsCrmUserResponseBody:
-    r"""OK"""
-    
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDetailsCrmUserResponse:
-    
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmUserResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class Connection:
+    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId'), 'exclude': lambda f: f is None }})
+    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    integration_id: Optional[ConnectionIntegrationIDEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
+    last_activity_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastActivityDate'), 'exclude': lambda f: f is None }})
+    native_org_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgURL'), 'exclude': lambda f: f is None }})
+    status: Optional[ConnectionStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_connection.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import connection as shared_connection
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneConnectionRequest:
+class GetOneCrmUserQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     
-    connection_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'connectionId', 'style': 'form', 'explode': True }})
-    r"""The ID of the connection for the customer's CRM account. This was generated when they connected their account."""
+
+@dataclasses.dataclass
+class GetOneCrmUserRequest:
+    query_params: GetOneCrmUserQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneConnectionResponseBody:
-    r"""OK"""
-    
-    connection: Optional[shared_connection.Connection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connection'), 'exclude': lambda f: f is None }})
+class GetOneCrmUserResponseBody:
+    user: Optional[shared_user.User] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneConnectionResponse:
-    
+class GetOneCrmUserResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneConnectionResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetOneCrmUserResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_contact.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import account as shared_account
+from ..shared import contact as shared_contact
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmAccountRequest:
-    
+class GetOneCrmContactQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+    email: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'email', 'style': 'form', 'explode': True }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmAccountResponseBody:
-    r"""OK"""
-    
-    account: Optional[shared_account.Account] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
-    r"""(Alias: company, organization) An organization involved with your business."""
+class GetOneCrmContactRequest:
+    query_params: GetOneCrmContactQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmAccountResponse:
+class GetOneCrmContactResponseBody:
+    contact: Optional[shared_contact.Contact] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetOneCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetOneCrmContactResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_call.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_email.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import call as shared_call
+from ..shared import email as shared_email
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmCallRequest:
-    
+class GetOneCrmEmailQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmCallResponseBody:
-    r"""OK"""
-    
-    call: Optional[shared_call.Call] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('call'), 'exclude': lambda f: f is None }})
+class GetOneCrmEmailRequest:
+    query_params: GetOneCrmEmailQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmCallResponse:
+class GetOneCrmEmailResponseBody:
+    email: Optional[shared_email.Email] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetOneCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmCallResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetOneCrmEmailResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_webhook.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,33 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import deal as shared_deal
+from ..shared import webhookmetadata as shared_webhookmetadata
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmDealRequest:
+class GetOneWebhookQueryParams:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'webhookId', 'style': 'form', 'explode': True }})
     
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+
+@dataclasses.dataclass
+class GetOneWebhookRequest:
+    query_params: GetOneWebhookQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmDealResponseBody:
-    r"""OK"""
-    
-    deal: Optional[shared_deal.Deal] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal'), 'exclude': lambda f: f is None }})
-    r"""(Alias: Opportunity) An object representing either the opportunity to sell a product to an Account, or in the case of an `isWon` deal, a product sold to an Account.
-    *CRM Caveats*:
-    - Pipedrive: Users must have \"Deal probability\" turned on for the given pipeline for probability to be configurable and returned.
-    """
+class GetOneWebhookResponseBody:
+    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneCrmDealResponse:
-    
+class GetOneWebhookResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetOneWebhookResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import event as shared_event
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmEventRequest:
-    
+class GetOneCrmEventQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+    
+
+@dataclasses.dataclass
+class GetOneCrmEventRequest:
+    query_params: GetOneCrmEventQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetOneCrmEventResponseBody:
-    r"""OK"""
-    
     event: Optional[shared_event.Event] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
-    r"""Events are a type of activity that has attendees and takes place at a certain point in time (i.e., has a start and end date).
-    For the currently supported CRMs, these are the objects Events most closely maps to:
-    - Salesforce = Events
-    - HubSpot = Meetings
-    - Pipedrive = Activities
-    """
     
 
 @dataclasses.dataclass
 class GetOneCrmEventResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetOneCrmEventResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_lead.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventattendee as shared_eventattendee
+from ..shared import leadupdate as shared_leadupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmEventAttendeeRequest:
+class PutCrmLeadRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    lead: Optional[shared_leadupdate.LeadUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
     
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+
+@dataclasses.dataclass
+class PutCrmLeadRequest:
+    request: Optional[PutCrmLeadRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmEventAttendeeResponseBody:
-    r"""OK"""
-    
-    event_attendee: Optional[shared_eventattendee.EventAttendee] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
-    r"""Event Attendees hold information about someone who attendeed or was invited to an event. Attendees are always associated with some Event and another person object such as a Contact, Lead, or Other."""
+class PutCrmLeadResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class GetOneCrmEventAttendeeResponse:
-    
+class PutCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PutCrmLeadResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/taskupdate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,19 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-@dataclasses.dataclass
-class GetOneCrmLeadRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmLeadResponseBody:
-    r"""OK"""
-    
-    lead: Optional[shared_lead.Lead] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
-    r"""A Lead represents an individual, or sometimes an organization, that is interested in purchasing your product (i.e., is a potential Deal).
-    *CRM Caveats*:
-    - HubSpot: we consider contacts with the `leadStatus` set to be leads.
-    """
-    
-
-@dataclasses.dataclass
-class GetOneCrmLeadResponse:
-    
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class TaskUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import note as shared_note
+from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmNoteRequest:
-    
+class GetOneCrmTaskQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmNoteResponseBody:
-    r"""OK"""
-    
-    note: Optional[shared_note.Note] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note'), 'exclude': lambda f: f is None }})
-    r"""A Note attached to some CRM Object."""
+class GetOneCrmTaskRequest:
+    query_params: GetOneCrmTaskQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmNoteResponse:
+class GetOneCrmTaskResponseBody:
+    task: Optional[shared_task.Task] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetOneCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetOneCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_note.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import task as shared_task
+from ..shared import note as shared_note
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmTaskRequest:
-    
+class GetOneCrmNoteQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmTaskResponseBody:
-    r"""OK"""
-    
-    task: Optional[shared_task.Task] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
-    r"""A task attached to some CRM object"""
+class GetOneCrmNoteRequest:
+    query_params: GetOneCrmNoteQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmTaskResponse:
+class GetOneCrmNoteResponseBody:
+    note: Optional[shared_note.Note] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetOneCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetOneCrmNoteResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_crm_user.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_accounts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import user as shared_user
+from ..shared import account as shared_account
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneCrmUserRequest:
-    
+class GetAllCrmAccountsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmUserResponseBody:
-    r"""OK"""
-    
-    user: Optional[shared_user.User] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user'), 'exclude': lambda f: f is None }})
-    r"""Users of the connected CRM platform. These are *not* the contacts or leads, but rather the user accounts from the connected CRM."""
+class GetAllCrmAccountsRequest:
+    query_params: GetAllCrmAccountsQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneCrmUserResponse:
+class GetAllCrmAccountsResponseBody:
+    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetAllCrmAccountsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmUserResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmAccountsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/get_one_webhook.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_note.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import webhookmetadata as shared_webhookmetadata
+from ..shared import note as shared_note
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
-class GetOneWebhookRequest:
+class GetBatchCrmNoteQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'webhookId', 'style': 'form', 'explode': True }})
+
+@dataclasses.dataclass
+class GetBatchCrmNoteRequest:
+    query_params: GetBatchCrmNoteQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetOneWebhookResponseBody:
-    r"""OK"""
-    
-    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
+class GetBatchCrmNoteResponseBody:
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class GetOneWebhookResponse:
-    
+class GetBatchCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneWebhookResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetBatchCrmNoteResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_account.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import accountcreate as shared_accountcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostCrmAccountRequestBody:
-    
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
     account: shared_accountcreate.AccountCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
     
 
+@dataclasses.dataclass
+class PostCrmAccountRequest:
+    request: Optional[PostCrmAccountRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostCrmAccountResponseBody:
-    r"""OK"""
-    
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class PostCrmAccountResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PostCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_call.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import callcreate as shared_callcreate
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmCallRequestBody:
+class GetBatchCrmUserQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    call: Optional[shared_callcreate.CallCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('call'), 'exclude': lambda f: f is None }})
+
+@dataclasses.dataclass
+class GetBatchCrmUserRequest:
+    query_params: GetBatchCrmUserQueryParams = dataclasses.field()
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmCallResponseBody:
-    r"""OK"""
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class GetBatchCrmUserResponseBody:
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class PostCrmCallResponse:
-    
+class GetBatchCrmUserResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmCallResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetBatchCrmUserResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_note.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import contactcreate as shared_contactcreate
+from ..shared import notecreate as shared_notecreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmContactRequestBody:
-    
+class PostCrmNoteRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    contact: shared_contactcreate.ContactCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
-    r"""Properties that a contact can be created with"""
+    note: shared_notecreate.NoteCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmContactResponseBody:
-    r"""OK"""
-    
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class PostCrmNoteRequest:
+    request: Optional[PostCrmNoteRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmContactResponse:
+class PostCrmNoteResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
+
+@dataclasses.dataclass
+class PostCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmContactResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PostCrmNoteResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_task.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import dealcreate as shared_dealcreate
+from ..shared import taskcreate as shared_taskcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmDealRequestBody:
-    
+class PostCrmTaskRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    deal: shared_dealcreate.DealCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
+    task: Optional[shared_taskcreate.TaskCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmDealResponseBody:
-    r"""OK"""
+class PostCrmTaskRequest:
+    request: Optional[PostCrmTaskRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PostCrmTaskResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmDealResponse:
-    
+class PostCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PostCrmTaskResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event_attendee.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,23 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import emailcreate as shared_emailcreate
+from ..shared import eventattendeecreate as shared_eventattendeecreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmEmailRequestBody:
-    
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    email: Optional[shared_emailcreate.EmailCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class PostCrmEmailResponseBody:
-    r"""OK"""
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class PostCrmEventAttendeeResponseBody:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
+    event_attendee: Optional[shared_eventattendeecreate.EventAttendeeCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class PostCrmEmailResponse:
-    
+class PostCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmEmailResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PostCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventcreate as shared_eventcreate
+from ..shared import eventupdate as shared_eventupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmEventRequestBody:
-    
+class PutCrmEventRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    event: Optional[shared_eventcreate.EventCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    event: Optional[shared_eventupdate.EventUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmEventResponseBody:
-    r"""OK"""
+class PutCrmEventRequest:
+    request: Optional[PutCrmEventRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PutCrmEventResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmEventResponse:
-    
+class PutCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmEventResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PutCrmEventResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event_attendee.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventattendeecreate as shared_eventattendeecreate
+from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmEventAttendeeResponseBody:
-    r"""OK"""
+class GetOneCrmEventAttendeeQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
-    event_attendee: Optional[shared_eventattendeecreate.EventAttendeeCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
+
+@dataclasses.dataclass
+class GetOneCrmEventAttendeeRequest:
+    query_params: GetOneCrmEventAttendeeQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmEventAttendeeResponse:
+class GetOneCrmEventAttendeeResponseBody:
+    event_attendee: Optional[shared_eventattendee.EventAttendee] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetOneCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetOneCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_deal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import leadcreate as shared_leadcreate
+from ..shared import dealcreate as shared_dealcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmLeadRequestBody:
-    
+class PostCrmDealRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    lead: shared_leadcreate.LeadCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead') }})
+    deal: shared_dealcreate.DealCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmLeadResponseBody:
-    r"""OK"""
+class PostCrmDealRequest:
+    request: Optional[PostCrmDealRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PostCrmDealResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmLeadResponse:
-    
+class PostCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PostCrmDealResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_contact.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import notecreate as shared_notecreate
+from ..shared import contactupdate as shared_contactupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmNoteRequestBody:
-    
+class PutCrmContactRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    note: shared_notecreate.NoteCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
-    r"""Create a new Note. You may only associate a note with at most one entity of each type upon creation."""
+    contact: shared_contactupdate.ContactUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmNoteResponseBody:
-    r"""OK"""
+class PutCrmContactRequest:
+    request: Optional[PutCrmContactRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PutCrmContactResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PostCrmNoteResponse:
-    
+class PutCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PutCrmContactResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_passthrough.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_notes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import datefilter as shared_datefilter
+from ..shared import note as shared_note
+from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-from typing import Any, Optional
+from typing import Optional
 from vesselapi import utils
 
-class PostCrmPassthroughRequestBodyMethod(str, Enum):
-    GET = 'GET'
-    POST = 'POST'
-    PUT = 'PUT'
-    PATCH = 'PATCH'
-    DELETE = 'DELETE'
 
+@dataclasses.dataclass
+class SearchCrmNotesQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmPassthroughRequestBody:
-    
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    method: PostCrmPassthroughRequestBodyMethod = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-    path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('path') }})
-    r"""The path to send the request to. Vessel handles the domain so for a request to Salesforce instead of using `https://mydomain.my.salesforce.com/services/data/v52.0/sobjects/Account` you would use `services/data/v52.0/sobjects/Account`."""
-    body: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
-    r"""The body of the request."""
-    query: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
-    r"""The query parameters to send with the request as key value pairs. These are appended to the URL when the request is sent to the CRM."""
+class SearchCrmNotesRequestBodyFilters:
+    content: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
+    content_html: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentHtml'), 'exclude': lambda f: f is None }})
+    content_text: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentText'), 'exclude': lambda f: f is None }})
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmPassthroughResponseBody:
-    r"""OK"""
+class SearchCrmNotesRequestBody:
+    filters: Optional[SearchCrmNotesRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
-    body: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
-    headers: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('headers'), 'exclude': lambda f: f is None }})
-    status_code: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
-    r"""The HTTP status code of the response from the downstream CRM."""
-    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
-    r"""The full URL that the request was sent to."""
+
+@dataclasses.dataclass
+class SearchCrmNotesRequest:
+    query_params: SearchCrmNotesQueryParams = dataclasses.field()
+    request: Optional[SearchCrmNotesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmPassthroughResponse:
+class SearchCrmNotesResponseBody:
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class SearchCrmNotesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmPassthroughResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[SearchCrmNotesResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/delete_webhook.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,26 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import taskcreate as shared_taskcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmTaskRequestBody:
-    
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    task: Optional[shared_taskcreate.TaskCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
+class DeleteWebhookRequestBody:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
+    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookId'), 'exclude': lambda f: f is None }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmTaskResponseBody:
-    r"""OK"""
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class DeleteWebhookRequest:
+    request: Optional[DeleteWebhookRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclasses.dataclass
-class PostCrmTaskResponse:
-    
+class DeleteWebhookResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_link_exchange.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_link_exchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import security as shared_security
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclasses.dataclass
 class PostLinkExchangeSecurity:
-    
-    vessel_api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header', 'field_name': 'vessel-api-token' }})
+    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostLinkExchangeRequestBody:
-    
     public_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('publicToken') }})
     
-class PostLinkExchangeResponseBodyIntegrationID(str, Enum):
-    SALESFORCE = 'salesforce'
-    HUBSPOT = 'hubspot'
-    PIPEDRIVE = 'pipedrive'
+
+@dataclasses.dataclass
+class PostLinkExchangeRequest:
+    security: PostLinkExchangeSecurity = dataclasses.field()
+    request: Optional[PostLinkExchangeRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
+class PostLinkExchangeResponseBodyIntegrationIDEnum(str, Enum):
+    SALESFORCE = "salesforce"
+    HUBSPOT = "hubspot"
+    PIPEDRIVE = "pipedrive"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostLinkExchangeResponseBody:
-    r"""Exchange for access token"""
-    
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
     connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
-    integration_id: PostLinkExchangeResponseBodyIntegrationID = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
+    integration_id: PostLinkExchangeResponseBodyIntegrationIDEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
     native_org_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgId') }})
     native_org_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgURL') }})
     
 
 @dataclasses.dataclass
 class PostLinkExchangeResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PostLinkExchangeResponseBody] = dataclasses.field(default=None)
-    r"""Exchange for access token"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_link_token.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/contactcreate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-@dataclasses.dataclass
-class PostLinkTokenSecurity:
-    
-    vessel_api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header', 'field_name': 'vessel-api-token' }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostLinkTokenResponseBody:
-    r"""Create link token"""
-    
-    link_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkToken'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class PostLinkTokenResponse:
+class ContactCreate:
+    r"""ContactCreate
+    Properties that a contact can be created with
+    """
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostLinkTokenResponseBody] = dataclasses.field(default=None)
-    r"""Create link token"""
+    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/post_webhook.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_webhook.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import webhookmetadata as shared_webhookmetadata
 from ..shared import webhookmetadatacreate as shared_webhookmetadatacreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostWebhookRequestBody:
-    
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
     webhook: Optional[shared_webhookmetadatacreate.WebhookMetadataCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
-    r"""Information describing a webhook"""
+    
+
+@dataclasses.dataclass
+class PostWebhookRequest:
+    request: Optional[PostWebhookRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostWebhookResponseBody:
-    r"""OK"""
-    
     webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class PostWebhookResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PostWebhookResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_account.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import accountupdate as shared_accountupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PutCrmAccountRequestBody:
-    
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
     account: shared_accountupdate.AccountUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
+@dataclasses.dataclass
+class PutCrmAccountRequest:
+    request: Optional[PutCrmAccountRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PutCrmAccountResponseBody:
-    r"""OK"""
-    
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
 class PutCrmAccountResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PutCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_call.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_deal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import callupdate as shared_callupdate
+from ..shared import dealupdate as shared_dealupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmCallRequestBody:
-    
+class PutCrmDealRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    call: shared_callupdate.CallUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('call') }})
+    deal: shared_dealupdate.DealUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmCallResponseBody:
-    r"""OK"""
+class PutCrmDealRequest:
+    request: Optional[PutCrmDealRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PutCrmDealResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PutCrmCallResponse:
-    
+class PutCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmCallResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PutCrmDealResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/delete_connection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import contactupdate as shared_contactupdate
+from ..shared import security as shared_security
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmContactRequestBody:
-    
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    contact: shared_contactupdate.ContactUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
-    r"""Update a Contact."""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class DeleteConnectionSecurity:
+    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmContactResponseBody:
-    r"""OK"""
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class DeleteConnectionRequestBody:
+    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
     
 
 @dataclasses.dataclass
-class PutCrmContactResponse:
+class DeleteConnectionRequest:
+    security: DeleteConnectionSecurity = dataclasses.field()
+    request: Optional[DeleteConnectionRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclasses.dataclass
+class DeleteConnectionResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmContactResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_note.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import dealupdate as shared_dealupdate
+from ..shared import noteupdate as shared_noteupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmDealRequestBody:
-    
+class PutCrmNoteRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    deal: shared_dealupdate.DealUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    note: shared_noteupdate.NoteUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmDealResponseBody:
-    r"""OK"""
+class PutCrmNoteRequest:
+    request: Optional[PutCrmNoteRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PutCrmNoteResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PutCrmDealResponse:
-    
+class PutCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PutCrmNoteResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import emailupdate as shared_emailupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PutCrmEmailRequestBody:
-    
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     email: Optional[shared_emailupdate.EmailUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     
 
+@dataclasses.dataclass
+class PutCrmEmailRequest:
+    request: Optional[PutCrmEmailRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PutCrmEmailResponseBody:
-    r"""OK"""
-    
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
 class PutCrmEmailResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PutCrmEmailResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventupdate as shared_eventupdate
+from ..shared import eventcreate as shared_eventcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmEventRequestBody:
-    
+class PostCrmEventRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    event: Optional[shared_eventupdate.EventUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
+    event: Optional[shared_eventcreate.EventCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmEventResponseBody:
-    r"""OK"""
+class PostCrmEventRequest:
+    request: Optional[PostCrmEventRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PostCrmEventResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PutCrmEventResponse:
-    
+class PostCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmEventResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PostCrmEventResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_events.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventattendeeupdate as shared_eventattendeeupdate
+from ..shared import event as shared_event
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmEventAttendeeResponseBody:
-    r"""OK"""
+class GetAllCrmEventsQueryParams:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
-    event_attendee: Optional[shared_eventattendeeupdate.EventAttendeeUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
+
+@dataclasses.dataclass
+class GetAllCrmEventsRequest:
+    query_params: GetAllCrmEventsQueryParams = dataclasses.field()
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmEventAttendeeResponse:
+class GetAllCrmEventsResponseBody:
+    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
+
+@dataclasses.dataclass
+class GetAllCrmEventsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[GetAllCrmEventsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_email.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import leadupdate as shared_leadupdate
+from ..shared import emailcreate as shared_emailcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmLeadRequestBody:
-    
+class PostCrmEmailRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    lead: Optional[shared_leadupdate.LeadUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
+    email: Optional[shared_emailcreate.EmailCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmLeadResponseBody:
-    r"""OK"""
+class PostCrmEmailRequest:
+    request: Optional[PostCrmEmailRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PostCrmEmailResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PutCrmLeadResponse:
-    
+class PostCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PostCrmEmailResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_lead.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import noteupdate as shared_noteupdate
+from ..shared import leadcreate as shared_leadcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmNoteRequestBody:
-    
+class PostCrmLeadRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    note: shared_noteupdate.NoteUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
-    r"""Update an existing Note. Please note that updating associations is not currently supported."""
+    lead: shared_leadcreate.LeadCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead') }})
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmNoteResponseBody:
-    r"""OK"""
+class PostCrmLeadRequest:
+    request: Optional[PostCrmLeadRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PostCrmLeadResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
 @dataclasses.dataclass
-class PutCrmNoteResponse:
-    
+class PostCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[PostCrmLeadResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/put_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/eventattendeecreate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,17 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import taskupdate as shared_taskupdate
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCrmTaskRequestBody:
-    
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    task: Optional[shared_taskupdate.TaskUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class PutCrmTaskResponseBody:
-    r"""OK"""
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    
-
-@dataclasses.dataclass
-class PutCrmTaskResponse:
-    
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class EventAttendeeCreate:
+    associated_object_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associatedObjectType') }})
+    event_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    association_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associationId'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_accounts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_accounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import account as shared_account
 from ..shared import datefilter as shared_datefilter
 from ..shared import numberfilter as shared_numberfilter
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclasses.dataclass
+class SearchCrmAccountsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmAccountsRequestBodyFilters:
-    
     annual_revenue: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
     city: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
     country: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
     description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     industry: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
@@ -33,43 +38,30 @@
     street: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('street'), 'exclude': lambda f: f is None }})
     website: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmAccountsRequestBody:
-    
     filters: Optional[SearchCrmAccountsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmAccountsRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmAccountsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmAccountsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmAccountsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmAccountsResponseBody:
-    r"""OK"""
-    
     accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmAccountsResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmAccountsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_calls.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_users.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,57 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import call as shared_call
 from ..shared import datefilter as shared_datefilter
 from ..shared import stringfilter as shared_stringfilter
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmCallsRequestBodyFilters:
+class SearchCrmUsersQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmUsersRequestBodyFilters:
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    date_: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'exclude': lambda f: f is None }})
-    description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    direction: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('direction'), 'exclude': lambda f: f is None }})
-    disposition: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disposition'), 'exclude': lambda f: f is None }})
+    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmCallsRequestBody:
-    
-    filters: Optional[SearchCrmCallsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmUsersRequestBody:
+    filters: Optional[SearchCrmUsersRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmCallsRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmCallsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmUsersRequest:
+    query_params: SearchCrmUsersQueryParams = dataclasses.field()
+    request: Optional[SearchCrmUsersRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmCallsResponseBody:
-    r"""OK"""
-    
-    calls: Optional[list[shared_call.Call]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('calls'), 'exclude': lambda f: f is None }})
+class SearchCrmUsersResponseBody:
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmCallsResponse:
-    
+class SearchCrmUsersResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmCallsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[SearchCrmUsersResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_contacts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_contacts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import contact as shared_contact
 from ..shared import datefilter as shared_datefilter
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclasses.dataclass
+class SearchCrmContactsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmContactsRequestBodyFilters:
-    
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
     email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
     last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
     mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
@@ -26,43 +31,30 @@
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmContactsRequestBody:
-    
     filters: Optional[SearchCrmContactsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmContactsRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmContactsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmContactsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmContactsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmContactsResponseBody:
-    r"""OK"""
-    
     contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmContactsResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmContactsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_deals.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_leads.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,61 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
-from ..shared import deal as shared_deal
-from ..shared import numberfilter as shared_numberfilter
+from ..shared import lead as shared_lead
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmDealsRequestBodyFilters:
+class SearchCrmLeadsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
-    amount: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    close_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmLeadsRequestBodyFilters:
+    account: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    expected_revenue: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expectedRevenue'), 'exclude': lambda f: f is None }})
+    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    is_closed: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isClosed'), 'exclude': lambda f: f is None }})
-    is_won: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isWon'), 'exclude': lambda f: f is None }})
+    job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    probability: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
-    stage: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
+    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmDealsRequestBody:
-    
-    filters: Optional[SearchCrmDealsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmLeadsRequestBody:
+    filters: Optional[SearchCrmLeadsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmDealsRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmDealsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmLeadsRequest:
+    query_params: SearchCrmLeadsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmLeadsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmDealsResponseBody:
-    r"""OK"""
-    
-    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
+class SearchCrmLeadsResponseBody:
+    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmDealsResponse:
-    
+class SearchCrmLeadsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmDealsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[SearchCrmLeadsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_emails.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_emails.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
 from ..shared import email as shared_email
 from ..shared import stringfilter as shared_stringfilter
 from ..shared import stringlistfilter as shared_stringlistfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclasses.dataclass
+class SearchCrmEmailsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEmailsRequestBodyFilters:
-    
     bcc: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
     body: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
     body_html: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
     cc: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
     from_: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from'), 'exclude': lambda f: f is None }})
     has_attachment: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasAttachment'), 'exclude': lambda f: f is None }})
@@ -34,43 +39,30 @@
     subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
     to: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEmailsRequestBody:
-    
     filters: Optional[SearchCrmEmailsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEmailsRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmEmailsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmEmailsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmEmailsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEmailsResponseBody:
-    r"""OK"""
-    
     emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEmailsResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmEmailsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_event_attendees.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_event_attendees.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,57 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import datefilter as shared_datefilter
 from ..shared import eventattendee as shared_eventattendee
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclasses.dataclass
+class SearchCrmEventAttendeesQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventAttendeesRequestBodyFilters:
-    
     associated_object_type: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associatedObjectType'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
     email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventAttendeesRequestBody:
-    
     filters: Optional[SearchCrmEventAttendeesRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEventAttendeesRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmEventAttendeesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmEventAttendeesQueryParams = dataclasses.field()
+    request: Optional[SearchCrmEventAttendeesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventAttendeesResponseBody:
-    r"""OK"""
-    
     event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEventAttendeesResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmEventAttendeesResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_events.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_events.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
 from ..shared import event as shared_event
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
+@dataclasses.dataclass
+class SearchCrmEventsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
+
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventsRequestBodyFilters:
-    
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
     description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
     end_date_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     is_all_day_event: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
     location: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
@@ -28,43 +33,30 @@
     subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
     type: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventsRequestBody:
-    
     filters: Optional[SearchCrmEventsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEventsRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmEventsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmEventsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmEventsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventsResponseBody:
-    r"""OK"""
-    
     events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
 class SearchCrmEventsResponse:
-    
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmEventsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_leads.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_deals.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,64 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
-from ..shared import lead as shared_lead
+from ..shared import deal as shared_deal
+from ..shared import numberfilter as shared_numberfilter
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmLeadsRequestBodyFilters:
+class SearchCrmDealsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
-    account: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmDealsRequestBodyFilters:
+    amount: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    close_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    expected_revenue: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expectedRevenue'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    is_closed: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isClosed'), 'exclude': lambda f: f is None }})
+    is_won: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isWon'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    probability: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
+    stage: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmLeadsRequestBody:
-    
-    filters: Optional[SearchCrmLeadsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmDealsRequestBody:
+    filters: Optional[SearchCrmDealsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmLeadsRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmLeadsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmDealsRequest:
+    query_params: SearchCrmDealsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmDealsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmLeadsResponseBody:
-    r"""OK"""
-    
-    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
+class SearchCrmDealsResponseBody:
+    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmLeadsResponse:
-    
+class SearchCrmDealsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmLeadsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[SearchCrmDealsResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_notes.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,61 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
-from ..shared import note as shared_note
 from ..shared import stringfilter as shared_stringfilter
+from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmNotesRequestBodyFilters:
+class SearchCrmTasksQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
-    content: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
-    content_html: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentHtml'), 'exclude': lambda f: f is None }})
-    content_text: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentText'), 'exclude': lambda f: f is None }})
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmTasksRequestBodyFilters:
+    body: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    due_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    is_done: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+    priority: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmNotesRequestBody:
-    
-    filters: Optional[SearchCrmNotesRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmTasksRequestBody:
+    filters: Optional[SearchCrmTasksRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmNotesRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmNotesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmTasksRequest:
+    query_params: SearchCrmTasksQueryParams = dataclasses.field()
+    request: Optional[SearchCrmTasksRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmNotesResponseBody:
-    r"""OK"""
-    
+class SearchCrmTasksResponseBody:
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
+    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
     
 
 @dataclasses.dataclass
-class SearchCrmNotesResponse:
-    
+class SearchCrmTasksResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmNotesResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+    response_body: Optional[SearchCrmTasksResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_tasks.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/emailcreate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,49 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import booleanfilter as shared_booleanfilter
-from ..shared import datefilter as shared_datefilter
-from ..shared import stringfilter as shared_stringfilter
-from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmTasksRequestBodyFilters:
+class EmailCreateContact:
+    r"""EmailCreateContact
+    Associated Contacts must participate in the email (i.e., have a role).
+    """
     
-    body: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    due_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    is_done: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    priority: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
-    status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    role: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('role'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmTasksRequestBody:
-    
-    filters: Optional[SearchCrmTasksRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class SearchCrmTasksRequest:
+class EmailCreateLead:
+    r"""EmailCreateLead
+    Associated Leads must participate in the email (i.e., have a role).
+    """
     
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmTasksRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    role: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('role'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmTasksResponseBody:
-    r"""OK"""
-    
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class SearchCrmTasksResponse:
-    
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmTasksResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class EmailCreate:
+    from_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})
+    subject: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject') }})
+    to: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    bcc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    body_html: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
+    cc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
+    contact: Optional[EmailCreateContact] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
+    lead: Optional[EmailCreateLead] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
+    message_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messageDate'), 'exclude': lambda f: f is None }})
+    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/operations/search_crm_users.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/email.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,43 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import datefilter as shared_datefilter
-from ..shared import stringfilter as shared_stringfilter
-from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmUsersRequestBodyFilters:
-    
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class SearchCrmUsersRequestBody:
-    
-    filters: Optional[SearchCrmUsersRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class SearchCrmUsersRequest:
-    
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmUsersRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class EmailAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmUsersResponseBody:
-    r"""OK"""
-    
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
-    
-
-@dataclasses.dataclass
-class SearchCrmUsersResponse:
-    
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmUsersResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class Email:
+    r"""Email
+    An email is a message sent from one person to another through an email service. Emails involve participants - the person who the email was sent to, or the person that sent it. Participants are usually a Contact, Lead, or User but in certain CRMs, can be a person not yet associated with a CRM object.
+    """
+    
+    associations: EmailAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    from_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    subject: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject') }})
+    to: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    bcc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    body_html: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
+    cc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
+    has_attachment: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasAttachment'), 'exclude': lambda f: f is None }})
+    is_bounced: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBounced'), 'exclude': lambda f: f is None }})
+    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
+    message_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messageDate'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/__init__.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from .account import *
 from .accountcreate import *
 from .accountupdate import *
 from .address import *
 from .booleanfilter import *
-from .call import *
-from .callcreate import *
-from .callupdate import *
 from .connection import *
 from .contact import *
 from .contactcreate import *
 from .contactupdate import *
 from .datefilter import *
 from .deal import *
 from .dealcreate import *
@@ -40,8 +35,8 @@
 from .task import *
 from .taskcreate import *
 from .taskupdate import *
 from .user import *
 from .webhookmetadata import *
 from .webhookmetadatacreate import *
 
-__all__ = ["Account","AccountAssociations","AccountCreate","AccountUpdate","Address","BooleanFilter","Call","CallAssociations","CallCreate","CallCreateDirection","CallDirection","CallUpdate","Connection","ConnectionIntegrationID","ConnectionStatus","Contact","ContactAssociations","ContactCreate","ContactUpdate","DateFilter","Deal","DealAssociations","DealCreate","DealUpdate","Email","EmailAssociations","EmailCreate","EmailCreateContact","EmailCreateContactRole","EmailCreateLead","EmailCreateLeadRole","EmailUpdate","Event","EventAssociations","EventAttendee","EventAttendeeAssociations","EventAttendeeCreate","EventAttendeeUpdate","EventCreate","EventUpdate","Field","FieldOptions","FieldType","Integration","IntegrationIntegrationID","Lead","LeadAssociations","LeadCreate","LeadUpdate","Note","NoteAssociations","NoteCreate","NoteUpdate","NumberFilter","Security","StringFilter","StringFilterMode","StringListFilter","Task","TaskAssociations","TaskCreate","TaskUpdate","User","UserAssociations","WebhookMetadata","WebhookMetadataCreate"]
+__all__ = ["Account","AccountAssociations","AccountCreate","AccountUpdate","Address","BooleanFilter","Connection","ConnectionIntegrationIDEnum","ConnectionStatusEnum","Contact","ContactAssociations","ContactCreate","ContactUpdate","DateFilter","Deal","DealAssociations","DealCreate","DealUpdate","Email","EmailAssociations","EmailCreate","EmailCreateContact","EmailCreateLead","EmailUpdate","Event","EventAssociations","EventAttendee","EventAttendeeAssociations","EventAttendeeCreate","EventAttendeeUpdate","EventCreate","EventUpdate","Field","FieldOptions","FieldTypeEnum","Integration","IntegrationIntegrationIDEnum","Lead","LeadAssociations","LeadCreate","LeadUpdate","Note","NoteAssociations","NoteCreate","NoteUpdate","NumberFilter","SchemeVesselAPIToken","Security","StringFilter","StringListFilter","Task","TaskAssociations","TaskCreate","TaskUpdate","User","UserAssociations","WebhookMetadata","WebhookMetadataCreate"]
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/account.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/event.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,43 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class AccountAssociations:
-    
-    call_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('callIds') }})
+class EventAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
     contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
     deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    email_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emailIds') }})
-    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
+    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
     lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
-    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
     owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this Account"""
-    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Account:
-    r"""(Alias: company, organization) An organization involved with your business."""
+class Event:
+    r"""Event
+    Events are a type of activity that has attendees and takes place at a certain point in time (i.e., has a start and end date).
+    For the currently supported CRMs, these are the objects Events most closely maps to:
+    - Salesforce = Events
+    - HubSpot = Meetings
+    - Pipedrive = Activities
+    """
     
-    associations: AccountAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    associations: EventAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
     created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the account was created"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
     modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the account was last modified"""
     native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
-    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    r"""A description of this Company/Account. Not supported by Pipedrive"""
-    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone number. Not supported by Pipedrive"""
-    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
+    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/accountcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/dealupdate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,18 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class AccountCreate:
-    
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+class DealUpdate:
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
-    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone | Not supported by Pipedrive"""
-    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    close_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
+    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/accountupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/task.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class AccountUpdate:
+class TaskAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
+    
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class Task:
+    r"""Task
+    A task attached to some CRM object
+    """
     
+    associations: TaskAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
-    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone| Not supported by Pipedrive"""
-    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/address.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/address.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Address:
-    
     city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
     country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
     postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
     state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
     street: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('street'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/booleanfilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/stringlistfilter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class BooleanFilter:
-    
-    equals: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
-    not_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
+class StringListFilter:
+    has: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has'), 'exclude': lambda f: f is None }})
+    has_every: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasEvery'), 'exclude': lambda f: f is None }})
+    has_some: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasSome'), 'exclude': lambda f: f is None }})
+    is_empty: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isEmpty'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/call.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/accountcreate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,21 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
+from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class CallAssociations:
-    
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this call"""
-    
-class CallDirection(str, Enum):
-    INBOUND = 'inbound'
-    OUTBOUND = 'outbound'
-    INTERNAL = 'internal'
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class Call:
-    
+class AccountCreate:
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    associations: Optional[CallAssociations] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations'), 'exclude': lambda f: f is None }})
-    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    r"""The timestamp that the call object was created"""
-    date_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'exclude': lambda f: f is None }})
-    r"""The date the call occurred"""
+    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    direction: Optional[CallDirection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('direction'), 'exclude': lambda f: f is None }})
-    disposition: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disposition'), 'exclude': lambda f: f is None }})
-    r"""Possibly an enum, See /details endpoint for values."""
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Unique Vessel Id."""
-    modified_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    r"""The timestamp the call object was last modified"""
-    native_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    r"""Id of the object in the connected CRM."""
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/callcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/noteupdate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,18 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
-class CallCreateDirection(str, Enum):
-    INBOUND = 'inbound'
-    OUTBOUND = 'outbound'
-    INTERNAL = 'internal'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class CallCreate:
+class NoteUpdate:
+    r"""NoteUpdate
+    Update an existing Note. Please note that updating associations is not currently supported.
+    """
     
-    direction: CallCreateDirection = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('direction') }})
-    disposition: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disposition') }})
-    r"""See /details endpoint for possible values."""
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
-    contact_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds'), 'exclude': lambda f: f is None }})
-    r"""The participants involved in this call. If this is an inbound call, this is the contacts that called, if this is an outbound call, this is the contacts that were called."""
-    date_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'exclude': lambda f: f is None }})
-    r"""The date the call occurred"""
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/callupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/emailupdate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class CallUpdate:
-    
-    disposition: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disposition') }})
-    r"""See /details endpoint for possible values."""
+class EmailUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
     owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/contact.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,42 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
+from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ContactAssociations:
-    
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    call_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('callIds') }})
+class AccountAssociations:
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
     deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    email_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emailIds') }})
-    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
     event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
     lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
     note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Contact:
-    r"""Information about an individual affiliated with another CRM Object (e.g., a Lead, a Deal, etc)"""
+class Account:
+    r"""Account
+    (Alias: company, organization) An organization involved with your business.
+    """
     
-    associations: ContactAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    associations: AccountAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
     created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the contact was created"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
     modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the contact was last modified"""
     native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    r"""The primary mobile phone number for this contact. Possibly the same as the phone number."""
+    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
     phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone number for this contact"""
+    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/contactcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/contactupdate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ContactCreate:
-    r"""Properties that a contact can be created with"""
+class ContactUpdate:
+    r"""ContactUpdate
+    Update a Contact.
+    """
     
-    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName') }})
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
     email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
     job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
     mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
     phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/contactupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/dealcreate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ContactUpdate:
-    r"""Update a Contact."""
-    
+class DealCreate:
+    close_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone"""
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
+    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/datefilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/accountupdate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
+from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DateFilter:
-    
-    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
-    gt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gt'), 'exclude': lambda f: f is None }})
-    gte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gte'), 'exclude': lambda f: f is None }})
-    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
-    lt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lt'), 'exclude': lambda f: f is None }})
-    lte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lte'), 'exclude': lambda f: f is None }})
-    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
-    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
+class AccountUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/dealcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadata.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Any, Optional
+from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DealCreate:
-    
-    close_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
-    r"""The Id of the account to associate this deal with"""
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
-    r"""Decimal probability of closing the deal"""
-    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
-    r"""The stage the deal is in. See /deal/details for possible value"""
+class WebhookMetadata:
+    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId'), 'exclude': lambda f: f is None }})
+    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookId'), 'exclude': lambda f: f is None }})
+    webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookUrl'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/email.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/lead.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,41 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class EmailAssociations:
-    
+class LeadAssociations:
     account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
     contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this email"""
+    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
+    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
+    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
+    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Email:
-    r"""An email is a message sent from one person to another through an email service. Emails involve participants - the person who the email was sent to, or the person that sent it. Participants are usually a Contact, Lead, or User but in certain CRMs, can be a person not yet associated with a CRM object."""
+class Lead:
+    r"""Lead
+    A Lead represents an individual, or sometimes an organization, that is interested in purchasing your product (i.e., is a potential Deal). 
+    *CRM Caveats*:
+    - HubSpot: we consider contacts with the `leadStatus` set to be leads.
+    """
     
-    associations: EmailAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    associations: LeadAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
     created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the email object was created"""
-    from_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})
-    r"""The email address that sent the email"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
     modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the email object was last modified"""
     native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
-    subject: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject') }})
-    r"""The subject of the email"""
-    to: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to') }})
-    r"""The email addresses that received the email"""
+    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    bcc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
-    r"""The email addresses that received a blind copy of the email"""
-    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
-    r"""The text formatted body of the email"""
-    body_html: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
-    r"""The html formatted body of the email"""
-    cc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
-    r"""The email addresses that received a copy of the email"""
-    has_attachment: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasAttachment'), 'exclude': lambda f: f is None }})
-    r"""If this email has attachment(s)"""
-    is_bounced: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBounced'), 'exclude': lambda f: f is None }})
-    r"""If this email was bounced"""
-    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
-    r"""If this email was sent to the user or sent by the user"""
-    message_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messageDate'), 'exclude': lambda f: f is None }})
-    r"""The date the email was created. This can be set when creating the email object and is not necessarily the same as the `createdTime` field."""
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""The status of the email (CRM specific, see /details)."""
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/event.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/deal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,42 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class EventAssociations:
-    
+class DealAssociations:
     account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
     contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
     owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this event"""
+    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
+    event_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Event:
-    r"""Events are a type of activity that has attendees and takes place at a certain point in time (i.e., has a start and end date).
-    For the currently supported CRMs, these are the objects Events most closely maps to:
-    - Salesforce = Events
-    - HubSpot = Meetings
-    - Pipedrive = Activities
+class Deal:
+    r"""Deal
+    (Alias: Opportunity) An object representing either the opportunity to sell a product to an Account, or in the case of an `isWon` deal, a product sold to an Account.
+    *CRM Caveats*:
+    - Pipedrive: Users must have \"Deal probability\" turned on for the given pipeline for probability to be configurable and returned.
     """
     
-    associations: EventAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    associations: DealAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    close_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate') }})
     created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the event was created"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
     modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the event was last modified"""
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
+    stage: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage') }})
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
-    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
-    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
-    r"""Where this event takes place. Can be virtual"""
-    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    expected_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expectedRevenue'), 'exclude': lambda f: f is None }})
+    is_closed: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isClosed'), 'exclude': lambda f: f is None }})
+    is_won: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isWon'), 'exclude': lambda f: f is None }})
+    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/eventcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/eventcreate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EventCreate:
-    
     end_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime') }})
     start_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime') }})
     account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
     contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
     deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
     is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
-    r"""Not supported by HubSpot and Pipedrive"""
     lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
     location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
     owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
     subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
     type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/field.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/field.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,53 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class FieldOptions:
-    
     key: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     
-class FieldType(str, Enum):
-    STRING = 'string'
-    NUMBER = 'number'
-    DATETIME = 'datetime'
-    DATE = 'date'
-    BOOLEAN = 'boolean'
-    REFERENCE = 'reference'
-    PHONE = 'phone'
-    URL = 'url'
-    ID = 'id'
-    EMAIL = 'email'
-    PERCENT = 'percent'
-    SINGLESELECT = 'singleselect'
-    MULTISELECT = 'multiselect'
-    ADDRESS = 'address'
-    DECIMAL = 'decimal'
-    TIME = 'time'
-    DATERANGE = 'daterange'
-    OBJECT = 'object'
+class FieldTypeEnum(str, Enum):
+    STRING = "string"
+    NUMBER = "number"
+    DATETIME = "datetime"
+    DATE = "date"
+    BOOLEAN = "boolean"
+    REFERENCE = "reference"
+    PHONE = "phone"
+    URL = "url"
+    ID = "id"
+    EMAIL = "email"
+    PERCENT = "percent"
+    SINGLESELECT = "singleselect"
+    MULTISELECT = "multiselect"
+    ADDRESS = "address"
+    DECIMAL = "decimal"
+    TIME = "time"
+    DATERANGE = "daterange"
+    OBJECT = "object"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Field:
-    r"""(Alias: property) A field is a key-value pair on a CRM Object that provides information about that object."""
+    r"""Field
+    (Alias: property) A field is a key-value pair on a CRM Object that provides information about that object.
+    """
     
     creatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creatable') }})
-    r"""If this field can be used when creating the object"""
     custom: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom') }})
-    r"""If this field is a custom field"""
     key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-    r"""The key in the CRM object (ex: annualRevenue, numberOfEmployees, etc)"""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    r"""The display name of this field (ex: number of employees, annual revenue, etc)"""
     required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})
-    r"""If this field is required when creating the object"""
-    type: FieldType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    type: FieldTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     universal: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('universal') }})
-    r"""If this is a field we've unified across CRMs"""
     updatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatable') }})
-    r"""If this field can be updated"""
     is_array: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isArray'), 'exclude': lambda f: f is None }})
-    r"""If this field is an array"""
     options: Optional[list[FieldOptions]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})
-    r"""Possible options for this field"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/integration.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/integration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from vesselapi import utils
 
-class IntegrationIntegrationID(str, Enum):
-    SALESFORCE = 'salesforce'
-    HUBSPOT = 'hubspot'
-    PIPEDRIVE = 'pipedrive'
+class IntegrationIntegrationIDEnum(str, Enum):
+    SALESFORCE = "salesforce"
+    HUBSPOT = "hubspot"
+    PIPEDRIVE = "pipedrive"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Integration:
-    
     icon_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('iconURL'), 'exclude': lambda f: f is None }})
-    r"""Base 64 data URI"""
-    integration_id: Optional[IntegrationIntegrationID] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
+    integration_id: Optional[IntegrationIntegrationIDEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_passthrough.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from typing import Any, Optional
 from vesselapi import utils
 
+class PostCrmPassthroughRequestBodyMethodEnum(str, Enum):
+    GET = "GET"
+    POST = "POST"
+    PUT = "PUT"
+    PATCH = "PATCH"
+    DELETE = "DELETE"
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class NoteAssociations:
+class PostCrmPassthroughRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    method: PostCrmPassthroughRequestBodyMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
+    path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('path') }})
+    body: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    query: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
     
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this note"""
+
+@dataclasses.dataclass
+class PostCrmPassthroughRequest:
+    request: Optional[PostCrmPassthroughRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Note:
-    r"""A Note attached to some CRM Object."""
+class PostCrmPassthroughResponseBody:
+    body: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    headers: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('headers'), 'exclude': lambda f: f is None }})
+    status_code: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
+    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
     
-    associations: NoteAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the note was created"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the note was last modified"""
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
-    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
-    r"""The body of the note"""
+
+@dataclasses.dataclass
+class PostCrmPassthroughResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmPassthroughResponseBody] = dataclasses.field(default=None)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/numberfilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/stringfilter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class NumberFilter:
-    
-    equals: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
-    gt: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gt'), 'exclude': lambda f: f is None }})
-    gte: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gte'), 'exclude': lambda f: f is None }})
-    in_: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
-    lt: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lt'), 'exclude': lambda f: f is None }})
-    lte: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lte'), 'exclude': lambda f: f is None }})
-    not_: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
-    not_in: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
+class StringFilter:
+    contains: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contains'), 'exclude': lambda f: f is None }})
+    ends_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endsWith'), 'exclude': lambda f: f is None }})
+    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
+    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
+    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
+    starts_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startsWith'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/stringfilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/leadcreate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
-class StringFilterMode(str, Enum):
-    INSENSITIVE = 'insensitive'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class StringFilter:
-    
-    contains: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contains'), 'exclude': lambda f: f is None }})
-    ends_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endsWith'), 'exclude': lambda f: f is None }})
-    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
-    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
-    mode: Optional[StringFilterMode] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode'), 'exclude': lambda f: f is None }})
-    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
-    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
-    starts_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startsWith'), 'exclude': lambda f: f is None }})
+class LeadCreate:
+    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName') }})
+    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/task.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/contact.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,39 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TaskAssociations:
-    
+class ContactAssociations:
     account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
     deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
+    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
     lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this Task"""
+    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
+    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Task:
-    r"""A task attached to some CRM object"""
+class Contact:
+    r"""Contact
+    Information about an individual affiliated with another CRM Object (e.g., a Lead, a Deal, etc)
+    """
     
-    associations: TaskAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    associations: ContactAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
     created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the task was created"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
     modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the task was last modified"""
     native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
-    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
-    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
-    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/user.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/notecreate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,22 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UserAssociations:
-    
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
-    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
-    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class User:
-    r"""Users of the connected CRM platform. These are *not* the contacts or leads, but rather the user accounts from the connected CRM."""
+class NoteCreate:
+    r"""NoteCreate
+    Create a new Note. You may only associate a note with at most one entity of each type upon creation.
+    """
     
-    associations: UserAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the user was created"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the user was last modified"""
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
+    content: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
     additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/webhookmetadata.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/booleanfilter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class WebhookMetadata:
-    
-    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId'), 'exclude': lambda f: f is None }})
-    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookId'), 'exclude': lambda f: f is None }})
-    webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookUrl'), 'exclude': lambda f: f is None }})
+class BooleanFilter:
+    equals: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    not_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
```

### Comparing `vesselapi-3.23.0/src/vesselapi/models/shared/webhookmetadatacreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadatacreate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class WebhookMetadataCreate:
-    r"""Information describing a webhook"""
+    r"""WebhookMetadataCreate
+    Information describing a webhook
+    """
     
     webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookUrl'), 'exclude': lambda f: f is None }})
-    r"""a valid URL"""
```

### Comparing `vesselapi-3.23.0/src/vesselapi/sdk.py` & `vesselapi-3.5.2/src/vesselapi/sdk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+__doc__ = """ SDK Documentation: Vessel's APIs requires an access token to be used together with your Vessel API token. Ensure the following headers are provided when making API calls:
 
+Key | Value | Description
+---------|----------|----------
+ vessel-api-token | `<VESSEL_API_TOKEN>` | The API token provided by us
+ 
+Additionally, in the query or body parameters of each request depending on whether it is a GET or POST, make sure to include the `accessToken` for the connection you want to access."""
 import requests as requests_http
 from . import utils
 from .accounts import Accounts
 from .attendees import Attendees
-from .calls import Calls
 from .connections import Connections
 from .contacts import Contacts
 from .deals import Deals
 from .emails import Emails
 from .events import Events
 from .integrations import Integrations
 from .leads import Leads
@@ -18,85 +22,75 @@
 from .tasks import Tasks
 from .tokens import Tokens
 from .users import Users
 from .webhooks import Webhooks
 from vesselapi.models import shared
 
 SERVERS = [
-    "https://api.vessel.land",
+	"https://api.vessel.land",
 ]
-"""Contains the list of servers available to the SDK"""
 
 class VesselAPI:
-    r"""API
-    Vessel's APIs requires an access token to be used together with your Vessel API token. Ensure the following headers are provided when making API calls:
+    r"""SDK Documentation: Vessel's APIs requires an access token to be used together with your Vessel API token. Ensure the following headers are provided when making API calls:
     
     Key | Value | Description
     ---------|----------|----------
      vessel-api-token | `<VESSEL_API_TOKEN>` | The API token provided by us
      
-    Additionally, in the query or body parameters of each request depending on whether it is a GET or POST, make sure to include the `accessToken` for the connection you want to access.
-    """
+    Additionally, in the query or body parameters of each request depending on whether it is a GET or POST, make sure to include the `accessToken` for the connection you want to access."""
     accounts: Accounts
     attendees: Attendees
-    calls: Calls
     connections: Connections
     contacts: Contacts
     deals: Deals
     emails: Emails
     events: Events
     integrations: Integrations
     leads: Leads
     links: Links
     notes: Notes
     passthrough: Passthrough
     tasks: Tasks
     tokens: Tokens
     users: Users
     webhooks: Webhooks
-
+    
     _client: requests_http.Session
     _security_client: requests_http.Session
+    _security: shared.Security
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "3.23.0"
-    _gen_version: str = "2.32.2"
+    _sdk_version: str = "3.5.2"
+    _gen_version: str = "1.8.5"
 
-    def __init__(self,
-                 security: shared.Security = None,
-                 server_url: str = None,
-                 url_params: dict[str, str] = None,
-                 client: requests_http.Session = None
-                 ) -> None:
-        """Instantiates the SDK configuring it with the provided parameters.
-        
-        :param security: The security details required for authentication
-        :type security: shared.Security
-        :param server_url: The server URL to use for all operations
-        :type server_url: str
-        :param url_params: Parameters to optionally template the server URL with
-        :type url_params: dict[str, str]
-        :param client: The requests.Session HTTP client to use for all operations
-        :type client: requests_http.Session        
-        """
+    def __init__(self) -> None:
         self._client = requests_http.Session()
-        
-        
-        if server_url is not None:
-            if url_params is not None:
-                self._server_url = utils.template_url(server_url, url_params)
-            else:
-                self._server_url = server_url
+        self._security_client = requests_http.Session()
+        self._init_sdks()
 
-        if client is not None:
-            self._client = client
+    def config_server_url(self, server_url: str, params: dict[str, str] = None):
+        if params is not None:
+            self._server_url = utils.template_url(server_url, params)
+        else:
+            self._server_url = server_url
+
+        self._init_sdks()
+    
+    
+
+    def config_client(self, client: requests_http.Session):
+        self._client = client
         
+        if self._security is not None:
+            self._security_client = utils.configure_security_client(self._client, self._security)
+        self._init_sdks()
+    
+    def config_security(self, security: shared.Security):
+        self._security = security
         self._security_client = utils.configure_security_client(self._client, security)
-        
-
         self._init_sdks()
     
     def _init_sdks(self):
         self.accounts = Accounts(
             self._client,
             self._security_client,
             self._server_url,
@@ -109,23 +103,14 @@
             self._client,
             self._security_client,
             self._server_url,
             self._language,
             self._sdk_version,
             self._gen_version
         )
-        
-        self.calls = Calls(
-            self._client,
-            self._security_client,
-            self._server_url,
-            self._language,
-            self._sdk_version,
-            self._gen_version
-        )
         
         self.connections = Connections(
             self._client,
             self._security_client,
             self._server_url,
             self._language,
             self._sdk_version,
```

### Comparing `vesselapi-3.23.0/src/vesselapi/tokens.py` & `vesselapi-3.5.2/src/vesselapi/tokens.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Tokens:
     _client: requests_http.Session
@@ -17,29 +15,27 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def create(self, security: operations.PostLinkTokenSecurity) -> operations.PostLinkTokenResponse:
+    def create(self, request: operations.PostLinkTokenRequest) -> operations.PostLinkTokenResponse:
         r"""Create Link Token
         Generates a link token to be used during the authentication flow. This token is passed to either the Vessel Link Component or `useVesselLink` hook.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/link/token'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
-        client = utils.configure_security_client(self._client, security)
         
-        http_res = client.request('POST', url, headers=headers)
+        client = utils.configure_security_client(self._client, request.security)
+        
+        http_res = client.request('POST', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostLinkTokenResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostLinkTokenResponseBody])
```

### Comparing `vesselapi-3.23.0/src/vesselapi/users.py` & `vesselapi-3.5.2/src/vesselapi/users.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import requests as requests_http
 from . import utils
 from typing import Optional
 from vesselapi.models import operations
 
 class Users:
     _client: requests_http.Session
@@ -17,138 +15,129 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
     def batch(self, request: operations.GetBatchCrmUserRequest) -> operations.GetBatchCrmUserResponse:
         r"""Get Batch Users
         Retrieve Users by a set of Id's
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/user/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmUserRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBatchCrmUserResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmUserResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmUserRequest) -> operations.GetDetailsCrmUserResponse:
         r"""Get User Details
         Get details about all users. 
         Details include the type, possible values, and other meta data about the fields.
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/user/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmUserRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDetailsCrmUserResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmUserResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmUserRequest) -> operations.GetOneCrmUserResponse:
         r"""Get User
         Retrieve a single User by Id
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/user'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmUserRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetOneCrmUserResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmUserResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmUsersRequest) -> operations.GetAllCrmUsersResponse:
         r"""Get All Users
         Retrieve all Users
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/users'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmUsersRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmUsersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmUsersResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmUsersRequest) -> operations.SearchCrmUsersResponse:
         r"""Search Users
         Search all Users using filters
         """
+        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/crm/users/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmUsersRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        query_params = utils.get_query_params(request.query_params)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchCrmUsersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
```

### Comparing `vesselapi-3.23.0/src/vesselapi/utils/retries.py` & `vesselapi-3.5.2/src/vesselapi/utils/retries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import random
 import time
 
 import requests
 
 
 class BackoffStrategy:
```

### Comparing `vesselapi-3.23.0/src/vesselapi/utils/utils.py` & `vesselapi-3.5.2/src/vesselapi/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import base64
 import json
 import re
 from dataclasses import Field, dataclass, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from email.message import Message
 from enum import Enum
-from typing import Any, Callable, Optional, Tuple, Union, get_args, get_origin
+from typing import Callable, Optional, Tuple, Union, get_args, get_origin
 from xmlrpc.client import boolean
 
 import dateutil.parser
 import requests
 from dataclasses_json import DataClassJsonMixin
 
 
@@ -28,17 +26,14 @@
 
         return self.client.request(method, url, **kwargs)
 
 
 def configure_security_client(client: requests.Session, security: dataclass):
     client = SecurityClient(client)
 
-    if security is None:
-        return client
-
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
         metadata = sec_field.metadata.get('security')
@@ -108,15 +103,15 @@
             raise Exception('not supported')
     elif scheme_type == "openIdConnect":
         client.client.headers[header_name] = value
     elif scheme_type == 'oauth2':
         client.client.headers[header_name] = value
     elif scheme_type == 'http':
         if sub_type == 'bearer':
-            client.client.headers[header_name] = value.lower().startswith('bearer ') and value or f'Bearer {value}'
+            client.client.headers[header_name] = value
         else:
             raise Exception('not supported')
     else:
         raise Exception('not supported')
 
 
 def _parse_basic_auth_scheme(client: SecurityClient, scheme: dataclass):
@@ -137,91 +132,72 @@
         if field_name == 'password':
             password = value
 
     data = f'{username}:{password}'.encode()
     client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
-                 gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(server_url: str, path: str, path_params: dataclass) -> str:
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
-            continue
-
         param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
+        if param_metadata.get('style', 'simple') == 'simple':
+            param = getattr(path_params, field.name)
+            if param is None:
+                continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+            if isinstance(param, list):
+                pp_vals: list[str] = []
+                for pp_val in param:
+                    if pp_val is None:
+                        continue
+                    pp_vals.append(_val_to_string(pp_val))
+                path = path.replace(
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            elif isinstance(param, dict):
+                pp_vals: list[str] = []
+                for pp_key in param:
+                    if param[pp_key] is None:
+                        continue
+                    if param_metadata.get('explode'):
+                        pp_vals.append(
+                            f"{pp_key}={_val_to_string(param[pp_key])}")
+                    else:
+                        pp_vals.append(
+                            f"{pp_key},{_val_to_string(param[pp_key])}")
+                path = path.replace(
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            elif not isinstance(param, (str, int, float, complex, bool)):
+                pp_vals: list[str] = []
+                param_fields: Tuple[Field, ...] = fields(param)
+                for param_field in param_fields:
+                    param_value_metadata = param_field.metadata.get(
+                        'path_param')
+                    if not param_value_metadata:
+                        continue
 
-        if param is None:
-            continue
+                    parm_name = param_value_metadata.get(
+                        'field_name', field.name)
 
-        f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
-            serialized_params = _get_serialized_params(
-                param_metadata, f_name, param)
-            for key, value in serialized_params.items():
+                    param_field_val = getattr(param, param_field.name)
+                    if param_field_val is None:
+                        continue
+                    if param_metadata.get('explode'):
+                        pp_vals.append(
+                            f"{parm_name}={_val_to_string(param_field_val)}")
+                    else:
+                        pp_vals.append(
+                            f"{parm_name},{_val_to_string(param_field_val)}")
                 path = path.replace(
-                    '{' + key + '}', value, 1)
-        else:
-            if param_metadata.get('style', 'simple') == 'simple':
-                if isinstance(param, list):
-                    pp_vals: list[str] = []
-                    for pp_val in param:
-                        if pp_val is None:
-                            continue
-                        pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-                elif isinstance(param, dict):
-                    pp_vals: list[str] = []
-                    for pp_key in param:
-                        if param[pp_key] is None:
-                            continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
-                        else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-                elif not isinstance(param, (str, int, float, complex, bool)):
-                    pp_vals: list[str] = []
-                    param_fields: Tuple[Field, ...] = fields(param)
-                    for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
-                        if not param_value_metadata:
-                            continue
-
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
-
-                        param_field_val = getattr(param, param_field.name)
-                        if param_field_val is None:
-                            continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
-                        else:
-                            pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-                else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            else:
+                path = path.replace(
+                    '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
     return server_url.removesuffix("/") + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
@@ -230,54 +206,40 @@
     for key, value in params.items():
         url_with_params = url_with_params.replace(
             '{' + key + '}', value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[
-    str, list[str]]:
+def get_query_params(query_params: dataclass) -> dict[str, list[str]]:
+    if query_params is None:
+        return {}
+
     params: dict[str, list[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
-            continue
-
         metadata = field.metadata.get('query_param')
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
-
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
-
         f_name = metadata.get("field_name")
         serialization = metadata.get('serialization', '')
         if serialization != '':
-            serialized_parms = _get_serialized_params(metadata, f_name, value)
-            for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
-                else:
-                    params[key] = [value]
+            params = params | _get_serialized_query_params(
+                metadata, f_name, getattr(query_params, param_name))
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
-                    metadata, f_name, value)
+                    metadata, f_name, getattr(query_params, param_name))
             elif style == 'form':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, ",")
-            elif style == 'pipeDelimited':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, "|")
+                params = params | _get_form_query_params(
+                    metadata, f_name, getattr(query_params, param_name))
             else:
                 raise Exception('not yet implemented')
     return params
 
 
 def get_headers(headers_params: dataclass) -> dict[str, str]:
     if headers_params is None:
@@ -296,16 +258,16 @@
 
         if value != '':
             headers[metadata.get('field_name', field.name)] = value
 
     return headers
 
 
-def _get_serialized_params(metadata: dict, field_name: str, obj: any) -> dict[str, str]:
-    params: dict[str, str] = {}
+def _get_serialized_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
+    params: dict[str, list[str]] = {}
 
     serialization = metadata.get('serialization', '')
     if serialization == 'json':
         params[metadata.get("field_name", field_name)] = marshal_json(obj)
 
     return params
 
@@ -328,23 +290,20 @@
                 continue
 
             if isinstance(obj_val, list):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
-                        params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                    if params.get(f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                        params[f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(_val_to_string(val))
             else:
                 params[
                     f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                     _val_to_string(obj_val)]
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if value is None:
@@ -372,52 +331,50 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, delimiter: str) -> dict[
-    str, list[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
-
-
-SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
-}
+def _get_form_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name)
 
 
-def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[
-    str, any, any]:
+def serialize_request_body(request: dataclass) -> Tuple[str, any, any]:
     if request is None:
         return None, None, None, None
 
-    if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request)
-
-    request_val = getattr(request, request_field_name)
+    request_val = getattr(request, "request")
+    if request_val is None:
+        raise Exception("request body not found")
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
-        if field.name == request_field_name:
+        if field.name == "request":
             request_metadata = field.metadata.get('request')
             break
 
-    if request_metadata is None:
-        raise Exception('invalid request type')
+    if request_metadata is not None:
+        # single request
+        return serialize_content_type('request', request_metadata.get('media_type', 'application/octet-stream'), request_val)
 
-    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    request_fields: Tuple[Field, ...] = fields(request_val)
+    for field in request_fields:
+        req = getattr(request_val, field.name)
+        if req is None:
+            continue
+
+        request_metadata = field.metadata.get('request')
+        if request_metadata is None:
+            raise Exception(
+                f'missing request tag on request body field {field.name}')
+
+        return serialize_content_type(field.name, request_metadata.get('media_type', 'application/octet-stream'), req)
 
 
 def serialize_content_type(field_name: str, media_type: str, request: dataclass) -> Tuple[str, any, list[list[any]]]:
     if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request), None
     if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
@@ -482,15 +439,15 @@
                         [field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
 def serialize_dict(original: dict, explode: bool, field_name, existing: Optional[dict[str, list[str]]]) -> dict[
-    str, list[str]]:
+        str, list[str]]:
     if existing is None:
         existing = []
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -522,15 +479,15 @@
             field_name = metadata.get('field_name', field.name)
 
             if metadata.get('json'):
                 form[field_name] = [marshal_json(val)]
             else:
                 if metadata.get('style', 'form') == 'form':
                     form = form | _populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")
+                        field_name, metadata.get('explode', True), val, _get_form_field_name)
                 else:
                     raise Exception(
                         f'Invalid form style for field {field.name}')
     elif isinstance(data, dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
@@ -544,16 +501,15 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, delimiter: str) -> \
-        dict[str, list[str]]:
+def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable) -> dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
         items = []
@@ -568,31 +524,31 @@
             if val is None:
                 continue
 
             if explode:
                 params[obj_field_name] = [_val_to_string(val)]
             else:
                 items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                    f'{obj_field_name},{_val_to_string(val)}')
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            params[field_name] = [','.join(items)]
     elif isinstance(obj, dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
                 params[key] = _val_to_string(value)
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f'{key},{_val_to_string(value)}')
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            params[field_name] = [','.join(items)]
     elif isinstance(obj, list):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
@@ -600,15 +556,15 @@
                 if not field_name in params:
                     params[field_name] = []
                 params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join([str(item) for item in items])]
+            params[field_name] = [','.join([str(item) for item in items])]
     else:
         params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
 def _serialize_header(explode: bool, obj: any) -> str:
@@ -740,22 +696,10 @@
 
 def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
     if isinstance(val, Enum):
-        return str(val.value)
+        return val.value
 
     return str(val)
-
-
-def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: dict[str, dict[str, dict[str, Any]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
-
-    return value
```

### Comparing `vesselapi-3.23.0/src/vesselapi.egg-info/SOURCES.txt` & `vesselapi-3.5.2/src/vesselapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 README.md
 setup.py
 src/vesselapi/__init__.py
 src/vesselapi/accounts.py
 src/vesselapi/attendees.py
-src/vesselapi/calls.py
 src/vesselapi/connections.py
 src/vesselapi/contacts.py
 src/vesselapi/deals.py
 src/vesselapi/emails.py
 src/vesselapi/events.py
 src/vesselapi/integrations.py
 src/vesselapi/leads.py
@@ -25,87 +24,80 @@
 src/vesselapi.egg-info/requires.txt
 src/vesselapi.egg-info/top_level.txt
 src/vesselapi/models/__init__.py
 src/vesselapi/models/operations/__init__.py
 src/vesselapi/models/operations/delete_connection.py
 src/vesselapi/models/operations/delete_webhook.py
 src/vesselapi/models/operations/get_all_crm_accounts.py
-src/vesselapi/models/operations/get_all_crm_calls.py
 src/vesselapi/models/operations/get_all_crm_connections.py
 src/vesselapi/models/operations/get_all_crm_contacts.py
 src/vesselapi/models/operations/get_all_crm_deals.py
 src/vesselapi/models/operations/get_all_crm_emails.py
 src/vesselapi/models/operations/get_all_crm_event_attendees.py
 src/vesselapi/models/operations/get_all_crm_events.py
 src/vesselapi/models/operations/get_all_crm_integrations.py
 src/vesselapi/models/operations/get_all_crm_leads.py
 src/vesselapi/models/operations/get_all_crm_notes.py
 src/vesselapi/models/operations/get_all_crm_tasks.py
 src/vesselapi/models/operations/get_all_crm_users.py
 src/vesselapi/models/operations/get_batch_crm_account.py
-src/vesselapi/models/operations/get_batch_crm_call.py
 src/vesselapi/models/operations/get_batch_crm_contact.py
 src/vesselapi/models/operations/get_batch_crm_deal.py
 src/vesselapi/models/operations/get_batch_crm_email.py
 src/vesselapi/models/operations/get_batch_crm_event.py
 src/vesselapi/models/operations/get_batch_crm_event_attendee.py
 src/vesselapi/models/operations/get_batch_crm_lead.py
 src/vesselapi/models/operations/get_batch_crm_note.py
 src/vesselapi/models/operations/get_batch_crm_task.py
 src/vesselapi/models/operations/get_batch_crm_user.py
 src/vesselapi/models/operations/get_details_crm_account.py
-src/vesselapi/models/operations/get_details_crm_call.py
 src/vesselapi/models/operations/get_details_crm_contact.py
 src/vesselapi/models/operations/get_details_crm_deal.py
 src/vesselapi/models/operations/get_details_crm_email.py
 src/vesselapi/models/operations/get_details_crm_event.py
 src/vesselapi/models/operations/get_details_crm_event_attendee.py
 src/vesselapi/models/operations/get_details_crm_lead.py
 src/vesselapi/models/operations/get_details_crm_note.py
 src/vesselapi/models/operations/get_details_crm_task.py
 src/vesselapi/models/operations/get_details_crm_user.py
 src/vesselapi/models/operations/get_one_connection.py
 src/vesselapi/models/operations/get_one_crm_account.py
-src/vesselapi/models/operations/get_one_crm_call.py
 src/vesselapi/models/operations/get_one_crm_contact.py
 src/vesselapi/models/operations/get_one_crm_deal.py
 src/vesselapi/models/operations/get_one_crm_email.py
 src/vesselapi/models/operations/get_one_crm_event.py
 src/vesselapi/models/operations/get_one_crm_event_attendee.py
 src/vesselapi/models/operations/get_one_crm_lead.py
 src/vesselapi/models/operations/get_one_crm_note.py
 src/vesselapi/models/operations/get_one_crm_task.py
 src/vesselapi/models/operations/get_one_crm_user.py
 src/vesselapi/models/operations/get_one_webhook.py
 src/vesselapi/models/operations/post_crm_account.py
-src/vesselapi/models/operations/post_crm_call.py
 src/vesselapi/models/operations/post_crm_contact.py
 src/vesselapi/models/operations/post_crm_deal.py
 src/vesselapi/models/operations/post_crm_email.py
 src/vesselapi/models/operations/post_crm_event.py
 src/vesselapi/models/operations/post_crm_event_attendee.py
 src/vesselapi/models/operations/post_crm_lead.py
 src/vesselapi/models/operations/post_crm_note.py
 src/vesselapi/models/operations/post_crm_passthrough.py
 src/vesselapi/models/operations/post_crm_task.py
 src/vesselapi/models/operations/post_link_exchange.py
 src/vesselapi/models/operations/post_link_token.py
 src/vesselapi/models/operations/post_webhook.py
 src/vesselapi/models/operations/put_crm_account.py
-src/vesselapi/models/operations/put_crm_call.py
 src/vesselapi/models/operations/put_crm_contact.py
 src/vesselapi/models/operations/put_crm_deal.py
 src/vesselapi/models/operations/put_crm_email.py
 src/vesselapi/models/operations/put_crm_event.py
 src/vesselapi/models/operations/put_crm_event_attendee.py
 src/vesselapi/models/operations/put_crm_lead.py
 src/vesselapi/models/operations/put_crm_note.py
 src/vesselapi/models/operations/put_crm_task.py
 src/vesselapi/models/operations/search_crm_accounts.py
-src/vesselapi/models/operations/search_crm_calls.py
 src/vesselapi/models/operations/search_crm_contacts.py
 src/vesselapi/models/operations/search_crm_deals.py
 src/vesselapi/models/operations/search_crm_emails.py
 src/vesselapi/models/operations/search_crm_event_attendees.py
 src/vesselapi/models/operations/search_crm_events.py
 src/vesselapi/models/operations/search_crm_leads.py
 src/vesselapi/models/operations/search_crm_notes.py
@@ -113,17 +105,14 @@
 src/vesselapi/models/operations/search_crm_users.py
 src/vesselapi/models/shared/__init__.py
 src/vesselapi/models/shared/account.py
 src/vesselapi/models/shared/accountcreate.py
 src/vesselapi/models/shared/accountupdate.py
 src/vesselapi/models/shared/address.py
 src/vesselapi/models/shared/booleanfilter.py
-src/vesselapi/models/shared/call.py
-src/vesselapi/models/shared/callcreate.py
-src/vesselapi/models/shared/callupdate.py
 src/vesselapi/models/shared/connection.py
 src/vesselapi/models/shared/contact.py
 src/vesselapi/models/shared/contactcreate.py
 src/vesselapi/models/shared/contactupdate.py
 src/vesselapi/models/shared/datefilter.py
 src/vesselapi/models/shared/deal.py
 src/vesselapi/models/shared/dealcreate.py
```

