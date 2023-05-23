# Comparing `tmp/slpkg-4.8.4.tar.gz` & `tmp/slpkg-4.8.6.tar.gz`

## Comparing `slpkg-4.8.4.tar` & `slpkg-4.8.6.tar`

### file list

```diff
@@ -1,104 +1,106 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:57:00.000000 slpkg-4.8.4/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-05-17 17:49:35.000000 slpkg-4.8.4/filelists/README
--rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-05-17 17:49:35.000000 slpkg-4.8.4/repositories.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4195 2023-05-17 17:49:35.000000 slpkg-4.8.4/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-05-17 17:49:35.000000 slpkg-4.8.4/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-05-17 17:49:35.000000 slpkg-4.8.4/.pyproject.toml
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-05-17 17:49:35.000000 slpkg-4.8.4/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8822 2023-05-17 17:49:35.000000 slpkg-4.8.4/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-05-17 17:49:35.000000 slpkg-4.8.4/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-05-17 17:49:35.000000 slpkg-4.8.4/configs/slpkg.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      754 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/check_updates_test.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-05-17 17:49:35.000000 slpkg-4.8.4/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-05-17 17:49:35.000000 slpkg-4.8.4/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-05-17 17:49:35.000000 slpkg-4.8.4/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    46324 2023-05-17 17:49:35.000000 slpkg-4.8.4/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     9644 2023-05-17 17:49:35.000000 slpkg-4.8.4/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-05-17 17:49:35.000000 slpkg-4.8.4/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-05-17 17:49:35.000000 slpkg-4.8.4/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-05-17 17:49:35.000000 slpkg-4.8.4/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/
--rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/dialog_configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1901 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7464 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    65522 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4370 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11497 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1160 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/sbos/sbo_generate.py
--rw-r--r--   0 dslackw   (1000) users      (100)    34008 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2437 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3156 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/models/models.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     5945 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5928 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/asciibox.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3801 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9691 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/error_messages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3445 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1334 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/logging_deps.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11666 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/new_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2002 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/multi_process.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3256 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/cleanings.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7847 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3864 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/toml_error_message.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6051 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6654 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      939 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3339 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3965 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    32240 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1518 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3609 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3089 2023-05-17 17:49:35.000000 slpkg-4.8.4/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-05-17 17:49:35.000000 slpkg-4.8.4/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/entry_points.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1286 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-05-17 17:56:56.000000 slpkg-4.8.4/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8561 2023-05-17 17:49:35.000000 slpkg-4.8.4/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-17 17:49:35.000000 slpkg-4.8.4/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-05-17 17:49:35.000000 slpkg-4.8.4/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:52:49.000000 slpkg-4.8.6/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-05-23 19:48:28.000000 slpkg-4.8.6/filelists/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-05-23 19:48:28.000000 slpkg-4.8.6/repositories.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      464 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4262 2023-05-23 19:48:28.000000 slpkg-4.8.6/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-05-23 19:48:28.000000 slpkg-4.8.6/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-05-23 19:48:28.000000 slpkg-4.8.6/.pyproject.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-05-23 19:48:28.000000 slpkg-4.8.6/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8822 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/slpkg.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      381 2023-05-23 19:48:28.000000 slpkg-4.8.6/configs/rules.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      765 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      256 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/check_updates_test.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-05-23 19:48:28.000000 slpkg-4.8.6/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-05-23 19:48:28.000000 slpkg-4.8.6/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-05-23 19:48:28.000000 slpkg-4.8.6/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    46721 2023-05-23 19:48:28.000000 slpkg-4.8.6/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9677 2023-05-23 19:48:28.000000 slpkg-4.8.6/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-05-23 19:48:28.000000 slpkg-4.8.6/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-05-23 19:48:28.000000 slpkg-4.8.6/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-05-23 19:48:28.000000 slpkg-4.8.6/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1892 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7441 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    65376 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4367 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11472 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1151 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    34125 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2627 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3174 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/models/models.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      887 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/rules.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6574 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5928 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/asciibox.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4110 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    10274 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/error_messages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3637 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1350 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/logging_deps.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    13634 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/new_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2058 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/multi_process.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3211 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/cleanings.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2195 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7857 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3867 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/toml_error_message.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6100 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6782 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      916 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3427 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4147 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    33217 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1609 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4041 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3245 2023-05-23 19:48:28.000000 slpkg-4.8.6/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-05-23 19:48:28.000000 slpkg-4.8.6/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/entry_points.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1301 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-05-23 19:52:45.000000 slpkg-4.8.6/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8603 2023-05-23 19:48:28.000000 slpkg-4.8.6/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-23 19:48:28.000000 slpkg-4.8.6/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-05-23 19:48:28.000000 slpkg-4.8.6/tools/gen_sbo_txt.sh
```

### Comparing `slpkg-4.8.4/filelists/multilib/README.ERIC` & `slpkg-4.8.6/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/filelists/multilib/README` & `slpkg-4.8.6/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/filelists/multilib/compat32.pkgs` & `slpkg-4.8.6/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/repositories.txt` & `slpkg-4.8.6/repositories.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slackbuild/slack-desc` & `slpkg-4.8.6/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slackbuild/slpkg.SlackBuild` & `slpkg-4.8.6/slackbuild/slpkg.SlackBuild`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,15 @@
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 # Install configuration files and creating lib directory
 mkdir -p $PKG/etc/$PRGNAM
 install -D -m0644 configs/slpkg.toml $PKG/etc/slpkg/slpkg.toml.new
 install -D -m0644 configs/repositories.toml $PKG/etc/slpkg/repositories.toml.new
 install -D -m0644 configs/blacklist.toml $PKG/etc/slpkg/blacklist.toml.new
+install -D -m0644 configs/rules.toml $PKG/etc/slpkg/rules.toml.new
 
 mkdir -p $PKG/usr/man/man1 & mkdir -p $PKG/usr/man/fr/man1
 cp man/slpkg.1 $PKG/usr/man/man1
 cp man/slpkg-fr.1 $PKG/usr/man/fr/man1/slpkg.1
 
 find $PKG/usr/man -type f -exec gzip -9 {} \;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz; rm $i ; done
```

### Comparing `slpkg-4.8.4/.pyproject.toml` & `slpkg-4.8.6/.pyproject.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/configs/repositories.toml` & `slpkg-4.8.6/configs/repositories.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/configs/slpkg.toml` & `slpkg-4.8.6/configs/slpkg.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/tests/test_configs.py` & `slpkg-4.8.6/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/tests/test_checks.py` & `slpkg-4.8.6/tests/test_checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 
 class TestPkgInstalled(unittest.TestCase):
 
     def setUp(self):
         self.bin_queries = SBoQueries('sbo')
         self.data = self.bin_queries.repository_data()
-        self.check = Check('sbo', self.data)
+        self.check = Check('sbo')
         self.packages = ['colored', 'sbo-create', 'sun']
 
     def test_check_exists(self):
-        self.assertIsNone(self.check.package_exists_in_the_database(self.packages))
+        self.assertIsNone(self.check.package_exists_in_the_database(self.packages, self.data))
 
     def test_check_unsupported(self):
-        self.assertIsNone(self.check.is_package_unsupported(self.packages))
+        self.assertIsNone(self.check.is_package_unsupported(self.packages, self.data))
 
     def test_check_is_installed(self):
         self.assertIsNone(self.check.is_package_installed(self.packages))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `slpkg-4.8.4/tests/test_utilities.py` & `slpkg-4.8.6/tests/test_utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def test_all_installed(self):
         self.assertIn(self.package, self.utils.installed_packages.values())
 
     def test_read_build_tag(self):
         self.assertEqual('1', self.utils.read_slackbuild_build_tag('slpkg', 'system', 'sbo'))
 
     def test_is_option(self):
-        self.assertTrue(True, self.utils.is_option(['-P', '--parallel'],
+        self.assertTrue(True, self.utils.is_option(('-P', '--parallel'),
                                                    ['-k', '-p', '-P', '--parallel', '--repository']))
 
     def test_get_file_size(self):
         self.assertEqual('2 MB', self.utils.get_file_size(Path('/var/log/packages/', self.package)))
 
     def test_apply_package_pattern(self):
         self.assertGreater(len(self.utils.apply_package_pattern(self.data, ['*'])), 1)
```

### Comparing `slpkg-4.8.4/tests/test_sbo_queries.py` & `slpkg-4.8.6/tests/test_sbo_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/tests/test_colors.py` & `slpkg-4.8.6/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/tests/check_updates_test.py` & `slpkg-4.8.6/tests/check_updates_test.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/tests/test_upgrade.py` & `slpkg-4.8.6/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/tests/test_bin_queries.py` & `slpkg-4.8.6/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/LICENSE` & `slpkg-4.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/install.sh` & `slpkg-4.8.6/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/ChangeLog.txt` & `slpkg-4.8.6/ChangeLog.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+4.8.6 - 21/05/2023
+Updated:
+- Load the database when used #172
+Fixed:
+- ValueError with search command
+- Updates some packages to the same version #169
+- For --skip-installed option
+Added:
+- Configuration file rules.toml
+
+4.8.5 - 18/05/2023
+Fixed:
+- Case-sensitive with commands find and search
+- For combination options with --repository= and --directory=
+- TypeError for repo-info command #171
+
 4.8.4 - 14/05/2023
 Added:
 - Case-insensitive pattern matching, --no-case option
 - Choose border color via configuration file
 - New processing status view for build, install, upgrade, remove
 Fixed:
 - Remove chosen dependencies
```

### Comparing `slpkg-4.8.4/man/slpkg.1` & `slpkg-4.8.6/man/slpkg.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH slpkg 1 "Orestiada, Greece" "slpkg 4.8.3" dslackw
+.TH slpkg 1 "Orestiada, Greece" "slpkg 4.8.5" dslackw
 .SH NAME
 .P
 slpkg \- Package manager utility for Slackware.
 .SH SYNOPSIS
 .P
 slpkg \c
 [\fICOMMAND\fR] [\fIOPTIONS\fR] [\fIFILELIST|PACKAGES...\fR]
@@ -109,15 +109,15 @@
 .RS
 Tracking the packages dependencies.
 .RE
 .SH OPTIONS
 .P
 .B -y, --yes
 .RS
-Answer Yes to all questions. (to be used with: -u, update, -U, upgrade, -L, clean-logs, -b, build,
+Answer Yes to all questions. (to be used with: -u, update, -U, upgrade, -b, build,
 -i, install, -R, remove, -d, download,)
 .RE
 .P
 .B -j, --jobs
 .RS
 Acceleration of SlackBuild scripts. When the \fB--jobs\fR flag is set, slpkg automatically detects the number
 of processors and enters it into the MAKEFLAGS variable. Some SlackBuilds fail when MAKEFLAGS is declared or
@@ -270,14 +270,16 @@
 .P
 Configuration file in the /etc/slpkg/slpkg.toml file.
 .P
 Repositories file in the /etc/slpkg/repositories.toml file.
 .P
 Blacklist file in the /etc/slpkg/blacklist.toml file.
 .P
+Rules file in the /etc/slpkg/rules.toml file.
+.P
 \fIslpkg_new-configs\fR command it's managing the .new configuration files easily and fast. Move, copy or remove them.
 .RE
 .SH REPORT BUGS
 .P
 Please report any found to: https://gitlab.com/dslackw/slpkg/-/issues.
 .P
 Note: With the issue, please reference the log file you will find in the /tmp/slpkg/logs/slpkg.log path and paste it too.
```

### Comparing `slpkg-4.8.4/man/slpkg-fr.1` & `slpkg-4.8.6/man/slpkg-fr.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/completion/slpkg` & `slpkg-4.8.6/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/dialog_configs.py` & `slpkg-4.8.6/slpkg/dialog_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/binaries/required.py` & `slpkg-4.8.6/slpkg/binaries/required.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,10 +51,10 @@
                     requires.append(sub)
 
         requires.reverse()
         return tuple(dict.fromkeys(requires))
 
     def remove_deps(self, requires: list) -> Generator:
         """ Remove requires that not in the repository or blacklisted. """
-        for dependency in requires:
-            if dependency in self.repository_packages:
-                yield dependency
+        for require in requires:
+            if require in self.repository_packages:
+                yield require
```

### Comparing `slpkg-4.8.4/slpkg/binaries/queries.py` & `slpkg-4.8.6/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/binaries/install.py` & `slpkg-4.8.6/slpkg/binaries/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,21 @@
         self.dependencies: list = []
         self.install_order: list = []
         self.binary_packages: list = []
         self.slackware_command: str = self.installpkg
         self.progress_message: str = f'{self.cyan}Installing{self.endc}'
 
         self.option_for_reinstall: bool = self.utils.is_option(
-            ['-r', '--reinstall'], flags)
+            ('-r', '--reinstall'), flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
-            ['-k', '--skip-installed'], flags)
+            ('-k', '--skip-installed'), flags)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-O', '--resolve-off'], flags)
+            ('-O', '--resolve-off'), flags)
 
         self.packages: list = self.utils.apply_package_pattern(data, packages)
 
     def execute(self) -> None:
         # self.creating_dependencies_list()
         self.creating_dependencies_list()
         self.remove_duplicate_from_dependencies_list()
@@ -78,18 +78,14 @@
 
     def creating_dependencies_list(self) -> None:
         if not self.option_for_resolve_off:
             for package in self.packages:
                 dependencies: tuple = Required(self.data, package).resolve()
 
                 for dependency in dependencies:
-                    # Skip installed package when the option --skip-installed is applied.
-                    if self.option_for_skip_installed and self.utils.is_package_installed(dependency):
-                        continue
-
                     self.dependencies.append(dependency)
 
     def remove_duplicate_from_dependencies_list(self) -> None:
         if self.dependencies:
             self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
     def add_dependencies_to_install_order(self) -> None:
@@ -120,41 +116,42 @@
                 installed_package: str = self.utils.is_package_installed(pkg)
                 self.view_message.view_skipping_packages(installed_package)
 
         self.download_the_binary_packages(package_urls)
 
     def download_the_binary_packages(self, package_urls: list) -> None:
         if package_urls:
