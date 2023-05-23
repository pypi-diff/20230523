# Comparing `tmp/enos-8.0.0a4.tar.gz` & `tmp/enos-8.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enos-8.0.0a4.tar", max compression
+gzip compressed data, was "enos-8.0.0a5.tar", max compression
```

## Comparing `enos-8.0.0a4.tar` & `enos-8.0.0a5.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    35148 2022-10-20 13:50:57.843485 enos-8.0.0a4/LICENSE
--rw-r--r--   0        0        0     3270 2023-04-25 13:33:13.806401 enos-8.0.0a4/README.rst
--rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/__init__.py
--rw-r--r--   0        0        0      529 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/enos.yml
--rw-r--r--   0        0        0      372 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/group_vars/all.yml
--rw-r--r--   0        0        0      378 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/init_os.yml
--rw-r--r--   0        0        0     4979 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/plugins/callback/influxdb_events.py
--rw-r--r--   0        0        0       44 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/defaults/main.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/backup.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/bench.yml
--rw-r--r--   0        0        0     1417 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/deploy.yml
--rw-r--r--   0        0        0      311 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/main.yml
--rw-r--r--   0        0        0      116 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/pull.yml
--rw-r--r--   0        0        0      280 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/defaults/main.yml
--rw-r--r--   0        0        0    23358 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/collectd.conf
--rw-r--r--   0        0        0       25 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/contextswitch.conf
--rw-r--r--   0        0        0      359 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/haproxy.conf
--rw-r--r--   0        0        0     9676 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/haproxy.py
--rw-r--r--   0        0        0      156 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/protocols.conf
--rw-r--r--   0        0        0      119 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-compute.conf
--rw-r--r--   0        0        0      353 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-haproxy.conf
--rw-r--r--   0        0        0      249 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-keystone.conf
--rw-r--r--   0        0        0       69 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-mariadb.conf
--rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-memcached.conf
--rw-r--r--   0        0        0      211 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-network.conf
--rw-r--r--   0        0        0      216 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-nova.conf
--rw-r--r--   0        0        0      128 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/files/tcpconns-rabbitmq.conf
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/backup.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/bench.yml
--rw-r--r--   0        0        0     1881 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/deploy.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/main.yml
--rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/tasks/pull.yml
--rw-r--r--   0        0        0      114 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/templates/influx.conf.j2
--rw-r--r--   0        0        0      386 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/templates/memcached.conf.j2
--rw-r--r--   0        0        0      455 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/templates/mysql.conf.j2
--rw-r--r--   0        0        0     1081 2022-11-07 08:45:07.825216 enos-8.0.0a4/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2
--rw-r--r--   0        0        0       42 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/defaults/main.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/backup.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/bench.yml
--rw-r--r--   0        0        0     1646 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/deploy.yml
--rw-r--r--   0        0        0      120 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/main.yml
--rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/grafana/tasks/pull.yml
--rw-r--r--   0        0        0       36 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/defaults/main.yml
--rw-r--r--   0        0        0    10241 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/files/config.toml
--rw-r--r--   0        0        0     9721 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/files/types.db
--rw-r--r--   0        0        0      357 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/backup.yml
--rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/bench.yml
--rw-r--r--   0        0        0     1582 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/deploy.yml
--rw-r--r--   0        0        0      207 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/destroy.yml
--rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/main.yml
--rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/influx/tasks/pull.yml
--rw-r--r--   0        0        0     1112 2023-04-25 13:33:13.806401 enos-8.0.0a4/enos/ansible/roles/init_os/tasks/deploy.yml
--rw-r--r--   0        0        0       40 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/init_os/tasks/main.yml
--rw-r--r--   0        0        0      493 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/ansible/roles/init_os/tasks/pull.yml
--rw-r--r--   0        0        0     3391 2023-05-15 13:45:52.493838 enos-8.0.0a4/enos/ansible/roles/init_os/templates/init.sh.j2
--rwxr-xr-x   0        0        0    25920 2023-05-09 14:37:44.792871 enos-8.0.0a4/enos/cli.py
--rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/__init__.py
--rw-r--r--   0        0        0     1815 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/chameleonbaremetal.py
--rw-r--r--   0        0        0     1293 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/chameleonkvm.py
--rw-r--r--   0        0        0     2417 2023-04-25 13:33:13.806401 enos-8.0.0a4/enos/provider/enos_vagrant.py
--rw-r--r--   0        0        0     5813 2023-04-25 13:33:13.806401 enos-8.0.0a4/enos/provider/g5k.py
--rw-r--r--   0        0        0      818 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/host.py
--rw-r--r--   0        0        0     2963 2023-04-25 13:33:13.806401 enos-8.0.0a4/enos/provider/openstack.py
--rw-r--r--   0        0        0     1636 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/provider.py
--rw-r--r--   0        0        0     2786 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/provider/static.py
--rw-r--r--   0        0        0     2757 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/provider/vmong5k.py
--rw-r--r--   0        0        0     9471 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/resources/inventory.sample
--rw-r--r--   0        0        0     9666 2022-11-08 12:27:03.004104 enos-8.0.0a4/enos/resources/multinode
--rw-r--r--   0        0        0    21559 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/resources/passwords.yml
--rw-r--r--   0        0        0      513 2022-11-07 08:45:34.949389 enos-8.0.0a4/enos/resources/workload/create-and-update-image.yaml
--rw-r--r--   0        0        0     1069 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/resources/workload/nova-boot-list-cc.yml
--rw-r--r--   0        0        0      715 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/resources/workload/run.yml
--rw-r--r--   0        0        0      189 2022-11-07 08:45:07.829217 enos-8.0.0a4/enos/services/__init__.py
--rw-r--r--   0        0        0    15121 2023-05-15 13:29:39.549786 enos-8.0.0a4/enos/services/kolla.py
--rw-r--r--   0        0        0     8376 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/services/rally.py
--rw-r--r--   0        0        0     3720 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/services/shaker.py
--rwxr-xr-x   0        0        0    11791 2022-11-07 10:41:09.316608 enos-8.0.0a4/enos/tasks/__init__.py
--rw-r--r--   0        0        0     5701 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/tasks/new.py
--rw-r--r--   0        0        0    12229 2023-05-15 13:29:39.549786 enos-8.0.0a4/enos/tasks/up.py
--rw-r--r--   0        0        0      911 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/templates/Vagrantfile.j2
--rw-r--r--   0        0        0    10240 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/templates/grafana_dashboard.json
--rw-r--r--   0        0        0     2049 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/templates/reservation.yaml.j2
--rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/utils/__init__.py
--rw-r--r--   0        0        0     3229 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/utils/build.py
--rw-r--r--   0        0        0     3285 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/utils/cli.py
--rw-r--r--   0        0        0     1932 2023-05-15 13:59:51.434142 enos-8.0.0a4/enos/utils/constants.py
--rw-r--r--   0        0        0     1009 2022-11-07 08:45:07.833218 enos-8.0.0a4/enos/utils/errors.py
--rw-r--r--   0        0        0     6257 2023-04-25 13:33:13.810401 enos-8.0.0a4/enos/utils/extra.py
--rw-r--r--   0        0        0     1907 2023-05-15 14:00:01.978094 enos-8.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 enos-8.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-10-20 13:50:57.843485 enos-8.0.0a5/LICENSE
+-rw-r--r--   0        0        0     3270 2023-04-25 13:33:13.806401 enos-8.0.0a5/README.rst
+-rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/__init__.py
+-rw-r--r--   0        0        0      529 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/enos.yml
+-rw-r--r--   0        0        0      372 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/group_vars/all.yml
+-rw-r--r--   0        0        0      378 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/init_os.yml
+-rw-r--r--   0        0        0     4979 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/plugins/callback/influxdb_events.py
+-rw-r--r--   0        0        0       44 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/cadvisor/defaults/main.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/cadvisor/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/cadvisor/tasks/bench.yml
+-rw-r--r--   0        0        0     1417 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/cadvisor/tasks/deploy.yml
+-rw-r--r--   0        0        0      311 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/cadvisor/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/cadvisor/tasks/main.yml
+-rw-r--r--   0        0        0      116 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/cadvisor/tasks/pull.yml
+-rw-r--r--   0        0        0      280 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/defaults/main.yml
+-rw-r--r--   0        0        0    23358 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/files/collectd.conf
+-rw-r--r--   0        0        0       25 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/collectd/files/contextswitch.conf
+-rw-r--r--   0        0        0      359 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/collectd/files/haproxy.conf
+-rw-r--r--   0        0        0     9676 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/files/haproxy.py
+-rw-r--r--   0        0        0      156 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/collectd/files/protocols.conf
+-rw-r--r--   0        0        0      119 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/collectd/files/tcpconns-compute.conf
+-rw-r--r--   0        0        0      353 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/collectd/files/tcpconns-haproxy.conf
+-rw-r--r--   0        0        0      249 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/collectd/files/tcpconns-keystone.conf
+-rw-r--r--   0        0        0       69 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/files/tcpconns-mariadb.conf
+-rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/files/tcpconns-memcached.conf
+-rw-r--r--   0        0        0      211 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/collectd/files/tcpconns-network.conf
+-rw-r--r--   0        0        0      216 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/collectd/files/tcpconns-nova.conf
+-rw-r--r--   0        0        0      128 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/files/tcpconns-rabbitmq.conf
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/tasks/bench.yml
+-rw-r--r--   0        0        0     1881 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/tasks/deploy.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/tasks/main.yml
+-rw-r--r--   0        0        0       70 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/tasks/pull.yml
+-rw-r--r--   0        0        0      114 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/templates/influx.conf.j2
+-rw-r--r--   0        0        0      386 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/templates/memcached.conf.j2
+-rw-r--r--   0        0        0      455 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/templates/mysql.conf.j2
+-rw-r--r--   0        0        0     1081 2022-11-07 08:45:07.825216 enos-8.0.0a5/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2
+-rw-r--r--   0        0        0       42 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/grafana/defaults/main.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/grafana/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/grafana/tasks/bench.yml
+-rw-r--r--   0        0        0     1646 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/grafana/tasks/deploy.yml
+-rw-r--r--   0        0        0      120 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/grafana/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/grafana/tasks/main.yml
+-rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/grafana/tasks/pull.yml
+-rw-r--r--   0        0        0       36 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/influx/defaults/main.yml
+-rw-r--r--   0        0        0    10241 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/influx/files/config.toml
+-rw-r--r--   0        0        0     9721 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/influx/files/types.db
+-rw-r--r--   0        0        0      357 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/influx/tasks/backup.yml
+-rw-r--r--   0        0        0        4 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/influx/tasks/bench.yml
+-rw-r--r--   0        0        0     1582 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/influx/tasks/deploy.yml
+-rw-r--r--   0        0        0      207 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/influx/tasks/destroy.yml
+-rw-r--r--   0        0        0       39 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/influx/tasks/main.yml
+-rw-r--r--   0        0        0      113 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/influx/tasks/pull.yml
+-rw-r--r--   0        0        0     1112 2023-04-25 13:33:13.806401 enos-8.0.0a5/enos/ansible/roles/init_os/tasks/deploy.yml
+-rw-r--r--   0        0        0       40 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/init_os/tasks/main.yml
+-rw-r--r--   0        0        0      493 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/ansible/roles/init_os/tasks/pull.yml
+-rw-r--r--   0        0        0     3391 2023-05-15 13:45:52.493838 enos-8.0.0a5/enos/ansible/roles/init_os/templates/init.sh.j2
+-rwxr-xr-x   0        0        0    25866 2023-05-23 16:45:13.891880 enos-8.0.0a5/enos/cli.py
+-rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/provider/__init__.py
+-rw-r--r--   0        0        0     1815 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/provider/chameleonbaremetal.py
+-rw-r--r--   0        0        0     1293 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/provider/chameleonkvm.py
+-rw-r--r--   0        0        0     2417 2023-04-25 13:33:13.806401 enos-8.0.0a5/enos/provider/enos_vagrant.py
+-rw-r--r--   0        0        0     5813 2023-04-25 13:33:13.806401 enos-8.0.0a5/enos/provider/g5k.py
+-rw-r--r--   0        0        0      818 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/provider/host.py
+-rw-r--r--   0        0        0     2963 2023-04-25 13:33:13.806401 enos-8.0.0a5/enos/provider/openstack.py
+-rw-r--r--   0        0        0     1636 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/provider/provider.py
+-rw-r--r--   0        0        0     2786 2023-04-25 13:33:13.810401 enos-8.0.0a5/enos/provider/static.py
+-rw-r--r--   0        0        0     2757 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/provider/vmong5k.py
+-rw-r--r--   0        0        0     9471 2023-05-23 16:20:12.336561 enos-8.0.0a5/enos/resources/inventory.sample
+-rw-r--r--   0        0        0     9666 2022-11-08 12:27:03.004104 enos-8.0.0a5/enos/resources/multinode
+-rw-r--r--   0        0        0    21559 2023-04-25 13:33:13.810401 enos-8.0.0a5/enos/resources/passwords.yml
+-rw-r--r--   0        0        0      513 2022-11-07 08:45:34.949389 enos-8.0.0a5/enos/resources/workload/create-and-update-image.yaml
+-rw-r--r--   0        0        0     1069 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/resources/workload/nova-boot-list-cc.yml
+-rw-r--r--   0        0        0      715 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/resources/workload/run.yml
+-rw-r--r--   0        0        0      189 2022-11-07 08:45:07.829217 enos-8.0.0a5/enos/services/__init__.py
+-rw-r--r--   0        0        0    15121 2023-05-15 13:29:39.549786 enos-8.0.0a5/enos/services/kolla.py
+-rw-r--r--   0        0        0     8386 2023-05-23 16:45:13.891880 enos-8.0.0a5/enos/services/rally.py
+-rw-r--r--   0        0        0     3702 2023-05-23 16:45:13.891880 enos-8.0.0a5/enos/services/shaker.py
+-rwxr-xr-x   0        0        0    11791 2023-05-23 16:20:12.336561 enos-8.0.0a5/enos/tasks/__init__.py
+-rw-r--r--   0        0        0     5701 2023-04-25 13:33:13.810401 enos-8.0.0a5/enos/tasks/new.py
+-rw-r--r--   0        0        0    12229 2023-05-15 13:29:39.549786 enos-8.0.0a5/enos/tasks/up.py
+-rw-r--r--   0        0        0      911 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/templates/Vagrantfile.j2
+-rw-r--r--   0        0        0    10240 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/templates/grafana_dashboard.json
+-rw-r--r--   0        0        0     2049 2023-04-25 13:33:13.810401 enos-8.0.0a5/enos/templates/reservation.yaml.j2
+-rw-r--r--   0        0        0        0 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/utils/__init__.py
+-rw-r--r--   0        0        0     3229 2023-04-25 13:33:13.810401 enos-8.0.0a5/enos/utils/build.py
+-rw-r--r--   0        0        0     3285 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/utils/cli.py
+-rw-r--r--   0        0        0     1932 2023-05-23 16:45:52.319659 enos-8.0.0a5/enos/utils/constants.py
+-rw-r--r--   0        0        0     1009 2022-11-07 08:45:07.833218 enos-8.0.0a5/enos/utils/errors.py
+-rw-r--r--   0        0        0     6257 2023-04-25 13:33:13.810401 enos-8.0.0a5/enos/utils/extra.py
+-rw-r--r--   0        0        0     1907 2023-05-23 16:45:59.011683 enos-8.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 enos-8.0.0a5/PKG-INFO
```

### Comparing `enos-8.0.0a4/LICENSE` & `enos-8.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/README.rst` & `enos-8.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/enos.yml` & `enos-8.0.0a5/enos/ansible/enos.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/plugins/callback/influxdb_events.py` & `enos-8.0.0a5/enos/ansible/plugins/callback/influxdb_events.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/cadvisor/tasks/deploy.yml` & `enos-8.0.0a5/enos/ansible/roles/cadvisor/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/collectd/files/collectd.conf` & `enos-8.0.0a5/enos/ansible/roles/collectd/files/collectd.conf`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/collectd/files/haproxy.py` & `enos-8.0.0a5/enos/ansible/roles/collectd/files/haproxy.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/collectd/tasks/deploy.yml` & `enos-8.0.0a5/enos/ansible/roles/collectd/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2` & `enos-8.0.0a5/enos/ansible/roles/collectd/templates/rabbitmq.conf.j2`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/grafana/tasks/deploy.yml` & `enos-8.0.0a5/enos/ansible/roles/grafana/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/influx/files/config.toml` & `enos-8.0.0a5/enos/ansible/roles/influx/files/config.toml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/influx/files/types.db` & `enos-8.0.0a5/enos/ansible/roles/influx/files/types.db`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/influx/tasks/deploy.yml` & `enos-8.0.0a5/enos/ansible/roles/influx/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/init_os/tasks/deploy.yml` & `enos-8.0.0a5/enos/ansible/roles/init_os/tasks/deploy.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/ansible/roles/init_os/templates/init.sh.j2` & `enos-8.0.0a5/enos/ansible/roles/init_os/templates/init.sh.j2`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/cli.py` & `enos-8.0.0a5/enos/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,26 +305,24 @@
     except MissingEnvState as err:
         if err.key in ['kolla-ansible', 'inventory', 'networks']:
             CLI.error(f"""\
             {err.key} could not be found in your enos environment.  Did you
             successfully run `enos up` and `enos os` first?""")
         else:
             CLI.critical(err)
