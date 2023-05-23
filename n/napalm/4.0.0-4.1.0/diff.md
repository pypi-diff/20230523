# Comparing `tmp/napalm-4.0.0.tar.gz` & `tmp/napalm-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm-4.0.0.tar", last modified: Mon Jul 11 11:41:02 2022, max compression
+gzip compressed data, was "napalm-4.1.0.tar", last modified: Tue May 23 17:42:28 2023, max compression
```

## Comparing `napalm-4.0.0.tar` & `napalm-4.1.0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.294617 napalm-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-11 11:40:53.000000 napalm-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-07-11 11:40:53.000000 napalm-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-07-11 11:41:02.294617 napalm-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7915 2022-07-11 11:40:53.000000 napalm-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.270617 napalm-4.0.0/napalm/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/_SUPPORTED_DRIVERS.py
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.274617 napalm-4.0.0/napalm/base/
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    67730 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4878 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/canonical_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.274617 napalm-4.0.0/napalm/base/clitools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/clitools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8542 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/clitools/cl_napalm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/clitools/cl_napalm_configure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/clitools/cl_napalm_test.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1315 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/clitools/cl_napalm_validate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/clitools/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2730 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    25559 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8404 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/mock.py
--rw-r--r--   0 runner    (1001) docker     (121)    10911 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/netmiko_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.278617 napalm-4.0.0/napalm/base/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22909 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/test/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/test/double.py
--rw-r--r--   0 runner    (1001) docker     (121)    20946 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/test/getters.py
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/test/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.278617 napalm-4.0.0/napalm/base/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/utils/jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/utils/string_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7854 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/base/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.278617 napalm-4.0.0/napalm/eos/
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    90230 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/eos.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/pyeapi_syntax_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.278617 napalm-4.0.0/napalm/eos/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.278617 napalm-4.0.0/napalm/eos/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19209 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/utils/cli_syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.278617 napalm-4.0.0/napalm/eos/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/utils/textfsm_templates/bgp_detail.tpl
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/utils/textfsm_templates/bgp_detail_multi_agent.tpl
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/utils/textfsm_templates/ntp_peers.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/utils/textfsm_templates/snmp_config.tpl
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/utils/textfsm_templates/vrf.tpl
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/eos/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.282617 napalm-4.0.0/napalm/ios/
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   152272 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/ios.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.282617 napalm-4.0.0/napalm/ios/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.270617 napalm-4.0.0/napalm/ios/utils/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.282617 napalm-4.0.0/napalm/ios/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_all_sum.tpl
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh.tpl
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh_afi.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors_detail.tpl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.282617 napalm-4.0.0/napalm/iosxr/
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    95105 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/iosxr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.286617 napalm-4.0.0/napalm/iosxr/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/delete_probes.j2
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/schedule_probes.j2
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/set_probes.j2
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/templates/snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.286617 napalm-4.0.0/napalm/iosxr_netconf/
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr_netconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13796 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr_netconf/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)   118814 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/iosxr_netconf/iosxr_netconf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.286617 napalm-4.0.0/napalm/junos/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)   101987 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/junos.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.286617 napalm-4.0.0/napalm/junos/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/delete_probes.j2
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/schedule_probes.j2
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/set_probes.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.290617 napalm-4.0.0/napalm/junos/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      621 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/utils/junos_views.py
--rw-r--r--   0 runner    (1001) docker     (121)    25464 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/junos/utils/junos_views.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.290617 napalm-4.0.0/napalm/nxapi_plumbing/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxapi_plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10417 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxapi_plumbing/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5365 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxapi_plumbing/device.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxapi_plumbing/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxapi_plumbing/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.290617 napalm-4.0.0/napalm/nxos/
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    66155 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/nxos.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.290617 napalm-4.0.0/napalm/nxos/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.290617 napalm-4.0.0/napalm/nxos/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.290617 napalm-4.0.0/napalm/nxos/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/utils/textfsm_templates/show_lldp_neighbors_detail.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/utils/textfsm_templates/snmp_config.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos/utils/textfsm_templates/users.tpl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.290617 napalm-4.0.0/napalm/nxos_ssh/
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    67442 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/nxos_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.294617 napalm-4.0.0/napalm/nxos_ssh/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/templates/delete_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/templates/delete_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/templates/delete_snmp_config.j2
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/templates/delete_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/templates/set_hostname.j2
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/templates/set_ntp_peers.j2
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/templates/set_ntp_servers.j2
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/templates/set_users.j2
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/templates/snmp_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.294617 napalm-4.0.0/napalm/nxos_ssh/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.294617 napalm-4.0.0/napalm/nxos_ssh/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/utils/textfsm_templates/snmp_config.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/utils/textfsm_templates/system_resources.tpl
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/nxos_ssh/utils/textfsm_templates/users.tpl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.294617 napalm-4.0.0/napalm/pyIOSXR/
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/pyIOSXR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/pyIOSXR/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    27425 2022-07-11 11:40:53.000000 napalm-4.0.0/napalm/pyIOSXR/iosxr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-11 11:41:02.274617 napalm-4.0.0/napalm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-07-11 11:41:02.000000 napalm-4.0.0/napalm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-07-11 11:41:02.000000 napalm-4.0.0/napalm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-11 11:41:02.000000 napalm-4.0.0/napalm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-07-11 11:41:02.000000 napalm-4.0.0/napalm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-11 11:41:02.000000 napalm-4.0.0/napalm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-11 11:41:02.000000 napalm-4.0.0/napalm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-11 11:40:53.000000 napalm-4.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-07-11 11:40:53.000000 napalm-4.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-07-11 11:41:02.294617 napalm-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-07-11 11:40:53.000000 napalm-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 17:42:19.000000 napalm-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 17:42:19.000000 napalm-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-23 17:42:28.085401 napalm-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-23 17:42:19.000000 napalm-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/_SUPPORTED_DRIVERS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67796 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/canonical_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/base/clitools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8542 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/cl_napalm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/cl_napalm_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/cl_napalm_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/cl_napalm_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/clitools/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23244 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/netmiko_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/base/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20970 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/test/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm/base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/utils/jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/utils/string_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/base/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93647 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/eos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/pyeapi_syntax_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/eos/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/eos/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19209 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/cli_syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/eos/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/bgp_detail.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/bgp_detail_multi_agent.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/ntp_peers.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/snmp_config.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/textfsm_templates/vrf.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/eos/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/ios/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153235 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/ios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/ios/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.069401 napalm-4.1.0/napalm/ios/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/ios/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_all_sum.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh_afi.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors_detail.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/iosxr/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95462 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/iosxr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.077401 napalm-4.1.0/napalm/iosxr/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/schedule_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/templates/snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/iosxr_netconf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr_netconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr_netconf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119196 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/iosxr_netconf/iosxr_netconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/junos/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103749 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/junos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/junos/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/schedule_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_probes.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/junos/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      621 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/utils/junos_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25648 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/junos/utils/junos_views.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxapi_plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxapi_plumbing/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66020 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/nxos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/utils/textfsm_templates/show_lldp_neighbors_detail.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/utils/textfsm_templates/snmp_config.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos/utils/textfsm_templates/users.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.081401 napalm-4.1.0/napalm/nxos_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69493 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/nxos_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/napalm/nxos_ssh/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/delete_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/delete_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/delete_snmp_config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/delete_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/set_hostname.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/set_ntp_peers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/set_ntp_servers.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/set_users.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/templates/snmp_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/napalm/nxos_ssh/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/napalm/nxos_ssh/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/utils/textfsm_templates/snmp_config.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/utils/textfsm_templates/system_resources.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/nxos_ssh/utils/textfsm_templates/users.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.085401 napalm-4.1.0/napalm/pyIOSXR/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/pyIOSXR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/pyIOSXR/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27426 2023-05-23 17:42:19.000000 napalm-4.1.0/napalm/pyIOSXR/iosxr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:42:28.073401 napalm-4.1.0/napalm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 17:42:28.000000 napalm-4.1.0/napalm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 17:42:19.000000 napalm-4.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-23 17:42:19.000000 napalm-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-23 17:42:28.085401 napalm-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-23 17:42:19.000000 napalm-4.1.0/setup.py
```

### Comparing `napalm-4.0.0/LICENSE` & `napalm-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/PKG-INFO` & `napalm-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: napalm
-Version: 4.0.0
+Version: 4.1.0
 Summary: Network Automation and Programmability Abstraction Layer with Multivendor support
 Home-page: https://github.com/napalm-automation/napalm
 Author: David Barroso, Kirk Byers, Mircea Ulinic
 Author-email: dbarrosop@dravetech.com, ping@mirceaulinic.net, ktbyers@twb-tech.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -168,9 +167,7 @@
 
 This project is maintained by David Barroso, Mircea Ulinic, and Kirk Byers and a set of other contributors.
 
 Originally it was hosted by the [Spotify][spotify] organization but due to the many contributions received by third parties we agreed creating a dedicated organization for NAPALM and give a big thanks to [Spotify][spotify] for the support.
 
 [spotify]: http://www.spotify.com
 [bigwave]: http://bigwaveit.org/
-
-
```

### Comparing `napalm-4.0.0/README.md` & `napalm-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/__init__.py` & `napalm-4.1.0/napalm/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/__init__.py` & `napalm-4.1.0/napalm/base/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/base.py` & `napalm-4.1.0/napalm/base/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 from types import TracebackType
 from typing import Optional, Dict, Type, Any, List, Union
 
 from typing_extensions import Literal
 
 from netmiko import ConnectHandler, NetMikoTimeoutException
+from netutils.interface import canonical_interface_name
 
 # local modules
 import napalm.base.exceptions
 import napalm.base.helpers
 from napalm.base import constants as c
 from napalm.base import validate
 from napalm.base.exceptions import ConnectionException
@@ -643,15 +644,16 @@
         Returns a dictionary containing the BGP configuration.
         Can return either the whole config, either the config only for a group or neighbor.
 
         :param group: Returns the configuration of a specific BGP group.
         :param neighbor: Returns the configuration of a specific BGP neighbor.
 
         Main dictionary keys represent the group name and the values represent a dictionary having
-        the keys below. Neighbors which aren't members of a group will be stored in a key named "_":
+        the keys below.  A default group named "_" will contain information regarding global
+        settings and any neighbors that are not members of a group.
 
             * type (string)
             * description (string)
             * apply_groups (string list)
             * multihop_ttl (int)
             * multipath (True/False)
             * local_address (string)
@@ -1800,12 +1802,10 @@
         return validate.compliance_report(
             self, validation_file=validation_file, validation_source=validation_source
         )
 
     def _canonical_int(self, interface: str) -> str:
         """Expose the helper function within this class."""
         if self.use_canonical_interface is True:
-            return napalm.base.helpers.canonical_interface_name(
-                interface, addl_name_map=None
-            )
+            return canonical_interface_name(interface, addl_name_map=None)
         else:
             return interface
```

### Comparing `napalm-4.0.0/napalm/base/clitools/cl_napalm.py` & `napalm-4.1.0/napalm/base/clitools/cl_napalm.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/clitools/cl_napalm_configure.py` & `napalm-4.1.0/napalm/base/clitools/cl_napalm_configure.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/clitools/cl_napalm_test.py` & `napalm-4.1.0/napalm/base/clitools/cl_napalm_test.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/clitools/cl_napalm_validate.py` & `napalm-4.1.0/napalm/base/clitools/cl_napalm_validate.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/clitools/helpers.py` & `napalm-4.1.0/napalm/base/clitools/helpers.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/constants.py` & `napalm-4.1.0/napalm/base/constants.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/exceptions.py` & `napalm-4.1.0/napalm/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/helpers.py` & `napalm-4.1.0/napalm/base/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper functions for the NAPALM base."""
+import ipaddress
 import itertools
 import logging
 
 # std libs
 import os
 import re
 import sys
@@ -10,31 +11,37 @@
 from collections.abc import Iterable
 
 # third party libs
 import jinja2
 import textfsm
 from lxml import etree
 from netaddr import EUI
-from netaddr import IPAddress
 from netaddr import mac_unix
 from netutils.config.parser import IOSConfigParser
 
+# Do not remove the below imports, functions were moved to netutils, but to not
+# break backwards compatibility, these should remain
+from netutils.interface import abbreviated_interface_name  # noqa
+from netutils.interface import canonical_interface_name  # noqa
+from netutils.constants import BASE_INTERFACES as base_interfaces  # noqa
+from netutils.constants import REVERSE_MAPPING as reverse_mapping  # noqa
+from netutils.interface import split_interface as _split_interface
+
 try:
     from ttp import quick_parse as ttp_quick_parse
 
     TTP_INSTALLED = True
 except ImportError:
     TTP_INSTALLED = False
 
 # local modules
 import napalm.base.exceptions
 from napalm.base import constants
 from napalm.base.models import ConfigDict
 from napalm.base.utils.jinja_filters import CustomJinjaFilters
-from napalm.base.canonical_map import base_interfaces, reverse_mapping
 
 T = TypeVar("T")
 R = TypeVar("R")
 
 # -------------------------------------------------------------------
 # Functional Global
 # -------------------------------------------------------------------
@@ -533,118 +540,42 @@
     Example:
 
     .. code-block:: python
 
         >>> ip('2001:0dB8:85a3:0000:0000:8A2e:0370:7334')
         u'2001:db8:85a3::8a2e:370:7334'
     """
