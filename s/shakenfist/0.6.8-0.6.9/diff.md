# Comparing `tmp/shakenfist-0.6.8.tar.gz` & `tmp/shakenfist-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakenfist-0.6.8.tar", last modified: Sun Nov  6 04:43:12 2022, max compression
+gzip compressed data, was "shakenfist-0.6.9.tar", last modified: Sun Nov  6 07:49:14 2022, max compression
```

## Comparing `shakenfist-0.6.8.tar` & `shakenfist-0.6.9.tar`

### file list

```diff
@@ -1,255 +1,255 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.888507 shakenfist-0.6.8/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       97 2021-09-25 23:09:33.000000 shakenfist-0.6.8/.coveragerc
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.844510 shakenfist-0.6.8/.github/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.860509 shakenfist-0.6.8/.github/workflows/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1677 2021-09-25 23:09:33.000000 shakenfist-0.6.8/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3593 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/configure-tests.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8237 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/functional-tests-debian-10-localhost.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8246 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/functional-tests-debian-11-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8252 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8603 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/functional-tests.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7903 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/nodelifecycle-tests.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      812 2022-09-25 06:31:57.000000 shakenfist-0.6.8/.github/workflows/publish-website.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1390 2022-09-25 06:31:59.000000 shakenfist-0.6.8/.github/workflows/python-unit-tests.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8659 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-develop-debian-10-localhost.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8671 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-develop-debian-11-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8679 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-develop-ubuntu-2004-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      208 2022-09-25 06:31:59.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-failure.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8659 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-debian-10-localhost.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8671 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-debian-11-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8695 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-released-debian-10-localhost.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8707 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-released-debian-11-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8715 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-released-ubuntu-2004-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8679 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-ubuntu-2004-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9164 2022-11-06 04:42:37.000000 shakenfist-0.6.8/.github/workflows/scheduled-tests.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       49 2021-09-25 23:09:33.000000 shakenfist-0.6.8/.stestr.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      507 2022-11-06 04:43:12.000000 shakenfist-0.6.8/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1192 2022-09-25 06:31:57.000000 shakenfist-0.6.8/BRANCHES.rst
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2021-09-25 23:09:33.000000 shakenfist-0.6.8/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1132 2022-11-06 04:43:12.888507 shakenfist-0.6.8/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      452 2021-09-25 23:09:33.000000 shakenfist-0.6.8/README.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.864508 shakenfist-0.6.8/deploy/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       52 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/.stestr.conf
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.864508 shakenfist-0.6.8/deploy/ansible/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    10115 2022-11-06 04:42:37.000000 shakenfist-0.6.8/deploy/ansible/ci-image.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2680 2022-11-06 04:42:37.000000 shakenfist-0.6.8/deploy/ansible/ci-include-common-localhost.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2797 2022-11-06 04:42:37.000000 shakenfist-0.6.8/deploy/ansible/ci-topology-localhost-released.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3747 2022-11-06 04:42:37.000000 shakenfist-0.6.8/deploy/ansible/ci-topology-localhost.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    13291 2022-11-06 04:42:37.000000 shakenfist-0.6.8/deploy/ansible/ci-topology-slim-primary-released.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    14241 2022-11-06 04:42:37.000000 shakenfist-0.6.8/deploy/ansible/ci-topology-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4173 2022-11-06 04:42:32.000000 shakenfist-0.6.8/deploy/ansible/deploy.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    24099 2022-11-06 04:42:37.000000 shakenfist-0.6.8/deploy/ansible/deploy.yml
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.864508 shakenfist-0.6.8/deploy/ansible/files/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      510 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/ansible/files/apache-site-primary.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1138 2022-11-06 04:42:32.000000 shakenfist-0.6.8/deploy/ansible/files/config
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      790 2021-10-18 08:23:52.000000 shakenfist-0.6.8/deploy/ansible/files/dhcp.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       79 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/ansible/files/dhcphosts.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3541 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/ansible/files/etcd.conf
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.864508 shakenfist-0.6.8/deploy/ansible/files/grafana/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    20520 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/ansible/files/grafana/grafana.ini
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2269 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/ansible/files/grafana/ldap.toml
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.844510 shakenfist-0.6.8/deploy/ansible/files/grafana/provisioning/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.864508 shakenfist-0.6.8/deploy/ansible/files/grafana/provisioning/dashboards/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      266 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/ansible/files/grafana/provisioning/dashboards/dashboards.yaml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    50088 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/ansible/files/grafana/provisioning/dashboards/shakenfist.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7193 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/ansible/files/libvirt.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      174 2021-12-28 09:58:25.000000 shakenfist-0.6.8/deploy/ansible/files/netplan-eth1.yaml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      273 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/ansible/files/rsyslog-client-01-sf.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      246 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/ansible/files/rsyslog-server-01-sf.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      365 2021-12-28 09:58:25.000000 shakenfist-0.6.8/deploy/ansible/files/sf.service
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      275 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/ansible/files/sfrc
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      112 2021-12-28 09:58:25.000000 shakenfist-0.6.8/deploy/ansible/files/shakenfist.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      373 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/ansible/hosts
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.864508 shakenfist-0.6.8/deploy/ansible/includes/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1968 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/ansible/includes/topology_add_node.yml
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.864508 shakenfist-0.6.8/deploy/ansible/tasks/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      685 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/ansible/tasks/build-wheel.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      282 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/ansible/tasks/distro-check.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    31769 2022-11-06 04:42:35.000000 shakenfist-0.6.8/deploy/getsf
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      342 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/install
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5225 2022-11-06 04:42:37.000000 shakenfist-0.6.8/deploy/nodelifecycletests.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      115 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/pyproject.toml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      296 2022-09-25 06:31:59.000000 shakenfist-0.6.8/deploy/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      175 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/requirements.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      617 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      690 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.864508 shakenfist-0.6.8/deploy/shakenfist_ci/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       34 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/shakenfist_ci/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/shakenfist_ci/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    18320 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/base.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.868508 shakenfist-0.6.8/deploy/shakenfist_ci/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/__init__.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.868508 shakenfist-0.6.8/deploy/shakenfist_ci/tests/files/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      161 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/files/console_scribbler_userdata
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      377 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/files/writedata_userdata
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9950 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_artifacts.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      929 2022-11-06 04:42:35.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_auth.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2510 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_boot.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3878 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_cloudinit.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7545 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_commandline_artifacts.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2919 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_commandline_network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2452 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_console_log.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3781 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_disk_specs.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1510 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_disks.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3162 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_floating_ips.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1324 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_metadata.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2287 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_multiple_nics.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2858 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_namespace.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    13361 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_networking.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1716 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_object_names.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4117 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_placement.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1244 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_serial_console.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    16718 2022-11-06 04:42:35.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_snapshots.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8171 2022-09-25 06:31:59.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_state_changes.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1610 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_system_namespace.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1564 2022-09-25 06:31:57.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_ubuntu.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2633 2021-12-28 09:58:25.000000 shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_upgrades.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2021-12-28 09:58:25.000000 shakenfist-0.6.8/deploy/test-requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      601 2022-09-25 06:29:44.000000 shakenfist-0.6.8/deploy/tox.ini
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    60429 2022-11-06 04:43:00.000000 shakenfist-0.6.8/deploy.tgz
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.868508 shakenfist-0.6.8/docs/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       14 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/CNAME
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.868508 shakenfist-0.6.8/docs/changelog/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4709 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/changelog/changelog_v02.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4266 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/changelog/changelog_v03.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2215 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/changelog/changelog_v04.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1144 2022-07-24 22:44:21.000000 shakenfist-0.6.8/docs/community.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.872508 shakenfist-0.6.8/docs/development/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4851 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/development/ci_api_coverage.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2776 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/development/git_usage.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9808 2021-12-28 09:58:25.000000 shakenfist-0.6.8/docs/development/io_performance_tuning.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2178 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/development/namespace_auth.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2870 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/development/release_process.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      689 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/development/standards.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2565 2021-12-28 09:58:25.000000 shakenfist-0.6.8/docs/development/state_machine.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      585 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/development/updating_docs.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    10187 2022-09-25 06:31:57.000000 shakenfist-0.6.8/docs/features.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    10315 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/index.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    10396 2022-07-24 22:44:21.000000 shakenfist-0.6.8/docs/installation.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2528 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/manifesto.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.872508 shakenfist-0.6.8/docs/networking/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1771 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/networking/overview.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    15355 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/networking/single_instance.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      927 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/power_states.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     6800 2021-09-25 23:09:33.000000 shakenfist-0.6.8/docs/usage.md
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    32084 2022-11-06 04:43:00.000000 shakenfist-0.6.8/docs.tgz
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.872508 shakenfist-0.6.8/examples/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5260 2021-09-25 23:09:33.000000 shakenfist-0.6.8/examples/configdrive-sample-ocata-plain.tgz
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    40926 2021-09-25 23:09:33.000000 shakenfist-0.6.8/examples/schema-v0_3_3.tgz
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1637 2021-09-25 23:09:33.000000 shakenfist-0.6.8/mkdocs.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3125 2021-09-25 23:09:33.000000 shakenfist-0.6.8/network-example.dia
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    16514 2021-09-25 23:09:33.000000 shakenfist-0.6.8/network-example.png
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      115 2022-09-25 06:31:57.000000 shakenfist-0.6.8/pyproject.toml
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)     1211 2021-09-25 23:09:33.000000 shakenfist-0.6.8/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1031 2022-11-06 04:42:35.000000 shakenfist-0.6.8/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      796 2022-11-06 04:43:12.888507 shakenfist-0.6.8/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1791 2021-12-28 09:58:25.000000 shakenfist-0.6.8/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.876507 shakenfist-0.6.8/shakenfist/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11890 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/artifact.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11205 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/baseobject.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      735 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/baseobjectmapping.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    22317 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/blob.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.876507 shakenfist-0.6.8/shakenfist/client/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/client/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1828 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/client/backup.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3401 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/client/ctl.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9426 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/config.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1331 2022-09-25 06:31:57.000000 shakenfist-0.6.8/shakenfist/constants.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.876507 shakenfist-0.6.8/shakenfist/daemons/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    17331 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/daemons/cleaner.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    15589 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/daemons/cluster.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2626 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/daemons/daemon.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1561 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/daemons/eventlog.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1594 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/daemons/external_api.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9955 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/daemons/main.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    19537 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/daemons/net.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    16862 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/daemons/queues.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    10643 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/daemons/resources.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      931 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/daemons/shim.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    10854 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/daemons/sidechannel.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2471 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/db.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3781 2022-09-25 06:31:57.000000 shakenfist-0.6.8/shakenfist/dhcp.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    21268 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/etcd.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5909 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/eventlog.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3208 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/exceptions.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.876507 shakenfist-0.6.8/shakenfist/external_api/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/external_api/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      280 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/admin.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7845 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/external_api/app.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    12347 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/artifact.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8384 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/auth.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    15353 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/base.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3203 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/blob.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    29613 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/instance.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1838 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/interface.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2329 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/label.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9968 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1830 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/external_api/node.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1791 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/snapshot.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1581 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/upload.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2484 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/external_api/util.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    15629 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/images.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    53346 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/instance.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4558 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/ipmanager.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7327 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/logutil.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1936 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/metrics.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    29324 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     6114 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/networkinterface.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5709 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/node.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    12078 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/scheduler.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8001 2022-09-25 06:31:57.000000 shakenfist-0.6.8/shakenfist/tasks.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.880507 shakenfist-0.6.8/shakenfist/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      851 2022-09-25 06:31:57.000000 shakenfist-0.6.8/shakenfist/tests/base.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.884507 shakenfist-0.6.8/shakenfist/tests/external_api/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    21471 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/tests/external_api/test_auth.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5037 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/tests/external_api/test_network.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.884507 shakenfist-0.6.8/shakenfist/tests/files/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1521 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/files/cirros-MD5SUMS-0.3.4
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3236 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/files/cirros-download
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      713 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/files/dhcp.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       79 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/files/dhcphosts.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      222 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/files/qemu-img-info
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2682 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/files/ubuntu-MD5SUMS-bionic
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2325 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/files/ubuntu-MD5SUMS-groovy
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4366 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/files/ubuntu-download
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9892 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/tests/mock_etcd.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2264 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/tests/test_baseobject.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1341 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/test_config.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5486 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/tests/test_daemon_cleaner.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9849 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/tests/test_dhcp.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    16641 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/tests/test_etcd.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    53859 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/tests/test_external_api.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    28106 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/tests/test_instance.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     6086 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/tests/test_ipmanager.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11564 2022-09-25 06:31:57.000000 shakenfist-0.6.8/shakenfist/tests/test_net.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1504 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/test_networkinterface.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    12460 2022-11-06 04:42:37.000000 shakenfist-0.6.8/shakenfist/tests/test_scheduler.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3757 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/tests/test_tasks.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      721 2022-09-25 06:31:57.000000 shakenfist-0.6.8/shakenfist/tests/test_util_general.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7341 2022-09-25 06:31:57.000000 shakenfist-0.6.8/shakenfist/tests/test_util_network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1756 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/upload.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.884507 shakenfist-0.6.8/shakenfist/util/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.8/shakenfist/util/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      491 2021-12-28 09:58:25.000000 shakenfist-0.6.8/shakenfist/util/callstack.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4453 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/util/general.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     6224 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/util/image.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4645 2022-09-25 06:31:57.000000 shakenfist-0.6.8/shakenfist/util/libvirt.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     6420 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/util/network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1711 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/util/process.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      187 2022-11-06 04:42:35.000000 shakenfist-0.6.8/shakenfist/util/random.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.876507 shakenfist-0.6.8/shakenfist.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1132 2022-11-06 04:43:12.000000 shakenfist-0.6.8/shakenfist.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7554 2022-11-06 04:43:12.000000 shakenfist-0.6.8/shakenfist.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2022-11-06 04:43:12.000000 shakenfist-0.6.8/shakenfist.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      182 2022-11-06 04:43:12.000000 shakenfist-0.6.8/shakenfist.egg-info/entry_points.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2022-11-06 04:43:12.000000 shakenfist-0.6.8/shakenfist.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       47 2022-11-06 04:43:12.000000 shakenfist-0.6.8/shakenfist.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      711 2022-11-06 04:43:12.000000 shakenfist-0.6.8/shakenfist.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       11 2022-11-06 04:43:12.000000 shakenfist-0.6.8/shakenfist.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      102 2022-11-06 04:42:35.000000 shakenfist-0.6.8/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 04:43:12.888507 shakenfist-0.6.8/tools/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4017 2022-09-25 06:31:59.000000 shakenfist-0.6.8/tools/clone_with_depends.py
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      580 2021-09-25 23:09:33.000000 shakenfist-0.6.8/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      654 2022-09-25 06:31:57.000000 shakenfist-0.6.8/tools/network_allocation_torture.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      978 2022-11-06 04:42:37.000000 shakenfist-0.6.8/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.810182 shakenfist-0.6.9/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       97 2021-09-25 23:09:33.000000 shakenfist-0.6.9/.coveragerc
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.749675 shakenfist-0.6.9/.github/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.765810 shakenfist-0.6.9/.github/workflows/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1677 2021-09-25 23:09:33.000000 shakenfist-0.6.9/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3593 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/configure-tests.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8237 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/functional-tests-debian-10-localhost.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8246 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/functional-tests-debian-11-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8252 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8603 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/functional-tests.tmpl
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7903 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/nodelifecycle-tests.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      812 2022-09-25 06:31:57.000000 shakenfist-0.6.9/.github/workflows/publish-website.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1390 2022-09-25 06:31:59.000000 shakenfist-0.6.9/.github/workflows/python-unit-tests.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8659 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-develop-debian-10-localhost.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8671 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-develop-debian-11-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8679 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-develop-ubuntu-2004-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      208 2022-09-25 06:31:59.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-failure.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8659 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-debian-10-localhost.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8671 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-debian-11-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8695 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-released-debian-10-localhost.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8707 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-released-debian-11-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8715 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-released-ubuntu-2004-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8679 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-ubuntu-2004-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9164 2022-11-06 04:42:37.000000 shakenfist-0.6.9/.github/workflows/scheduled-tests.tmpl
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       49 2021-09-25 23:09:33.000000 shakenfist-0.6.9/.stestr.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      507 2022-11-06 07:49:14.000000 shakenfist-0.6.9/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1192 2022-09-25 06:31:57.000000 shakenfist-0.6.9/BRANCHES.rst
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2021-09-25 23:09:33.000000 shakenfist-0.6.9/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1132 2022-11-06 07:49:14.810182 shakenfist-0.6.9/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      452 2021-09-25 23:09:33.000000 shakenfist-0.6.9/README.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.769844 shakenfist-0.6.9/deploy/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       52 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/.stestr.conf
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.769844 shakenfist-0.6.9/deploy/ansible/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    10115 2022-11-06 04:42:37.000000 shakenfist-0.6.9/deploy/ansible/ci-image.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2680 2022-11-06 04:42:37.000000 shakenfist-0.6.9/deploy/ansible/ci-include-common-localhost.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2797 2022-11-06 04:42:37.000000 shakenfist-0.6.9/deploy/ansible/ci-topology-localhost-released.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3747 2022-11-06 04:42:37.000000 shakenfist-0.6.9/deploy/ansible/ci-topology-localhost.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    13291 2022-11-06 04:42:37.000000 shakenfist-0.6.9/deploy/ansible/ci-topology-slim-primary-released.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    14241 2022-11-06 04:42:37.000000 shakenfist-0.6.9/deploy/ansible/ci-topology-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4173 2022-11-06 04:42:32.000000 shakenfist-0.6.9/deploy/ansible/deploy.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    24099 2022-11-06 04:42:37.000000 shakenfist-0.6.9/deploy/ansible/deploy.yml
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.769844 shakenfist-0.6.9/deploy/ansible/files/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      510 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/ansible/files/apache-site-primary.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1138 2022-11-06 04:42:32.000000 shakenfist-0.6.9/deploy/ansible/files/config
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      790 2021-10-18 08:23:52.000000 shakenfist-0.6.9/deploy/ansible/files/dhcp.tmpl
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       79 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/ansible/files/dhcphosts.tmpl
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3541 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/ansible/files/etcd.conf
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.769844 shakenfist-0.6.9/deploy/ansible/files/grafana/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    20520 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/ansible/files/grafana/grafana.ini
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2269 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/ansible/files/grafana/ldap.toml
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.753708 shakenfist-0.6.9/deploy/ansible/files/grafana/provisioning/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.769844 shakenfist-0.6.9/deploy/ansible/files/grafana/provisioning/dashboards/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      266 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/ansible/files/grafana/provisioning/dashboards/dashboards.yaml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    50088 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/ansible/files/grafana/provisioning/dashboards/shakenfist.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7193 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/ansible/files/libvirt.tmpl
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      174 2021-12-28 09:58:25.000000 shakenfist-0.6.9/deploy/ansible/files/netplan-eth1.yaml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      273 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/ansible/files/rsyslog-client-01-sf.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      246 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/ansible/files/rsyslog-server-01-sf.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      365 2021-12-28 09:58:25.000000 shakenfist-0.6.9/deploy/ansible/files/sf.service
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      275 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/ansible/files/sfrc
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      112 2021-12-28 09:58:25.000000 shakenfist-0.6.9/deploy/ansible/files/shakenfist.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      373 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/ansible/hosts
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.769844 shakenfist-0.6.9/deploy/ansible/includes/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1968 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/ansible/includes/topology_add_node.yml
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.769844 shakenfist-0.6.9/deploy/ansible/tasks/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      685 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/ansible/tasks/build-wheel.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      282 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/ansible/tasks/distro-check.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    31769 2022-11-06 04:42:35.000000 shakenfist-0.6.9/deploy/getsf
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      342 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/install
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5225 2022-11-06 04:42:37.000000 shakenfist-0.6.9/deploy/nodelifecycletests.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      115 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/pyproject.toml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      296 2022-09-25 06:31:59.000000 shakenfist-0.6.9/deploy/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      175 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/requirements.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      617 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      690 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.773878 shakenfist-0.6.9/deploy/shakenfist_ci/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       34 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/shakenfist_ci/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/shakenfist_ci/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    18320 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/base.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.773878 shakenfist-0.6.9/deploy/shakenfist_ci/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/__init__.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.773878 shakenfist-0.6.9/deploy/shakenfist_ci/tests/files/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      161 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/files/console_scribbler_userdata
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      377 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/files/writedata_userdata
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9950 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_artifacts.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      929 2022-11-06 04:42:35.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_auth.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2510 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_boot.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3878 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_cloudinit.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7545 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_commandline_artifacts.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2919 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_commandline_network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2452 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_console_log.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3781 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_disk_specs.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1510 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_disks.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3162 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_floating_ips.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1324 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_metadata.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2287 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_multiple_nics.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2858 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_namespace.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    13361 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_networking.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1716 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_object_names.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4117 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_placement.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1244 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_serial_console.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    16718 2022-11-06 04:42:35.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_snapshots.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8171 2022-09-25 06:31:59.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_state_changes.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1610 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_system_namespace.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1564 2022-09-25 06:31:57.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_ubuntu.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2633 2021-12-28 09:58:25.000000 shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_upgrades.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2021-12-28 09:58:25.000000 shakenfist-0.6.9/deploy/test-requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      601 2022-09-25 06:29:44.000000 shakenfist-0.6.9/deploy/tox.ini
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    60429 2022-11-06 07:49:02.000000 shakenfist-0.6.9/deploy.tgz
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.773878 shakenfist-0.6.9/docs/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       14 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/CNAME
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.773878 shakenfist-0.6.9/docs/changelog/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4709 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/changelog/changelog_v02.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4266 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/changelog/changelog_v03.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2215 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/changelog/changelog_v04.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1144 2022-07-24 22:44:21.000000 shakenfist-0.6.9/docs/community.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.777912 shakenfist-0.6.9/docs/development/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4851 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/development/ci_api_coverage.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2776 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/development/git_usage.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9808 2021-12-28 09:58:25.000000 shakenfist-0.6.9/docs/development/io_performance_tuning.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2178 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/development/namespace_auth.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2870 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/development/release_process.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      689 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/development/standards.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2565 2021-12-28 09:58:25.000000 shakenfist-0.6.9/docs/development/state_machine.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      585 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/development/updating_docs.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    10187 2022-09-25 06:31:57.000000 shakenfist-0.6.9/docs/features.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    10315 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/index.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    10396 2022-07-24 22:44:21.000000 shakenfist-0.6.9/docs/installation.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2528 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/manifesto.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.777912 shakenfist-0.6.9/docs/networking/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1771 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/networking/overview.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    15355 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/networking/single_instance.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      927 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/power_states.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     6800 2021-09-25 23:09:33.000000 shakenfist-0.6.9/docs/usage.md
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    32084 2022-11-06 07:49:02.000000 shakenfist-0.6.9/docs.tgz
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.777912 shakenfist-0.6.9/examples/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5260 2021-09-25 23:09:33.000000 shakenfist-0.6.9/examples/configdrive-sample-ocata-plain.tgz
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    40926 2021-09-25 23:09:33.000000 shakenfist-0.6.9/examples/schema-v0_3_3.tgz
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1637 2021-09-25 23:09:33.000000 shakenfist-0.6.9/mkdocs.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3125 2021-09-25 23:09:33.000000 shakenfist-0.6.9/network-example.dia
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    16514 2021-09-25 23:09:33.000000 shakenfist-0.6.9/network-example.png
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      115 2022-09-25 06:31:57.000000 shakenfist-0.6.9/pyproject.toml
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)     1211 2021-09-25 23:09:33.000000 shakenfist-0.6.9/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1031 2022-11-06 04:42:35.000000 shakenfist-0.6.9/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      796 2022-11-06 07:49:14.810182 shakenfist-0.6.9/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1791 2021-12-28 09:58:25.000000 shakenfist-0.6.9/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.785979 shakenfist-0.6.9/shakenfist/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11890 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/artifact.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11205 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/baseobject.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      735 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/baseobjectmapping.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    22317 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/blob.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.785979 shakenfist-0.6.9/shakenfist/client/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/client/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1828 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/client/backup.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3401 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/client/ctl.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9426 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/config.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1331 2022-09-25 06:31:57.000000 shakenfist-0.6.9/shakenfist/constants.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.785979 shakenfist-0.6.9/shakenfist/daemons/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    17331 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/daemons/cleaner.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    15594 2022-11-06 07:48:51.000000 shakenfist-0.6.9/shakenfist/daemons/cluster.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2626 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/daemons/daemon.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1561 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/daemons/eventlog.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1594 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/daemons/external_api.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9955 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/daemons/main.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    19537 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/daemons/net.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    16862 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/daemons/queues.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    10643 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/daemons/resources.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      931 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/daemons/shim.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    10854 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/daemons/sidechannel.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2471 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/db.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3781 2022-09-25 06:31:57.000000 shakenfist-0.6.9/shakenfist/dhcp.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    21268 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/etcd.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5909 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/eventlog.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3208 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/exceptions.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.794047 shakenfist-0.6.9/shakenfist/external_api/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/external_api/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      280 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/admin.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7845 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/external_api/app.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    12347 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/artifact.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8384 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/auth.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    15353 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/base.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3203 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/blob.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    29613 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/instance.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1838 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/interface.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2329 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/label.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9968 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1830 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/external_api/node.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1791 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/snapshot.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1581 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/upload.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2484 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/external_api/util.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    15629 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/images.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    53346 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/instance.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4558 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/ipmanager.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7327 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/logutil.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1936 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/metrics.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    29324 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     6114 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/networkinterface.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5709 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/node.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    12078 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/scheduler.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8001 2022-09-25 06:31:57.000000 shakenfist-0.6.9/shakenfist/tasks.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.802115 shakenfist-0.6.9/shakenfist/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      851 2022-09-25 06:31:57.000000 shakenfist-0.6.9/shakenfist/tests/base.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.802115 shakenfist-0.6.9/shakenfist/tests/external_api/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    21471 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/tests/external_api/test_auth.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5037 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/tests/external_api/test_network.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.802115 shakenfist-0.6.9/shakenfist/tests/files/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1521 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/files/cirros-MD5SUMS-0.3.4
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3236 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/files/cirros-download
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      713 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/files/dhcp.tmpl
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       79 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/files/dhcphosts.tmpl
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      222 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/files/qemu-img-info
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2682 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/files/ubuntu-MD5SUMS-bionic
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2325 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/files/ubuntu-MD5SUMS-groovy
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4366 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/files/ubuntu-download
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9892 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/tests/mock_etcd.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2264 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/tests/test_baseobject.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1341 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/test_config.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5486 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/tests/test_daemon_cleaner.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9849 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/tests/test_dhcp.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    16641 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/tests/test_etcd.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    53859 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/tests/test_external_api.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    28106 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/tests/test_instance.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     6086 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/tests/test_ipmanager.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11564 2022-09-25 06:31:57.000000 shakenfist-0.6.9/shakenfist/tests/test_net.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1504 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/test_networkinterface.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    12460 2022-11-06 04:42:37.000000 shakenfist-0.6.9/shakenfist/tests/test_scheduler.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3757 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/tests/test_tasks.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      721 2022-09-25 06:31:57.000000 shakenfist-0.6.9/shakenfist/tests/test_util_general.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7341 2022-09-25 06:31:57.000000 shakenfist-0.6.9/shakenfist/tests/test_util_network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1756 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/upload.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.806149 shakenfist-0.6.9/shakenfist/util/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:33.000000 shakenfist-0.6.9/shakenfist/util/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      491 2021-12-28 09:58:25.000000 shakenfist-0.6.9/shakenfist/util/callstack.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4453 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/util/general.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     6224 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/util/image.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4645 2022-09-25 06:31:57.000000 shakenfist-0.6.9/shakenfist/util/libvirt.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     6420 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/util/network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1711 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/util/process.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      187 2022-11-06 04:42:35.000000 shakenfist-0.6.9/shakenfist/util/random.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.785979 shakenfist-0.6.9/shakenfist.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1132 2022-11-06 07:49:14.000000 shakenfist-0.6.9/shakenfist.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7554 2022-11-06 07:49:14.000000 shakenfist-0.6.9/shakenfist.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2022-11-06 07:49:14.000000 shakenfist-0.6.9/shakenfist.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      182 2022-11-06 07:49:14.000000 shakenfist-0.6.9/shakenfist.egg-info/entry_points.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2022-11-06 07:49:14.000000 shakenfist-0.6.9/shakenfist.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       47 2022-11-06 07:49:14.000000 shakenfist-0.6.9/shakenfist.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      711 2022-11-06 07:49:14.000000 shakenfist-0.6.9/shakenfist.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       11 2022-11-06 07:49:14.000000 shakenfist-0.6.9/shakenfist.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      102 2022-11-06 04:42:35.000000 shakenfist-0.6.9/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-11-06 07:49:14.806149 shakenfist-0.6.9/tools/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4017 2022-09-25 06:31:59.000000 shakenfist-0.6.9/tools/clone_with_depends.py
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      580 2021-09-25 23:09:33.000000 shakenfist-0.6.9/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      654 2022-09-25 06:31:57.000000 shakenfist-0.6.9/tools/network_allocation_torture.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      978 2022-11-06 04:42:37.000000 shakenfist-0.6.9/tox.ini
```

### Comparing `shakenfist-0.6.8/.github/workflows/codeql-analysis.yml` & `shakenfist-0.6.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/configure-tests.py` & `shakenfist-0.6.9/.github/workflows/configure-tests.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/functional-tests-debian-10-localhost.yml` & `shakenfist-0.6.9/.github/workflows/functional-tests-debian-10-localhost.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/functional-tests-debian-11-slim-primary.yml` & `shakenfist-0.6.9/.github/workflows/functional-tests-debian-11-slim-primary.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml` & `shakenfist-0.6.9/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/functional-tests.tmpl` & `shakenfist-0.6.9/.github/workflows/functional-tests.tmpl`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/nodelifecycle-tests.yml` & `shakenfist-0.6.9/.github/workflows/nodelifecycle-tests.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/publish-website.yml` & `shakenfist-0.6.9/.github/workflows/publish-website.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/python-unit-tests.yml` & `shakenfist-0.6.9/.github/workflows/python-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests-develop-debian-10-localhost.yml` & `shakenfist-0.6.9/.github/workflows/scheduled-tests-develop-debian-10-localhost.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests-develop-debian-11-slim-primary.yml` & `shakenfist-0.6.9/.github/workflows/scheduled-tests-develop-debian-11-slim-primary.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests-develop-ubuntu-2004-slim-primary.yml` & `shakenfist-0.6.9/.github/workflows/scheduled-tests-develop-ubuntu-2004-slim-primary.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-debian-10-localhost.yml` & `shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-debian-10-localhost.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-debian-11-slim-primary.yml` & `shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-debian-11-slim-primary.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-released-debian-10-localhost.yml` & `shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-released-debian-10-localhost.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-released-debian-11-slim-primary.yml` & `shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-released-debian-11-slim-primary.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-released-ubuntu-2004-slim-primary.yml` & `shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-released-ubuntu-2004-slim-primary.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests-v06-ubuntu-2004-slim-primary.yml` & `shakenfist-0.6.9/.github/workflows/scheduled-tests-v06-ubuntu-2004-slim-primary.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/.github/workflows/scheduled-tests.tmpl` & `shakenfist-0.6.9/.github/workflows/scheduled-tests.tmpl`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/BRANCHES.rst` & `shakenfist-0.6.9/BRANCHES.rst`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/LICENSE` & `shakenfist-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/PKG-INFO` & `shakenfist-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist
-Version: 0.6.8
+Version: 0.6.9
 Summary: Shaken Fist: an opinionated minimal cloud
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: # Shaken Fist: Opinionated to the point of being impolite
         ![Python application](https://github.com/shakenfist/shakenfist/workflows/Python%20application/badge.svg)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shakenfist Version: 0.6.8 Summary: Shaken Fist: an
+Metadata-Version: 2.1 Name: shakenfist Version: 0.6.9 Summary: Shaken Fist: an
 opinionated minimal cloud Home-page: https://madebymikal.com/shakenfist Author:
 Michael Still Author-email: mikal@stillhq.com License: Apache2 Description: #
 Shaken Fist: Opinionated to the point of being impolite ![Python application]
 (https://github.com/shakenfist/shakenfist/workflows/Python%20application/
 badge.svg) [Package_version] **Documentation:** https://shakenfist.com/
 **Source Code:** https://github.com/shakenfist/shakenfist Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology Classifier: Intended
```