+            print(f'Started to download total ({self.cyan}{len(package_urls)}{self.endc}) packages:\n')
+        if package_urls:
             down = Downloader(self.tmp_slpkg, package_urls, self.flags)
             down.download()
             print()
 
     def continue_to_install(self, name: str) -> bool:
         """ Skip installed package when the option --skip-installed is applied
             and continue to install if the package is upgradable or the --reinstall option
             applied.
          """
         if not self.utils.is_package_installed(name):
             return True
 
-        if self.upgrade.is_package_upgradeable(name):
-            return True
-
-        if self.utils.is_package_installed(name) and self.option_for_reinstall:
+        if self.utils.is_package_installed(name) and not self.option_for_skip_installed:
             return True
 
         return False
 
     def checksum_binary_packages(self) -> None:
         for package in self.binary_packages:
             name: str = self.utils.split_package(Path(package).stem)['name']
             pkg_checksum: str = self.data[name]['checksum']
             self.check_md5.md5sum(self.tmp_slpkg, package, pkg_checksum)
 
     def install_packages(self) -> None:
+        if self.binary_packages:
+            print(f'Started the processing of ({self.cyan}{len(self.binary_packages)}{self.endc}) packages:\n')
         for package in self.binary_packages:
             command: str = f'{self.slackware_command} {self.tmp_slpkg}/{package}'
             self.multi_proc.process(command, package, self.progress_message)
 
             if not self.option_for_resolve_off:
                 name: str = self.utils.split_package(Path(package).stem)['name']
                 self.logs_deps.logging(name)
```

### Comparing `slpkg-4.8.4/slpkg/install_data.py` & `slpkg-4.8.6/slpkg/install_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,41 @@
 # -*- coding: utf-8 -*-
 
 import re
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
+from slpkg.views.asciibox import AsciiBox
 from slpkg.repositories import Repositories
 from slpkg.models.models import session as Session
 from slpkg.models.models import (SBoTable, PonceTable,
                                  BinariesTable, LastRepoUpdated)
 
 
 class InstallData(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
         self.session = Session
         self.utils = Utilities()
         self.repos = Repositories()
+        self.ascii = AsciiBox()
 
-    def last_updated(self, repo_file: Path) -> str:
+    def last_updated(self, changelog_file: Path) -> str:
         """ Reads the first date of the changelog file."""
-        lines: list = self.utils.read_text_file(repo_file)
+        lines: list = self.utils.read_text_file(changelog_file)
         days = ('Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun')
         for line in lines:
             if line.startswith(days):
                 return line.replace('\n', '')
 
+    def view_done_message(self):
+        print(f'{self.yellow}{self.ascii.done}{self.endc}\n')
+
     def install_sbo_data(self) -> None:
         """ Install the data for SBo repository. """
         sbo_tags = [
             'SLACKBUILD NAME:',
             'SLACKBUILD LOCATION:',
             'SLACKBUILD FILES:',
             'SLACKBUILD VERSION:',
@@ -41,15 +46,14 @@
             'SLACKBUILD MD5SUM_x86_64:',
             'SLACKBUILD REQUIRES:',
             'SLACKBUILD SHORT DESCRIPTION:'
         ]
 
         path_slackbuilds: Path = Path(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
         path_changelog: Path = Path(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
-
         slackbuilds_txt: list = self.utils.read_text_file(path_slackbuilds)
 
         cache: list = []  # init cache
 
         print(f"Updating the database for '{self.cyan}{self.repos.sbo_repo_name}{self.endc}'... ", end='', flush=True)
 
         for i, line in enumerate(slackbuilds_txt, 1):
@@ -68,19 +72,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache after 11 lines
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.sbo_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_ponce_data(self) -> None:
         """ Install the data for SBo repository. """
         sbo_tags = [
             'SLACKBUILD NAME:',
             'SLACKBUILD LOCATION:',
             'SLACKBUILD FILES:',
             'SLACKBUILD VERSION:',
@@ -90,15 +93,14 @@
             'SLACKBUILD MD5SUM_x86_64:',
             'SLACKBUILD REQUIRES:',
             'SLACKBUILD SHORT DESCRIPTION:'
         ]
 
         path_slackbuilds = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
         path_changelog: Path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
-
         slackbuilds_txt: list = self.utils.read_text_file(path_slackbuilds)
 
         cache: list = []  # init cache
 
         print(f"Updating the database for '{self.cyan}{self.repos.ponce_repo_name}{self.endc}'... ", end='', flush=True)
 
         for i, line in enumerate(slackbuilds_txt, 1):
@@ -117,19 +119,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache after 11 lines
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.ponce_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_slack_data(self) -> None:
         """ Install the data for slackware repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slack_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -208,19 +209,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slack_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_slack_extra_data(self) -> None:
         """ Install the data for slackware extra repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slack_extra_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -299,19 +299,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slack_extra_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_slack_patches_data(self) -> None:
         """ Install the data for slackware patches repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slack_patches_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -390,19 +389,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slack_patches_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_alien_data(self) -> None:
         """ Install the data for alien repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.alien_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -487,19 +485,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.alien_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_multilib_data(self) -> None:
         """ Install the data for multilib repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.multilib_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -578,19 +575,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.multilib_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_restricted_data(self) -> None:
         """ Install the data for multilib repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.restricted_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -669,19 +665,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.restricted_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_gnome_data(self) -> None:
         """ Install the data for gnome repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.gnome_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -761,19 +756,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.gnome_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_msb_data(self) -> None:
         """ Install the data for msb repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.msb_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -852,19 +846,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.msb_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_csb_data(self) -> None:
         """ Install the data for csb repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.csb_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -943,19 +936,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.csb_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_conraid_data(self) -> None:
         """ Install the data for conraid repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.conraid_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -1035,19 +1027,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.conraid_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_slackonly_data(self) -> None:
         """ Install the data for slackonly repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slackonly_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -1132,19 +1123,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slackonly_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_salixos_data(self) -> None:
         """ Install the data for salixos repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.salixos_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -1237,19 +1227,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.salixos_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_salixos_extra_data(self) -> None:
         """ Install the data for salixos_extra repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.salixos_extra_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -1343,19 +1332,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.salixos_extra_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_salixos_patches_data(self) -> None:
         """ Install the data for salixos_patches repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.salixos_patches_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -1449,19 +1437,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.salixos_patches_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_slackel_data(self) -> None:
         """ Install the data for slackel repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slackel_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -1554,19 +1541,18 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slackel_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
 
+        self.view_done_message()
+
     def install_slint_data(self) -> None:
         """ Install the data for slint repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slint_repo_name}{self.endc}'... ",
               end='', flush=True)
 
         checksums_dict: dict = {}
         pkg_tag = [
@@ -1659,11 +1645,10 @@
                 self.session.add(data)
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slint_repo_name, date=last_updated)
         self.session.add(date)
-
-        print(f'{self.byellow}Done{self.endc}\n')
-
         self.session.commit()
+
+        self.view_done_message()
```

### Comparing `slpkg-4.8.4/slpkg/repositories.py` & `slpkg-4.8.6/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/repo_info.py` & `slpkg-4.8.6/slpkg/repo_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if self.name_alignment < 1:
             self.name_alignment: int = 1
 
         self.enabled: int = 0
         self.total_packages: int = 0
 
         self.option_for_repository: bool = self.utils.is_option(
-            ['-o', '--repository='], flags)
+            ('-o', '--repository='), flags)
 
     def info(self) -> None:
         """ Prints information about repositories. """
         self.view_the_title()
 
         if self.option_for_repository:
             self.view_the_repository_information()
@@ -58,15 +58,15 @@
         return count
 
     def last_repository_updated(self, repository: str) -> str:
         date: str = self.session.query(
             LastRepoUpdated.date).where(
             LastRepoUpdated.repo == repository).first()
 
-        if date[0] is None:
+        if date is None:
             date: tuple = ('',)
 
         return date[0]
 
     def view_the_title(self) -> None:
         title: str = f'repositories information:'.title()
         if self.option_for_repository:
```

### Comparing `slpkg-4.8.4/slpkg/sbos/queries.py` & `slpkg-4.8.6/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/sbos/slackbuild.py` & `slpkg-4.8.6/slpkg/sbos/slackbuild.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,24 +50,24 @@
         self.install_order: list = []
         self.dependencies: list = []
         self.slackware_command: str = str()
         self.slackware_command: str = self.installpkg
         self.progress_message: str = f'{self.cyan}Installing{self.endc}'
 
         self.option_for_reinstall: bool = self.utils.is_option(
-            ['-r', '--reinstall'], flags)
+            ('-r', '--reinstall'), flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
-            ['-k', '--skip-installed'], flags)
+            ('-k', '--skip-installed'), flags)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-O', '--resolve-off'], flags)
+            ('-O', '--resolve-off'), flags)
 
         self.option_for_jobs: bool = self.utils.is_option(
-            ['-j', '--jobs'], flags)
+            ('-j', '--jobs'), flags)
 
         self.slackbuilds: list = self.utils.apply_package_pattern(data, slackbuilds)
 
         # Patch the TAG from configs if changed.
         self.repo_tag: str = self.repos.repositories[repository]['repo_tag']
         if self.repos.repositories[repository]['patch_tag']:
             self.repo_tag: str = self.repos.repositories[repository]['repo_tag']
@@ -98,18 +98,14 @@
 
     def creating_dependencies_list(self) -> None:
         if not self.option_for_resolve_off:
             for slackbuild in self.slackbuilds:
                 dependencies: tuple = Requires(self.data, slackbuild).resolve()
 
                 for dependency in dependencies:
-                    # Skip installed package when the option --skip-installed is applied.
-                    if self.option_for_skip_installed and self.utils.is_package_installed(dependency):
-                        continue
-
                     self.dependencies.append(dependency)
 
     def remove_duplicate_from_dependencies_list(self) -> None:
         self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
     def add_dependencies_to_install_order(self) -> None:
         self.install_order.extend(self.dependencies)