-    addr_obj = IPAddress(addr)
+    scope = ""
+    if "%" in addr:
+        addr, scope = addr.split("%", 1)
+    addr_obj = ipaddress.ip_address(addr)
     if version and addr_obj.version != version:
         raise ValueError("{} is not an ipv{} address".format(addr, version))
-    return str(addr_obj)
+    if addr_obj.version == 6 and addr_obj.ipv4_mapped is not None:
+        return_addr = "%s:%s" % ("::ffff", addr_obj.ipv4_mapped)
+    else:
+        return_addr = str(addr_obj)
+    if scope:
+        return_addr = "%s%%%s" % (return_addr, scope)
+    return return_addr
 
 
 def as_number(as_number_val: str) -> int:
     """Convert AS Number to standardized asplain notation as an integer."""
     as_number_str = str(as_number_val)
     if "." in as_number_str:
         big, little = as_number_str.split(".")
         return (int(big) << 16) + int(little)
     else:
         return int(as_number_str)
 
 
 def split_interface(intf_name: str) -> Tuple[str, str]:
     """Split an interface name based on first digit, slash, or space match."""
-    head = intf_name.rstrip(r"/\0123456789. ")
-    tail = intf_name[len(head) :].lstrip()
-    return (head, tail)
-
-
-def canonical_interface_name(
-    interface: str, addl_name_map: Optional[Dict[str, str]] = None
-) -> str:
-    """Function to return an interface's canonical name (fully expanded name).
-
-    Use of explicit matches used to indicate a clear understanding on any potential
-    match. Regex and other looser matching methods were not implmented to avoid false
-    positive matches. As an example, it would make sense to do "[P|p][O|o]" which would
-    incorrectly match PO = POS and Po = Port-channel, leading to a false positive, not
-    easily troubleshot, found, or known.
-
-    :param interface: The interface you are attempting to expand.
-    :param addl_name_map: A dict containing key/value pairs that updates
-    the base mapping. Used if an OS has specific differences. e.g. {"Po": "PortChannel"} vs
-    {"Po": "Port-Channel"}
-    :type addl_name_map: optional
-    """
-
-    name_map = {}
-    name_map.update(base_interfaces)
-    interface_type, interface_number = split_interface(interface)
-
-    if isinstance(addl_name_map, dict):
-        name_map.update(addl_name_map)
-    # check in dict for mapping
-    if name_map.get(interface_type):
-        long_int = name_map.get(interface_type)
-        assert isinstance(long_int, str)
-        return long_int + str(interface_number)
-    # if nothing matched, return the original name
-    else:
-        return interface
-
-
-def abbreviated_interface_name(
-    interface: str,
-    addl_name_map: Optional[Dict[str, str]] = None,
-    addl_reverse_map: Optional[Dict[str, str]] = None,
-) -> str:
-    """Function to return an abbreviated representation of the interface name.
-
-    :param interface: The interface you are attempting to abbreviate.
-    :param addl_name_map: A dict containing key/value pairs that updates
-    the base mapping. Used if an OS has specific differences. e.g. {"Po": "PortChannel"} vs
-    {"Po": "Port-Channel"}
-    :type addl_name_map: optional
-    :param addl_reverse_map: A dict containing key/value pairs that updates
-    the reverse mapping. Used if an OS has specific differences. e.g. {"PortChannel": "Po"} vs
-    {"PortChannel": "po"}
-    :type addl_reverse_map: optional
-    """
-
-    name_map = {}
-    name_map.update(base_interfaces)
-    interface_type, interface_number = split_interface(interface)
-
-    if isinstance(addl_name_map, dict):
-        name_map.update(addl_name_map)
-
-    rev_name_map = {}
-    rev_name_map.update(reverse_mapping)
-
-    if isinstance(addl_reverse_map, dict):
-        rev_name_map.update(addl_reverse_map)
-
-    # Try to ensure canonical type.
-    if name_map.get(interface_type):
-        canonical_type = name_map.get(interface_type)
-    else:
-        canonical_type = interface_type
-
-    assert isinstance(canonical_type, str)
-
-    try:
-        abbreviated_name = rev_name_map[canonical_type] + str(interface_number)
-        return abbreviated_name
-    except KeyError:
-        pass
-
-    # If abbreviated name lookup fails, return original name
-    return interface
+    return _split_interface(interface=intf_name)
 
 
 def transform_lldp_capab(capabilities: Union[str, Any]) -> List[str]:
     if capabilities and isinstance(capabilities, str):
         capabilities = capabilities.strip().lower().split(",")
         return sorted(
             [constants.LLDP_CAPAB_TRANFORM_TABLE[c.strip()] for c in capabilities]
```

### Comparing `napalm-4.0.0/napalm/base/mock.py` & `napalm-4.1.0/napalm/base/mock.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/models.py` & `napalm-4.1.0/napalm/base/models.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/netmiko_helpers.py` & `napalm-4.1.0/napalm/base/netmiko_helpers.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/test/base.py` & `napalm-4.1.0/napalm/base/test/base.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/test/conftest.py` & `napalm-4.1.0/napalm/base/test/conftest.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/test/double.py` & `napalm-4.1.0/napalm/base/test/double.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/test/getters.py` & `napalm-4.1.0/napalm/base/test/getters.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
         return get_lldp_neighbors_detail
 
     @wrap_test_cases
     def test_get_bgp_config(self, test_case):
         """Test get_bgp_config."""
         get_bgp_config = self.device.get_bgp_config()
-        assert len(get_bgp_config) > 0
+        assert get_bgp_config == {} or len(get_bgp_config) > 0
 
         for bgp_group in get_bgp_config.values():
             assert helpers.test_model(models.BPGConfigGroupDict, bgp_group)
             for bgp_neighbor in bgp_group.get("neighbors", {}).values():
                 assert helpers.test_model(models.BGPConfigNeighborDict, bgp_neighbor)
 
         return get_bgp_config
```

### Comparing `napalm-4.0.0/napalm/base/test/helpers.py` & `napalm-4.1.0/napalm/base/test/helpers.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/utils/jinja_filters.py` & `napalm-4.1.0/napalm/base/utils/jinja_filters.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/base/utils/string_parsers.py` & `napalm-4.1.0/napalm/base/utils/string_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Common methods to normalize a string """
 import re
-from typing import Union, List, Iterable, Dict, Optional
+import struct
+from typing import Union, List, Iterable, Dict, Optional, Tuple
 
 
 def convert(text: str) -> Union[str, int]:
     """Convert text to integer, if it is a digit."""
     if text.isdigit():
         return int(text)
     return text
@@ -46,15 +47,15 @@
         line_data = line.split(separator)
         if len(line_data) > 1:
             dictionary[line_data[0].strip()] = "".join(line_data[1:]).strip()
         elif len(line_data) == 1:
             dictionary[line_data[0].strip()] = None
         else:
             raise Exception(
-                "Something went wrong parsing the colo separated string {}".format(line)
+                f"Something went wrong parsing the colon separated string:\n\n{line}"
             )
     return dictionary
 
 
 def hyphen_range(string: str) -> List[int]:
     """
     Expands a string of numbers separated by commas and hyphens into a list of integers.
@@ -129,7 +130,18 @@
                     'Unrecognized unit "{}" in uptime:{}'.format(unit, uptime)
                 )
 
     if not uptime_dict:
         raise Exception("Unrecognized uptime string:{}".format(uptime))
 
     return uptime_seconds
+
+
+def parse_fixed_width(text: str, *fields: int) -> List[Tuple[str, ...]]:
+    len = sum(fields)
+    fmtstring = " ".join(f"{fw}s" for fw in fields)
+    unpack = struct.Struct(fmtstring).unpack_from
+
+    def parse(line: str) -> Tuple[str, ...]:
+        return tuple([str(s.decode()) for s in unpack(line.ljust(len).encode())])
+
+    return [parse(s) for s in text.splitlines()]
```

### Comparing `napalm-4.0.0/napalm/base/validate.py` & `napalm-4.1.0/napalm/base/validate.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/eos/__init__.py` & `napalm-4.1.0/napalm/eos/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/eos/eos.py` & `napalm-4.1.0/napalm/eos/eos.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,29 @@
 """
 
 # std libs
 import re
 import time
 import importlib
 import inspect
+import ipaddress
 import json
 import socket
 
 from datetime import datetime
 from collections import defaultdict
-from netaddr import IPAddress
-from netaddr import IPNetwork
-
-from netaddr.core import AddrFormatError
 
 # third party libs
 import pyeapi
 from pyeapi.eapilib import ConnectionError, EapiConnection
 from netmiko import ConfigInvalidException
 
 # NAPALM base
 import napalm.base.helpers
+from napalm.base.netmiko_helpers import netmiko_args
 from napalm.base.base import NetworkDriver
 from napalm.base.utils import string_parsers
 from napalm.base.exceptions import (
     CommitError,
     ConnectionException,
     MergeConfigException,
     ReplaceConfigException,
@@ -94,17 +92,20 @@
     def __init__(self, hostname, username, password, timeout=60, optional_args=None):
         """
         Initialize EOS Driver.
 
         Optional args:
             * lock_disable (True/False): force configuration lock to be disabled (for external lock
                 management).
+            * force_cfg_session_invalid (True/False): force invalidation of the config session
+                in case of failure.
             * enable_password (True/False): Enable password for privilege elevation
             * eos_autoComplete (True/False): Allow for shortening of cli commands
-            * transport (string): pyeapi transport, defaults to eos_transport if set
+            * transport (string): transport, eos_transport is a fallback for compatibility.
+                - ssh (uses Netmiko)
                 - socket
                 - http_local
                 - http
                 - https
                 - https_certs
                 - A subclass of EapiConnection
                 - a string that identifies a module and class that is a subclass of EapiConnection
@@ -122,53 +123,55 @@
         self.timeout = timeout
         self.config_session = None
         self.locked = False
         self.cli_version = 1
 
         self.platform = "eos"
         self.profile = [self.platform]
+        self.optional_args = optional_args or {}
 
-        self._process_optional_args(optional_args or {})
+        self.enablepwd = self.optional_args.pop("enable_password", "")
+        self.eos_autoComplete = self.optional_args.pop("eos_autoComplete", None)
+        self.fn0039_config = self.optional_args.pop("eos_fn0039_config", False)
 
-    def _process_optional_args(self, optional_args):
         # Define locking method
-        self.lock_disable = optional_args.get("lock_disable", False)
+        self.lock_disable = self.optional_args.pop("lock_disable", False)
+
+        self.force_cfg_session_invalid = self.optional_args.pop(
+            "force_cfg_session_invalid", False
+        )
 
-        self.enablepwd = optional_args.pop("enable_password", "")
-        self.eos_autoComplete = optional_args.pop("eos_autoComplete", None)
         # eos_transport is there for backwards compatibility, transport is the preferred method