### Comparing `shakenfist-0.6.8/deploy/ansible/ci-image.yml` & `shakenfist-0.6.9/deploy/ansible/ci-image.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/ci-include-common-localhost.yml` & `shakenfist-0.6.9/deploy/ansible/ci-include-common-localhost.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/ci-topology-localhost-released.yml` & `shakenfist-0.6.9/deploy/ansible/ci-topology-localhost-released.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/ci-topology-localhost.yml` & `shakenfist-0.6.9/deploy/ansible/ci-topology-localhost.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/ci-topology-slim-primary-released.yml` & `shakenfist-0.6.9/deploy/ansible/ci-topology-slim-primary-released.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/ci-topology-slim-primary.yml` & `shakenfist-0.6.9/deploy/ansible/ci-topology-slim-primary.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/deploy.py` & `shakenfist-0.6.9/deploy/ansible/deploy.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/deploy.yml` & `shakenfist-0.6.9/deploy/ansible/deploy.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/files/config` & `shakenfist-0.6.9/deploy/ansible/files/config`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/files/dhcp.tmpl` & `shakenfist-0.6.9/deploy/ansible/files/dhcp.tmpl`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/files/etcd.conf` & `shakenfist-0.6.9/deploy/ansible/files/etcd.conf`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/files/grafana/grafana.ini` & `shakenfist-0.6.9/deploy/ansible/files/grafana/grafana.ini`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/files/grafana/ldap.toml` & `shakenfist-0.6.9/deploy/ansible/files/grafana/ldap.toml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/files/grafana/provisioning/dashboards/shakenfist.json` & `shakenfist-0.6.9/deploy/ansible/files/grafana/provisioning/dashboards/shakenfist.json`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/files/libvirt.tmpl` & `shakenfist-0.6.9/deploy/ansible/files/libvirt.tmpl`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/includes/topology_add_node.yml` & `shakenfist-0.6.9/deploy/ansible/includes/topology_add_node.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/ansible/tasks/build-wheel.yml` & `shakenfist-0.6.9/deploy/ansible/tasks/build-wheel.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/getsf` & `shakenfist-0.6.9/deploy/getsf`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/nodelifecycletests.sh` & `shakenfist-0.6.9/deploy/nodelifecycletests.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/setup.cfg` & `shakenfist-0.6.9/deploy/setup.cfg`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/setup.py` & `shakenfist-0.6.9/deploy/setup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/base.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/base.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_artifacts.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_auth.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_boot.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_boot.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_cloudinit.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_cloudinit.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_commandline_artifacts.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_commandline_artifacts.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_commandline_network.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_commandline_network.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_console_log.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_console_log.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_disk_specs.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_disk_specs.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_disks.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_disks.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_floating_ips.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_floating_ips.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_metadata.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_multiple_nics.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_multiple_nics.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_namespace.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_networking.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_networking.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_object_names.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_object_names.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_placement.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_placement.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_serial_console.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_serial_console.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_snapshots.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_state_changes.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_state_changes.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_system_namespace.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_system_namespace.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_ubuntu.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_ubuntu.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/shakenfist_ci/tests/test_upgrades.py` & `shakenfist-0.6.9/deploy/shakenfist_ci/tests/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy/tox.ini` & `shakenfist-0.6.9/deploy/tox.ini`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/deploy.tgz` & `shakenfist-0.6.9/deploy.tgz`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/changelog/changelog_v02.md` & `shakenfist-0.6.9/docs/changelog/changelog_v02.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/changelog/changelog_v03.md` & `shakenfist-0.6.9/docs/changelog/changelog_v03.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/changelog/changelog_v04.md` & `shakenfist-0.6.9/docs/changelog/changelog_v04.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/community.md` & `shakenfist-0.6.9/docs/community.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/development/ci_api_coverage.md` & `shakenfist-0.6.9/docs/development/ci_api_coverage.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/development/git_usage.md` & `shakenfist-0.6.9/docs/development/git_usage.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/development/io_performance_tuning.md` & `shakenfist-0.6.9/docs/development/io_performance_tuning.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/development/namespace_auth.md` & `shakenfist-0.6.9/docs/development/namespace_auth.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/development/release_process.md` & `shakenfist-0.6.9/docs/development/release_process.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/development/standards.md` & `shakenfist-0.6.9/docs/development/standards.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/development/state_machine.md` & `shakenfist-0.6.9/docs/development/state_machine.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/development/updating_docs.md` & `shakenfist-0.6.9/docs/development/updating_docs.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/features.md` & `shakenfist-0.6.9/docs/features.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/index.md` & `shakenfist-0.6.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/installation.md` & `shakenfist-0.6.9/docs/installation.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/manifesto.md` & `shakenfist-0.6.9/docs/manifesto.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/networking/overview.md` & `shakenfist-0.6.9/docs/networking/overview.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/networking/single_instance.md` & `shakenfist-0.6.9/docs/networking/single_instance.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/power_states.md` & `shakenfist-0.6.9/docs/power_states.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs/usage.md` & `shakenfist-0.6.9/docs/usage.md`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/docs.tgz` & `shakenfist-0.6.9/docs.tgz`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/examples/configdrive-sample-ocata-plain.tgz` & `shakenfist-0.6.9/examples/configdrive-sample-ocata-plain.tgz`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/examples/schema-v0_3_3.tgz` & `shakenfist-0.6.9/examples/schema-v0_3_3.tgz`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/mkdocs.yml` & `shakenfist-0.6.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/network-example.dia` & `shakenfist-0.6.9/network-example.dia`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/network-example.png` & `shakenfist-0.6.9/network-example.png`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/release.sh` & `shakenfist-0.6.9/release.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/requirements.txt` & `shakenfist-0.6.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/setup.cfg` & `shakenfist-0.6.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/setup.py` & `shakenfist-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/artifact.py` & `shakenfist-0.6.9/shakenfist/artifact.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/baseobject.py` & `shakenfist-0.6.9/shakenfist/baseobject.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/baseobjectmapping.py` & `shakenfist-0.6.9/shakenfist/baseobjectmapping.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/blob.py` & `shakenfist-0.6.9/shakenfist/blob.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/client/backup.py` & `shakenfist-0.6.9/shakenfist/client/backup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/client/ctl.py` & `shakenfist-0.6.9/shakenfist/client/ctl.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/config.py` & `shakenfist-0.6.9/shakenfist/config.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/constants.py` & `shakenfist-0.6.9/shakenfist/constants.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/cleaner.py` & `shakenfist-0.6.9/shakenfist/daemons/cleaner.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/cluster.py` & `shakenfist-0.6.9/shakenfist/daemons/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                     blob_uuid = blob_index['blob_uuid']
                     b = Blob.from_db(blob_uuid)
                     if b:
                         # NOTE(mikal): I've decided not to include blob replication
                         # cost in this number, as that is a decision the cluster
                         # deployer machines (its a config option), not a decision
                         # the owner of the blob makes.