+            raise err
         sys.exit(1)
     except yaml.YAMLError as err:
         error_loc = ""
         if hasattr(err, 'problem_mark'):
             loc = getattr(err, 'problem_mark')
             error_loc = f"at {loc.line+1}:{loc.column+1}"
         CLI.error(f'Syntax error in the file "{workload / "run.yam"}" '
                   + error_loc)
         sys.exit(1)
-    except Exception as e:
-        CLI.critical(str(e))
-        sys.exit(1)
 
 
 def backup(**kwargs):
     """\
     USAGE:
       enos backup [--backup_dir=BACKUP_DIR] [-e ENV]
```

### Comparing `enos-8.0.0a4/enos/provider/chameleonbaremetal.py` & `enos-8.0.0a5/enos/provider/chameleonbaremetal.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/provider/chameleonkvm.py` & `enos-8.0.0a5/enos/provider/chameleonkvm.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/provider/enos_vagrant.py` & `enos-8.0.0a5/enos/provider/enos_vagrant.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/provider/g5k.py` & `enos-8.0.0a5/enos/provider/g5k.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/provider/host.py` & `enos-8.0.0a5/enos/provider/host.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/provider/openstack.py` & `enos-8.0.0a5/enos/provider/openstack.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/provider/provider.py` & `enos-8.0.0a5/enos/provider/provider.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/provider/static.py` & `enos-8.0.0a5/enos/provider/static.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/provider/vmong5k.py` & `enos-8.0.0a5/enos/provider/vmong5k.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/resources/inventory.sample` & `enos-8.0.0a5/enos/resources/inventory.sample`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/resources/multinode` & `enos-8.0.0a5/enos/resources/multinode`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/resources/passwords.yml` & `enos-8.0.0a5/enos/resources/passwords.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/resources/workload/create-and-update-image.yaml` & `enos-8.0.0a5/enos/resources/workload/create-and-update-image.yaml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/resources/workload/nova-boot-list-cc.yml` & `enos-8.0.0a5/enos/resources/workload/nova-boot-list-cc.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/resources/workload/run.yml` & `enos-8.0.0a5/enos/resources/workload/run.yml`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/services/kolla.py` & `enos-8.0.0a5/enos/services/kolla.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/services/rally.py` & `enos-8.0.0a5/enos/services/rally.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,25 +34,26 @@
         Args:
           agents: The list of agents to deploy Rally OpenStack on.
           environment_name: Name of this rally environment.
 
         Reference:
           https://github.com/openstack/rally-openstack
         """