@@ -137,18 +133,15 @@
         """
         if self.mode == 'build':
             return True
 
         if not self.utils.is_package_installed(name):
             return True
 
-        if self.upgrade.is_package_upgradeable(name):
-            return True
-
-        if self.utils.is_package_installed(name) and self.option_for_reinstall:
+        if self.utils.is_package_installed(name) and not self.option_for_skip_installed:
             return True
 
         return False
 
     def prepare_slackbuilds_for_build(self) -> None:
         for sbo in self.install_order:
             if self.continue_build_or_install(sbo):
@@ -167,14 +160,16 @@
                 if self.os_arch == 'x86_64' and self.data[sbo]['download64']:
                     self.sources[sbo] = self.data[sbo]['download64'].split()
                 else:
                     self.sources[sbo] = self.data[sbo]['download'].split()
 
     def download_the_sources(self) -> None:
         if self.sources:
+            print(f'Started to download total ({self.cyan}{len(self.sources)}{self.endc}) sources:\n')
+        if self.sources:
             for package, sbo_sources in self.sources.items():
                 down_urls = Downloader(Path(self.build_path, package), sbo_sources, self.flags)
                 down_urls.download()
             print()
 
             self.checksum_downloaded_sources()
 
@@ -189,14 +184,16 @@
                 checksums: list = self.data[sbo]['md5sum'].split()
                 sources: list = self.data[sbo]['download'].split()
 
             for source, checksum in zip(sources, checksums):
                 self.check_md5.md5sum(path, source, checksum)
 
     def build_and_install_the_slackbuilds(self) -> None:
+        if self.install_order:
+            print(f'Started the processing of ({self.cyan}{len(self.install_order)}{self.endc}) packages:\n')
         for sbo in self.install_order:
             if self.continue_build_or_install(sbo):
                 self.patch_slackbuild_tag(sbo)
                 self.build_the_script(self.build_path, sbo)
 
                 if self.mode in ('install', 'upgrade'):
                     self.install_package(sbo)
@@ -237,15 +234,15 @@
 
     def build_the_script(self, path: Path, name: str) -> None:
         self.set_makeflags()
         folder: Path = Path(path, name)
         filename: str = f'{name}.SlackBuild'
         command: str = f'{folder}/./{filename}'
         self.utils.change_owner_privileges(folder)
-        progress_message: str = f'{self.red}Build{self.endc}'
+        progress_message: str = f'{self.red}Building{self.endc}'
         self.multi_proc.process(command, filename, progress_message)
 
     def set_progress_message(self):
         if self.mode == 'upgrade' or self.option_for_reinstall:
             self.progress_message: str = f'{self.cyan}Upgrading{self.endc}'
 
     def set_slackware_command(self) -> None:
```

### Comparing `slpkg-4.8.4/slpkg/sbos/dependencies.py` & `slpkg-4.8.6/slpkg/sbos/dependencies.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,10 +29,10 @@
 
         requires.reverse()
 
         return tuple(dict.fromkeys(requires))
 
     def remove_deps(self, requires: list) -> Generator:
         """ Remove requires that not in the repository or blacklisted. """
-        for dependency in requires:
-            if dependency in self.repository_packages:
-                yield dependency
+        for require in requires:
+            if require in self.repository_packages:
+                yield require
```

### Comparing `slpkg-4.8.4/slpkg/sbos/sbo_generate.py` & `slpkg-4.8.6/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/update_repository.py` & `slpkg-4.8.6/slpkg/update_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,18 @@
         self.check_updates = CheckUpdates(flags, repository)
 
         self.repos_for_update: dict = {}
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_repository: bool = self.utils.is_option(
-            ['-o', '--repository='], flags)
+            ('-o', '--repository='), flags)
 
         self.option_for_install_data: bool = self.utils.is_option(
-            ['-a', '--install-data'], flags)
+            ('-a', '--install-data'), flags)
 
     def update_the_repositories(self) -> None:
         if not any(list(self.repos_for_update.values())):
             self.view.question()
             for repo in self.repos_for_update:
                 self.repos_for_update[repo] = True
         else:
@@ -73,25 +73,29 @@
             self.repos.salixos_extra_repo_name: self.salixos_extra_repository,
             self.repos.salixos_patches_repo_name: self.salixos_patches_repository,
             self.repos.slackel_repo_name: self.slackel_repository,
             self.repos.slint_repo_name: self.slint_repository
         }
 
         if self.option_for_repository:
-            print(f"Downloading the '{self.green}{self.repository}{self.endc}' repository "
-                  f"in the '{self.repos.repositories[self.repository]['path']}' folder, please wait...\n")
+            if not self.option_for_install_data:
+                self.view_downloading_message(self.repository)
             repositories[self.repository]()
         else:
-            for repo, value in self.repos_for_update.items():
-                if value:
-                    print(f"Downloading the '{self.green}{repo}{self.endc}' repository "
-                          f"in the '{self.repos.repositories[repo]['path']}' folder, please wait...\n")
+            for repo, update in self.repos_for_update.items():
+                if update:
+                    if not self.option_for_install_data:
+                        self.view_downloading_message(repo)
                     repositories[repo]()
         print()
 
+    def view_downloading_message(self, repo: str) -> None:
+        print(f"Downloading the '{self.green}{repo}{self.endc}' repository "
+              f"in the '{self.repos.repositories[repo]['path']}' folder, please wait...\n")
+
     def slack_repository(self):
         if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.slack_repo_path)
 
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
@@ -611,26 +615,26 @@
                   f'last update and now.{self.endc}')
 
     def repositories(self) -> None:
         queue = Queue()
         message: str = 'Checking for news, please wait...'
 
         # Starting multiprocessing
-        p1 = Process(target=self.check_for_updates, args=(queue,))
-        p2 = Process(target=self.progress.progress_bar, args=(message,))
+        process_1 = Process(target=self.check_for_updates, args=(queue,))
+        process_2 = Process(target=self.progress.progress_bar, args=(message,))
 
-        p1.start()
-        p2.start()
+        process_1.start()
+        process_2.start()
 
         # Wait until process 1 finish
-        p1.join()
+        process_1.join()
 
         # Terminate process 2 if process 1 finished
-        if not p1.is_alive():
-            p2.terminate()
+        if not process_1.is_alive():
+            process_2.terminate()
 
         # Restore the terminal cursor
         print('\x1b[?25h', self.endc, end='')
 
         self.repos_for_update: dict = queue.get()
         self.update_the_repositories()
```

### Comparing `slpkg-4.8.4/slpkg/progress_bar.py` & `slpkg-4.8.6/slpkg/progress_bar.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,29 +15,26 @@
         super(Configs, self).__init__()
         self.spinner = PixelSpinner
         self.ascii = AsciiBox()
 
         self.color: str = self.endc
         self.spinners: dict = {}
         self.spinners_color: dict = {}
+        self.bar_message: str = str()
 
     def progress_bar(self, message: str, filename=None) -> None:
         """ Creating progress bar. """
         self.assign_spinners()
         self.assign_spinner_colors()
         self.set_spinner()
         self.set_color()
-
-        bar_message: str = f"{self.endc}{message} "
-        if filename:
-            bar_message: str = (f"{'':>2}{self.red}{self.ascii.bullet}{self.endc} {filename}: "
-                                f"{message}... ")
+        self.set_the_spinner_message(filename, message)
 
         if self.spinning_bar:
-            bar_spinner = self.spinner(f'{bar_message}{self.color}')
+            bar_spinner = self.spinner(f'{self.bar_message}{self.color}')
             # print('\033[F', end='', flush=True)
             try:
                 while True:
                     time.sleep(0.1)
                     bar_spinner.next()
             except KeyboardInterrupt:
                 raise SystemExit(1)
@@ -62,14 +59,20 @@
             'blue': self.blue,
             'cyan': self.cyan,
             'grey': self.grey,
             'red': self.red,
             'white': self.endc
         }
 
+    def set_the_spinner_message(self, filename: str, message: str) -> None:
+        self.bar_message: str = f"{self.endc}{message} "
+        if filename:
+            self.bar_message: str = (f"{'':>2}{self.red}{self.ascii.bullet}{self.endc} {filename}: "
+                                     f"{message}... ")
+
     def set_spinner(self) -> None:
         try:
             self.spinner: str = self.spinners[self.progress_spinner]
         except KeyError:
             self.spinner = PixelSpinner
 
     def set_color(self) -> None:
```

### Comparing `slpkg-4.8.4/slpkg/downloader.py` & `slpkg-4.8.6/slpkg/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,28 +28,28 @@
         self.downloader_tools: dict = {
             'wget': self.wget_downloader,
             'wget2': self.wget_downloader,
             'curl': self.curl_downloader,
             'lftp': self.lftp_downloader
         }
         self.option_for_parallel: bool = self.utils.is_option(
-            ['-P', '--parallel'], flags)
+            ('-P', '--parallel'), flags)
 
     def download(self) -> None:
         """ Starting the processing for downloading. """
-        process: list = []
+        processes: list = []
 
         if self.parallel_downloads or self.option_for_parallel:
             for url in self.urls:
-                p1 = Process(target=self.tools, args=(url,))
-                process.append(p1)
-                p1.start()
+                proc = Process(target=self.tools, args=(url,))
+                processes.append(proc)
+                proc.start()
 
-            for proc in process:
-                proc.join()
+            for process in processes:
+                process.join()
         else:
             for url in self.urls:
                 self.tools(url)
 
     def tools(self, url: str) -> None:
         path: str = urlparse(url).path
         self.filename: str = unquote(Path(path).name)
```

### Comparing `slpkg-4.8.4/slpkg/models/models.py` & `slpkg-4.8.6/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/views/view_package.py` & `slpkg-4.8.6/slpkg/views/view_package.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,98 +15,125 @@
         super(Configs, self).__init__()
         self.flags: list = flags
         self.repository: str = repository
 
         self.utils = Utilities()
         self.repos = Repositories()
 
+        self.repository_packages: tuple = ()
+        self.readme: list = []
+        self.info_file: list = []
+        self.repo_build_tag: str = str()
+        self.mirror: str = str()
+        self.homepage: str = str()
+        self.maintainer: str = str()
+        self.email: str = str()
+        self.dependencies: str = str()
+        self.repo_tar_suffix: str = str()
+
         self.option_for_pkg_version: bool = self.utils.is_option(
-            ['-p', '--pkg-version'], flags)
+            ('-p', '--pkg-version'), flags)
 
     def slackbuild(self, data: dict, slackbuilds: list) -> None:
         """ View slackbuild packages information. """
         repo: dict = {
             self.repos.sbo_repo_name: self.repos.sbo_repo_tar_suffix,
             self.repos.ponce_repo_name: str()
         }
-        repo_tar_suffix: str = repo[self.repository]
-        repository_packages: tuple = tuple(data.keys())
+        self.repo_tar_suffix: str = repo[self.repository]
+        self.repository_packages: tuple = tuple(data.keys())
 
         for sbo in slackbuilds:
             for name, item in data.items():
 
                 if sbo == name or sbo == '*':
                     path_file: Path = Path(self.repos.repositories[self.repository]['path'],
                                            item['location'], name, 'README')
-                    readme: list = self.utils.read_text_file(path_file)
-
                     path_info: Path = Path(self.repos.repositories[self.repository]['path'],
                                            item['location'], name, f'{name}.info')
-                    info_file: list = self.utils.read_text_file(path_info)
-
-                    repo_build_tag: str = self.utils.read_slackbuild_build_tag(
-                        name, item['location'], self.repository)
 
-                    mirror: str = self.repos.repositories[self.repository]['mirror'][0]
-
-                    maintainer = email = homepage = str()
-                    for line in info_file:
-                        if line.startswith('HOMEPAGE'):
-                            homepage: str = line[10:-2].strip()
-                        if line.startswith('MAINTAINER'):
-                            maintainer: str = line[12:-2].strip()
-                        if line.startswith('EMAIL'):
-                            email: str = line[7:-2].strip()
-
-                    deps: str = (', '.join([f'{self.cyan}{pkg}' for pkg in item['requires'].split()]))
-                    if self.option_for_pkg_version:
-                        deps: str = (', '.join(
-                            [f"{self.cyan}{pkg}{self.endc}-{self.yellow}{data[pkg]['version']}"
-                             f"{self.green}" for pkg in item['requires'].split()
-                             if pkg in repository_packages]))
-
-                    print(f"Name: {self.green}{name}{self.endc}\n"
-                          f"Version: {self.green}{item['version']}{self.endc}\n"
-                          f"Build: {self.green}{repo_build_tag}{self.endc}\n"
-                          f"Requires: {self.green}{deps}{self.endc}\n"
-                          f"Homepage: {self.blue}{homepage}{self.endc}\n"
-                          f"Download SlackBuild: {self.blue}{mirror}"
-                          f"{item['location']}/{name}{repo_tar_suffix}{self.endc}\n"
-                          f"Download sources: {self.blue}{item['download']}{self.endc}\n"
-                          f"Download_x86_64 sources: {self.blue}{item['download64']}{self.endc}\n"
-                          f"Md5sum: {self.yellow}{item['md5sum']}{self.endc}\n"
-                          f"Md5sum_x86_64: {self.yellow}{item['md5sum64']}{self.endc}\n"
-                          f"Files: {self.green}{item['files']}{self.endc}\n"
-                          f"Description: {self.green}{item['description']}{self.endc}\n"
-                          f"Category: {self.red}{item['location']}{self.endc}\n"
-                          f"SBo url: {self.blue}{mirror}{item['location']}/{name}{self.endc}\n"
-                          f"Maintainer: {self.yellow}{maintainer}{self.endc}\n"
-                          f"Email: {self.yellow}{email}{self.endc}\n"
-                          f"\nREADME: {self.cyan}{''.join(readme)}{self.endc}")
+                    self.read_the_readme_file(path_file)
+                    self.read_the_info_file(path_info)
+                    self.read_repo_build_tag(name, item)
+                    self.assign_the_sbo_mirror()
+                    self.assign_the_info_file_variables()
+                    self.assign_dependencies(item)
+                    self.assign_dependencies_with_version(item, data)
+                    self.view_slackbuild_package(name, item)
+
+    def read_the_readme_file(self, path_file: Path) -> None:
+        self.readme: list = self.utils.read_text_file(path_file)
+
+    def read_the_info_file(self, path_info: Path) -> None:
+        self.info_file: list = self.utils.read_text_file(path_info)
+
+    def read_repo_build_tag(self, name: str, item: dict) -> None:
+        self.repo_build_tag: str = self.utils.read_slackbuild_build_tag(
+             name, item['location'], self.repository)
+
+    def assign_the_sbo_mirror(self) -> None:
+        self.mirror: str = self.repos.repositories[self.repository]['mirror'][0]
+
+    def assign_the_info_file_variables(self) -> None:
+        for line in self.info_file:
+            if line.startswith('HOMEPAGE'):
+                self.homepage: str = line[10:-2].strip()
+            if line.startswith('MAINTAINER'):
+                self.maintainer: str = line[12:-2].strip()
+            if line.startswith('EMAIL'):
+                self.email: str = line[7:-2].strip()
+
+    def assign_dependencies(self, item: dict) -> None:
+        self.dependencies: str = (', '.join([f'{self.cyan}{pkg}' for pkg in item['requires'].split()]))
+
+    def assign_dependencies_with_version(self, item: dict, data: dict) -> None:
+        if self.option_for_pkg_version:
+            self.dependencies: str = (', '.join(
+                [f"{self.cyan}{pkg}{self.endc}-{self.yellow}{data[pkg]['version']}"
+                 f"{self.green}" for pkg in item['requires'].split()
+                 if pkg in self.repository_packages]))
+
+    def view_slackbuild_package(self, name: str, item: dict) -> None:
+        print(f"Name: {self.green}{name}{self.endc}\n"
+              f"Version: {self.green}{item['version']}{self.endc}\n"
+              f"Build: {self.green}{self.repo_build_tag}{self.endc}\n"
+              f"Requires: {self.green}{self.dependencies}{self.endc}\n"
+              f"Homepage: {self.blue}{self.homepage}{self.endc}\n"
+              f"Download SlackBuild: {self.blue}{self.mirror}"
+              f"{item['location']}/{name}{self.repo_tar_suffix}{self.endc}\n"
+              f"Download sources: {self.blue}{item['download']}{self.endc}\n"
+              f"Download_x86_64 sources: {self.blue}{item['download64']}{self.endc}\n"
+              f"Md5sum: {self.yellow}{item['md5sum']}{self.endc}\n"
+              f"Md5sum_x86_64: {self.yellow}{item['md5sum64']}{self.endc}\n"
+              f"Files: {self.green}{item['files']}{self.endc}\n"
+              f"Description: {self.green}{item['description']}{self.endc}\n"
+              f"Category: {self.red}{item['location']}{self.endc}\n"
+              f"SBo url: {self.blue}{self.mirror}{item['location']}/{name}{self.endc}\n"
+              f"Maintainer: {self.yellow}{self.maintainer}{self.endc}\n"
+              f"Email: {self.yellow}{self.email}{self.endc}\n"
+              f"\nREADME: {self.cyan}{''.join(self.readme)}{self.endc}")
 
     def package(self, data: dict, packages: list) -> None:
         """ View binary packages information. """
-        repository_packages: tuple = tuple(data.keys())
+        self.repository_packages: tuple = tuple(data.keys())
         for package in packages:
             for name, item in data.items():
-
                 if package == name or package == '*':
-                    deps: str = (', '.join([f"{self.cyan}{pkg}" for pkg in item['requires'].split()]))
-                    if self.option_for_pkg_version:
-                        deps: str = (', '.join(
-                            [f"{self.cyan}{pkg}{self.endc} {self.yellow}{data[pkg]['requires']}"
-                             f"{self.green}" for pkg in item['requires'].split()
-                             if pkg in repository_packages]))
-
-                    print(f"Name: {self.green}{name}{self.endc}\n"
-                          f"Version: {self.green}{item['version']}{self.endc}\n"
-                          f"Package: {self.cyan}{item['package']}{self.endc}\n"
-                          f"Download: {self.blue}{item['mirror']}{item['location']}/{item['package']}{self.endc}\n"
-                          f"Md5sum: {item['checksum']}\n"
-                          f"Mirror: {self.blue}{item['mirror']}{self.endc}\n"
-                          f"Location: {self.red}{item['location']}{self.endc}\n"
-                          f"Size Comp: {self.yellow}{item['size_comp']} KB{self.endc}\n"
-                          f"Size Uncomp: {self.yellow}{item['size_uncomp']} KB{self.endc}\n"
-                          f"Requires: {self.green}{deps}{self.endc}\n"
-                          f"Conflicts: {item['conflicts']}\n"
-                          f"Suggests: {item['suggests']}\n"
-                          f"Description: {item['description']}\n")
+
+                    self.assign_dependencies(item)
+                    self.assign_dependencies_with_version(item, data)
+                    self.view_binary_package(name, item)
+
+    def view_binary_package(self, name: str, item: dict) -> None:
+        print(f"Name: {self.green}{name}{self.endc}\n"
+              f"Version: {self.green}{item['version']}{self.endc}\n"
+              f"Package: {self.cyan}{item['package']}{self.endc}\n"
+              f"Download: {self.blue}{item['mirror']}{item['location']}/{item['package']}{self.endc}\n"
+              f"Md5sum: {item['checksum']}\n"
+              f"Mirror: {self.blue}{item['mirror']}{self.endc}\n"
+              f"Location: {self.red}{item['location']}{self.endc}\n"
+              f"Size Comp: {self.yellow}{item['size_comp']} KB{self.endc}\n"
+              f"Size Uncomp: {self.yellow}{item['size_uncomp']} KB{self.endc}\n"
+              f"Requires: {self.green}{self.dependencies}{self.endc}\n"
+              f"Conflicts: {item['conflicts']}\n"
+              f"Suggests: {item['suggests']}\n"
+              f"Description: {item['description']}\n")
```

### Comparing `slpkg-4.8.4/slpkg/views/version.py` & `slpkg-4.8.6/slpkg/views/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 8, 4)
+        self.version_info: tuple = (4, 8, 6)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.8.4/slpkg/views/cli_menu.py` & `slpkg-4.8.6/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/views/asciibox.py` & `slpkg-4.8.6/slpkg/views/asciibox.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/views/help_commands.py` & `slpkg-4.8.6/slpkg/views/help_commands.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,18 @@
         self.command: str = command
         self.flags: list = flags
 
     def view(self) -> None:
         self.flags.reverse()  # Put first the short options.
 
         help_commands: dict = {
+            '-h': "Show this message and exit.",
+            '--help': "Show this message and exit.",
+            '-v': "Print version and exit.",
+            '--version': "Print version and exit.",
             'update': "Updates the package list and the database.",
             'upgrade': "Upgrade all the installed packages if the newer version exists in the repository.",
             'check-updates': "Check if there is any news on the repositories ChangeLog.txt file.",
             'repo-info': "View information related to repositories, such as which repositories are active, "
                          "when they were upgraded, and how many packages they contain.",
             'configs': "Edit the configuration '/etc/slpkg/slpkg.toml' file.",
             'clean-logs': "Cleans dependencies log tracking. After that procedure you should remove dependencies "
@@ -35,15 +39,16 @@
                       "if you are using '--file-pattern=' option.",
             'find': "Find your installed packages on your system.",
             'view': "View information packages from the repository and get everything in your terminal.",
             'search': "Search and match packages from the repository.",
             'dependees': "Show which packages depend on.",
             'tracking': "Tracking the package dependencies."
         }
-
+        help_commands['-h'] = help_commands['--help']
+        help_commands['-v'] = help_commands['--version']
         help_commands['-u'] = help_commands['update']
         help_commands['-U'] = help_commands['upgrade']
         help_commands['-c'] = help_commands['check-updates']
         help_commands['-I'] = help_commands['repo-info']
         help_commands['-g'] = help_commands['configs']
         help_commands['-L'] = help_commands['clean-logs']
         help_commands['-D'] = help_commands['clean-tmp']
```

### Comparing `slpkg-4.8.4/slpkg/views/views.py` & `slpkg-4.8.6/slpkg/views/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,36 +10,39 @@
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.views.asciibox import AsciiBox
 
 
 class ViewMessage(Configs):
 
-    def __init__(self, flags: list, repository=None, data=None):
+    def __init__(self, flags=None, repository=None, data=None):
         super(Configs, self).__init__()
+        if flags is None:
+            flags: list = []
         self.flags: list = flags
         self.repository = repository
         self.data: dict = data
 
         self.utils = Utilities()
         self.dialogbox = DialogBox()
         self.ascii = AsciiBox()
         self.upgrade = Upgrade(repository, data)
 
         self.download_only = None
+        self.summary_message: str = str()
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-O', '--resolve-off'], flags)
+            ('-O', '--resolve-off'), flags)
 
         self.option_for_reinstall: bool = self.utils.is_option(
-            ['-r', '--reinstall'], flags)
+            ('-r', '--reinstall'), flags)
 
         self.option_for_yes: bool = self.utils.is_option(
-            ['-y', '--yes'], flags)
+            ('-y', '--yes'), flags)
 
     def build_packages(self, slackbuilds: list, dependencies: list) -> None:
         mode: str = 'build'
         self.ascii.draw_package_title('The following packages will be build:',
                                       'slpkg build packages')
 
         for slackbuild in slackbuilds:
@@ -163,15 +166,14 @@
             print(f'{self.yellow}{dep[0]}{self.endc}')
             self.ascii.draw_log_package(dep[1])
 
         print('Note: After cleaning you should remove them one by one.')
 
     def view_summary(self, packages: list, dependencies: list, option: str) -> None:
         packages.extend(dependencies)
-        summary_message: str = str()
         install = upgrade = remove = size_comp = size_uncomp = size_rmv = int()
 
         for pkg in packages:
             installed: str = self.utils.is_package_installed(pkg)
 
             if self.is_binary:
                 # size_comp += int(self.data[pkg][4]) <- It's going to replace with this
@@ -194,41 +196,47 @@
                 upgrade += 1
             elif installed and option == 'remove':
                 remove += 1
 
         self.ascii.draw_bottom_line()
 
         if option in ['install', 'upgrade']:
-            summary_message: str = (
-                f'{self.grey}Total {install} packages will be '
-                f'installed and {upgrade} will be upgraded, and total '
-                f'{self.utils.convert_file_sizes(size_comp)} will be downloaded and '
-                f'{self.utils.convert_file_sizes(size_uncomp)} will be installed.{self.endc} '
-            )
-
+            self.set_summary_for_install_and_upgrade(install, upgrade, size_comp, size_uncomp)
         elif option == 'build':
-            summary_message: str = (
-                f'{self.grey}Total {len(packages)} packages '
-                f'will be build in {self.tmp_path} folder.{self.endc}'
-            )
-
+            self.set_summary_for_build(packages)
         elif option == 'remove':
-            summary_message: str = (
-                f'{self.grey}Total {remove} packages '
-                f'will be removed and {self.utils.convert_file_sizes(size_rmv)} '
-                f'of space will be freed up.{self.endc}'
-            )
-
+            self.set_summary_for_remove(remove, size_rmv)
         elif option == 'download':
-            summary_message: str = (
-                f'{self.grey}Total {len(packages)} packages and {self.utils.convert_file_sizes(size_comp)} '
-                f'will be downloaded in {self.download_only} folder.{self.endc}'
-            )
+            self.set_summary_for_download(packages, size_comp)
+
+        print(self.summary_message)
 
-        print(summary_message)
+    def set_summary_for_install_and_upgrade(self, install: int, upgrade: int, size_comp: int, size_uncomp: int) -> None:
+        self.summary_message: str = (
+            f'{self.grey}Total {install} packages will be '
+            f'installed and {upgrade} will be upgraded, and total '
+            f'{self.utils.convert_file_sizes(size_comp)} will be downloaded and '
+            f'{self.utils.convert_file_sizes(size_uncomp)} will be installed.{self.endc} ')
+
+    def set_summary_for_build(self, packages: list) -> None:
+        self.summary_message: str = (
+            f'{self.grey}Total {len(packages)} packages '
+            f'will be build in {self.tmp_path} folder.{self.endc}')
+
+    def set_summary_for_remove(self, remove: int, size_rmv: int) -> None:
+        self.summary_message: str = (
+            f'{self.grey}Total {remove} packages '
+            f'will be removed and {self.utils.convert_file_sizes(size_rmv)} '
+            f'of space will be freed up.{self.endc}')
+
+    def set_summary_for_download(self, packages: list, size_comp: int) -> None:
+        self.summary_message: str = (
+            f'{self.grey}Total {len(packages)} packages and {self.utils.convert_file_sizes(size_comp)} '
+            f'will be downloaded in {self.download_only} folder.{self.endc}'
+        )
 
     def build_package_and_version(self, package: str) -> str:
         installed_package: str = self.utils.is_package_installed(package)
         version: str = self.utils.split_package(installed_package)['version']
         return f'{package}-{version}'
 
     def view_skipping_packages(self, filename: str) -> None:
```

### Comparing `slpkg-4.8.4/slpkg/checks.py` & `slpkg-4.8.6/slpkg/checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,46 +9,50 @@
 
 from slpkg.models.models import SBoTable, PonceTable, BinariesTable
 
 
 class Check(Configs):
     """ Some checks before proceed. """
 
-    def __init__(self, repository: str, data: dict):
+    def __init__(self, repository: str):
         super(Configs, self).__init__()
-        self.data: dict = data
         self.repository = repository
 
         self.errors = Errors()
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.session = Session
-
+        self.count_rows: int = 0
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
-    def package_exists_in_the_database(self, packages: list) -> None:
+        self.sbo_table: dict = {
+            self.repos.sbo_repo_name: SBoTable,
+            self.repos.ponce_repo_name: PonceTable
+        }
+
+    def package_exists_in_the_database(self, packages: list, data: dict) -> None:
         not_packages: list = []
 
         for pkg in packages:
-            if not self.data.get(pkg) and pkg != '*':
+            if not data.get(pkg) and pkg != '*':
                 not_packages.append(pkg)
 
         if not_packages:
             self.errors.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists",
                                             exit_status=1)
 
-    def is_package_unsupported(self, slackbuilds: list) -> None:
+    def is_package_unsupported(self, slackbuilds: list, data: dict) -> None:
         """ Checking for unsupported slackbuilds. """
         for sbo in slackbuilds:
             if sbo != '*':
-                if self.os_arch == 'x86_64' and self.data[sbo]['download64']:
-                    sources: list = self.data[sbo]['download64'].split()
+                if self.os_arch == 'x86_64' and data[sbo]['download64']:
+                    sources: list = data[sbo]['download64'].split()
                 else:
-                    sources: list = self.data[sbo]['download'].split()
+                    sources: list = data[sbo]['download'].split()
 
                 if 'UNSUPPORTED' in sources:
                     self.errors.raise_error_message(f"Package '{sbo}' unsupported by arch",
                                                     exit_status=1)
 
     def is_package_installed(self, packages: list) -> None:
         """ Checking for installed packages. """
@@ -60,30 +64,31 @@
 
         if not_found:
             self.errors.raise_error_message(f'Not found \'{", ".join(not_found)}\' installed packages',
                                             exit_status=1)
 
     def is_database_empty(self) -> None:
         """ Checking for empty table and database file. """
-        count: int = 0
-        sbo_table: dict = {
-            self.repos.sbo_repo_name: SBoTable,
-            self.repos.ponce_repo_name: PonceTable
-        }
-
         if self.repository == '*':
-            for repository, item in self.repos.repositories.items():
-                if item['path']:
-                    if self.utils.is_binary_repo(repository):
-                        count += self.session.query(BinariesTable.id).where(
-                            BinariesTable.repo == repository).count()
-                    else:
-                        count += self.session.query(sbo_table[repository].id).count()
+            self.count_of_repositories()
         else:
-            if self.is_binary:
-                count: int = self.session.query(BinariesTable.id).where(BinariesTable.repo == self.repository).count()
-            else:
-                count: int = self.session.query(sbo_table[self.repository].id).count()
+            self.count_of_repository()
 
-        if count == 0:
+        if self.count_rows == 0:
             self.errors.raise_error_message("You need to update the package lists first, run:\n\n"
-                                            "              $ slpkg update", exit_status=1)
+                                            f"{'':>14}$ slpkg update", exit_status=1)
+
+    def count_of_repositories(self) -> None:
+        for repository, item in self.repos.repositories.items():
+            if item['path'] and item['enable']:
+                if self.utils.is_binary_repo(repository):
+                    self.count_rows += self.session.query(BinariesTable.id).where(
+                        BinariesTable.repo == repository).count()
+                else:
+                    self.count_rows += self.session.query(self.sbo_table[repository].id).count()
+
+    def count_of_repository(self) -> None:
+        if self.is_binary:
+            self.count_rows: int = self.session.query(
+                BinariesTable.id).where(BinariesTable.repo == self.repository).count()
+        else:
+            self.count_rows: int = self.session.query(self.sbo_table[self.repository].id).count()
```

### Comparing `slpkg-4.8.4/slpkg/logging_deps.py` & `slpkg-4.8.6/slpkg/logging_deps.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,10 +32,10 @@
         if exist:
             self.session.query(
                 LogsDependencies).filter(
                 LogsDependencies.name == name).update(
                 {LogsDependencies.requires: ' '.join(requires)})
 
         elif requires:
-            deps: list = LogsDependencies(name=name, requires=' '.join(requires))
-            self.session.add(deps)
+            dependencies: list = LogsDependencies(name=name, requires=' '.join(requires))
+            self.session.add(dependencies)
         self.session.commit()
```

### Comparing `slpkg-4.8.4/slpkg/new_configs.py` & `slpkg-4.8.6/slpkg/new_configs.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 
     def __init__(self, options: list):
         self.options: list = options
         self.etc_path: Path = Path('/etc/slpkg')
         self.slpkg_config: Path = Path(self.etc_path, 'slpkg.toml')
         self.repositories_config: Path = Path(self.etc_path, 'repositories.toml')
         self.blacklist_config: Path = Path(self.etc_path, 'blacklist.toml')
+        self.rules_config: Path = Path(self.etc_path, 'rules.toml')
         self.slpkg_config_new: Path = Path(self.etc_path, 'slpkg.toml.new')
         self.repositories_config_new: Path = Path(self.etc_path, 'repositories.toml.new')
         self.blacklist_config_new: Path = Path(self.etc_path, 'blacklist.toml.new')
+        self.rules_config_new: Path = Path(self.etc_path, 'rules.toml.new')
 
         self.bold: str = '\033[1m'
         self.red: str = '\x1b[91m'
         self.bred: str = f'{self.bold}{self.red}'
         self.green: str = '\x1b[32m'
         self.bgreen: str = f'{self.bold}{self.green}'
         self.yellow: str = '\x1b[93m'
@@ -53,39 +55,41 @@
             self.violet: str = str()
             self.endc: str = str()
 
     def check(self) -> None:
         """ Checks for .new files. """
         print('\nChecking for NEW configuration files...')
         if (self.slpkg_config_new.is_file() or self.blacklist_config_new.is_file()
-                or self.repositories_config_new.is_file()):
+                or self.repositories_config_new.is_file() or self.rules_config_new.is_file()):
             print('\nThere are NEW files:\n')
 
             if self.slpkg_config_new.is_file():
                 print(f"{self.bgreen:>12}{self.slpkg_config_new}{self.endc}")
 
             if self.repositories_config_new.is_file():
                 print(f"{self.bgreen:>12}{self.repositories_config_new}{self.endc}")
 
             if self.blacklist_config_new.is_file():
                 print(f"{self.bgreen:>12}{self.blacklist_config_new}{self.endc}")
 
+            if self.rules_config_new.is_file():
+                print(f"{self.bgreen:>12}{self.rules_config_new}{self.endc}")
+
             print(f'\nWhat would you like to do ({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                   f'{self.byellow}R{self.endc}/{self.byellow}P{self.endc})?\n')
 
             print(f"{'':>2}({self.byellow}K{self.endc})eep the old files and consider '.new' files later.\n"
                   f"{'':>2}({self.byellow}O{self.endc})verwrite all old files with the new ones.\n"
                   f"{'':>5}The old files will be stored with the suffix '.orig'.\n"
                   f"{'':>2}({self.byellow}R{self.endc})emove all '.new' files.\n"
                   f"{'':>2}({self.byellow}P{self.endc})rompt K, O, R, D, V selection for every single file.\n")
 
             self.menu()
 
-        elif (not self.slpkg_config_new.is_file() and not self.blacklist_config_new.is_file()
-              and not self.repositories_config_new.is_file()):
+        else:
             print(f"\n{'No .new files found.':>23}\n")
 
     def menu(self) -> None:
         """ Menu of choices. """
         choice: str = input('Choice: ')
 
         choice: str = choice.lower()
@@ -112,14 +116,17 @@
             self.overwrite_config_file()
 
         if self.repositories_config_new.is_file():
             self.overwrite_repositories_file()
 
         if self.blacklist_config_new.is_file():
             self.overwrite_blacklist_file()
+
+        if self.rules_config_new.is_file():
+            self.overwrite_rules_file()
         print()  # new line
 
     def overwrite_config_file(self) -> None:
         """ Copy tne slpkg.toml.new file and rename the old to .orig. """
         if self.slpkg_config.is_file():
             shutil.copy(self.slpkg_config, f"{self.slpkg_config}.orig")
             print(f"\ncp {self.green}{self.slpkg_config}{self.endc} -> {self.slpkg_config}.orig")
@@ -141,20 +148,30 @@
         if self.blacklist_config.is_file():
             shutil.copy(self.blacklist_config, f"{self.blacklist_config}.orig")
             print(f"\ncp {self.green}{self.blacklist_config}{self.endc} -> {self.blacklist_config}.orig")
 
         shutil.move(self.blacklist_config_new, self.blacklist_config)
         print(f"mv {self.blacklist_config_new} -> {self.green}{self.blacklist_config}{self.endc}")
 
+    def overwrite_rules_file(self) -> None:
+        """ Copy tne rules.toml.new file and rename the old to .orig. """
+        if self.rules_config.is_file():
+            shutil.copy(self.rules_config, f"{self.rules_config}.orig")
+            print(f"\ncp {self.green}{self.rules_config}{self.endc} -> {self.rules_config}.orig")
+
+        shutil.move(self.rules_config_new, self.rules_config)
+        print(f"mv {self.rules_config_new} -> {self.green}{self.rules_config}{self.endc}")
+
     def remove(self) -> None:
         """ Removes the .new files. """
         print()  # new line
         self.remove_config_new_file()
         self.remove_repositories_new_file()
         self.remove_blacklist_new_file()
+        self.remove_rules_new_file()
         print()  # new line
 
     def remove_config_new_file(self) -> None:
         """ Remove slpkg.toml.new file. """
         if self.slpkg_config_new.is_file():
             self.slpkg_config_new.unlink()
             print(f"rm {self.red}{self.slpkg_config_new}{self.endc}")
@@ -167,14 +184,20 @@
 
     def remove_blacklist_new_file(self) -> None:
         """ Remove blacklist.toml.new file. """
         if self.blacklist_config_new.is_file():
             self.blacklist_config_new.unlink()
             print(f"rm {self.red}{self.blacklist_config_new}{self.endc}")
 
+    def remove_rules_new_file(self) -> None:
+        """ Remove rules.toml.new file. """
+        if self.rules_config_new.is_file():
+            self.rules_config_new.unlink()
+            print(f"rm {self.red}{self.rules_config_new}{self.endc}")
+
     def prompt(self) -> None:
         """ Prompt K, O, R selection for every single file. """
         print(f"\n{'':>2}({self.byellow}K{self.endc})eep, ({self.byellow}O{self.endc})verwrite, "
               f"({self.byellow}R{self.endc})emove, ({self.byellow}D{self.endc})iff, "
               f"({self.byellow}V{self.endc})imdiff\n")
 
         if self.slpkg_config_new.is_file():
@@ -182,15 +205,18 @@
 
         if self.repositories_config_new.is_file():
             self.prompt_repositories_config()
 
         if self.blacklist_config_new.is_file():
             self.prompt_blacklist_config()
 
-    def prompt_slpkg_config(self):
+        if self.rules_config_new.is_file():
+            self.prompt_rules_config()
+
+    def prompt_slpkg_config(self) -> None:
         make: str = input(f'{self.bgreen}{self.slpkg_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
                           f'{self.byellow}V{self.endc}): ')
 
         if make.lower() == 'k':
             pass
@@ -202,15 +228,15 @@
             self.remove_config_new_file()
             print()  # new line
         if make.lower() == 'd':
             self.diff_files(self.slpkg_config_new, self.slpkg_config)
         if make.lower() == 'v':
             self.vimdiff(self.slpkg_config_new, self.slpkg_config)
 
-    def prompt_repositories_config(self):
+    def prompt_repositories_config(self) -> None:
         make: str = input(f'{self.bgreen}{self.repositories_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
                           f'{self.byellow}V{self.endc}): ')
 
         if make.lower() == 'k':
             pass
@@ -222,15 +248,15 @@
             self.remove_repositories_new_file()
             print()  # new line
         if make.lower() == 'd':
             self.diff_files(self.repositories_config_new, self.repositories_config)
         if make.lower() == 'v':
             self.vimdiff(self.repositories_config_new, self.repositories_config)
 
-    def prompt_blacklist_config(self):
+    def prompt_blacklist_config(self) -> None:
         make: str = input(f'{self.bgreen}{self.blacklist_config_new}{self.endc} - '
                           f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
                           f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
                           f'{self.byellow}V{self.endc}): ')
 
         if make.lower() == 'k':
             pass
@@ -242,14 +268,34 @@
             self.remove_blacklist_new_file()
             print()  # new line
         if make.lower() == 'd':
             self.diff_files(self.blacklist_config_new, self.blacklist_config)
         if make.lower() == 'v':
             self.vimdiff(self.blacklist_config_new, self.blacklist_config)
 
+    def prompt_rules_config(self) -> None:
+        make: str = input(f'{self.bgreen}{self.rules_config_new}{self.endc} - '
+                          f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
+                          f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
+                          f'{self.byellow}V{self.endc}): ')
+
+        if make.lower() == 'k':
+            pass
+        if make.lower() == 'o':
+            self.overwrite_rules_file()
+            print()  # new line
+        if make.lower() == 'r':
+            print()  # new line
+            self.remove_rules_new_file()
+            print()  # new line
+        if make.lower() == 'd':
+            self.diff_files(self.rules_config_new, self.rules_config)
+        if make.lower() == 'v':
+            self.vimdiff(self.rules_config_new, self.rules_config)
+
     @staticmethod
     def diff_files(file2: Any, file1: Any) -> None:
         """ Diff the .new and the current file. """
         with open(file1, 'r') as f1:
             with open(file2, 'r') as f2:
                 diff = difflib.context_diff(
                     f1.readlines(),
```

### Comparing `slpkg-4.8.4/slpkg/cleanings.py` & `slpkg-4.8.6/slpkg/cleanings.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,19 @@
                                  SBoTable, PonceTable, BinariesTable,
                                  LastRepoUpdated)
 
 
 class Cleanings(Configs):
     """ Cleans the logs from packages. """
 
-    def __init__(self, flags: list):
+    def __init__(self):
         super(Configs, self).__init__()
-        self.flags: list = flags
         self.session = Session
 
-        self.view = ViewMessage(flags)
+        self.view = ViewMessage()
         self.repos = Repositories()
         self.utils = Utilities()
 
     def tmp(self) -> None:
         print('Deleting of local data:\n')
 
         for file in self.tmp_slpkg.glob('*'):
@@ -78,14 +77,14 @@
         Base.metadata.drop_all(bind=engine, tables=tables)
 
         # Deletes local downloaded data.
         self.delete_repositories_data()
 
         print(f"{self.byellow}Successfully cleared!{self.endc}\n\n"
               "You need to update the package lists now:\n\n"
-              "  $ slpkg update\n")
+              f"{'':>2}$ slpkg update\n")
 
     def delete_repositories_data(self) -> None:
         """ Deletes local folders with the repository downloaded data. """
         for item in self.repos.repositories.values():
             if item['path'].exists() and isinstance(item['path'], PosixPath):
                 shutil.rmtree(item['path'])
```

### Comparing `slpkg-4.8.4/slpkg/checksum.py` & `slpkg-4.8.6/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/dialog_box.py` & `slpkg-4.8.6/slpkg/dialog_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         more_kwargs: dict = {}
 
         if self.dialog:
             more_kwargs.update({"item_help": True})
 
             code, tags = self.d.checklist(text=text, choices=choices, title=title, height=height,  width=width,
                                           list_height=list_height, help_status=True, **more_kwargs)
-
         else:
             code: bool = False
             tags: list = packages
 
         return code, tags
 
     def mixedform(self, text: str, title: str, elements: list, height: int, width: int) -> Tuple[bool, list]:
```

### Comparing `slpkg-4.8.4/slpkg/configs.py` & `slpkg-4.8.6/slpkg/configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/utilities.py` & `slpkg-4.8.6/slpkg/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,22 +74,21 @@
         name: str = '-'.join(package.split('-')[:-3])
         version: str = ''.join(package[len(name):].split('-')[:-2])
         arch: str = ''.join(package[len(name + version) + 2:].split('-')[:-1])
         build_tag: str = package.split('-')[-1]
         build: str = ''.join(re.findall(r'\d+', build_tag[:2]))
         pkg_tag: str = build_tag[len(build):]
 
-        split: dict[str] = {
+        return {
             'name': name,
             'version': version,
             'arch': arch,
             'build': build,
             'tag': pkg_tag
         }
-        return split
 
     def finished_time(self, elapsed_time: float) -> None:
         """ Printing the elapsed time. """
         print(f'\n{self.yellow}Finished successfully:{self.endc}',
               time.strftime(f'{self.cyan}%H:%M:%S{self.endc}',
                             time.gmtime(elapsed_time)))
 
@@ -103,15 +102,15 @@
 
             for line in lines:
                 if line.startswith('BUILD=$'):
                     build = ''.join(re.findall(r'\d+', line))
         return build
 
     @staticmethod
-    def is_option(options: list, flags: list) -> bool:
+    def is_option(options: tuple, flags: list) -> bool:
         """ Checking if the option is applied. """
         for option in options:
             if option in flags:
                 return True
 
     def read_packages_from_file(self, file: Path) -> Generator:
         """ Reads packages from file and split these to list. """
@@ -189,23 +188,24 @@
 
     def is_binary_repo(self, repo: str) -> bool:
         """ Checks if the repository is binary. """
         if repo in tuple(self.repos.repositories.keys())[2:]:
             return True
 
     @staticmethod
-    def change_owner_privileges(folder: Path):
+    def change_owner_privileges(folder: Path) -> None:
         """ Changes thw owner privileges. """
         os.chown(folder, 0, 0)
         for file in os.listdir(folder):
             os.chown(Path(folder, file), 0, 0)
 
     @staticmethod
     def case_insensitive_pattern_matching(packages: list, data: dict) -> list:
         """ Case-insensitive pattern matching packages. """
         repo_packages: tuple = tuple(data.keys())
         for package in packages:
             for pkg in repo_packages:
-                if package == pkg.lower():
+                if package.lower() == pkg.lower():
                     packages.append(pkg)
                     packages.remove(package)
+                    break
         return packages
```

### Comparing `slpkg-4.8.4/slpkg/dependees.py` & `slpkg-4.8.6/slpkg/dependees.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,18 @@
         self.hl: str = self.ascii.horizontal_line
         self.var: str = self.ascii.vertical_and_right
         self.package_version: str = str()
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_full_reverse: bool = self.utils.is_option(
-            ['-E', '--full-reverse'], flags)
+            ('-E', '--full-reverse'), flags)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
-            ['-p', '--pkg-version'], flags)
+            ('-p', '--pkg-version'), flags)
 
     def find(self) -> None:
         self.view_the_title()
 
         for package in self.packages:
             dependees: dict = dict(self.find_requires(package))
             self.view_the_main_package(package)
@@ -84,14 +84,14 @@
 
             self.view_dependency_line(n, dependency)
 
             if self.option_for_full_reverse:
                 self.view_full_reverse(n, dependees, requires)
 
     def view_full_reverse(self, n: int, dependees: dict, requires: str) -> None:
-        str_requires: str = f"{'':>5}{self.var}{self.hl} {self.violet}{requires}{self.endc}"
+        line_requires: str = f"{'':>5}{self.var}{self.hl} {self.violet}{requires}{self.endc}"
         if n == len(dependees):
-            str_requires: str = f"{'':>5}{self.llc}{self.hl} {self.violet}{requires}{self.endc}"
-        print(str_requires)
+            line_requires: str = f"{'':>5}{self.llc}{self.hl} {self.violet}{requires}{self.endc}"
+        print(line_requires)
 
     def view_summary_of_dependees(self, dependees: dict, package: str) -> None:
         print(f'\n{self.grey}{len(dependees)} dependees for {package}{self.endc}\n')
```

### Comparing `slpkg-4.8.4/slpkg/toml_error_message.py` & `slpkg-4.8.6/slpkg/toml_error_message.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/check_updates.py` & `slpkg-4.8.6/slpkg/check_updates.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.http = PoolManager()
         self.proxy_default_headers = make_headers(
             proxy_basic_auth=f'{self.proxy_username}:{self.proxy_password}')
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_repository: bool = self.utils.is_option(
-            ['-o', '--repository='], flags)
+            ('-o', '--repository='), flags)
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
 
     def check_the_repositories(self) -> dict:
@@ -140,22 +140,22 @@
         if True not in self.compare.values():
             print(f'\n{self.endc}{self.yellow}No updated packages since the last check.{self.endc}')
 
     def updates(self) -> None:
         message: str = 'Checking for news, please wait...'
 
         # Starting multiprocessing
-        p1 = Process(target=self.check_for_updates)
-        p2 = Process(target=self.progress.progress_bar, args=(message,))
+        process_1 = Process(target=self.check_for_updates)
+        process_2 = Process(target=self.progress.progress_bar, args=(message,))
 
-        p1.start()
-        p2.start()
+        process_1.start()
+        process_2.start()
 
         # Wait until process 1 finish
-        p1.join()
+        process_1.join()
 
         # Terminate process 2 if process 1 finished
-        if not p1.is_alive():
-            p2.terminate()
+        if not process_1.is_alive():
+            process_2.terminate()
 
         # Restore the terminal cursor
         print('\x1b[?25h', self.endc)
```

### Comparing `slpkg-4.8.4/slpkg/remove_packages.py` & `slpkg-4.8.6/slpkg/remove_packages.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,18 @@
         self.packages_for_remove: list = []
         self.installed_dependencies: list = []
         self.dependencies: list = []
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-O', '--resolve-off'], flags)
+            ('-O', '--resolve-off'), flags)
 
         self.option_for_yes: bool = self.utils.is_option(
-            ['-y', '--yes'], flags)
+            ('-y', '--yes'), flags)
 
     def remove(self) -> None:
         self.query_logs_dependencies()
         self.add_packages_for_remove()
         self.save_dependencies_for_remove()
         self.remove_doubles_dependencies()
         self.remove_doubles_installed_dependencies()
@@ -77,27 +77,28 @@
                         installed: str = self.utils.is_package_installed(require)
                         if installed and require not in self.packages:
                             self.dependencies.append(require)
 
     def remove_doubles_dependencies(self) -> None:
         self.dependencies: list = list(set(self.dependencies))
 
-    def remove_doubles_installed_dependencies(self):
+    def remove_doubles_installed_dependencies(self) -> None:
         self.installed_dependencies: list = list(set(self.installed_dependencies))
 
-    def update_installed_dependencies_for_remove(self):
+    def update_installed_dependencies_for_remove(self) -> None:
         for dependency in self.dependencies:
             installed: str = self.utils.is_package_installed(dependency)
             if installed and dependency not in self.packages:
                 self.installed_dependencies.append(installed)
 
     def add_installed_dependencies_to_remove(self) -> None:
         self.packages_for_remove.extend(self.installed_dependencies)
 
     def remove_packages(self) -> None:
+        print(f'Started of removing total ({self.cyan}{len(self.packages_for_remove)}{self.endc}) packages:\n')
         for package in self.packages_for_remove:
             command: str = f'{self.removepkg} {package}'
             name: str = self.utils.split_package(package)['name']
             progress_message: str = f'{self.bold}{self.red}Removing{self.endc}'
 
             dependencies: list = self.is_dependency(name)
             if dependencies:
```

### Comparing `slpkg-4.8.4/slpkg/blacklist.py` & `slpkg-4.8.6/slpkg/blacklist.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 # -*- coding: utf-8 -*-
 
 import tomli
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.toml_error_message import TomlErrors
-from slpkg.models.models import session as Session
 
 
 class Blacklist(Configs):
     """ Reads and returns the blacklist. """
 
     def __init__(self):
         super(Configs, self).__init__()
-        self.session = Session
 
         self.errors = TomlErrors()
         self.blacklist_file_toml = Path(self.etc_path, 'blacklist.toml')
 
-    def packages(self) -> list:
+    def packages(self) -> tuple:
         """ Reads the blacklist file. """
+        packages: tuple = tuple()
         if self.blacklist_file_toml.is_file():
             try:
                 with open(self.blacklist_file_toml, 'rb') as black:
-                    return tomli.load(black)['BLACKLIST']['PACKAGES']
+                    packages: tuple = tuple(tomli.load(black)['BLACKLIST']['PACKAGES'])
             except (tomli.TOMLDecodeError, KeyError) as error:
                 self.errors.raise_toml_error_message(error, self.blacklist_file_toml)
 
-        return []
+        return packages
```

### Comparing `slpkg-4.8.4/slpkg/download_only.py` & `slpkg-4.8.6/slpkg/download_only.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.sbo_repo: dict = {
             self.repos.sbo_repo_name: self.repos.sbo_repo_path,
             self.repos.ponce_repo_name: self.repos.ponce_repo_path
         }
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
         self.option_for_directory: bool = self.utils.is_option(
-            ['-z', '--directory='], flags)
+            ('-z', '--directory='), flags)
 
     def packages(self, packages: list) -> None:
         packages: list = self.utils.apply_package_pattern(self.data, packages)
         self.view.download_packages(packages, self.directory)
         self.view.question()
         self.set_download_path()
         start: float = time.time()
@@ -81,10 +81,11 @@
     def copy_slackbuild_scripts(self, name: str) -> None:
         repo_path_package: Path = Path(self.sbo_repo[self.repository], self.data[name]['location'], name)
         if not Path(self.download_path, name).is_dir():
             shutil.copytree(repo_path_package, Path(self.download_path, name))
         print(f"{self.byellow}Copying{self.endc}: {repo_path_package} -> {Path(self.download_path, name)}")
 
     def download_the_sources(self) -> None:
-        print('\nDownloading the sources:')
-        down = Downloader(self.download_path, self.urls, self.flags)
-        down.download()
+        if self.urls:
+            print(f'\nStarted to download total ({self.cyan}{len(self.urls)}{self.endc}) sources:\n')
+            down = Downloader(self.download_path, self.urls, self.flags)
+            down.download()
```

### Comparing `slpkg-4.8.4/slpkg/tracking.py` & `slpkg-4.8.6/slpkg/tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,20 @@
         self.vl: str = self.ascii.vertical_line
         self.package_version: str = str()
         self.package_dependency_version: str = str()
         self.package_requires: tuple = tuple()
         self.package_line: str = str()
         self.require_line: str = str()
         self.count_requires: int = 0
+        self.require_length: int = 0
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
-            ['-p', '--pkg-version'], flags)
+            ('-p', '--pkg-version'), flags)
 
     def package(self) -> None:
         self.view_the_title()
 
         for package in self.packages:
             self.count_requires: int = 0
 
@@ -76,15 +77,15 @@
             self.set_package_version(package)
             self.package_line: str = f'{self.yellow}{package} {self.package_version}{self.endc}'
 
     def set_the_package_require_line(self, require: str) -> None:
         self.require_line: str = f'{self.cyan}{require}{self.endc}'
         if self.option_for_pkg_version:
             self.set_package_dependency_version(require)
-            self.require_line: str = (f'{self.cyan}{require}{self.endc}'
+            self.require_line: str = (f'{self.cyan}{require:<{self.require_length}}{self.endc}'
                                       f'{self.package_dependency_version}')
 
     def set_package_dependency_version(self, require: str) -> None:
         try:
             self.package_dependency_version: str = f"{'':>1}(not included)"
             if self.data.get(require):
                 self.package_dependency_version: str = f"{'':>1}{self.yellow}{self.data[require]['version']}{self.endc}"
@@ -92,10 +93,12 @@
             self.package_dependency_version: str = str()
 
     def set_package_version(self, package: str) -> None:
         self.package_version: str = self.data[package]['version']
 
     def set_package_requires(self, package: str) -> None:
         self.package_requires: tuple = self.data[package]['requires'].split()
+        if self.package_requires:
+            self.require_length: int = max(len(name) for name in self.package_requires)
 
     def view_summary_of_tracking(self, package: str) -> None:
         print(f'\n{self.grey}{self.count_requires} dependencies for {package}{self.endc}\n')
```

### Comparing `slpkg-4.8.4/slpkg/logging_config.py` & `slpkg-4.8.6/slpkg/logging_config.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.4/slpkg/main.py` & `slpkg-4.8.6/slpkg/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,33 +30,28 @@
 from slpkg.logging_config import LoggingConfig
 from slpkg.find_installed import FindInstalled
 from slpkg.views.view_package import ViewPackage
 from slpkg.remove_packages import RemovePackages
 from slpkg.update_repository import UpdateRepository
 
 
-class Argparse(Configs):
+class Menu(Configs):
 
     def __init__(self, args: list):
         super(Configs).__init__()
         self.args: list = args
         self.flags: list = []
         self.directory: Path = self.tmp_slpkg
 
-        self.dialogbox = DialogBox()
         self.utils = Utilities()
         self.usage = Usage()
-        self.form_configs = FormConfigs()
         self.repos = Repositories()
 
         self.repository: str = self.repos.default_repository
 
-        if len(args) == 0 or '' in args:
-            self.usage.help_short(1)
-
         self.data: dict = {}
         self.flag_yes: str = '--yes'
         self.flag_short_yes: str = '-y'
         self.flag_jobs: str = '--jobs'
         self.flag_short_jobs: str = '-j'
         self.flag_resolve_off: str = '--resolve-off'
         self.flag_short_resolve_off: str = '-O'
@@ -79,25 +74,25 @@
         self.flag_no_case: str = '--no-case'
         self.flag_short_no_case: str = '-m'
         self.flag_repository: str = '--repository='
         self.flag_short_repository: str = '-o'
         self.flag_directory: str = '--directory='
         self.flag_short_directory: str = '-z'
 
-        self.flag_searches: list = [
+        self.flag_searches: tuple = (
             self.flag_short_search,
             self.flag_search
-        ]
+        )
 
-        self.flag_no_cases: list = [
+        self.flag_no_cases: tuple = (
             self.flag_no_case,
             self.flag_short_no_case
-        ]
+        )
 
-        self.options: list = [
+        self.options: tuple = (
             self.flag_yes,
             self.flag_short_yes,
             self.flag_jobs,
             self.flag_short_jobs,
             self.flag_resolve_off,
             self.flag_short_resolve_off,
             self.flag_reinstall,
@@ -118,15 +113,15 @@
             self.flag_short_parallel,
             self.flag_no_case,
             self.flag_short_no_case,
             self.flag_repository,
             self.flag_short_repository,
             self.flag_directory,
             self.flag_short_directory,
-        ]
+        )
 
         self.commands: dict = {
             '--help': [],
             '--version': [],
             'help': [],
             'update': [
                 self.flag_yes,
@@ -159,22 +154,16 @@
                 self.flag_short_repository
             ],
             'repo-info': [
                 self.flag_repository,
                 self.flag_short_repository
             ],
             'configs': [],
-            'clean-logs': [
-                self.flag_yes,
-                self.flag_short_yes
-            ],
-            'clean-data': [
-                self.flag_yes,
-                self.flag_short_yes
-            ],
+            'clean-logs': [],
+            'clean-data': [],
             'clean-tmp': [],
             'build': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_jobs,
                 self.flag_short_jobs,
                 self.flag_resolve_off,
@@ -307,38 +296,39 @@
         self.split_options()
         self.split_options_from_args()
         self.move_options()
         self.invalid_options()
         self.check_for_repositories()
 
         self.is_binary: bool = self.utils.is_binary_repo(self.repository)
-
-        if self.repository != '*':
-            if self.is_binary:
-                self.data: dict = BinQueries(self.repository).repository_data()
-            else:
-                self.data: dict = SBoQueries(self.repository).repository_data()
-
-        self.check = Check(self.repository, self.data)
+        self.check = Check(self.repository)
+        self.choose = ChoosePackages(self.repository)
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
 
         logger = logging.getLogger(LoggingConfig.date_time)
         logger.info(f'{self.__class__.__name__}: '
                     f'{self.__class__.__init__.__name__}: '
                     f'{args=}, {self.flags=}, {self.repository=}')
 
+    def load_database(self):
+        if self.repository != '*' and not self.data:
+            if self.is_binary:
+                self.data: dict = BinQueries(self.repository).repository_data()
+            else:
+                self.data: dict = SBoQueries(self.repository).repository_data()
+
     def check_for_repositories(self) -> None:
         """ Checks combination for binaries use repositories only and if repository exists. """
-        except_options: list = [
+        except_options: tuple = (
             '-s', 'search',
-        ]
+        )
         if self.repository == '*' and not self.utils.is_option(except_options, self.args):
             self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
         elif self.repository not in list(self.repos.repositories.keys()) and self.repository != '*':
             self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
         if self.repository != '*':
@@ -409,31 +399,35 @@
         """
         for arg in self.args:
 
             if arg.startswith(self.flag_directory):
                 self.directory: str = arg.split('=')[1]
                 self.args.remove(arg)
                 self.args.append(self.flag_directory)