-        transport = optional_args.get(
-            "transport", optional_args.get("eos_transport", "https")
+        transport = self.optional_args.get(
+            "transport", self.optional_args.get("eos_transport", "https")
         )
-        self.fn0039_config = optional_args.pop("eos_fn0039_config", False)
         self.transport = transport
-        if transport == "ssh":
-            self.transport_class = "ssh"
-            init_args = ["port"]
-        else:
-            # Parse pyeapi transport class
-            self.transport_class = self._parse_transport(transport)
-            # ([1:]) to omit self
-            init_args = inspect.getfullargspec(self.transport_class.__init__)[0][1:]
-
-        filter_args = ["host", "username", "password", "timeout", "lock_disable"]
 
         if transport == "ssh":
-            self.netmiko_optional_args = {
-                k: v
-                for k, v in optional_args.items()
-                if k in init_args and k not in filter_args
-            }
+            self._process_optional_args_ssh(self.optional_args)
         else:
-            init_args.append("enforce_verification")  # Not an arg for unknown reason
-            self.eapi_kwargs = {
-                k: v
-                for k, v in optional_args.items()
-                if k in init_args and k not in filter_args
-            }
+            self._process_optional_args_eapi(self.optional_args)
+
+    def _process_optional_args_ssh(self, optional_args):
+        self.transport_class = None
+        self.netmiko_optional_args = netmiko_args(optional_args)
+
+    def _process_optional_args_eapi(self, optional_args):
+        # Parse pyeapi transport class
+        self.transport_class = self._parse_transport(self.transport)
+
+        # ([1:]) to omit self
+        init_args = inspect.getfullargspec(self.transport_class.__init__)[0][1:]
+        filter_args = ["host", "username", "password", "timeout"]
+        init_args.append("enforce_verification")  # Not an arg for unknown reason
+        self.eapi_kwargs = {
+            k: v
+            for k, v in optional_args.items()
+            if k in init_args and k not in filter_args
+        }
 
     def _parse_transport(self, transport):
         if inspect.isclass(transport) and issubclass(transport, EapiConnection):
             # Subclass of EapiConnection
             return transport
         elif "." in transport:
             # Try to resolve string import to module and getattr to class
@@ -191,28 +194,29 @@
             # All methods failed, raise exception
             raise ConnectionException("Unknown transport: {}".format(transport))
 
     def open(self):
         """Implementation of NAPALM method open."""
         if self.transport == "ssh":
             self.device = self._netmiko_open(
-                "arista_eos", netmiko_optional_args=self.netmiko_optional_args
+                device_type="arista_eos",
+                netmiko_optional_args=self.netmiko_optional_args,
             )
             # let's try to determine if we need to use new EOS cli syntax
             sh_ver = self._run_commands(["show version"])
             if EOSVersion(sh_ver[0]["version"]) >= EOSVersion("4.23.0"):
                 self.cli_version = 2
         else:
             try:
                 connection = self.transport_class(
                     host=self.hostname,
                     username=self.username,
                     password=self.password,
                     timeout=self.timeout,
-                    **self.eapi_kwargs
+                    **self.eapi_kwargs,
                 )
 
                 if self.device is None:
                     self.device = Node(connection, enablepwd=self.enablepwd)
                 # does not raise an Exception if unusable
 
                 # let's try to determine if we need to use new EOS cli syntax
@@ -227,15 +231,17 @@
                 # either if HTTP(S) agent is not enabled
                 # show management api http-commands
                 raise ConnectionException(str(ce))
 
     def close(self):
         """Implementation of NAPALM method close."""
         self.discard_config()
-        if hasattr(self.device.connection, "close") and callable(
+        if self.transport == "ssh":
+            self._netmiko_close()
+        elif hasattr(self.device.connection, "close") and callable(
             self.device.connection.close
         ):
             self.device.connection.close()
 
     def is_alive(self):
         if self.transport == "ssh":
             null = chr(0)
@@ -278,14 +284,35 @@
                 except json.decoder.JSONDecodeError:
                     cmd_json = {}
                 ret.append(cmd_json)
             return ret
         else:
             return self.device.run_commands(commands, **kwargs)
 
+    def _obtain_lock(self, wait_time=None):
+        """
+        EOS internally creates config sessions when using commit-confirm.
+
+        This can cause issues obtaining the configuration lock:
+
+        cfg-2034--574620864-0 completed
+        cfg-2034--574620864-1 pending
+        """
+        if wait_time:
+            start_time = time.time()
+            while time.time() - start_time < wait_time:
+                try:
+                    self._lock()
+                    return
+                except SessionLockedException:
+                    time.sleep(1)
+
+        # One last try
+        return self._lock()
+
     def _lock(self):
         sess = self._run_commands(["show configuration sessions"])[0]["sessions"]
         if [
             k
             for k, v in sess.items()
             if v["state"] == "pending" and k != self.config_session
         ]:
@@ -381,15 +408,15 @@
         return ret
 
     def _load_config(self, filename=None, config=None, replace=True):
         if self.config_session is None:
             self.config_session = "napalm_{}".format(datetime.now().microsecond)
 
         if not self.lock_disable:
-            self._lock()
+            self._obtain_lock(wait_time=10)
 
         commands = []
         commands.append("configure session {}".format(self.config_session))
         if replace:
             commands.append("rollback clean-config")
 
         if filename is not None:
@@ -426,15 +453,15 @@
                 if replace:
                     raise ReplaceConfigException(msg)
                 else:
                     raise MergeConfigException(msg)
             return None
 
         try:
-            if not any(l == "end" for l in commands):
+            if not any(cmd == "end" for cmd in commands):
                 commands.append("end")  # exit config mode
             if self.eos_autoComplete is not None:
                 self._run_commands(
                     commands,
                     autoComplete=self.eos_autoComplete,
                     fn0039_transform=self.fn0039_config,
                 )
@@ -517,21 +544,23 @@
             self.config_session = None
         else:
             raise CommitError("No pending commit-confirm found!")
 
     def discard_config(self):
         """Implementation of NAPALM method discard_config."""
         if self.config_session is not None:
-            commands = ["configure session {}".format(self.config_session), "abort"]
-            if self.transport == "ssh":
-                # For some reason when testing with vEOS 4.26.1F this
-                # doesn't work with the normal wrapper.
-                self._run_commands(["", commands[0]])
-            else:
-                self.device.run_commands(commands)
+            try:
+                commands = [f"configure session {self.config_session} abort"]
+                self._run_commands(commands, encoding="text")
+            except Exception:
+                # If discard fails, you might want to invalidate the config_session (esp. Salt)
+                # The config_session in EOS is used as the config lock.
+                if self.force_cfg_session_invalid:
+                    self.config_session = None
+                raise
             self.config_session = None
 
     def rollback(self):
         """Implementation of NAPALM method rollback."""
 
         # Commit-confirm check and abort
         pending_commits = self._get_pending_commits()
@@ -652,21 +681,21 @@
                 tx_errors=counters.get("totalOutErrors", -1),
                 rx_errors=counters.get("totalInErrors", -1),
             )
         return interface_counters
 
     def get_bgp_neighbors(self):
         def get_re_group(res, key, default=None):
-            """Small helper to retrive data from re match groups"""
+            """Small helper to retrieve data from re match groups"""
             try:
                 return res.group(key)
             except KeyError:
                 return default
 
-        NEIGHBOR_FILTER = "bgp neighbors vrf all | include remote AS | remote router ID |IPv[46] (Unicast|6PE):.*[0-9]+|^Local AS|Desc|BGP state"  # noqa
+        NEIGHBOR_FILTER = "bgp neighbors vrf all | include IPv[46] (Unicast|6PE):.*[0-9]+ | grep -v ' IPv[46] Unicast:/.' | remote AS |^Local AS|Desc|BGP state |remote router ID"  # noqa
         output_summary_cmds = self._run_commands(
             ["show ipv6 bgp summary vrf all", "show ip bgp summary vrf all"],
             encoding="json",
         )
         output_neighbor_cmds = self._run_commands(
             ["show ip " + NEIGHBOR_FILTER, "show ipv6 " + NEIGHBOR_FILTER],
             encoding="text",
@@ -973,14 +1002,15 @@
             "apply-groups": "apply_groups",
             "remove-private-as": "remove_private_as",
             "ebgp-multihop": "multihop_ttl",
             "remote-as": "remote_as",
             "local-v4-addr": "local_address",
             "local-v6-addr": "local_address",
             "local-as": "local_as",
+            "next-hop-self": "nhs",
             "description": "description",
             "import-policy": "import_policy",
             "export-policy": "export_policy",
         }
 
         _PEER_FIELD_MAP_ = {
             "description": "description",
@@ -1030,25 +1060,32 @@
                 }
             )
             group_dict.update(
                 {"prefix_limit": {}, "neighbors": {}, "local_as": local_as}
             )  # few more default values
             return group_dict
 
-        def default_neighbor_dict(local_as):
+        def default_neighbor_dict(local_as, group_dict):
             neighbor_dict = {}
             neighbor_dict.update(
                 {
                     key: _DATATYPE_DEFAULT_.get(_PROPERTY_TYPE_MAP_.get(prop))
                     for prop, key in _PEER_FIELD_MAP_.items()
                 }
             )  # populating with default values
             neighbor_dict.update(
                 {"prefix_limit": {}, "local_as": local_as, "authentication_key": ""}
             )  # few more default values
+            neighbor_dict.update(
+                {
+                    key: group_dict.get(key)
+                    for key in _GROUP_FIELD_MAP_.values()
+                    if key in group_dict and key in _PEER_FIELD_MAP_.values()
+                }
+            )  # copy in values from group dict if present
             return neighbor_dict
 
         def parse_options(options, default_value=False):
 
             if not options:
                 return {}
 
@@ -1128,25 +1165,31 @@
             bgp_conf_line_details = bgp_conf_line.split()
             group_or_neighbor = str(bgp_conf_line_details[0])
             options = bgp_conf_line_details[1:]
             try:
                 # will try to parse the neighbor name
                 # which sometimes is the IP Address of the neigbor
                 # or the name of the BGP group
-                IPAddress(group_or_neighbor)
+                ipaddress.ip_address(group_or_neighbor)
                 # if passes the test => it is an IP Address, thus a Neighbor!
                 peer_address = group_or_neighbor
-                if peer_address not in bgp_neighbors:
-                    bgp_neighbors[peer_address] = default_neighbor_dict(local_as)
+                group_name = None
                 if options[0] == "peer-group":
-                    bgp_neighbors[peer_address]["__group"] = options[1]
+                    group_name = options[1]
                 # EOS > 4.23.0 only supports the new syntax
                 # https://www.arista.com/en/support/advisories-notices/fieldnotices/7097-field-notice-39
                 elif options[0] == "peer" and options[1] == "group":
-                    bgp_neighbors[peer_address]["__group"] = options[2]
+                    group_name = options[2]
+                if peer_address not in bgp_neighbors:
+                    bgp_neighbors[peer_address] = default_neighbor_dict(
+                        local_as, bgp_config.get(group_name, {})
+                    )
+
+                if group_name:
+                    bgp_neighbors[peer_address]["__group"] = group_name
 
                 # in the config, neighbor details are lister after
                 # the group is specified for the neighbor:
                 #
                 # neighbor 192.168.172.36 peer-group 4-public-anycast-peers
                 # neighbor 192.168.172.36 remote-as 12392
                 # neighbor 192.168.172.36 maximum-routes 200
@@ -1156,32 +1199,42 @@
                 # that way we avoid one more loop to
                 # match the neighbors with the group they belong to
                 # directly will apend the neighbor in the neighbor list of the group at the end
 
                 bgp_neighbors[peer_address].update(
                     parse_options(options, default_value)
                 )
-            except AddrFormatError:
+            except ValueError:
                 # exception trying to parse group name
                 # group_or_neighbor represents the name of the group
                 group_name = group_or_neighbor
                 if group and group_name != group:
                     continue
                 if group_name not in bgp_config.keys():
                     bgp_config[group_name] = default_group_dict(local_as)
                 bgp_config[group_name].update(parse_options(options, default_value))
 
+        bgp_config["_"] = default_group_dict(local_as)
+
         for peer, peer_details in bgp_neighbors.items():
             peer_group = peer_details.pop("__group", None)
             if not peer_group:
                 peer_group = "_"
             if peer_group not in bgp_config:
                 bgp_config[peer_group] = default_group_dict(local_as)
             bgp_config[peer_group]["neighbors"][peer] = peer_details
 
+        [
+            v.pop("nhs", None) for v in bgp_config.values()
+        ]  # remove NHS from group-level dictionary
+
+        if local_as == 0:
+            # BGP not running
+            return {}
+
         return bgp_config
 
     def get_arp_table(self, vrf=""):
         arp_table = []
 
         try:
             commands = ["show arp vrf all"]