-        self.rsc = {'all': agents}
+        self.rsc = agents
         self.env_name = environment_name
+        self._tasks = []
 
         RallyOpenStack.pull(agents)
 
     @staticmethod
     def pull(agents: List[elib.Host]):
         'Installs Rally OpenStack'
         logging.info("Pull: installing rally in a virtual environment")
 
-        with elib.play_on(roles={'all': agents},
+        with elib.play_on(roles=agents,
                           priors=[elib.api.__python3__],
                           gather_facts=False) as yaml:
             yaml.pip(**title(f'install virtualenv {VENV}'), name='virtualenv')
 
             # XXX: https://cryptography.io/en/3.4.7/installation.html#rust
             yaml.pip(**title('upgrade pip for cryptography dependency'),
                      name='pip',
@@ -60,15 +61,15 @@
                      virtualenv=VENV,
                      virtualenv_python='python3')
 
             # XXX: We fix the version of decorator because of a bug when doing
             # `rally task ...`. See
             # https://bugs.launchpad.net/rally/+bug/1922707
             yaml.pip(**title(f'install {PKG} in {VENV}'),
-                     name=[PKG, 'decorator==4.4.2'],
+                     name=[PKG, 'decorator==4.4.2', 'sqlalchemy<2'],
                      state='present',
                      virtualenv=VENV)
 
     def deploy(self, openstack_auth: Dict[str, str], reset=False):
         'Deploying a Rally environment'
         logging.info(f"Deploy: Rally environment {self.env_name}")
 
@@ -140,22 +141,22 @@
                  + f' --tag="{_tag}"'
                  + f' --deployment="{self.env_name}"'),
                 ignore_errors=True,
                 **title(f'execute {scenario_name} (may take a while...)'))
 
         # Get the uuid and mark the scenario done in the tasks tracker
         uuid_by_hosts = {
-            host: values['stdout']
-            for host, values
+            result.host: result.payload['stdout']
+            for result
             in elib.run_command(
                 f'{VENV}/bin/rally task list --uuids-only'
                 f'  --deployment="{self.env_name}"'
                 f'  --tag {_tag}',
                 roles=self.rsc,
-                pattern_hosts=pattern_hosts).get('ok', {}).items()}
+                pattern_hosts=pattern_hosts)}
 
         logging.info(f"Scenario finished with uuid {uuid_by_hosts}")
         self._tasks.append((scenario_name, uuid_by_hosts))
 
     def backup(self, destination: Path, pattern_hosts: str = "all"):
         'Generates json/html reports and backup them'
         logging.info(f"Backup Rally reports for tasks {self._tasks}")