+                break
 
             try:
                 if arg.startswith(self.flag_short_directory):
                     self.directory: str = self.args[self.args.index(arg) + 1]
                     self.args.remove(self.directory)
+                    break
             except IndexError:
                 self.directory: Path = self.tmp_slpkg
 
             if arg.startswith(self.flag_repository):
                 self.repository: str = arg.split('=')[1]
                 self.args.remove(arg)
                 self.args.append(self.flag_repository)
+                break
 
             try:
                 if arg.startswith(self.flag_short_repository):
                     self.repository: str = self.args[self.args.index(arg) + 1]
                     self.args.remove(self.repository)
+                    break
             except IndexError:
                 self.repository: str = str()
 
     def move_options(self) -> None:
         """ Move options to the flags and removes from the arguments. """
         new_args: list = []
 
@@ -451,109 +445,32 @@
             file = Path(self.args[1])
             packages: list = list(self.utils.read_packages_from_file(file))
         else:
             packages: list = list(set(self.args[1:]))
 
         return packages
 
-    def choose_packages(self, packages: list, method: str) -> list:
-        """ Choose packages with dialog utility and -S, --search flag. """
-        height: int = 10
-        width: int = 70
-        list_height: int = 0
-        choices: list = []
-        title: str = f' Choose packages you want to {method} '
-
-        repo_packages: list = list(self.data.keys())
-
-        if method in ['remove', 'find']:
-            installed: list = list(self.utils.installed_packages.values())
-
-            for package in installed:
-                package_name: str = self.utils.split_package(package)['name']
-                package_version: str = self.utils.split_package(package)['version']
-
-                for pkg in packages:
-                    if pkg in package or pkg == '*':
-                        choices.extend([(package_name, package_version, False, f'Package: {package}')])
-
-        elif method == 'upgrade':
-            for pkg in packages:
-                for package in repo_packages:
-
-                    if pkg == package:
-                        inst_pkg: str = self.utils.is_package_installed(package)
-                        inst_package_version: str = self.utils.split_package(inst_pkg)['version']
-                        inst_package_build: str = self.utils.split_package(inst_pkg)['build']
-                        repo_ver: str = self.data[package]['version']
-
-                        if self.is_binary:
-                            bin_pkg: str = self.data[package]['package']
-                            repo_build_tag: str = self.utils.split_package(bin_pkg[:-4])['build']
-                        else:
-                            repo_location: str = self.data[package]['location']
-                            repo_build_tag: str = self.utils.read_slackbuild_build_tag(
-                                package, repo_location, self.repository
-                            )
-
-                        choices.extend([(package, f'{inst_package_version} -> {repo_ver}', True,
-                                         f'Installed: {package}-{inst_package_version} Build: {inst_package_build} -> '
-                                        f'Available: {repo_ver} Build: {repo_build_tag}')])
-        else:
-            for pkg in packages:
-                for package in repo_packages:
-
-                    if pkg in package or pkg == '*':
-                        version: str = self.data[package]['version']
-                        choices.extend([(package, version, False, f'Package: {package}-{version} '
-                                       f'> {self.repository}')])
-
-        if not choices:
-            return packages
-
-        text: str = f'There are {len(choices)} packages:'
-        code, packages = self.dialogbox.checklist(text, packages, title, height,
-                                                  width, list_height, choices)
-        if code == 'cancel' or not packages:
-            os.system('clear')
-            raise SystemExit()
-
-        os.system('clear')
-
-        return packages
-
-    def help(self) -> None:
-        if len(self.args) == 1:
-            self.usage.help(0)
-        self.usage.help_short(1)
-
-    def version(self) -> None:
-        if len(self.args) == 1:
-            version = Version()
-            version.view()
-            raise SystemExit()
-        self.usage.help_short(1)
-
     def update(self) -> None:
         if len(self.args) == 1:
             update = UpdateRepository(self.flags, self.repository)
             update.repositories()
             raise SystemExit()
         self.usage.help_short(1)
 
     def upgrade(self) -> None:
-        command: str = Argparse.upgrade.__name__
+        command: str = Menu.upgrade.__name__
 
         if len(self.args) == 1:
+            self.load_database()
             self.check.is_database_empty()
 
             upgrade = Upgrade(self.repository, self.data)
             packages: list = list(upgrade.packages())
 
-            packages: list = self.choose_packages(packages, command)
+            packages: list = self.choose.packages(self.data, packages, command)
 
             if not packages:
                 print('\nEverything is up-to-date!\n')
                 raise SystemExit()
 
             if self.is_binary:
                 install = Packages(
@@ -578,222 +495,205 @@
     def repo_info(self) -> None:
         if len(self.args) == 1:
             repo = RepoInfo(self.flags, self.repository)
             repo.info()
             raise SystemExit()
         self.usage.help_short(1)
 
-    def edit_configs(self) -> None:
-        if len(self.args) == 1:
-            self.form_configs.edit()
-            raise SystemExit()
-        self.usage.help_short(1)
-
-    def clean_logs(self) -> None:
-        if len(self.args) == 1:
-            clean = Cleanings(self.flags)
-            clean.logs_dependencies()
-            raise SystemExit()
-        self.usage.help_short(1)
-
-    def clean_tmp(self) -> None:
-        if len(self.args) == 1:
-            clean = Cleanings(self.flags)
-            clean.tmp()
-            raise SystemExit()
-        self.usage.help_short(1)
-
-    def clean_data(self) -> None:
-        if len(self.args) == 1:
-            clean = Cleanings(self.flags)
-            clean.db_tables()
-            raise SystemExit()
-        self.usage.help_short(1)
-
     def build(self) -> None:
-        command: str = Argparse.build.__name__
+        command: str = Menu.build.__name__
 
         if len(self.args) >= 2:
+            self.load_database()
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
                 packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
 
             if self.utils.is_option(self.flag_searches, self.flags):
-                packages: list = self.choose_packages(packages, command)
+                packages: list = self.choose.packages(self.data, packages, command)
 
-            self.check.package_exists_in_the_database(packages)
-            self.check.is_package_unsupported(packages)
+            self.check.package_exists_in_the_database(packages, self.data)
+            self.check.is_package_unsupported(packages, self.data)
 
             if self.repository in list(self.repos.repositories.keys())[:2]:
                 build = Slackbuilds(
                     self.repository, self.data, packages, self.flags, mode=command
                 )
                 build.execute()
             else:
                 self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
             raise SystemExit()
         self.usage.help_short(1)
 
     def install(self) -> None:
-        command: str = Argparse.install.__name__
+        command: str = Menu.install.__name__
 
         if len(self.args) >= 2:
+            self.load_database()
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
                 packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
 
             if self.utils.is_option(self.flag_searches, self.flags):
-                packages: list = self.choose_packages(packages, command)
+                packages: list = self.choose.packages(self.data, packages, command)
 
-            self.check.package_exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages, self.data)
 
             if self.is_binary:
                 install = Packages(self.repository, self.data, packages, self.flags, mode=command)
                 install.execute()
             else:
-                self.check.is_package_unsupported(packages)
+                self.check.is_package_unsupported(packages, self.data)
                 install = Slackbuilds(self.repository, self.data, packages, self.flags, mode=command)
                 install.execute()
             raise SystemExit()
         self.usage.help_short(1)
 
     def download(self) -> None:
-        command: str = Argparse.download.__name__
+        command: str = Menu.download.__name__
 
         if len(self.args) >= 2:
+            self.load_database()
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
                 packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
 
             if self.utils.is_option(self.flag_searches, self.flags):
-                packages: list = self.choose_packages(packages, command)
+                packages: list = self.choose.packages(self.data, packages, command)
 
-            self.check.package_exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages, self.data)
             down_only = DownloadOnly(self.directory, self.flags, self.data, self.repository)
             down_only.packages(packages)
             raise SystemExit()
         self.usage.help_short(1)
 
     def remove(self) -> None:
-        command: str = Argparse.remove.__name__
+        command: str = Menu.remove.__name__
 
         if len(self.args) >= 2:
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
-                packages: list = self.choose_packages(packages, command)
+                packages: list = self.choose.packages(self.data, packages, command)
 
             self.check.is_package_installed(packages)
 
             remove = RemovePackages(packages, self.flags)
             remove.remove()
             raise SystemExit()
         self.usage.help_short(1)
 
     def find(self) -> None:
-        command: str = Argparse.find.__name__
+        command: str = Menu.find.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                self.load_database()
                 packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
 
             if self.utils.is_option(self.flag_searches, self.flags):
-                packages: list = self.choose_packages(packages, command)
+                self.load_database()
+                packages: list = self.choose.packages(self.data, packages, command)
 
             find = FindInstalled(self.flags, packages)
             find.find()
             raise SystemExit()
         self.usage.help_short(1)
 
     def view(self) -> None:
-        command: str = Argparse.view.__name__
+        command: str = Menu.view.__name__
 
         if len(self.args) >= 2:
+            self.load_database()
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
                 packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
 
             if self.utils.is_option(self.flag_searches, self.flags):
-                packages: list = self.choose_packages(packages, command)
+                packages: list = self.choose.packages(self.data, packages, command)
 
-            self.check.package_exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages, self.data)
 
             view = ViewPackage(self.flags, self.repository)
 
             if self.is_binary:
                 view.package(self.data, packages)
             else:
                 view.slackbuild(self.data, packages)
             raise SystemExit()
         self.usage.help_short(1)
 
     def search(self) -> None:
-        command: str = Argparse.search.__name__
+        command: str = Menu.search.__name__
 
         if len(self.args) >= 2:
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
+                self.load_database()
                 packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
 
             if self.utils.is_option(self.flag_searches, self.flags):
-                packages: list = self.choose_packages(packages, command)
+                self.load_database()
+                packages: list = self.choose.packages(self.data, packages, command)
 
-            pkgs = SearchPackage(self.flags, self.data, packages, self.repository)
+            pkgs = SearchPackage(self.flags, packages, self.repository)
             pkgs.search()
             raise SystemExit()
         self.usage.help_short(1)
 
     def dependees(self) -> None:
-        command: str = Argparse.dependees.__name__
+        command: str = Menu.dependees.__name__
 
         if len(self.args) >= 2:
+            self.load_database()
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
                 packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
 
             if self.utils.is_option(self.flag_searches, self.flags):
-                packages: list = self.choose_packages(packages, command)
+                packages: list = self.choose.packages(self.data, packages, command)
 
-            self.check.package_exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages, self.data)
 
             dependees = Dependees(self.data, packages, self.flags, self.repository)
             dependees.find()
             raise SystemExit()
         self.usage.help_short(1)
 
     def tracking(self) -> None:
-        command: str = Argparse.tracking.__name__
+        command: str = Menu.tracking.__name__
 
         if len(self.args) >= 2:
+            self.load_database()
             self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_no_cases, self.flags) or not self.case_sensitive:
                 packages: list = self.utils.case_insensitive_pattern_matching(packages, self.data)
 
             if self.utils.is_option(self.flag_searches, self.flags):
-                packages: list = self.choose_packages(packages, command)
+                packages: list = self.choose.packages(self.data, packages, command)
 
-            self.check.package_exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages, self.data)
 
             tracking = Tracking(self.data, packages, self.flags, self.repository)
             tracking.package()
             raise SystemExit()
         self.usage.help_short(1)
 
     def help_for_commands(self) -> None:
@@ -807,61 +707,198 @@
                 logger.exception(f'{self.__class__.__name__}: '
                                  f'{self.__class__.help_for_commands.__name__}')
                 self.usage.help_minimal(f"{self.prog_name}: invalid argument '{''.join(self.args[1])}'")
         else:
             self.usage.help_short(1)
 
 
+class SubMenu:
+    """ Sub menu that separate from the main menu because of
+    have no options to manage here. """
+
+    def __init__(self, args: list):
+        self.args: list = args
+        self.usage = Usage()
+        self.form_configs = FormConfigs()
+        self.clean = Cleanings()
+
+    def help(self) -> None:
+        if len(self.args) == 1:
+            self.usage.help(0)
+        self.usage.help_short(1)
+
+    def version(self) -> None:
+        if len(self.args) == 1:
+            version = Version()
+            version.view()
+            raise SystemExit()
+        self.usage.help_short(1)
+
+    def edit_configs(self) -> None:
+        if len(self.args) == 1:
+            self.form_configs.edit()
+            raise SystemExit()
+        self.usage.help_short(1)
+
+    def clean_logs(self) -> None:
+        if len(self.args) == 1:
+            self.clean.logs_dependencies()
+            raise SystemExit()
+        self.usage.help_short(1)
+
+    def clean_tmp(self) -> None:
+        if len(self.args) == 1:
+            self.clean.tmp()
+            raise SystemExit()
+        self.usage.help_short(1)
+
+    def clean_data(self) -> None:
+        if len(self.args) == 1:
+            self.clean.db_tables()
+            raise SystemExit()
+        self.usage.help_short(1)
+
+
+class ChoosePackages:
+    """ Choose packages with dialog utility and -S, --search flag. """
+
+    def __init__(self, repository: str):
+        self.repository: str = repository
+
+        self.utils = Utilities()
+        self.dialogbox = DialogBox()
+
+        self.is_binary: bool = self.utils.is_binary_repo(repository)
+
+    def packages(self, data: dict, packages: list, method: str) -> list:
+        height: int = 10
+        width: int = 70
+        list_height: int = 0
+        choices: list = []
+        title: str = f' Choose packages you want to {method} '
+
+        repo_packages: list = list(data.keys())
+
+        if method in ['remove', 'find']:
+            installed: list = list(self.utils.installed_packages.values())
+
+            for package in installed:
+                package_name: str = self.utils.split_package(package)['name']
+                package_version: str = self.utils.split_package(package)['version']
+
+                for pkg in packages:
+                    if pkg in package or pkg == '*':
+                        choices.extend([(package_name, package_version, False, f'Package: {package}')])
+
+        elif method == 'upgrade':
+            for pkg in packages:
+                for package in repo_packages:
+
+                    if pkg == package:
+                        inst_pkg: str = self.utils.is_package_installed(package)
+                        inst_package_version: str = self.utils.split_package(inst_pkg)['version']
+                        inst_package_build: str = self.utils.split_package(inst_pkg)['build']
+                        repo_ver: str = data[package]['version']
+
+                        if self.is_binary:
+                            bin_pkg: str = data[package]['package']
+                            repo_build_tag: str = self.utils.split_package(bin_pkg[:-4])['build']
+                        else:
+                            repo_location: str = data[package]['location']
+                            repo_build_tag: str = self.utils.read_slackbuild_build_tag(
+                                package, repo_location, self.repository
+                            )
+
+                        choices.extend([(package, f'{inst_package_version} -> {repo_ver}', True,
+                                         f'Installed: {package}-{inst_package_version} Build: {inst_package_build} -> '
+                                        f'Available: {repo_ver} Build: {repo_build_tag}')])
+        else:
+            for pkg in packages:
+                for package in repo_packages:
+
+                    if pkg in package or pkg == '*':
+                        version: str = data[package]['version']
+                        choices.extend([(package, version, False, f'Package: {package}-{version} '
+                                       f'> {self.repository}')])
+
+        if not choices:
+            return packages
+
+        text: str = f'There are {len(choices)} packages:'
+        code, packages = self.dialogbox.checklist(text, packages, title, height,
+                                                  width, list_height, choices)
+        if code == 'cancel' or not packages:
+            os.system('clear')
+            raise SystemExit()
+
+        os.system('clear')
+
+        return packages
+
+
 def main() -> None:
     args: list = sys.argv
     args.pop(0)