@@ -1419,15 +1472,15 @@
         else:
             vrfs = [vrf]
 
         if protocol.lower() == "direct":
             protocol = "connected"
 
         ipv = ""
-        if IPNetwork(destination).version == 6:
+        if ipaddress.ip_network(destination).version == 6:
             ipv = "v6"
 
         commands = []
         for _vrf in vrfs:
             commands.append(
                 "show ip{ipv} route vrf {_vrf} {destination} {longer} {protocol} detail".format(
                     ipv=ipv,
@@ -1526,15 +1579,15 @@
                             )
                         try:
                             remote_address = napalm.base.helpers.ip(
                                 bgp_route_details.get("routeDetail", {})
                                 .get("peerEntry", {})
                                 .get("peerAddr", "")
                             )
-                        except AddrFormatError:
+                        except ValueError:
                             remote_address = napalm.base.helpers.ip(
                                 bgp_route_details.get("peerEntry", {}).get(
                                     "peerAddr", ""
                                 )
                             )
                         local_preference = bgp_route_details.get("localPreference")
                         next_hop = napalm.base.helpers.ip(
@@ -1905,15 +1958,15 @@
         if not neighbor_address:
             commands.append("show ip bgp neighbors vrf all")
             commands.append("show ipv6 bgp neighbors vrf all")
             summary_commands.append("show ip bgp summary vrf all")
             summary_commands.append("show ipv6 bgp summary vrf all")
         else:
             try:
-                peer_ver = IPAddress(neighbor_address).version
+                peer_ver = ipaddress.ip_address(neighbor_address).version
             except Exception as e:
                 raise e
 
             if peer_ver == 4:
                 commands.append("show ip bgp neighbors %s vrf all" % neighbor_address)
                 summary_commands.append("show ip bgp summary vrf all")
             elif peer_ver == 6:
@@ -2073,23 +2126,67 @@
             return {"startup": "", "running": "", "candidate": str(output[0]["output"])}
         elif retrieve == "candidate":
             # If we get here it means that we want the candidate but there is none.
             return {"startup": "", "running": "", "candidate": ""}
         else:
             raise Exception("Wrong retrieve filter: {}".format(retrieve))
 
-    def _show_vrf(self):
+    def _show_vrf_json(self):
         commands = ["show vrf"]
 
-        # This command has no JSON yet
+        vrfs = self._run_commands(commands)[0]["vrfs"]
+        return [
+            {
+                "name": k,
+                "interfaces": [i for i in v["interfaces"]],
+                "route_distinguisher": v["routeDistinguisher"],
+            }
+            for k, v in vrfs.items()
+        ]
+
+    def _show_vrf_text(self):
+        commands = ["show vrf"]
+
+        # This command has no JSON in EOS < 4.23
         raw_output = self._run_commands(commands, encoding="text")[0].get("output", "")
 
-        output = napalm.base.helpers.textfsm_extractor(self, "vrf", raw_output)
+        width_line = raw_output.splitlines()[2]  # Line with dashes
+        fields = width_line.split(" ")
+        widths = [len(f) + 1 for f in fields]
+        widths[-1] -= 1
+
+        parsed_lines = string_parsers.parse_fixed_width(raw_output, *widths)
+
+        vrfs = []
+        vrf = {}
+        current_vrf = None
+        for line in parsed_lines[3:]:
+            line = [t.strip() for t in line]
+            if line[0]:
+                if current_vrf:
+                    vrfs.append(vrf)
+                current_vrf = line[0]
+                vrf = {
+                    "name": current_vrf,
+                    "interfaces": list(),
+                }
+            if line[1]:
+                vrf["route_distinguisher"] = line[1]
+            if line[4]:
+                vrf["interfaces"].extend([t.strip() for t in line[4].split(",") if t])
+        if current_vrf:
+            vrfs.append(vrf)
+
+        return vrfs
 
-        return output
+    def _show_vrf(self):
+        if self.cli_version == 2:
+            return self._show_vrf_json()
+        else:
+            return self._show_vrf_text()
 
     def _get_vrfs(self):
         output = self._show_vrf()
 
         vrfs = [str(vrf["name"]) for vrf in output]
 
         vrfs.append("default")
@@ -2114,31 +2211,34 @@
             for interface_raw in vrf.get("interfaces", []):
                 interface = interface_raw.split(",")
                 for line in interface:
                     if line.strip() != "":
                         interfaces[str(line.strip())] = {}
                         all_vrf_interfaces[str(line.strip())] = {}
 
-            vrfs[str(vrf["name"])] = {
-                "name": str(vrf["name"]),
-                "type": "L3VRF",
+            vrfs[vrf["name"]] = {
+                "name": vrf["name"],
+                "type": "DEFAULT_INSTANCE" if vrf["name"] == "default" else "L3VRF",
                 "state": {"route_distinguisher": vrf["route_distinguisher"]},
                 "interfaces": {"interface": interfaces},
             }
-        all_interfaces = self.get_interfaces_ip().keys()
-        vrfs["default"] = {
-            "name": "default",
-            "type": "DEFAULT_INSTANCE",
-            "state": {"route_distinguisher": ""},
-            "interfaces": {
-                "interface": {
-                    k: {} for k in all_interfaces if k not in all_vrf_interfaces.keys()
-                }
-            },
-        }
+        if "default" not in vrfs:
+            all_interfaces = self.get_interfaces_ip().keys()
+            vrfs["default"] = {
+                "name": "default",
+                "type": "DEFAULT_INSTANCE",
+                "state": {"route_distinguisher": ""},
+                "interfaces": {
+                    "interface": {
+                        k: {}
+                        for k in all_interfaces
+                        if k not in all_vrf_interfaces.keys()
+                    }
+                },
+            }
 
         if name:
             if name in vrfs:
                 return {str(name): vrfs[name]}
             return {}
         else:
             return vrfs
```

### Comparing `napalm-4.0.0/napalm/eos/pyeapi_syntax_wrapper.py` & `napalm-4.1.0/napalm/eos/pyeapi_syntax_wrapper.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/eos/templates/delete_snmp_config.j2` & `napalm-4.1.0/napalm/eos/templates/delete_snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/eos/templates/snmp_config.j2` & `napalm-4.1.0/napalm/eos/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/eos/utils/cli_syntax.py` & `napalm-4.1.0/napalm/eos/utils/cli_syntax.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/eos/utils/textfsm_templates/bgp_detail.tpl` & `napalm-4.1.0/napalm/eos/utils/textfsm_templates/bgp_detail.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/eos/utils/textfsm_templates/bgp_detail_multi_agent.tpl` & `napalm-4.1.0/napalm/eos/utils/textfsm_templates/bgp_detail_multi_agent.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/eos/utils/textfsm_templates/vrf.tpl` & `napalm-4.1.0/napalm/eos/utils/textfsm_templates/vrf.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/eos/utils/versions.py` & `napalm-4.1.0/napalm/eos/utils/versions.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/ios/__init__.py` & `napalm-4.1.0/napalm/ios/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/ios/ios.py` & `napalm-4.1.0/napalm/ios/ios.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,45 +10,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 import copy
 import functools
+import ipaddress
 import os
 import re
 import socket
 import telnetlib
 import tempfile
 import uuid
 from collections import defaultdict
 
-from netaddr import IPNetwork
-from netaddr.core import AddrFormatError
 from netmiko import FileTransfer, InLineTransfer
 
 import napalm.base.constants as C
 import napalm.base.helpers
 from napalm.base.base import NetworkDriver
 from napalm.base.exceptions import (
     ReplaceConfigException,
     MergeConfigException,
     ConnectionClosedException,
     CommandErrorException,
     CommitConfirmException,
 )
 from napalm.base.helpers import (
-    canonical_interface_name,
     transform_lldp_capab,
     textfsm_extractor,
-    split_interface,
-    abbreviated_interface_name,
     generate_regex_or,
     sanitize_configs,
 )
+from netaddr.core import AddrFormatError
+from netutils.interface import (
+    abbreviated_interface_name,
+    canonical_interface_name,
+    split_interface,
+)
 from napalm.base.netmiko_helpers import netmiko_args
 
 # Easier to store these as constants
 HOUR_SECONDS = 3600
 DAY_SECONDS = 24 * HOUR_SECONDS
 WEEK_SECONDS = 7 * DAY_SECONDS
 YEAR_SECONDS = 365 * DAY_SECONDS
@@ -477,18 +479,18 @@
         current_prompt = self.device.find_prompt().strip()
         terminating_char = current_prompt[-1]
         # Look for trailing pattern that includes '#' and '>'
         pattern1 = r"[>#{}]\s*$".format(terminating_char)
         # Handle special username removal pattern
         pattern2 = r".*all username.*confirm"
         patterns = rf"(?:{pattern1}|{pattern2})"
-        output = self.device.send_command(cmd, expect_string=patterns)
+        output = self.device.send_command(cmd, expect_string=patterns, read_timeout=90)
         loop_count = 50
         new_output = output
-        for i in range(loop_count):
+        for _ in range(loop_count):
             if re.search(pattern2, new_output):
                 # Send confirmation if username removal
                 new_output = self.device.send_command_timing(
                     "\n", strip_prompt=False, strip_command=False
                 )
                 output += new_output
             else:
@@ -981,18 +983,34 @@
         neighbors_detail = self.get_lldp_neighbors_detail()
         for intf_name, entries in neighbors_detail.items():
             lldp[intf_name] = []
             for lldp_entry in entries:
                 hostname = lldp_entry["remote_system_name"]
                 port = lldp_entry["remote_port"]
                 # Match IOS behaviour of taking remote chassis ID
-                # When lacking a system name (in show lldp neighbors)
+                # when lacking a system name (in show lldp neighbors)
+
+                # We can't assume remote_chassis_id or remote_port are MAC Addresses
+                # See IEEE 802.1AB-2005 and rfc2922, specifically PtopoChassisId
                 if not hostname:
-                    hostname = napalm.base.helpers.mac(lldp_entry["remote_chassis_id"])
-                    port = napalm.base.helpers.mac(port)
+                    try:
+                        hostname = napalm.base.helpers.mac(
+                            lldp_entry["remote_chassis_id"]
+                        )
+                    except AddrFormatError:
+                        hostname = lldp_entry["remote_chassis_id"]
+
+                # If port is a mac-address, normalize it.
+                # The MAC helper library will normalize "15" to "00:00:00:00:00:0F"
+                if port.count(":") == 5 or port.count("-") == 5 or port.count(".") == 2:
+                    try:
+                        port = napalm.base.helpers.mac(port)
+                    except AddrFormatError:
+                        pass
+
                 lldp_dict = {"port": port, "hostname": hostname}
                 lldp[intf_name].append(lldp_dict)
 
         return lldp
 
     def get_lldp_neighbors_detail(self, interface=""):
         lldp = {}
@@ -1441,14 +1459,19 @@
             return prefix_limit
 
         # Get BGP config using netutils because some old devices dont support "| sec bgp"
         cfg = self.get_config(retrieve="running")
         bgp_config_list = napalm.base.helpers.netutils_parse_objects(
             "router bgp", cfg["running"]
         )
+
+        # No BGP configuration
+        if not bgp_config_list:
+            return {}
+
         bgp_asn = napalm.base.helpers.regex_find_txt(
             r"router bgp (\d+)", bgp_config_list, default=0
         )
         # Get a list of all neighbors and groups in the config
         all_neighbors = set()
         all_groups = set()
         bgp_group_neighbors = {}
@@ -1511,15 +1534,17 @@
             import_policy = napalm.base.helpers.regex_find_txt(
                 r"route-map ([^\s]+) in", neighbor_config
             )
             local_address = napalm.base.helpers.regex_find_txt(
                 r" update-source (\w+)", neighbor_config
             )
             local_as = napalm.base.helpers.regex_find_txt(
-                r"local-as (\d+)", neighbor_config, default=0
+                r"local-as (\d+)",
+                neighbor_config,
+                default=bgp_asn,
             )
             password = napalm.base.helpers.regex_find_txt(
                 r"password (?:[0-9] )?([^\']+\')", neighbor_config
             )
             nhs = bool(
                 napalm.base.helpers.regex_find_txt(r" next-hop-self", neighbor_config)
             )
@@ -1545,37 +1570,40 @@
                 "local_address": local_address,
                 "local_as": local_as,
                 "authentication_key": password,
                 "nhs": nhs,
                 "route_reflector_client": route_reflector_client,
             }
 
+        # Do not include the no-group ("_") if a group argument is passed in
+        # unless group argument is "_"
+        if not group or group == "_":
+            bgp_config["_"] = {
+                "apply_groups": [],
+                "description": "",
+                "local_as": bgp_asn,
+                "type": "",
+                "import_policy": "",
+                "export_policy": "",
+                "local_address": "",
+                "multipath": False,
+                "multihop_ttl": 0,
+                "remote_as": 0,
+                "remove_private_as": False,
+                "prefix_limit": {},
+                "neighbors": bgp_group_neighbors.get("_", {}),
+            }
+
         # Get the peer-group level config for each group
         for group_name in bgp_group_neighbors.keys():
             # If a group is passed in params, only continue on that group
             if group:
                 if group_name != group:
                     continue
-            # Default no group
             if group_name == "_":
-                bgp_config["_"] = {
-                    "apply_groups": [],
-                    "description": "",
-                    "local_as": 0,
-                    "type": "",
-                    "import_policy": "",
-                    "export_policy": "",
-                    "local_address": "",
-                    "multipath": False,
-                    "multihop_ttl": 0,
-                    "remote_as": 0,
-                    "remove_private_as": False,
-                    "prefix_limit": {},
-                    "neighbors": bgp_group_neighbors.get("_", {}),
-                }
                 continue
             neighbor_config = napalm.base.helpers.netutils_parse_objects(
                 group_name, bgp_config_list
             )
             multipath = False
             afi_list = napalm.base.helpers.netutils_parse_parents(
                 r"\s+address-family.*", group_name, bgp_config_list
@@ -1589,15 +1617,15 @@
                 )
                 if multipath:
                     break
             description = napalm.base.helpers.regex_find_txt(
                 r" description ([^\']+)\'", neighbor_config
             )
             local_as = napalm.base.helpers.regex_find_txt(
-                r"local-as (\d+)", neighbor_config, default=0
+                r"local-as (\d+)", neighbor_config, default=bgp_asn
             )
             import_policy = napalm.base.helpers.regex_find_txt(
                 r"route-map ([^\s]+) in", neighbor_config
             )
             export_policy = napalm.base.helpers.regex_find_txt(
                 r"route-map ([^\s]+) out", neighbor_config
             )
@@ -3001,15 +3029,15 @@
                 matchbgpattr = RE_BGP_REMOTE_AS.search(outbgpnei)
                 if matchbgpattr:
                     bgpras = matchbgpattr.group(1)
                 else:
                     # next-hop is not known in this vrf, route leaked from
                     # other vrf or from vpnv4 table?
                     # get remote AS nr. from as-path if it is ebgp neighbor
-                    # localy sourced prefix is not in routing table as a bgp route (i hope...)
+                    # locally sourced prefix is not in routing table as a bgp route (i hope...)
                     if search_re_dict["bgpie"]["result"] == "external":
                         bgpras = (
                             search_re_dict["aspath"]["result"]
                             .split(" ")[0]
                             .replace("(", "")
                         )
                     else:
@@ -3070,25 +3098,25 @@
             raise NotImplementedError("Longer prefixes not yet supported for IOS")
 
         output = []
         # Placeholder for vrf arg
         vrf = ""
         ip_version = None
         try:
-            ip_version = IPNetwork(destination).version
-        except AddrFormatError:
+            ip_version = ipaddress.ip_network(destination).version
+        except ValueError:
             return "Please specify a valid destination!"
         if ip_version == 4:  # process IPv4 routing table
             if vrf == "":
                 vrfs = sorted(self._get_vrfs(ip_version))
             else:
                 vrfs = [vrf]  # VRFs where IPv4 is enabled
             vrfs.append("default")  # global VRF
-            ipnet_dest = IPNetwork(destination)
-            prefix = str(ipnet_dest.network)
+            ipnet_dest = ipaddress.ip_network(destination)
+            prefix = str(ipnet_dest.network_address)
             netmask = ""
             routes = {}
             if "/" in destination:
                 netmask = str(ipnet_dest.netmask)
                 routes = {destination: []}
             commands = []
             for _vrf in vrfs:
```

### Comparing `napalm-4.0.0/napalm/ios/templates/snmp_config.j2` & `napalm-4.1.0/napalm/ios/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_all_sum.tpl` & `napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_all_sum.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh.tpl` & `napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh_afi.tpl` & `napalm-4.1.0/napalm/ios/utils/textfsm_templates/ip_bgp_neigh_afi.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors_detail.tpl` & `napalm-4.1.0/napalm/ios/utils/textfsm_templates/show_lldp_neighbors_detail.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/iosxr/__init__.py` & `napalm-4.1.0/napalm/iosxr/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/iosxr/constants.py` & `napalm-4.1.0/napalm/iosxr/constants.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/iosxr/iosxr.py` & `napalm-4.1.0/napalm/iosxr/iosxr.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # import stdlib
 import re
 import copy
+import ipaddress
 from collections import defaultdict
 import logging
 
 # import third party lib
 from lxml import etree as ETREE
 
-from netaddr import IPAddress  # needed for traceroute, to check IP version
-from netaddr.core import AddrFormatError
-
 from napalm.pyIOSXR import IOSXR
 from napalm.pyIOSXR.exceptions import ConnectError
 from napalm.pyIOSXR.exceptions import TimeoutError
 from napalm.pyIOSXR.exceptions import InvalidInputError
 from napalm.pyIOSXR.exceptions import XMLCLIError
 
 # import NAPALM base
@@ -985,14 +983,30 @@
 
         # here begins actual method...
 
         rpc_command = "<Get><Configuration><BGP><Instance><Naming>\
         <InstanceName>default</InstanceName></Naming></Instance></BGP></Configuration></Get>"
         result_tree = ETREE.fromstring(self.device.make_rpc_call(rpc_command))
 
+        # Check if BGP is not configured.
+        get_tag = result_tree.find("./Get")
+        if get_tag is not None:
+            bgp_not_found = get_tag.attrib.get("ItemNotFound")
+            if bgp_not_found:
+                return {}
+
+        bgp_asn = napalm.base.helpers.convert(
+            int,
+            napalm.base.helpers.find_txt(
+                result_tree,
+                "Get/Configuration/BGP/Instance[1]/InstanceAS/FourByteAS/Naming/AS",
+            ),
+            0,
+        )
+
         if not group:
             neighbor = ""
 
         bgp_group_neighbors = {}
         for bgp_neighbor in result_tree.xpath(".//Neighbor"):
             group_name = napalm.base.helpers.find_txt(
                 bgp_neighbor, "NeighborGroupAddMember"
@@ -1008,15 +1022,17 @@
             if neighbor and peer != neighbor:
                 continue
             description = napalm.base.helpers.find_txt(bgp_neighbor, "Description")
             peer_as = napalm.base.helpers.convert(
                 int, napalm.base.helpers.find_txt(bgp_neighbor, "RemoteAS/AS_YY"), 0
             )
             local_as = napalm.base.helpers.convert(
-                int, napalm.base.helpers.find_txt(bgp_neighbor, "LocalAS/AS_YY"), 0
+                int,
+                napalm.base.helpers.find_txt(bgp_neighbor, "LocalAS/AS_YY"),
+                bgp_asn,
             )
             af_table = napalm.base.helpers.find_txt(
                 bgp_neighbor, "NeighborAFTable/NeighborAF/Naming/AFName"
             )
             prefix_limit = napalm.base.helpers.convert(
                 int,
                 napalm.base.helpers.find_txt(
@@ -1100,15 +1116,15 @@
                 )
                 == "true"
             )
             peer_as = napalm.base.helpers.convert(
                 int, napalm.base.helpers.find_txt(bgp_group, "RemoteAS/AS_YY"), 0
             )
             local_as = napalm.base.helpers.convert(
-                int, napalm.base.helpers.find_txt(bgp_group, "LocalAS/AS_YY"), 0
+                int, napalm.base.helpers.find_txt(bgp_group, "LocalAS/AS_YY"), bgp_asn
             )
             multihop_ttl = napalm.base.helpers.convert(
                 int,
                 napalm.base.helpers.find_txt(bgp_group, "EBGPMultihop/MaxHopCount"),
                 0,
             )
             local_addr_raw = napalm.base.helpers.find_txt(
@@ -1162,30 +1178,30 @@
                 "prefix_limit": build_prefix_limit(
                     af_table, prefix_limit, prefix_percent, prefix_timeout
                 ),
                 "neighbors": bgp_group_neighbors.get(group_name, {}),
             }
             if group and group == group_name:
                 break
-        if "" in bgp_group_neighbors.keys():
-            bgp_config["_"] = {
-                "apply_groups": [],
-                "description": "",
-                "local_as": 0,
-                "type": "",
-                "import_policy": "",
-                "export_policy": "",
-                "local_address": "",
-                "multipath": False,
-                "multihop_ttl": 0,
-                "remote_as": 0,
-                "remove_private_as": False,
-                "prefix_limit": {},
-                "neighbors": bgp_group_neighbors.get("", {}),
-            }
+
+        bgp_config["_"] = {
+            "apply_groups": [],
+            "description": "",
+            "local_as": bgp_asn,
+            "type": "",
+            "import_policy": "",
+            "export_policy": "",
+            "local_address": "",
+            "multipath": False,
+            "multihop_ttl": 0,
+            "remote_as": 0,
+            "remove_private_as": False,
+            "prefix_limit": {},
+            "neighbors": bgp_group_neighbors.get("", {}),
+        }
 
         return bgp_config
 
     def get_bgp_neighbors_detail(self, neighbor_address=""):
 
         bgp_neighbors_detail = {}
 
@@ -1729,16 +1745,16 @@
         if len(dest_split) == 2:
             prefix_tag = "<PrefixLength>{prefix_length}</PrefixLength>".format(
                 prefix_length=dest_split[1]
             )
 
         ipv = 4
         try:
-            ipv = IPAddress(network).version
-        except AddrFormatError:
+            ipv = ipaddress.ip_address(network).version
+        except ValueError:
             logger.error("Wrong destination IP Address format supplied to get_route_to")
             raise TypeError("Wrong destination IP Address!")
 
         if ipv == 6:
             route_info_rpc_command = (
                 "<Get><Operational><IPV6_RIB><VRFTable><VRF><Naming><VRFName>"
                 "default</VRFName></Naming><AFTable><AF><Naming><AFName>IPv6</AFName></Naming>"
@@ -2183,16 +2199,16 @@
         vrf=C.TRACEROUTE_VRF,
     ):
 
         traceroute_result = {}
 
         ipv = 4
         try:
-            ipv = IPAddress(destination).version
-        except AddrFormatError:
+            ipv = ipaddress.ip_address(destination).version
+        except ValueError:
             logger.error(
                 "Incorrect format of IP Address in traceroute \
              with value provided:%s"
                 % (str(destination))
             )
             return {"error": "Wrong destination IP Address!"}
```

### Comparing `napalm-4.0.0/napalm/iosxr/templates/delete_probes.j2` & `napalm-4.1.0/napalm/iosxr/templates/delete_probes.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/iosxr/templates/set_probes.j2` & `napalm-4.1.0/napalm/iosxr/templates/set_probes.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/iosxr/templates/snmp_config.j2` & `napalm-4.1.0/napalm/iosxr/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/iosxr_netconf/__init__.py` & `napalm-4.1.0/napalm/iosxr_netconf/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/iosxr_netconf/constants.py` & `napalm-4.1.0/napalm/iosxr_netconf/constants.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/iosxr_netconf/iosxr_netconf.py` & `napalm-4.1.0/napalm/iosxr_netconf/iosxr_netconf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,24 @@
 
 from __future__ import unicode_literals
 
 # import stdlib
 import re
 import copy
 import difflib
+import ipaddress
 import logging
 
 # import third party lib
 from ncclient import manager
 from ncclient.xml_ import to_ele
 from ncclient.operations.rpc import RPCError
 from ncclient.operations.errors import TimeoutExpiredError
 from lxml import etree as ETREE
 from lxml.etree import XMLSyntaxError
-from netaddr import IPAddress  # needed for traceroute, to check IP version
-from netaddr.core import AddrFormatError
 
 # import NAPALM base
 from napalm.iosxr_netconf import constants as C
 from napalm.iosxr.utilities import strip_config_header
 from napalm.base.base import NetworkDriver
 import napalm.base.helpers
 from napalm.base.exceptions import ConnectionException
@@ -1363,17 +1362,33 @@
         rpc_reply = self.device.get_config(
             source="running", filter=("subtree", C.BGP_CFG_RPC_REQ_FILTER)
         ).xml
 
         # Converts string to etree
         result_tree = ETREE.fromstring(rpc_reply)
 
+        data_ele = result_tree.find("./{*}data")
+        # If there are no children in "<data>", then there is no BGP configured
+        bgp_configured = bool(len(data_ele.getchildren()))
+        if not bgp_configured:
+            return {}
+
         if not group:
             neighbor = ""
 
+        bgp_asn = napalm.base.helpers.convert(
+            int,
+            self._find_txt(
+                result_tree,
+                ".//bgpc:bgp/bgpc:instance/bgpc:instance-as/bgpc:four-byte-as/bgpc:as",
+                default=0,
+                namespaces=C.NS,
+            ),
+        )
+
         bgp_group_neighbors = {}
         bgp_neighbor_xpath = ".//bgpc:bgp/bgpc:instance/bgpc:instance-as/\
              bgpc:four-byte-as/bgpc:default-vrf/bgpc:bgp-entity/bgpc:neighbors/bgpc:neighbor"
         for bgp_neighbor in result_tree.xpath(bgp_neighbor_xpath, namespaces=C.NS):
             group_name = self._find_txt(
                 bgp_neighbor,
                 "./bgpc:neighbor-group-add-member",
@@ -1427,15 +1442,15 @@
                     bgp_neighbor,
                     "./bgpc:local-as/bgpc:as-yy",
                     default="",
                     namespaces=C.NS,
                 ),
                 0,
             )
-            local_as = local_as_x * 65536 + local_as_y
+            local_as = (local_as_x * 65536 + local_as_y) or bgp_asn
             af_table = self._find_txt(
                 bgp_neighbor,
                 "./bgpc:neighbor-afs/bgpc:neighbor-af/bgpc:af-name",
                 default="",
                 namespaces=C.NS,
             )
             prefix_limit = napalm.base.helpers.convert(
@@ -1594,15 +1609,15 @@
                     bgp_group,
                     "./bgpc:local-as/bgpc:as-yy",
                     default="",
                     namespaces=C.NS,
                 ),
                 0,
             )
-            local_as = local_as_x * 65536 + local_as_y
+            local_as = (local_as_x * 65536 + local_as_y) or bgp_asn
             multihop_ttl = napalm.base.helpers.convert(
                 int,
                 self._find_txt(
                     bgp_group,
                     "./bgpc:ebgp-multihop/bgpc:max-hop-count",
                     default="",
                     namespaces=C.NS,
@@ -1676,30 +1691,30 @@
                 "prefix_limit": build_prefix_limit(
                     af_table, prefix_limit, prefix_percent, prefix_timeout
                 ),
                 "neighbors": bgp_group_neighbors.get(group_name, {}),
             }
             if group and group == group_name:
                 break
-        if "" in bgp_group_neighbors.keys():
-            bgp_config["_"] = {
-                "apply_groups": [],
-                "description": "",
-                "local_as": 0,
-                "type": "",
-                "import_policy": "",
-                "export_policy": "",
-                "local_address": "",
-                "multipath": False,
-                "multihop_ttl": 0,
-                "remote_as": 0,
-                "remove_private_as": False,
-                "prefix_limit": {},
-                "neighbors": bgp_group_neighbors.get("", {}),
-            }
+
+        bgp_config["_"] = {
+            "apply_groups": [],
+            "description": "",
+            "local_as": bgp_asn,
+            "type": "",
+            "import_policy": "",
+            "export_policy": "",
+            "local_address": "",
+            "multipath": False,
+            "multihop_ttl": 0,
+            "remote_as": 0,
+            "remove_private_as": False,
+            "prefix_limit": {},
+            "neighbors": bgp_group_neighbors.get("", {}),
+        }
 
         return bgp_config
 
     def get_bgp_neighbors_detail(self, neighbor_address=""):
         """Detailed view of the BGP neighbors operational data."""
 
         def get_vrf_neighbors_detail(
@@ -2477,16 +2492,16 @@
         network = dest_split[0]
         prefix_length = 0
         if len(dest_split) == 2:
             prefix_length = dest_split[1]
 
         ipv = 4
         try:
-            ipv = IPAddress(network).version
-        except AddrFormatError:
+            ipv = ipaddress.ip_address(network).version
+        except ValueError:
             logger.error("Wrong destination IP Address format supplied to get_route_to")
             raise TypeError("Wrong destination IP Address!")
 
         if ipv == 6:
             route_info_rpc_command = (C.ROUTE_IPV6_RPC_REQ_FILTER).format(
                 network=network, prefix_length=prefix_length
             )
@@ -2948,16 +2963,16 @@
         vrf=C.TRACEROUTE_VRF,
     ):
         """Execute traceroute and return results."""
         traceroute_result = {}
 
         ipv = 4
         try:
-            ipv = IPAddress(destination).version
-        except AddrFormatError:
+            ipv = ipaddress.ip_address(destination).version
+        except ValueError:
             logger.error(
                 "Incorrect format of IP Address in traceroute \
              with value provided:%s"
                 % (str(destination))
             )
             return {"error": "Wrong destination IP Address!"}
 
@@ -3135,15 +3150,15 @@
 
         parser = ETREE.XMLParser(remove_blank_text=True)
         # Validate XML config strings and remove rpc-reply tag
         for datastore in config:
             if config[datastore] != "":
                 if encoding == "cli":
                     cli_tree = ETREE.XML(config[datastore], parser=parser)[0]
-                    if cli_tree:
+                    if len(cli_tree):
                         config[datastore] = cli_tree[0].text.strip()
                     else:
                         config[datastore] = ""
                 else:
                     config[datastore] = ETREE.tostring(
                         self._filter_config_tree(
                             ETREE.XML(config[datastore], parser=parser)[0]
```

### Comparing `napalm-4.0.0/napalm/junos/__init__.py` & `napalm-4.1.0/napalm/junos/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/junos/constants.py` & `napalm-4.1.0/napalm/junos/constants.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/junos/junos.py` & `napalm-4.1.0/napalm/junos/junos.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,18 +172,18 @@
                 self.device.cu.unlock()
                 self.locked = False
             except JnrpUnlockError as jue:
                 raise UnlockError(jue)
 
     def _rpc(self, get, child=None, **kwargs):
         """
-        This allows you to construct an arbitrary RPC call to retreive common stuff. For example:
+        This allows you to construct an arbitrary RPC call to retrieve common stuff. For example:
         Configuration:  get: "<get-configuration/>"
         Interface information:  get: "<get-interface-information/>"
-        A particular interfacece information:
+        A particular interface information:
               get: "<get-interface-information/>"
               child: "<interface-name>ge-0/0/0</interface-name>"
         """
         rpc = etree.fromstring(get)
 
         if child:
             rpc.append(etree.fromstring(child))
@@ -1165,15 +1165,15 @@
                         d[k] = u[k]
                 else:
                     d = {k: u[k]}
             return d
 
         def build_prefix_limit(**args):
             """
-            Transform the lements of a dictionary into nested dictionaries.
+            Transform the elements of a dictionary into nested dictionaries.
 
             Example:
                 {
                     'inet_unicast_limit': 500,
                     'inet_unicast_teardown_threshold': 95,
                     'inet_unicast_teardown_timeout': 5
                 }
@@ -1246,21 +1246,48 @@
         }
         _GROUP_FIELDS_DATATYPE_MAP_.update(_COMMON_FIELDS_DATATYPE_)
 
         _DATATYPE_DEFAULT_ = {str: "", int: 0, bool: False, list: []}
 
         bgp_config = {}
 
-        if group:
+        routing_options = junos_views.junos_routing_config_table(self.device)
+        routing_options.get(options=self.junos_config_options)
+
+        bgp_asn_obj = routing_options.xml.find(
+            "./routing-options/autonomous-system/as-number"
+        )
+        system_bgp_asn = int(bgp_asn_obj.text) if bgp_asn_obj is not None else 0
+
+        # No BGP peer-group i.e. "_" key is a special case.
+        if group and group != "_":
             bgp = junos_views.junos_bgp_config_group_table(self.device)
             bgp.get(group=group, options=self.junos_config_options)
         else:
             bgp = junos_views.junos_bgp_config_table(self.device)
             bgp.get(options=self.junos_config_options)
             neighbor = ""  # if no group is set, no neighbor should be set either
+
+            # Only set no peer-group if BGP is actually configured.
+            if bgp.items() or system_bgp_asn:
+                bgp_config["_"] = {
+                    "apply_groups": [],
+                    "description": "",
+                    "local_as": system_bgp_asn,
+                    "type": "",
+                    "import_policy": "",
+                    "export_policy": "",
+                    "local_address": "",
+                    "multipath": False,
+                    "multihop_ttl": 0,
+                    "remote_as": 0,
+                    "remove_private_as": False,
+                    "prefix_limit": {},
+                    "neighbors": {},
+                }
         bgp_items = bgp.items()
 
         if neighbor:
             neighbor_ip = napalm.base.helpers.ip(neighbor)
 
         # Get all policies configured in one go and check if "next-hop self" is found in each policy
         # Save the result in a dict indexed by policy name (junos policy-statement)
@@ -1279,74 +1306,90 @@
             bgp_group_name = bgp_group[0]
             bgp_group_details = bgp_group[1]
             bgp_config[bgp_group_name] = {
                 field: _DATATYPE_DEFAULT_.get(datatype)
                 for field, datatype in _GROUP_FIELDS_DATATYPE_MAP_.items()
                 if "_prefix_limit" not in field
             }
-            for elem in bgp_group_details:
-                if not ("_prefix_limit" not in elem[0] and elem[1] is not None):
+
+            # Always overwrite with the system local_as (this will either be
+            # valid or will be zero i.e. the same as the default value).
+            bgp_config[bgp_group_name]["local_as"] = system_bgp_asn
+
+            for key, value in bgp_group_details:
+                if "_prefix_limit" in key or value is None:
                     continue
-                datatype = _GROUP_FIELDS_DATATYPE_MAP_.get(elem[0])
+                datatype = _GROUP_FIELDS_DATATYPE_MAP_.get(key)
                 default = _DATATYPE_DEFAULT_.get(datatype)
-                key = elem[0]
-                value = elem[1]
+
                 if key in ["export_policy", "import_policy"]:
                     if isinstance(value, list):
                         value = " ".join(value)
                 if key == "local_address":
                     value = napalm.base.helpers.convert(
                         napalm.base.helpers.ip, value, value
                     )
+                if key == "apply_groups":
+                    # Ensure apply_groups value is wrapped in a list
+                    if isinstance(value, str):
+                        value = [value]
                 if key == "neighbors":
                     bgp_group_peers = value
                     continue
                 bgp_config[bgp_group_name].update(
                     {key: napalm.base.helpers.convert(datatype, value, default)}
                 )
             prefix_limit_fields = {}
-            for elem in bgp_group_details:
-                if "_prefix_limit" in elem[0] and elem[1] is not None:
-                    datatype = _GROUP_FIELDS_DATATYPE_MAP_.get(elem[0])
+            for key, value in bgp_group_details:
+                if "_prefix_limit" in key and value is not None:
+                    datatype = _GROUP_FIELDS_DATATYPE_MAP_.get(key)
                     default = _DATATYPE_DEFAULT_.get(datatype)
                     prefix_limit_fields.update(
                         {
-                            elem[0].replace(
+                            key.replace(
                                 "_prefix_limit", ""
-                            ): napalm.base.helpers.convert(datatype, elem[1], default)
+                            ): napalm.base.helpers.convert(datatype, value, default)
                         }
                     )
             bgp_config[bgp_group_name]["prefix_limit"] = build_prefix_limit(
                 **prefix_limit_fields
             )
             if "multihop" in bgp_config[bgp_group_name].keys():
                 # Delete 'multihop' key from the output
                 del bgp_config[bgp_group_name]["multihop"]
                 if bgp_config[bgp_group_name]["multihop_ttl"] == 0:
                     # Set ttl to default value 64
                     bgp_config[bgp_group_name]["multihop_ttl"] = 64
 
             bgp_config[bgp_group_name]["neighbors"] = {}
+            bgp_group_remote_as = bgp_config[bgp_group_name]["remote_as"]
             for bgp_group_neighbor in bgp_group_peers.items():
                 bgp_peer_address = napalm.base.helpers.ip(bgp_group_neighbor[0])
                 if neighbor and bgp_peer_address != neighbor:
                     continue  # if filters applied, jump over all other neighbors
                 bgp_group_details = bgp_group_neighbor[1]
+
+                # Set defaults for this BGP peer
                 bgp_peer_details = {
                     field: _DATATYPE_DEFAULT_.get(datatype)
                     for field, datatype in _PEER_FIELDS_DATATYPE_MAP_.items()
                     if "_prefix_limit" not in field
                 }
-                for elem in bgp_group_details:
-                    if not ("_prefix_limit" not in elem[0] and elem[1] is not None):
+
+                # Always overwrite with the system local_as (this will either be
+                # valid or will be zero i.e. the same as the default value).
+                bgp_peer_details["local_as"] = system_bgp_asn
+                # Always set the default remote-as as the Peer-Group remote-as
+                bgp_peer_details["remote_as"] = bgp_group_remote_as
+
+                for key, value in bgp_group_details:
+                    if "_prefix_limit" in key or value is None:
                         continue
-                    datatype = _PEER_FIELDS_DATATYPE_MAP_.get(elem[0])
+                    datatype = _PEER_FIELDS_DATATYPE_MAP_.get(key)
                     default = _DATATYPE_DEFAULT_.get(datatype)
-                    key = elem[0]
-                    value = elem[1]
                     if key in ["export_policy"]:
                         # next-hop self is applied on export IBGP sessions
                         bgp_peer_details["nhs"] = _check_nhs(value, nhs_policies)
                     if key in ["export_policy", "import_policy"]:
                         if isinstance(value, list):
                             value = " ".join(value)
                     if key == "local_address":
@@ -1366,25 +1409,23 @@
                         bgp_peer_details["route_reflector_client"] = True
                         # we do not want cluster in the output
                         del bgp_peer_details["cluster"]
 
                 if "cluster" in bgp_config[bgp_group_name].keys():
                     bgp_peer_details["route_reflector_client"] = True
                 prefix_limit_fields = {}
-                for elem in bgp_group_details:
-                    if "_prefix_limit" in elem[0] and elem[1] is not None:
-                        datatype = _PEER_FIELDS_DATATYPE_MAP_.get(elem[0])
+                for key, value in bgp_group_details:
+                    if "_prefix_limit" in key and value is not None:
+                        datatype = _PEER_FIELDS_DATATYPE_MAP_.get(key)
                         default = _DATATYPE_DEFAULT_.get(datatype)
                         prefix_limit_fields.update(
                             {
-                                elem[0].replace(
+                                key.replace(
                                     "_prefix_limit", ""
-                                ): napalm.base.helpers.convert(
-                                    datatype, elem[1], default
-                                )
+                                ): napalm.base.helpers.convert(datatype, value, default)
                             }
                         )
                 bgp_peer_details["prefix_limit"] = build_prefix_limit(
                     **prefix_limit_fields
                 )
                 bgp_config[bgp_group_name]["neighbors"][
                     bgp_peer_address
@@ -1820,15 +1861,15 @@
         rt_kargs = {"destination": destination}
         if protocol and isinstance(destination, str):
             rt_kargs["protocol"] = protocol
 
         try:
             routes_table.get(**rt_kargs)
         except RpcTimeoutError:
-            # on devices with milions of routes
+            # on devices with millions of routes
             # in case the destination is too generic (e.g.: 10/8)
             # will take very very long to determine all routes and
             # moreover will return a huge list
             raise CommandTimeoutException(
                 "Too many routes returned! Please try with a longer prefix or a specific protocol!"
             )
         except RpcError as rpce:
```

### Comparing `napalm-4.0.0/napalm/junos/templates/delete_snmp_config.j2` & `napalm-4.1.0/napalm/junos/templates/delete_snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/junos/templates/delete_users.j2` & `napalm-4.1.0/napalm/junos/templates/delete_users.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/junos/templates/set_probes.j2` & `napalm-4.1.0/napalm/junos/templates/set_probes.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/junos/templates/set_users.j2` & `napalm-4.1.0/napalm/junos/templates/set_users.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/junos/templates/snmp_config.j2` & `napalm-4.1.0/napalm/junos/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/junos/utils/junos_views.py` & `napalm-4.1.0/napalm/junos/utils/junos_views.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/junos/utils/junos_views.yml` & `napalm-4.1.0/napalm/junos/utils/junos_views.yml`

 * *Files 1% similar despite different names*

```diff
@@ -398,14 +398,23 @@
     inet6_unicast_teardown_timeout_prefix_limit: {family/inet6/unicast/prefix-limit/teardown/idle-timeout/timeout: int}
     inet6_unicast_novalidate_prefix_limit: {family/inet6/unicast/prefix-limit/no-validate: int}
     inet6_flow_limit_prefix_limit: {family/inet6/flow/prefix-limit/maximum: int}
     inet6_flow_teardown_threshold_prefix_limit: {family/inet6/flow/prefix-limit/teardown/limit-threshold: int}
     inet6_flow_teardown_timeout_prefix_limit: {family/inet6/flow/prefix-limit/teardown/idle-timeout/timeout: int}
     inet6_flow_novalidate_prefix_limit: {family/inet6/flow/prefix-limit/no-validate: unicode}
 
+junos_routing_config_table:
+  get: "routing-options/autonomous-system"
+  view: junos_routing_config_view
+
+junos_routing_config_view:
+  fields:
+    local_system_as: autonomous-system
+
+
 ####
 #### BGP Neighbors and Routing Tables Stats
 ####
 
 junos_bgp_tables_summary_table:
   rpc: get-bgp-summary-information
   args:
```

### Comparing `napalm-4.0.0/napalm/nxapi_plumbing/__init__.py` & `napalm-4.1.0/napalm/nxapi_plumbing/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/nxapi_plumbing/api_client.py` & `napalm-4.1.0/napalm/nxapi_plumbing/api_client.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/nxapi_plumbing/device.py` & `napalm-4.1.0/napalm/nxapi_plumbing/device.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/nxapi_plumbing/errors.py` & `napalm-4.1.0/napalm/nxapi_plumbing/errors.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/nxos/__init__.py` & `napalm-4.1.0/napalm/nxos/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/nxos/nxos.py` & `napalm-4.1.0/napalm/nxos/nxos.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
+import ipaddress
 import json
 import os
 import re
 import tempfile
 import time
 import uuid
 
@@ -38,19 +39,18 @@
 )
 
 from typing_extensions import (
     TypedDict,
     DefaultDict,
 )
 
-from netaddr import IPAddress
-from netaddr.core import AddrFormatError
 from netmiko import file_transfer
 from requests.exceptions import ConnectionError
 from netutils.config.compliance import diff_network_config
+from netutils.interface import canonical_interface_name
 
 import napalm.base.constants as c
 
 # import NAPALM Base
 import napalm.base.helpers
 from napalm.base import NetworkDriver
 from napalm.base.exceptions import CommandErrorException
@@ -229,15 +229,15 @@
           ip router ospf 100 area 0.0.0.1
         ...
 
         Diff that respects the required command hierarchy:
         interface loopback0
           ip address 10.1.4.5/32
         """
-        running_config = self.get_config(retrieve="running")["running"]
+        running_config = self.get_config(retrieve="running", full=True)["running"]
         return diff_network_config(self.merge_candidate, running_config, "cisco_nxos")
 
     def _get_diff(self) -> str:
         """Get a diff between running config and a proposed file."""
         diff: List[str] = []
         self._create_sot_file()
         diff_out = self._send_command(
@@ -352,16 +352,16 @@
             * ip_address (str)
             * rtt (float)
         """
         ping_dict: models.PingResultDict = {}
 
         version = ""
         try:
-            version = "6" if IPAddress(destination).version == 6 else ""
-        except AddrFormatError:
+            version = "6" if ipaddress.ip_address(destination).version == 6 else ""
+        except ValueError:
             # Allow use of DNS names
             pass
 
         command = "ping{version} {destination}".format(
             version=version, destination=destination
         )
         command += " timeout {}".format(timeout)
@@ -466,16 +466,16 @@
 
         traceroute_result: models.TracerouteResultDict = {}
         timeout = 5  # seconds
         probes = 3  # 3 probes/jop and this cannot be changed on NXOS!
 
         version = ""
         try:
-            version = "6" if IPAddress(destination).version == 6 else ""
-        except AddrFormatError:
+            version = "6" if ipaddress.ip_address(destination).version == 6 else ""
+        except ValueError:
             # Allow use of DNS names
             pass
 
         if source:
             source_opt = "source {source}".format(source=source)
             command = "traceroute{version} {destination} {source_opt}".format(
                 version=version, destination=destination, source_opt=source_opt
@@ -679,15 +679,15 @@
             )
             lldp_entry[
                 "remote_system_enable_capab"
             ] = napalm.base.helpers.transform_lldp_capab(
                 lldp_entry["remote_system_enable_capab"]
             )
             # Turn the interfaces into their long version
-            local_intf = napalm.base.helpers.canonical_interface_name(local_intf)
+            local_intf = canonical_interface_name(local_intf)
             lldp.setdefault(local_intf, [])
             lldp[local_intf].append(lldp_entry)  # type: ignore
 
         return lldp
 
     @staticmethod
     def _get_table_rows(
@@ -735,21 +735,17 @@
         else:
             vlan_str = vlan_s
 
         for vls in vlan_str.split(","):
             find = re.findall(find_regexp, vls.strip())
             if find:
                 for i in range(int(find[0][1]), int(find[0][2]) + 1):
-                    vlans.append(
-                        napalm.base.helpers.canonical_interface_name(
-                            find[0][0] + str(i)
-                        )
-                    )
+                    vlans.append(canonical_interface_name(find[0][0] + str(i)))
             else:
-                vlans.append(napalm.base.helpers.canonical_interface_name(vls.strip()))
+                vlans.append(canonical_interface_name(vls.strip()))
         return vlans
 
     @abstractmethod
     def _send_config(self, commands: Union[str, List]) -> List[str]:
         raise NotImplementedError
 
     @abstractmethod
```

### Comparing `napalm-4.0.0/napalm/nxos/templates/snmp_config.j2` & `napalm-4.1.0/napalm/nxos/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/nxos/utils/textfsm_templates/show_lldp_neighbors_detail.tpl` & `napalm-4.1.0/napalm/nxos/utils/textfsm_templates/show_lldp_neighbors_detail.tpl`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/nxos_ssh/__init__.py` & `napalm-4.1.0/napalm/nxos_ssh/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/nxos_ssh/nxos_ssh.py` & `napalm-4.1.0/napalm/nxos_ssh/nxos_ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # import stdlib
 from builtins import super
+import ipaddress
 import re
 import socket
+from collections import defaultdict
 
-# import third party lib
-from netaddr import IPAddress, IPNetwork
-from netaddr.core import AddrFormatError
+# import external lib
+from netutils.interface import canonical_interface_name
 
 # import NAPALM Base
 from napalm.base import helpers
 from napalm.base.exceptions import CommandErrorException, ReplaceConfigException
 from napalm.nxos import NXOSDriverBase
 
 # Easier to store these as constants
@@ -114,15 +115,15 @@
         else:
             is_enabled = True
         is_up = bool("up" in protocol)
 
     else:
         # More standard is up, next line admin state is lines
         match = re.search(re_intf_name_state, interface)
-        intf_name = helpers.canonical_interface_name(match.group("intf_name"))
+        intf_name = canonical_interface_name(match.group("intf_name"))
         intf_state = match.group("intf_state").strip()
         is_up = True if intf_state == "up" else False
 
         admin_state_present = re.search("admin state is", interface)
         if admin_state_present:
             # Parse cases where 'admin state' string exists
             for x_pattern in [re_is_enabled_1, re_is_enabled_2]:
@@ -452,29 +453,23 @@
         """
         Wrapper for Netmiko's send_command method.
 
         raw_text argument is not used and is for code sharing with NX-API.
         """
         return self.device.send_command(command, cmd_verify=cmd_verify)
 
-    def _send_command_list(self, commands, expect_string=None):
-        """Wrapper for Netmiko's send_command method (for list of commands."""
-        output = ""
-        for command in commands:
-            output += self.device.send_command(
-                command,
-                strip_prompt=False,
-                strip_command=False,
-                expect_string=expect_string,
-            )
-        return output
+    def _send_command_list(self, commands, expect_string=None, **kwargs):
+        """Send a list of commands using Netmiko"""
+        return self.device.send_multiline(
+            commands, expect_string=expect_string, **kwargs
+        )
 
     def _send_config(self, commands):
         if isinstance(commands, str):
-            commands = (command for command in commands.splitlines() if command)
+            commands = [command for command in commands.splitlines() if command]
         return self.device.send_config_set(commands)
 
     @staticmethod
     def parse_uptime(uptime_str):
         """
         Extract the uptime string from the given Cisco IOS Device.
         Return the uptime in seconds as an integer
@@ -520,46 +515,48 @@
         except (socket.error, EOFError):
             # If unable to send, we can tell for sure that the connection is unusable,
             # hence return False.
             return {"is_alive": False}
         return {"is_alive": self.device.remote_conn.transport.is_active()}
 
     def _copy_run_start(self):
-
         output = self.device.save_config()
         if "complete" in output.lower():
             return True
         else:
             msg = "Unable to save running-config to startup-config!"
             raise CommandErrorException(msg)
 
     def _load_cfg_from_checkpoint(self):
-
         commands = [
             "terminal dont-ask",
             "rollback running-config file {}".format(self.candidate_cfg),
             "no terminal dont-ask",
         ]
 
         try:
-            rollback_result = self._send_command_list(commands, expect_string=r"[#>]")
+            rollback_result = self._send_command_list(
+                commands, expect_string=r"[#>]", read_timeout=90
+            )
         finally:
             self.changed = True
         msg = rollback_result
         if "Rollback failed." in msg:
             raise ReplaceConfigException(msg)
 
     def rollback(self):
         if self.changed:
             commands = [
                 "terminal dont-ask",
                 "rollback running-config file {}".format(self.rollback_cfg),
                 "no terminal dont-ask",
             ]
-            result = self._send_command_list(commands, expect_string=r"[#>]")
+            result = self._send_command_list(
+                commands, expect_string=r"[#>]", read_timeout=90
+            )
             if "completed" not in result.lower():
                 raise ReplaceConfigException(result)
             # If hostname changes ensure Netmiko state is updated properly
             self._netmiko_device.set_base_prompt()
             self._copy_run_start()
             self.changed = False
 
@@ -655,15 +652,15 @@
             r"(?:^---------+$|^Port .*$|^ .*$)", "", show_int_status, flags=re.M
         )
         for line in show_int_status.splitlines():
             if not line:
                 continue
             interface = line.split()[0]
             # Return canonical interface name
-            interface_list.append(helpers.canonical_interface_name(interface))
+            interface_list.append(canonical_interface_name(interface))
 
         return {
             "uptime": float(uptime),
             "vendor": vendor,
             "os_version": str(os_version),
             "serial_number": str(serial_number),
             "model": str(model),
@@ -795,14 +792,69 @@
             raise TypeError("Please enter a valid list of commands!")
 
         for command in commands:
             output = self._send_command(command)
             cli_output[str(command)] = output
         return cli_output
 
+    def get_network_instances(self, name=""):
+        """
+        get_network_instances implementation for NX-OS
+        """
+
+        # command 'show vrf detail | json' returns all VRFs with detailed information in JSON format
+        # format: list of dictionaries with keys such as 'vrf_name' and 'rd'
+        vrf_table_raw = self._get_command_table(
+            "show vrf detail | json", "TABLE_vrf", "ROW_vrf"
+        )
+
+        # command 'show vrf interface' returns all interfaces including their assigned VRF
+        # format: list of dictionaries with keys 'if_name', 'vrf_name', 'vrf_id' and 'soo'
+        intf_table_raw = self._get_command_table(
+            "show vrf interface | json", "TABLE_if", "ROW_if"
+        )
+
+        # create a dictionary with key = 'vrf_name' and value = list of interfaces
+        vrf_intfs = defaultdict(list)
+        for intf in intf_table_raw:
+            vrf_intfs[intf["vrf_name"]].append(str(intf["if_name"]))
+
+        vrfs = {}
+        for vrf in vrf_table_raw:
+            vrf_name = str(vrf.get("vrf_name"))
+            vrfs[vrf_name] = {}
+            vrfs[vrf_name]["name"] = vrf_name
+
+            # differentiate between VRF type 'DEFAULT_INSTANCE' and 'L3VRF'
+            if vrf_name == "default":
+                vrfs[vrf_name]["type"] = "DEFAULT_INSTANCE"
+            else:
+                vrfs[vrf_name]["type"] = "L3VRF"
+
+            vrfs[vrf_name]["state"] = {"route_distinguisher": str(vrf.get("rd"))}
+
+            # convert list of interfaces (vrf_intfs[vrf_name]) to expected format
+            # format = dict with key = interface name and empty values
+            vrfs[vrf_name]["interfaces"] = {}
+            vrfs[vrf_name]["interfaces"]["interface"] = dict.fromkeys(
+                vrf_intfs[vrf_name], {}
+            )
+
+        # if name of a specific VRF was passed as an argument
+        # only return results for this particular VRF
+
+        if name:
+            if name in vrfs.keys():
+                return {str(name): vrfs[name]}
+            else:
+                return {}
+        # else return results for all VRFs
+        else:
+            return vrfs
+
     def get_environment(self):
         """
         Get environment facts.
 
         power and fan are currently not implemented
         cpu is using 1-minute average
         """
@@ -949,15 +1001,15 @@
         command = "show ntp peers"
         output = self._send_command(command)
 
         for line in output.splitlines():
             # Skip first two lines and last line of command output
             if line == "" or "-----" in line or "Peer IP Address" in line:
                 continue
-            elif IPAddress(len(line.split()[0])).is_unicast:
+            elif not ipaddress.ip_address(len(line.split()[0])).is_multicast:
                 peer_addr = line.split()[0]
                 ntp_entities[peer_addr] = {}
             else:
                 raise ValueError("Did not correctly find a Peer IP Address")
 
         return ntp_entities
 
@@ -1135,15 +1187,15 @@
                 static = False
             if mac_type.lower() in ["dynamic"]:
                 active = True
             else:
                 active = False
             return {
                 "mac": helpers.mac(mac),
-                "interface": helpers.canonical_interface_name(interface),
+                "interface": canonical_interface_name(interface),
                 "vlan": int(vlan),
                 "static": static,
                 "active": active,
                 "moves": -1,
                 "last_move": -1.0,
             }
 
@@ -1154,15 +1206,14 @@
         output = re.sub(r"^[\*\+GOCE]", "", output, flags=re.M)
         output = re.sub(r"^\(R\)", "", output, flags=re.M)
         output = re.sub(r"^\(T\)", "", output, flags=re.M)
         output = re.sub(r"^\(F\)", "", output, flags=re.M)
         output = re.sub(r"vPC Peer-Link", "vPC-Peer-Link", output, flags=re.M)
 
         for line in output.splitlines():
-
             # Every 500 Mac's Legend is reprinted, regardless of terminal length
             if re.search(r"^Legend", line):
                 continue
             elif re.search(r"^\s+\* \- primary entry", line):
                 continue
             elif re.search(r"^\s+age \-", line):
                 continue
@@ -1336,16 +1387,16 @@
         if longer:
             raise NotImplementedError("Longer prefixes not yet supported for NXOS")
         longer_pref = ""  # longer_prefixes support, for future use
         vrf = ""
 
         ip_version = None
         try:
-            ip_version = IPNetwork(destination).version
-        except AddrFormatError:
+            ip_version = ipaddress.ip_network(destination).version
+        except ValueError:
             return "Please specify a valid destination!"
         if ip_version == 4:  # process IPv4 routing table
             routes = {}
             if vrf:
                 send_cmd = "show ip route vrf {vrf} {destination} {longer}".format(
                     vrf=vrf, destination=destination, longer=longer_pref
                 ).rstrip()
@@ -1405,15 +1456,15 @@
                             # rest_of_line = viastr.group('rest')
                             # use only routes from specified protocol
                             if protocol and protocol != nh_source:
                                 continue
                             # routing protocol process number, for future use
                             # nh_source_proc_nr = viastr.group('procnr)
                             if nh_int:
-                                nh_int_canon = helpers.canonical_interface_name(nh_int)
+                                nh_int_canon = canonical_interface_name(nh_int)
                             else:
                                 nh_int_canon = ""
                             route_entry = {
                                 "protocol": nh_source,
                                 "outgoing_interface": nh_int_canon,
                                 "age": nh_age,
                                 "current_active": nh_used,
```

### Comparing `napalm-4.0.0/napalm/nxos_ssh/templates/snmp_config.j2` & `napalm-4.1.0/napalm/nxos_ssh/templates/snmp_config.j2`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/pyIOSXR/__init__.py` & `napalm-4.1.0/napalm/pyIOSXR/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/pyIOSXR/exceptions.py` & `napalm-4.1.0/napalm/pyIOSXR/exceptions.py`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/napalm/pyIOSXR/iosxr.py` & `napalm-4.1.0/napalm/pyIOSXR/iosxr.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,15 +686,15 @@
                     "confirmed needs to be between 30 and 300 seconds", self
                 )
         rpc_command += "/>"
         self._execute_rpc(rpc_command)
 
     def discard_config(self):
         """
-        Clear uncommited changes in the current session.
+        Clear uncommitted changes in the current session.
 
         Clear previously loaded configuration on the device without committing it.
         """
         rpc_command = "<Clear/>"
         self._execute_rpc(rpc_command)
 
     def rollback(self, rb_id=1):
```

### Comparing `napalm-4.0.0/napalm.egg-info/PKG-INFO` & `napalm-4.1.0/napalm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: napalm
-Version: 4.0.0
+Version: 4.1.0
 Summary: Network Automation and Programmability Abstraction Layer with Multivendor support
 Home-page: https://github.com/napalm-automation/napalm
 Author: David Barroso, Kirk Byers, Mircea Ulinic
 Author-email: dbarrosop@dravetech.com, ping@mirceaulinic.net, ktbyers@twb-tech.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -168,9 +167,7 @@
 
 This project is maintained by David Barroso, Mircea Ulinic, and Kirk Byers and a set of other contributors.
 
 Originally it was hosted by the [Spotify][spotify] organization but due to the many contributions received by third parties we agreed creating a dedicated organization for NAPALM and give a big thanks to [Spotify][spotify] for the support.
 
 [spotify]: http://www.spotify.com
 [bigwave]: http://bigwaveit.org/
-
-
```

### Comparing `napalm-4.0.0/napalm.egg-info/SOURCES.txt` & `napalm-4.1.0/napalm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napalm-4.0.0/setup.cfg` & `napalm-4.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 license_file = LICENSE
 
 [pylama]
-linters = mccabe,pep8,pyflakes
+linters = mccabe,pycodestyle,pyflakes
 ignore = D203,C901,E203
 skip = .tox/*,.env/*,.venv/*
 
-[pylama:pep8]
+[pylama:pycodestyle]
 max_line_length = 100
 
 [tool:pytest]
 norecursedirs = 
 	.git
 	.tox
 	.env
```

### Comparing `napalm-4.0.0/setup.py` & `napalm-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = fs.read()
 
 
 __author__ = "David Barroso <dbarrosop@dravetech.com>"
 
 setup(
     name="napalm",
-    version="4.0.0",
+    version="4.1.0",
     packages=find_packages(exclude=("test*",)),
     test_suite="test_base",
     author="David Barroso, Kirk Byers, Mircea Ulinic",
     author_email="dbarrosop@dravetech.com, ping@mirceaulinic.net, ktbyers@twb-tech.com",
     description="Network Automation and Programmability Abstraction Layer with Multivendor support",
     license="Apache 2.0",
     long_description=long_description,
```