```

### Comparing `enos-8.0.0a4/enos/services/shaker.py` & `enos-8.0.0a5/enos/services/shaker.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 
         Args:
           agents: The list of agents to deploy Shaker OpenStack on.
 
         Reference:
           https://opendev.org/performa/shaker
         """
-        self.rsc = {'all': agents}
+        self.rsc = agents
         self.home = "~/shaker_home_" + str(uuid.uuid4())
         Shaker.pull(agents)
 
     @staticmethod
     def pull(agents: List[elib.Host]):
         'Pulling the docker image of Shaker '
         logging.info("Pull: get docker image for Shaker")
 
-        with elib.play_on(roles={'all': agents},
+        with elib.play_on(roles=agents,
                           gather_facts=False) as yaml:
             yaml.docker_image(
                 **title(f'pulling docker image {IMG}'),
                 name=IMG, source='pull', state='present')
 
     def deploy(self, openstack_auth: Dict[str, str], reset=False):
         'Deploying a Shaker environment'
```

### Comparing `enos-8.0.0a4/enos/tasks/__init__.py` & `enos-8.0.0a5/enos/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/tasks/new.py` & `enos-8.0.0a5/enos/tasks/new.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/tasks/up.py` & `enos-8.0.0a5/enos/tasks/up.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/templates/Vagrantfile.j2` & `enos-8.0.0a5/enos/templates/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/templates/grafana_dashboard.json` & `enos-8.0.0a5/enos/templates/grafana_dashboard.json`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/templates/reservation.yaml.j2` & `enos-8.0.0a5/enos/templates/reservation.yaml.j2`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/utils/build.py` & `enos-8.0.0a5/enos/utils/build.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/utils/cli.py` & `enos-8.0.0a5/enos/utils/cli.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/utils/constants.py` & `enos-8.0.0a5/enos/utils/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 # fake interface a give it the neutron_external_interface role
 NEUTRON_EXTERNAL_INTERFACE = 'neutron_external_interface'
 
 # In case we need to create a fake interface, this will be the nic name.
 FAKE_NEUTRON_EXTERNAL_INTERFACE = 'nei'
 
 # ENOS Setup
-VERSION = '8.0.0a4'
+VERSION = '8.0.0a5'
```

### Comparing `enos-8.0.0a4/enos/utils/errors.py` & `enos-8.0.0a5/enos/utils/errors.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/enos/utils/extra.py` & `enos-8.0.0a5/enos/utils/extra.py`

 * *Files identical despite different names*

### Comparing `enos-8.0.0a4/pyproject.toml` & `enos-8.0.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enos"
-version = "8.0.0a4"
+version = "8.0.0a5"
 description = "Experimental eNvironment for OpenStack"
 authors = ["Didier Iscovery <discovery-dev@inria.fr>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 homepage = "https://github.com/BeyondTheClouds/enos"
 documentation = "https://beyondtheclouds.github.io/enos/"
 keywords = ["OpenStack", "Evaluation", "Grid'5000", "Chameleon", "Vagrant"]
```

### Comparing `enos-8.0.0a4/PKG-INFO` & `enos-8.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enos
-Version: 8.0.0a4
+Version: 8.0.0a5
 Summary: Experimental eNvironment for OpenStack
 Home-page: https://github.com/BeyondTheClouds/enos
 License: GPL-3.0-or-later
 Keywords: OpenStack,Evaluation,Grid'5000,Chameleon,Vagrant
 Author: Didier Iscovery
 Author-email: discovery-dev@inria.fr
 Requires-Python: >=3.8,<4.0
```