-
     usage = Usage()
-    argparse = Argparse(args)
 
+    if len(args) == 0 or '' in args:
+        usage.help_short(1)
+
+    sub_menu = SubMenu(args)
+    arguments_no_options: dict[str] = {
+        '-h': sub_menu.help,
+        '--help': sub_menu.help,
+        '-v': sub_menu.version,
+        '--version': sub_menu.version,
+        'configs': sub_menu.edit_configs,
+        '-g': sub_menu.edit_configs,
+        'clean-logs': sub_menu.clean_logs,
+        '-L': sub_menu.clean_logs,
+        'clean-data': sub_menu.clean_data,
+        '-T': sub_menu.clean_data,
+        'clean-tmp': sub_menu.clean_tmp,
+        '-D': sub_menu.clean_tmp
+    }
+
+    try:
+        arguments_no_options[args[0]]()
+    except (KeyError, IndexError):
+        pass
+    except KeyboardInterrupt:
+        raise SystemExit(1)
+
+    menu = Menu(args)
     arguments: dict[str] = {
-        '-h': argparse.help,
-        '--help': argparse.help,
-        '-v': argparse.version,
-        '--version': argparse.version,
-        'help': argparse.help_for_commands,
-        'update': argparse.update,
-        '-u': argparse.update,
-        'upgrade': argparse.upgrade,
-        '-U': argparse.upgrade,
-        'check-updates': argparse.check_updates,
-        '-c': argparse.check_updates,
-        'repo-info': argparse.repo_info,
-        '-I': argparse.repo_info,
-        'configs': argparse.edit_configs,
-        '-g': argparse.edit_configs,
-        'clean-logs': argparse.clean_logs,
-        '-L': argparse.clean_logs,
-        'clean-data': argparse.clean_data,
-        '-T': argparse.clean_data,
-        'clean-tmp': argparse.clean_tmp,
-        '-D': argparse.clean_tmp,
-        'build': argparse.build,
-        '-b': argparse.build,
-        'install': argparse.install,
-        '-i': argparse.install,
-        'download': argparse.download,
-        '-d': argparse.download,
-        'remove': argparse.remove,
-        '-R': argparse.remove,
-        'view': argparse.view,
-        '-w': argparse.view,
-        'find': argparse.find,
-        '-f': argparse.find,
-        'search': argparse.search,
-        '-s': argparse.search,
-        'dependees': argparse.dependees,
-        '-e': argparse.dependees,
-        'tracking': argparse.tracking,
-        '-t': argparse.tracking
+        'help': menu.help_for_commands,
+        'update': menu.update,
+        '-u': menu.update,
+        'upgrade': menu.upgrade,
+        '-U': menu.upgrade,
+        'check-updates': menu.check_updates,
+        '-c': menu.check_updates,
+        'repo-info': menu.repo_info,
+        '-I': menu.repo_info,
+        'build': menu.build,
+        '-b': menu.build,
+        'install': menu.install,
+        '-i': menu.install,
+        'download': menu.download,
+        '-d': menu.download,
+        'remove': menu.remove,
+        '-R': menu.remove,
+        'view': menu.view,
+        '-w': menu.view,
+        'find': menu.find,
+        '-f': menu.find,
+        'search': menu.search,
+        '-s': menu.search,
+        'dependees': menu.dependees,
+        '-e': menu.dependees,
+        'tracking': menu.tracking,
+        '-t': menu.tracking
     }
 
     try:
         arguments[args[0]]()
     except (KeyError, IndexError):
         logger = logging.getLogger(LoggingConfig.date_time)
         logger.exception(main.__name__)
```

### Comparing `slpkg-4.8.4/slpkg/find_installed.py` & `slpkg-4.8.6/slpkg/find_installed.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,39 +12,39 @@
         super(Configs, self).__init__()
         self.packages: list = packages
 
         self.utils = Utilities()
         self.matching: list = []
 
         self.option_for_no_case: bool = self.utils.is_option(
-            ['-m', '--no-case'], flags)
+            ('-m', '--no-case'), flags)
 
     def find(self) -> None:
         self.view_title()
-        for pkg in self.packages:
-            for package in self.utils.installed_packages.values():
+        for package in self.packages:
+            for name in self.utils.installed_packages.values():
 
-                if self.option_for_no_case:
-                    pkg: str = pkg.lower()
-                    package: str = package.lower()
-
-                if pkg in package or pkg == '*':
-                    self.matching.append(package)
+                if package in name or package == '*' or self.is_not_case_sensitive(package, name):
+                    self.matching.append(name)
         self.matched()
 
-    def view_title(self):
+    def view_title(self) -> None:
         print(f'The list below shows the installed packages '
               f'that contains \'{", ".join([p for p in self.packages])}\' files:\n')
 
     def matched(self) -> None:
         if self.matching:
             self.view_matched_packages()
         else:
             print('\nDoes not match any package.\n')
 
-    def view_matched_packages(self):
+    def view_matched_packages(self) -> None:
         for package in self.matching:
             print(f'{self.cyan}{package}{self.endc}')
         self.view_summary()
 
-    def view_summary(self):
+    def view_summary(self) -> None:
         print(f'\n{self.grey}Total found {len(self.matching)} packages.{self.endc}')
+
+    def is_not_case_sensitive(self, package: str, name: str) -> bool:
+        if self.option_for_no_case:
+            return package.lower() in name.lower()
```

### Comparing `slpkg-4.8.4/slpkg/upgrade.py` & `slpkg-4.8.6/slpkg/upgrade.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 from typing import Generator
 from packaging.version import parse, InvalidVersion
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 from slpkg.logging_config import LoggingConfig
+from slpkg.rules import Rules
 
 
 class Upgrade(Configs):
     """ Upgrade the installed packages. """
 
     def __init__(self, repository: str, data: dict):
         super(Configs, self).__init__()
         self.repository: str = repository
         self.data: dict = data
 
         self.utils = Utilities()
         self.repos = Repositories()
+        self.rules = Rules()
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
@@ -54,14 +56,20 @@
                 repo_package: str = self.data[name]['package']
                 repo_package_build: str = self.utils.split_package(repo_package)['build']
             else:
                 repo_location: str = self.data[name]['location']
                 repo_package_build: str = self.utils.read_slackbuild_build_tag(
                     name, repo_location, self.repository)
 
+        # Patches installed version to matching with repository package version.
+        # It fixes installed package version, packages like nvidia-kernel and virtualbox-kernel
+        # that contain the kernel version with package version.
+        if name in self.rules.packages():
+            inst_package_version = f"{inst_package_version[:len(repo_package_version)]}"
+
         repository_package: str = f'{name}-{repo_package_version}'
         installed_package: str = f'{name}-{inst_package_version}'
 
         try:
             if parse(repository_package) > parse(installed_package):
                 return True
```

### Comparing `slpkg-4.8.4/slpkg/search.py` & `slpkg-4.8.6/slpkg/search.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from slpkg.repositories import Repositories
 from slpkg.binaries.queries import BinQueries
 
 
 class SearchPackage(Configs):
     """ Search packages from the repositories. """
 
-    def __init__(self, flags: list, data: dict, packages: list, repository: str):
+    def __init__(self, flags: list, packages: list, repository: str):
         super(Configs, self).__init__()
-        self.data: dict = data
         self.packages: list = packages
         self.repository: str = repository
 
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.matching: int = 0
+        self.repo_data: dict = {}
         self.data_dict: dict = {}
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_no_case: bool = self.utils.is_option(
-            ['-m', '--no-case'], flags)
+            ('-m', '--no-case'), flags)
 
     def search(self) -> None:
         print(f'The list below shows the repo '
               f'packages that contains \'{", ".join([p for p in self.packages])}\':\n')
 
         if self.repository == '*':
             self.search_to_all_repositories()
@@ -39,46 +39,49 @@
 
         self.summary_of_searching()
 
     def search_to_all_repositories(self) -> None:
         for repo, item in self.repos.repositories.items():
             if item['enable']:  # Check if the repository is enabled
                 if self.utils.is_binary_repo(repo):
-                    data: dict = BinQueries(repo).repository_data()
+                    self.repo_data: dict = BinQueries(repo).repository_data()
                 else:
-                    data: dict = SBoQueries(repo).repository_data()
-                self.search_for_the_packages(data, repo)
+                    self.repo_data: dict = SBoQueries(repo).repository_data()
+                self.search_for_the_packages(repo)
 
     def search_to_the_repository(self) -> None:
         if self.is_binary:
-            data: dict = BinQueries(self.repository).repository_data()
+            self.repo_data: dict = BinQueries(self.repository).repository_data()
         else:
-            data: dict = SBoQueries(self.repository).repository_data()
-        self.search_for_the_packages(data, self.repository)
+            self.repo_data: dict = SBoQueries(self.repository).repository_data()
+        self.search_for_the_packages(self.repository)
 
-    def search_for_the_packages(self, data: dict, repo: str) -> None:
+    def search_for_the_packages(self, repo: str) -> None:
         for package in self.packages:
-            for name, data_pkg in data.items():
+            for name, data_pkg in self.repo_data.items():
 
-                if self.option_for_no_case:
-                    package: str = package.lower()
-                    name: str = name.lower()
-
-                if package in name or package == '*':
+                if package in name or package == '*' or self.is_not_case_sensitive(package, name):
                     self.matching += 1
 
                     self.data_dict[self.matching] = {
                         'repository': repo,
                         'name': name,
                         'version': data_pkg['version']
                     }
 
     def summary_of_searching(self) -> None:
-        name_length: int = max(len(name['name']) for name in self.data_dict.values())
+        try:
+            name_length: int = max(len(name['name']) for name in self.data_dict.values())
+        except ValueError:
+            name_length: int = 1
         if self.matching:
             for item in self.data_dict.values():
                 print(f"{item['repository']}: {self.cyan}{item['name']:<{name_length}}{self.endc} "
                       f"{self.yellow}{item['version']}{self.endc}")
 
             print(f'\n{self.grey}Total found {self.matching} packages.{self.endc}')
         else:
             print('\nDoes not match any package.\n')
+
+    def is_not_case_sensitive(self, package: str, name: str) -> bool:
+        if self.option_for_no_case:
+            return package.lower() in name.lower()
```

### Comparing `slpkg-4.8.4/setup.cfg` & `slpkg-4.8.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slpkg
-version = 4.8.4
+version = 4.8.6
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = dslackw@gmail.com
 description = Package manager utility for Slackware Linux.
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls =
```

### Comparing `slpkg-4.8.4/slpkg.egg-info/SOURCES.txt` & `slpkg-4.8.6/slpkg.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 slpkg/main.py
 slpkg/multi_process.py
 slpkg/new_configs.py
 slpkg/progress_bar.py
 slpkg/remove_packages.py
 slpkg/repo_info.py
 slpkg/repositories.py
+slpkg/rules.py
 slpkg/search.py
 slpkg/toml_error_message.py
 slpkg/tracking.py
 slpkg/update_repository.py
 slpkg/upgrade.py
 slpkg/utilities.py
 slpkg.egg-info/PKG-INFO
```

### Comparing `slpkg-4.8.4/slpkg.egg-info/PKG-INFO` & `slpkg-4.8.6/slpkg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.8.4
+Version: 4.8.6
 Summary: Package manager utility for Slackware Linux.
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
 Author-email: dslackw@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
```

### Comparing `slpkg-4.8.4/README.md` & `slpkg-4.8.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 10. [Repositories](#Repositories)
 11. [Multilib Packages](#Multilib-Packages)
 12. [Issues](#Issues)
 13. [Donate](#Donate)
 14. [Support](#Support)
 15. [Copyright](#Copyright)
 
-<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install_packages.png" width="400" height="200">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_logo.png" width="400" height="200">
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/poweredbyslack.gif" width="200" height="50">
 
 
 ### About
 
 Slpkg is a software package manager that installs, updates and removes packages on [Slackware](https://www.slackware.com)-based systems.
 It automatically calculates dependencies and figures out what things need to happen to install packages.
@@ -56,16 +56,16 @@
 $ slpkg tracking --pkg-version Flask awscli pychess
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="900">
 
 ### Installation
 
 ```
-$ tar xvf slpkg-4.8.4.tar.gz
-$ cd slpkg-4.8.4
+$ tar xvf slpkg-4.8.6.tar.gz
+$ cd slpkg-4.8.6
 $ ./install.sh
 ```
 
 ### Requirements
 
 ```
 SQLAlchemy >= 1.4.46
@@ -82,15 +82,15 @@
 
 The majority of trials have been made in Slackware x86_64 'stable' environment.
 
 
 ### Command Line Tool Usage
 
 ```
-slpkg - version 4.8.4
+slpkg - version 4.8.6
 
 USAGE:
   slpkg [COMMAND] [OPTIONS] [FILELIST|PACKAGES...]
 
 DESCRIPTION:
   Package manager utility for Slackware.
 
@@ -199,14 +199,17 @@
     General configuration of slpkg
     
 /etc/slpkg/repositories.toml
     Repositories configuration
 
 /etc/slpkg/blacklist.toml
     Blacklist of packages
+        
+/etc/slpkg/rules.toml
+    Rules of packages.
 ```
 
 ### Repositories
 
 This is the list of the supported repositories:
 
 * [Slackbuilds](https://slackbuilds.org/)
```

### Comparing `slpkg-4.8.4/tools/gen_sbo_txt.sh` & `slpkg-4.8.6/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