-                        total_used_storage += b.size
+                        total_used_storage += int(b.size)
 
                 a.add_event2('usage', extra={'bytes': total_used_storage},
                              suppress_event_logging=True)
 
             return True
 
         return False
```

### Comparing `shakenfist-0.6.8/shakenfist/daemons/daemon.py` & `shakenfist-0.6.9/shakenfist/daemons/daemon.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/eventlog.py` & `shakenfist-0.6.9/shakenfist/daemons/eventlog.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/external_api.py` & `shakenfist-0.6.9/shakenfist/daemons/external_api.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/main.py` & `shakenfist-0.6.9/shakenfist/daemons/main.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/net.py` & `shakenfist-0.6.9/shakenfist/daemons/net.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/queues.py` & `shakenfist-0.6.9/shakenfist/daemons/queues.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/resources.py` & `shakenfist-0.6.9/shakenfist/daemons/resources.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/shim.py` & `shakenfist-0.6.9/shakenfist/daemons/shim.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/daemons/sidechannel.py` & `shakenfist-0.6.9/shakenfist/daemons/sidechannel.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/db.py` & `shakenfist-0.6.9/shakenfist/db.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/dhcp.py` & `shakenfist-0.6.9/shakenfist/dhcp.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/etcd.py` & `shakenfist-0.6.9/shakenfist/etcd.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/eventlog.py` & `shakenfist-0.6.9/shakenfist/eventlog.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/exceptions.py` & `shakenfist-0.6.9/shakenfist/exceptions.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/app.py` & `shakenfist-0.6.9/shakenfist/external_api/app.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/artifact.py` & `shakenfist-0.6.9/shakenfist/external_api/artifact.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/auth.py` & `shakenfist-0.6.9/shakenfist/external_api/auth.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/base.py` & `shakenfist-0.6.9/shakenfist/external_api/base.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/blob.py` & `shakenfist-0.6.9/shakenfist/external_api/blob.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/instance.py` & `shakenfist-0.6.9/shakenfist/external_api/instance.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/interface.py` & `shakenfist-0.6.9/shakenfist/external_api/interface.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/label.py` & `shakenfist-0.6.9/shakenfist/external_api/label.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/network.py` & `shakenfist-0.6.9/shakenfist/external_api/network.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/node.py` & `shakenfist-0.6.9/shakenfist/external_api/node.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/snapshot.py` & `shakenfist-0.6.9/shakenfist/external_api/snapshot.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/upload.py` & `shakenfist-0.6.9/shakenfist/external_api/upload.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/external_api/util.py` & `shakenfist-0.6.9/shakenfist/external_api/util.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/images.py` & `shakenfist-0.6.9/shakenfist/images.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/instance.py` & `shakenfist-0.6.9/shakenfist/instance.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/ipmanager.py` & `shakenfist-0.6.9/shakenfist/ipmanager.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/logutil.py` & `shakenfist-0.6.9/shakenfist/logutil.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/metrics.py` & `shakenfist-0.6.9/shakenfist/metrics.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/network.py` & `shakenfist-0.6.9/shakenfist/network.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/networkinterface.py` & `shakenfist-0.6.9/shakenfist/networkinterface.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/node.py` & `shakenfist-0.6.9/shakenfist/node.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/scheduler.py` & `shakenfist-0.6.9/shakenfist/scheduler.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tasks.py` & `shakenfist-0.6.9/shakenfist/tasks.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/base.py` & `shakenfist-0.6.9/shakenfist/tests/base.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/external_api/test_auth.py` & `shakenfist-0.6.9/shakenfist/tests/external_api/test_auth.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/external_api/test_network.py` & `shakenfist-0.6.9/shakenfist/tests/external_api/test_network.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/files/cirros-MD5SUMS-0.3.4` & `shakenfist-0.6.9/shakenfist/tests/files/cirros-MD5SUMS-0.3.4`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/files/cirros-download` & `shakenfist-0.6.9/shakenfist/tests/files/cirros-download`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/files/dhcp.tmpl` & `shakenfist-0.6.9/shakenfist/tests/files/dhcp.tmpl`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/files/ubuntu-MD5SUMS-bionic` & `shakenfist-0.6.9/shakenfist/tests/files/ubuntu-MD5SUMS-bionic`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/files/ubuntu-MD5SUMS-groovy` & `shakenfist-0.6.9/shakenfist/tests/files/ubuntu-MD5SUMS-groovy`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/files/ubuntu-download` & `shakenfist-0.6.9/shakenfist/tests/files/ubuntu-download`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/mock_etcd.py` & `shakenfist-0.6.9/shakenfist/tests/mock_etcd.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_baseobject.py` & `shakenfist-0.6.9/shakenfist/tests/test_baseobject.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_config.py` & `shakenfist-0.6.9/shakenfist/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_daemon_cleaner.py` & `shakenfist-0.6.9/shakenfist/tests/test_daemon_cleaner.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_dhcp.py` & `shakenfist-0.6.9/shakenfist/tests/test_dhcp.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_etcd.py` & `shakenfist-0.6.9/shakenfist/tests/test_etcd.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_external_api.py` & `shakenfist-0.6.9/shakenfist/tests/test_external_api.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_instance.py` & `shakenfist-0.6.9/shakenfist/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_ipmanager.py` & `shakenfist-0.6.9/shakenfist/tests/test_ipmanager.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_net.py` & `shakenfist-0.6.9/shakenfist/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_networkinterface.py` & `shakenfist-0.6.9/shakenfist/tests/test_networkinterface.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_scheduler.py` & `shakenfist-0.6.9/shakenfist/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_tasks.py` & `shakenfist-0.6.9/shakenfist/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_util_general.py` & `shakenfist-0.6.9/shakenfist/tests/test_util_general.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/tests/test_util_network.py` & `shakenfist-0.6.9/shakenfist/tests/test_util_network.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/upload.py` & `shakenfist-0.6.9/shakenfist/upload.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/util/general.py` & `shakenfist-0.6.9/shakenfist/util/general.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/util/image.py` & `shakenfist-0.6.9/shakenfist/util/image.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/util/libvirt.py` & `shakenfist-0.6.9/shakenfist/util/libvirt.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/util/network.py` & `shakenfist-0.6.9/shakenfist/util/network.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist/util/process.py` & `shakenfist-0.6.9/shakenfist/util/process.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist.egg-info/PKG-INFO` & `shakenfist-0.6.9/shakenfist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist
-Version: 0.6.8
+Version: 0.6.9
 Summary: Shaken Fist: an opinionated minimal cloud
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: # Shaken Fist: Opinionated to the point of being impolite
         ![Python application](https://github.com/shakenfist/shakenfist/workflows/Python%20application/badge.svg)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shakenfist Version: 0.6.8 Summary: Shaken Fist: an
+Metadata-Version: 2.1 Name: shakenfist Version: 0.6.9 Summary: Shaken Fist: an
 opinionated minimal cloud Home-page: https://madebymikal.com/shakenfist Author:
 Michael Still Author-email: mikal@stillhq.com License: Apache2 Description: #
 Shaken Fist: Opinionated to the point of being impolite ![Python application]
 (https://github.com/shakenfist/shakenfist/workflows/Python%20application/
 badge.svg) [Package_version] **Documentation:** https://shakenfist.com/
 **Source Code:** https://github.com/shakenfist/shakenfist Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology Classifier: Intended
```

### Comparing `shakenfist-0.6.8/shakenfist.egg-info/SOURCES.txt` & `shakenfist-0.6.9/shakenfist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/shakenfist.egg-info/requires.txt` & `shakenfist-0.6.9/shakenfist.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/tools/clone_with_depends.py` & `shakenfist-0.6.9/tools/clone_with_depends.py`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/tools/flake8wrap.sh` & `shakenfist-0.6.9/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/tools/network_allocation_torture.sh` & `shakenfist-0.6.9/tools/network_allocation_torture.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-0.6.8/tox.ini` & `shakenfist-0.6.9/tox.ini`

 * *Files identical despite different names*

