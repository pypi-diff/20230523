# Comparing `tmp/pynecone-0.1.31a1.tar.gz` & `tmp/pynecone-0.1.32a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.31a1.tar", max compression
+gzip compressed data, was "pynecone-0.1.32a0.tar", max compression
```

## Comparing `pynecone-0.1.31a1.tar` & `pynecone-0.1.32a0.tar`

### file list

```diff
@@ -1,157 +1,161 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.31a1/LICENSE
--rw-r--r--   0        0        0     7876 2023-05-17 17:15:44.662291 pynecone-0.1.31a1/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.31a1/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-05-16 19:12:26.220987 pynecone-0.1.31a1/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.31a1/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.31a1/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.31a1/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.31a1/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.31a1/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-05-15 02:04:07.604581 pynecone-0.1.31a1/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.31a1/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     2345 2023-05-17 03:31:04.693336 pynecone-0.1.31a1/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     2999 2023-05-15 02:04:07.604822 pynecone-0.1.31a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.31a1/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.31a1/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   254417 2023-05-15 02:04:07.606023 pynecone-0.1.31a1/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.31a1/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0      927 2023-05-15 02:04:07.606305 pynecone-0.1.31a1/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.31a1/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.31a1/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.31a1/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     7657 2023-05-17 03:31:04.693493 pynecone-0.1.31a1/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1363 2023-05-15 02:04:07.606665 pynecone-0.1.31a1/pynecone/__init__.py
--rw-r--r--   0        0        0    20075 2023-05-15 02:04:07.606864 pynecone-0.1.31a1/pynecone/app.py
--rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.31a1/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.31a1/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     6290 2023-05-17 03:31:04.693642 pynecone-0.1.31a1/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.31a1/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7384 2023-05-15 02:04:07.607425 pynecone-0.1.31a1/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     6390 2023-05-15 17:32:17.391279 pynecone-0.1.31a1/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.31a1/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.31a1/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.31a1/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.31a1/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.31a1/pynecone/components/base/head.py
--rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.31a1/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.31a1/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    22653 2023-05-17 03:31:04.693829 pynecone-0.1.31a1/pynecone/components/component.py
--rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.31a1/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.31a1/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.31a1/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.31a1/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.31a1/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.31a1/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.31a1/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.31a1/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5157 2023-05-15 02:04:07.609333 pynecone-0.1.31a1/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.31a1/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.31a1/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.31a1/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.31a1/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.31a1/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.31a1/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.31a1/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.31a1/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.31a1/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.31a1/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1109 2023-05-16 05:05:39.515505 pynecone-0.1.31a1/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.31a1/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2454 2023-05-17 03:31:04.693986 pynecone-0.1.31a1/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      578 2023-05-17 03:31:04.694099 pynecone-0.1.31a1/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0     1949 2023-05-17 03:31:04.694210 pynecone-0.1.31a1/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0     2965 2023-05-17 03:31:04.694346 pynecone-0.1.31a1/pynecone/components/forms/formcontrol.py
--rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.31a1/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2880 2023-05-17 03:31:04.694475 pynecone-0.1.31a1/pynecone/components/forms/input.py
--rw-r--r--   0        0        0     3897 2023-05-17 03:31:04.694607 pynecone-0.1.31a1/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.31a1/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2670 2023-05-17 03:31:04.694745 pynecone-0.1.31a1/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3043 2023-05-17 03:31:04.694864 pynecone-0.1.31a1/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2853 2023-05-17 03:31:04.694977 pynecone-0.1.31a1/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3506 2023-05-17 03:31:04.695098 pynecone-0.1.31a1/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3124 2023-05-17 03:31:04.695208 pynecone-0.1.31a1/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1552 2023-05-17 03:31:04.695316 pynecone-0.1.31a1/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1531 2023-05-17 03:31:04.695426 pynecone-0.1.31a1/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2915 2023-05-17 03:31:04.695540 pynecone-0.1.31a1/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.31a1/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.31a1/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.31a1/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.31a1/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.31a1/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.31a1/pynecone/components/layout/box.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.31a1/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3844 2023-05-17 03:31:04.695669 pynecone-0.1.31a1/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.31a1/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.31a1/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     2843 2023-05-17 03:31:04.695778 pynecone-0.1.31a1/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.31a1/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.31a1/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.31a1/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.31a1/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.31a1/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.31a1/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.31a1/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.31a1/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.31a1/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.31a1/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0     1524 2023-05-17 03:31:04.695901 pynecone-0.1.31a1/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.31a1/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1400 2023-05-17 03:31:04.696029 pynecone-0.1.31a1/pynecone/components/media/image.py
--rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.31a1/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.31a1/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1083 2023-05-15 02:04:07.616009 pynecone-0.1.31a1/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.31a1/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.31a1/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.31a1/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-17 03:31:04.696401 pynecone-0.1.31a1/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     4681 2023-05-17 03:31:04.696630 pynecone-0.1.31a1/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5530 2023-05-17 03:31:04.696777 pynecone-0.1.31a1/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4917 2023-05-17 03:31:04.696908 pynecone-0.1.31a1/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5688 2023-05-17 03:31:04.697043 pynecone-0.1.31a1/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1949 2023-05-17 03:31:04.697172 pynecone-0.1.31a1/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.31a1/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.31a1/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.31a1/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5018 2023-05-17 03:31:04.697339 pynecone-0.1.31a1/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.31a1/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.31a1/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.31a1/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      358 2023-05-15 02:04:07.618079 pynecone-0.1.31a1/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3288 2023-05-15 02:04:07.618181 pynecone-0.1.31a1/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.31a1/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.31a1/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.31a1/pynecone/config.py
--rw-r--r--   0        0        0     8974 2023-05-17 17:15:44.662475 pynecone-0.1.31a1/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.31a1/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.31a1/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.31a1/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.31a1/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.31a1/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1283 2023-05-15 02:04:07.619213 pynecone-0.1.31a1/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.31a1/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.31a1/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10647 2023-05-15 17:32:17.393442 pynecone-0.1.31a1/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.31a1/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.31a1/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.31a1/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.31a1/pynecone/model.py
--rw-r--r--   0        0        0     7979 2023-05-15 17:32:17.393651 pynecone-0.1.31a1/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.31a1/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.31a1/pynecone/route.py
--rw-r--r--   0        0        0    29790 2023-05-15 02:04:07.621653 pynecone-0.1.31a1/pynecone/state.py
--rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.31a1/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.31a1/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     5318 2023-05-17 19:50:01.519902 pynecone-0.1.31a1/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.31a1/pynecone/utils/console.py
--rw-r--r--   0        0        0     3517 2023-05-17 19:50:01.520070 pynecone-0.1.31a1/pynecone/utils/exec.py
--rw-r--r--   0        0        0    11320 2023-05-17 17:15:44.663013 pynecone-0.1.31a1/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.31a1/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.31a1/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    10033 2023-05-17 03:31:04.698132 pynecone-0.1.31a1/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.31a1/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.31a1/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4389 2023-05-15 02:04:07.623635 pynecone-0.1.31a1/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.31a1/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30918 2023-05-17 03:31:04.698348 pynecone-0.1.31a1/pynecone/vars.py
--rw-r--r--   0        0        0     1798 2023-05-17 19:50:13.403900 pynecone-0.1.31a1/pyproject.toml
--rw-r--r--   0        0        0     9407 1970-01-01 00:00:00.000000 pynecone-0.1.31a1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.32a0/LICENSE
+-rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.32a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.32a0/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-05-22 20:45:24.544118 pynecone-0.1.32a0/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.32a0/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.32a0/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.32a0/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.32a0/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.32a0/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.32a0/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.32a0/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     2318 2023-05-22 21:40:04.765646 pynecone-0.1.32a0/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.32a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.32a0/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.32a0/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   254417 2023-05-15 02:04:07.606023 pynecone-0.1.32a0/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-05-22 21:40:04.766038 pynecone-0.1.32a0/pynecone/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.32a0/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0      927 2023-05-18 18:20:32.022198 pynecone-0.1.32a0/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.32a0/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.32a0/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.32a0/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     7656 2023-05-22 21:40:04.766251 pynecone-0.1.32a0/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1363 2023-05-15 02:04:07.606665 pynecone-0.1.32a0/pynecone/__init__.py
+-rw-r--r--   0        0        0    19719 2023-05-22 21:40:04.766707 pynecone-0.1.32a0/pynecone/app.py
+-rw-r--r--   0        0        0     2524 2023-05-18 00:14:14.759391 pynecone-0.1.32a0/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.32a0/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6178 2023-05-22 21:40:04.766968 pynecone-0.1.32a0/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.32a0/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7384 2023-05-15 02:04:07.607425 pynecone-0.1.32a0/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     6786 2023-05-22 21:40:04.767170 pynecone-0.1.32a0/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.32a0/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.32a0/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.32a0/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.32a0/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.32a0/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.32a0/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.32a0/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    22794 2023-05-22 21:40:04.767506 pynecone-0.1.32a0/pynecone/components/component.py
+-rw-r--r--   0        0        0      496 2023-05-22 21:40:04.767804 pynecone-0.1.32a0/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.32a0/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.32a0/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.32a0/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.32a0/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.32a0/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.32a0/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.32a0/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5157 2023-05-15 02:04:07.609333 pynecone-0.1.32a0/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2188 2023-05-22 21:40:04.768093 pynecone-0.1.32a0/pynecone/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-05-22 21:40:04.768839 pynecone-0.1.32a0/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.32a0/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.32a0/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1613 2023-05-22 21:40:04.768963 pynecone-0.1.32a0/pynecone/components/disclosure/transition.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.32a0/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.32a0/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.32a0/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.32a0/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.32a0/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.32a0/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.32a0/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1109 2023-05-18 04:03:34.423606 pynecone-0.1.32a0/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.32a0/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.32a0/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.32a0/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.32a0/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0     2965 2023-05-18 00:14:14.761116 pynecone-0.1.32a0/pynecone/components/forms/formcontrol.py
+-rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.32a0/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-05-18 00:14:14.761287 pynecone-0.1.32a0/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.32a0/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.32a0/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.32a0/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.32a0/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.32a0/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3506 2023-05-18 00:14:14.762103 pynecone-0.1.32a0/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.32a0/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1552 2023-05-18 00:14:14.762398 pynecone-0.1.32a0/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1531 2023-05-18 00:14:14.762541 pynecone-0.1.32a0/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.32a0/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.32a0/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.32a0/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.32a0/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.32a0/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.32a0/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.32a0/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.32a0/pynecone/components/layout/card.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.32a0/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.32a0/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.32a0/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.32a0/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     3167 2023-05-22 21:40:04.769250 pynecone-0.1.32a0/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.32a0/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.32a0/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.32a0/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.32a0/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.32a0/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.32a0/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.32a0/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.32a0/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.32a0/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.32a0/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.32a0/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.32a0/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1400 2023-05-18 00:14:14.763528 pynecone-0.1.32a0/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.32a0/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.32a0/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1083 2023-05-15 02:04:07.616009 pynecone-0.1.32a0/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.32a0/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.32a0/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.32a0/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.32a0/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.32a0/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.32a0/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.32a0/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-05-18 00:14:14.764341 pynecone-0.1.32a0/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.32a0/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.32a0/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.32a0/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.32a0/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-05-18 00:14:14.764773 pynecone-0.1.32a0/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.32a0/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.32a0/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.32a0/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      358 2023-05-15 02:04:07.618079 pynecone-0.1.32a0/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3288 2023-05-15 02:04:07.618181 pynecone-0.1.32a0/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.32a0/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.32a0/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.32a0/pynecone/config.py
+-rw-r--r--   0        0        0     9018 2023-05-22 21:40:04.769502 pynecone-0.1.32a0/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.32a0/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.32a0/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.32a0/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.32a0/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.32a0/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1283 2023-05-15 02:04:07.619213 pynecone-0.1.32a0/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.32a0/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.32a0/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10647 2023-05-15 17:32:17.393442 pynecone-0.1.32a0/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.32a0/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.32a0/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.32a0/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.32a0/pynecone/model.py
+-rw-r--r--   0        0        0     7918 2023-05-22 21:40:04.769687 pynecone-0.1.32a0/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.32a0/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.32a0/pynecone/route.py
+-rw-r--r--   0        0        0    29790 2023-05-15 02:04:07.621653 pynecone-0.1.32a0/pynecone/state.py
+-rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.32a0/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.32a0/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     7211 2023-05-22 21:40:04.770022 pynecone-0.1.32a0/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.32a0/pynecone/utils/console.py
+-rw-r--r--   0        0        0     5091 2023-05-22 21:40:04.770472 pynecone-0.1.32a0/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11334 2023-05-18 00:14:14.765753 pynecone-0.1.32a0/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.32a0/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.32a0/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    10033 2023-05-17 03:31:04.698132 pynecone-0.1.32a0/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.32a0/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.32a0/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4394 2023-05-18 00:14:14.765933 pynecone-0.1.32a0/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.32a0/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30928 2023-05-18 00:14:14.766310 pynecone-0.1.32a0/pynecone/vars.py
+-rw-r--r--   0        0        0     1798 2023-05-23 17:33:51.794649 pynecone-0.1.32a0/pyproject.toml
+-rw-r--r--   0        0        0     9407 1970-01-01 00:00:00.000000 pynecone-0.1.32a0/PKG-INFO
```

### Comparing `pynecone-0.1.31a1/LICENSE` & `pynecone-0.1.32a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/README.md` & `pynecone-0.1.32a0/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.32a0/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.32a0/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.32a0/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.32a0/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 {% extends "web/pages/base_page.js.jinja2" %}
 
 {% block declaration %}
 {% for custom_code in custom_codes %}
 {{custom_code}}
 {% endfor %}
 
-{% for name, url in endpoints.items() %}
-const {{name}} = {{url|json_dumps}}
-{% endfor %}
 {% endblock %}
 
 {% block export %}
 export default function Component() {
   const [{{state_name}}, {{state_name|react_setter}}] = useState({{initial_state|json_dumps}})
   const [{{const.result}}, {{const.result|react_setter}}] = useState({{const.initial_result|json_dumps}})
   const {{const.router}} = useRouter()
   const {{const.socket}} = useRef(null)
   const { isReady } = {{const.router}}
   const { {{const.color_mode}}, {{const.toggle_color_mode}} } = {{const.use_color_mode}}()
-
+  const focusRef = useRef();
+  
   const Event = (events, _e) => {
       preventDefault(_e);
       {{state_name|react_setter}}({
         ...{{state_name}},
         events: [...{{state_name}}.events, ...events],
       })
   }
@@ -33,15 +31,15 @@
   })
 
   useEffect(()=>{
     if(!isReady) {
       return;
     }
     if (!{{const.socket}}.current) {
-      connect({{const.socket}}, {{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.event_endpoint}}, {{transports}})
+      connect({{const.socket}}, {{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{transports}})
     }
     const update = async () => {
       if ({{const.result}}.{{const.state}} != null){
         {{state_name|react_setter}}({
           ...{{const.result}}.{{const.state}},
           events: [...{{state_name}}.{{const.events}}, ...{{const.result}}.{{const.events}}],
         })
@@ -51,14 +49,16 @@
           {{const.events}}: [],
           {{const.processing}}: false,
         })
       }
 
       await updateState({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
     }
+    if (focusRef.current)
+      focusRef.current.focus();
     update()
   })
   useEffect(() => {
     const change_complete = () => Event([E('{{state_name}}.{{const.hydrate}}', {})])
     {{const.router}}.events.on('routeChangeComplete', change_complete)
     return () => {
       {{const.router}}.events.off('routeChangeComplete', change_complete)
```

### Comparing `pynecone-0.1.31a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.32a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 {% endmacro %}
 
 {# Rendering self close tag. #}
 {# Args: #}
 {#     component: component dictionary #}
 {% macro render_self_close_tag(component) %}
 {%- if component.name|length %}
-<{{ component.name }} {{- render_props(component.props) }}/>
+<{{ component.name }} {{- render_props(component.props) }}{% if component.autofocus %} ref={focusRef} {% endif %}/>
 {%- else %}
   {{- component.contents }}
 {%- endif %}
 {% endmacro %}
 
 {# Rendering close tag with args and props. #}
 {# Args: #}
@@ -58,15 +58,15 @@
 {%- endmacro %}
 
 
 {# Rendering iterable component. #}
 {# Args: #}
 {#     component: component dictionary #}
 {% macro render_iterable_tag(component) %}
-{ {{- component.iterable_state }}.map(({{ component.arg_name }}, {{ component.arg_index }}) => (
+{ {%- if component.iterable_type == 'dict' -%}Object.entries({{- component.iterable_state }}){%- else -%}{{- component.iterable_state }}{%- endif -%}.map(({{ component.arg_name }}, {{ component.arg_index }}) => (
   {% for child in component.children %}
   {{ render(child) }}
   {% endfor %}
 ))}
 {%- endmacro %}
```

### Comparing `pynecone-0.1.31a1/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.32a0/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/.templates/web/package.json` & `pynecone-0.1.32a0/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.32a0/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.32a0/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.32a0/pynecone/.templates/web/utils/state.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,16 @@
 // State management for Pynecone web apps.
 import axios from "axios";
 import io from "socket.io-client";
 import JSON5 from "json5";
-import config from "../pynecone.json";
+import env from "env.json";
 
-const UPLOAD = config.uploadUrl;
+const PINGURL = env.pingUrl
+const EVENTURL = env.eventUrl
+const UPLOADURL = env.uploadUrl
 // Global variable to hold the token.
 let token;
 
 // Key for the token in the session storage.
 const TOKEN_KEY = "token";
 
 // Dictionary holding component references.
@@ -123,15 +125,15 @@
  * Process an event off the event queue.
  * @param queue_event The current event
  * @param state The state with the event queue.
  * @param setResult The function to set the result.
  */
 export const applyRestEvent = async (queue_event, state, setResult) => {
     if (queue_event.handler == "uploadFiles") {
-        await uploadFiles(state, setResult, queue_event.name, UPLOAD);
+        await uploadFiles(state, setResult, queue_event.name);
     }
 };
 
 /**
  * Process an event off the event queue.
  * @param state The state with the event queue.
  * @param setState The function to set the state.
@@ -195,21 +197,20 @@
 export const connect = async (
     socket,
     state,
     setState,
     result,
     setResult,
     router,
-    endpoint,
     transports
 ) => {
     // Get backend URL object from the endpoint
-    const endpoint_url = new URL(endpoint);
+    const endpoint_url = new URL(EVENTURL);
     // Create the socket.
-    socket.current = io(endpoint, {
+    socket.current = io(EVENTURL, {
         path: endpoint_url["pathname"],
         transports: transports,
         autoUnref: false,
     });
 
     // Once the socket is open, hydrate the page.
     socket.current.on("connect", () => {
@@ -232,15 +233,15 @@
  * Upload files to the server.
  *
  * @param state The state to apply the delta to.
  * @param setResult The function to set the result.
  * @param handler The handler to use.
  * @param endpoint The endpoint to upload to.
  */
-export const uploadFiles = async (state, setResult, handler, endpoint) => {
+export const uploadFiles = async (state, setResult, handler) => {
     const files = state.files;
 
     // return if there's no file to upload
     if (files.length == 0) {
         return;
     }
 
@@ -255,15 +256,15 @@
             "files",
             files[i],
             getToken() + ":" + handler + ":" + files[i].name
         );
     }
 
     // Send the file to the server.
-    await axios.post(endpoint, formdata, headers).then((response) => {
+    await axios.post(UPLOADURL, formdata, headers).then((response) => {
         // Apply the delta and set the result.
         const update = response.data;
         applyDelta(state, update.delta);
 
         // Set processing to false and return.
         setResult({
             processing: false,
@@ -299,11 +300,11 @@
 };
 
 /**
  * Prevent the default event.
  * @param event
  */
 export const preventDefault = (event) => {
-    if (event && event.hasOwnProperty("preventDefault")) {
+    if (event && event.preventDefault) {
         event.preventDefault();
     }
 };
```

### Comparing `pynecone-0.1.31a1/pynecone/__init__.py` & `pynecone-0.1.32a0/pynecone/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/app.py` & `pynecone-0.1.32a0/pynecone/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,31 +374,21 @@
         ):
             self.pages[froute(constants.ROOT_404)] = component
         if not any(
             page.startswith("[...") or page.startswith("[[...") for page in self.pages
         ):
             self.pages[froute(constants.SLUG_404)] = component
 
-    def compile(self, force_compile: bool = False):
-        """Compile the app and output it to the pages folder.
-
-        If the config environment is set to production, the app will
-        not be compiled.
-
-        Args:
-            force_compile: Whether to force the app to compile.
-        """
+    def compile(self):
+        """Compile the app and output it to the pages folder."""
         for render, kwargs in DECORATED_ROUTES:
             self.add_page(render, **kwargs)
 
         # Get the env mode.
         config = get_config()
-        if config.env != constants.Env.DEV and not force_compile:
-            print("Skipping compilation in non-dev mode.")
-            return
 
         # Update models during hot reload.
         if config.db_url is not None:
             Model.create_all()
 
         # Empty the .web pages directory
         compiler.purge_web_pages_dir()
```

### Comparing `pynecone-0.1.31a1/pynecone/base.py` & `pynecone-0.1.32a0/pynecone/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def json(self) -> str:
         """Convert the object to a json string.
 
         Returns:
             The object as a json string.
         """
-        return self.__config__.json_dumps(self.dict())
+        return self.__config__.json_dumps(self.dict(), default=list)
 
     def set(self: PcType, **kwargs) -> PcType:
         """Set multiple fields and return the object.
 
         Args:
             **kwargs: The fields and values to set.
```

### Comparing `pynecone-0.1.31a1/pynecone/compiler/compiler.py` & `pynecone-0.1.32a0/pynecone/compiler/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,14 @@
     imports = utils.merge_imports(DEFAULT_IMPORTS, component.get_imports())
     imports = utils.compile_imports(imports)
 
     # Compile the code to render the component.
     return templates.PAGE.render(
         imports=imports,
         custom_codes=component.get_custom_code(),
-        endpoints={
-            constant.name: constant.get_url() for constant in constants.Endpoint
-        },
         initial_state=utils.compile_state(state),
         state_name=state.get_name(),
         hooks=component.get_hooks(),
         render=component.render(),
         transports=constants.Transports.POLLING_WEBSOCKET.get_transports(),
     )
```

### Comparing `pynecone-0.1.31a1/pynecone/compiler/templates.py` & `pynecone-0.1.32a0/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/compiler/utils.py` & `pynecone-0.1.32a0/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/__init__.py` & `pynecone-0.1.32a0/pynecone/components/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 unordered_list = UnorderedList.create
 stat = Stat.create
 stat_arrow = StatArrow.create
 stat_group = StatGroup.create
 stat_help_text = StatHelpText.create
 stat_label = StatLabel.create
 stat_number = StatNumber.create
+tag = Tag.create
+tag_label = TagLabel.create
+tag_left_icon = TagLeftIcon.create
+tag_right_icon = TagRightIcon.create
+tag_close_button = TagCloseButton.create
 table = Table.create
 table_caption = TableCaption.create
 table_container = TableContainer.create
 tbody = Tbody.create
 td = Td.create
 tfoot = Tfoot.create
 th = Th.create
@@ -57,18 +62,27 @@
 accordion_panel = AccordionPanel.create
 tab = Tab.create
 tab_list = TabList.create
 tab_panel = TabPanel.create
 tab_panels = TabPanels.create
 tabs = Tabs.create
 visually_hidden = VisuallyHidden.create
+fade = Fade.create
+scale_fade = ScaleFade.create
+slide = Slide.create
+slide_fade = SlideFade.create
+collapse = Collapse.create
 alert = Alert.create
 alert_description = AlertDescription.create
 alert_icon = AlertIcon.create
 alert_title = AlertTitle.create
+card = Card.create
+card_body = CardBody.create
+card_footer = CardFooter.create
+card_header = CardHeader.create
 circular_progress = CircularProgress.create
 circular_progress_label = CircularProgressLabel.create
 progress = Progress.create
 skeleton = Skeleton.create
 skeleton_circle = SkeletonCircle.create
 skeleton_text = SkeletonText.create
 spinner = Spinner.create
```

### Comparing `pynecone-0.1.31a1/pynecone/components/base/bare.py` & `pynecone-0.1.32a0/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/base/document.py` & `pynecone-0.1.32a0/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/base/link.py` & `pynecone-0.1.32a0/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/base/meta.py` & `pynecone-0.1.32a0/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/component.py` & `pynecone-0.1.32a0/pynecone/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 
     # The class name for the component.
     class_name: Any = None
 
     # Special component props.
     special_props: Set[Var] = set()
 
+    # Whether the component should take the focus once the page is loaded
+    autofocus: bool = False
+
     @classmethod
     def __init_subclass__(cls, **kwargs):
         """Set default properties.
 
         Args:
             **kwargs: The kwargs to pass to the superclass.
         """
@@ -416,14 +419,15 @@
                 id=self.id,
                 class_name=self.class_name,
             ).set(
                 children=[child.render() for child in self.children],
                 contents=str(tag.contents),
                 props=tag.format_props(),
             ),
+            autofocus=self.autofocus,
         )
 
     def _get_custom_code(self) -> Optional[str]:
         """Get custom code for the component.
 
         Returns:
             The custom code.
```

### Comparing `pynecone-0.1.31a1/pynecone/components/datadisplay/code.py` & `pynecone-0.1.32a0/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.32a0/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.32a0/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/datadisplay/list.py` & `pynecone-0.1.32a0/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.32a0/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/datadisplay/table.py` & `pynecone-0.1.32a0/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.32a0/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.32a0/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/feedback/alert.py` & `pynecone-0.1.32a0/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.32a0/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/feedback/progress.py` & `pynecone-0.1.32a0/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.32a0/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/feedback/spinner.py` & `pynecone-0.1.32a0/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/__init__.py` & `pynecone-0.1.32a0/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/button.py` & `pynecone-0.1.32a0/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/checkbox.py` & `pynecone-0.1.32a0/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.32a0/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/editable.py` & `pynecone-0.1.32a0/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/formcontrol.py` & `pynecone-0.1.32a0/pynecone/components/forms/formcontrol.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.32a0/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/input.py` & `pynecone-0.1.32a0/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/numberinput.py` & `pynecone-0.1.32a0/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/pininput.py` & `pynecone-0.1.32a0/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/radio.py` & `pynecone-0.1.32a0/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.32a0/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/select.py` & `pynecone-0.1.32a0/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/slider.py` & `pynecone-0.1.32a0/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/switch.py` & `pynecone-0.1.32a0/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/textarea.py` & `pynecone-0.1.32a0/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/forms/upload.py` & `pynecone-0.1.32a0/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/graphing/plotly.py` & `pynecone-0.1.32a0/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/graphing/victory.py` & `pynecone-0.1.32a0/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/__init__.py` & `pynecone-0.1.32a0/pynecone/components/layout/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Convenience functions to define layout components."""
 
 from .aspect_ratio import AspectRatio
 from .box import Box
+from .card import Card, CardBody, CardFooter, CardHeader
 from .center import Center, Circle, Square
 from .cond import Cond, cond
 from .container import Container
 from .flex import Flex
 from .foreach import Foreach
 from .fragment import Fragment
 from .grid import Grid, GridItem, ResponsiveGrid
```

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/box.py` & `pynecone-0.1.32a0/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/cond.py` & `pynecone-0.1.32a0/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/flex.py` & `pynecone-0.1.32a0/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/foreach.py` & `pynecone-0.1.32a0/pynecone/components/layout/foreach.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 """Create a list of components from an iterable."""
 from __future__ import annotations
 
-from typing import Any, Callable, List
+from typing import Any, Callable, Iterable
 
 from pynecone.components.component import Component
 from pynecone.components.layout.fragment import Fragment
 from pynecone.components.tags import IterTag
 from pynecone.vars import BaseVar, Var, get_unique_variable_name
 
 
 class Foreach(Component):
     """A component that takes in an iterable and a render function and renders a list of components."""
 
     # The iterable to create components from.
-    iterable: Var[List]
+    iterable: Var[Iterable]
 
     # A function from the render args to the component.
     render_fn: Callable = Fragment.create
 
     @classmethod
-    def create(cls, iterable: Var[List], render_fn: Callable, **props) -> Foreach:
+    def create(cls, iterable: Var[Iterable], render_fn: Callable, **props) -> Foreach:
         """Create a foreach component.
 
         Args:
             iterable: The iterable to create components from.
             render_fn: A function from the render args to the component.
             **props: The attributes to pass to each child component.
 
         Returns:
             The foreach component.
 
         Raises:
             TypeError: If the iterable is of type Any.
         """
         try:
-            type_ = iterable.type_.__args__[0]
+            type_ = (
+                iterable.type_
+                if iterable.type_.mro()[0] == dict
+                else iterable.type_.__args__[0]
+            )
         except Exception:
             type_ = Any
         iterable = Var.create(iterable)  # type: ignore
         if iterable.type_ == Any:
             raise TypeError(
                 f"Could not foreach over var of type Any. (If you are trying to foreach over a state var, add a type annotation to the var.)"
             )
@@ -57,15 +61,19 @@
         """Render the component.
 
         Returns:
             The dictionary for template of component.
         """
         tag = self._render()
         try:
-            type_ = self.iterable.type_.__args__[0]
+            type_ = (
+                self.iterable.type_
+                if self.iterable.type_.mro()[0] == dict
+                else self.iterable.type_.__args__[0]
+            )
         except Exception:
             type_ = Any
         arg = BaseVar(
             name=get_unique_variable_name(),
             type_=type_,
         )
         index_arg = tag.get_index_var_arg()
@@ -80,8 +88,9 @@
             ).set(
                 children=[component.render()],
                 props=tag.format_props(),
             ),
             iterable_state=tag.iterable.full_name,
             arg_name=arg.name,
             arg_index=index_arg,
+            iterable_type=tag.iterable.type_.mro()[0].__name__,
         )
```

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/grid.py` & `pynecone-0.1.32a0/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/html.py` & `pynecone-0.1.32a0/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/responsive.py` & `pynecone-0.1.32a0/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/stack.py` & `pynecone-0.1.32a0/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/layout/wrap.py` & `pynecone-0.1.32a0/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/media/avatar.py` & `pynecone-0.1.32a0/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/media/icon.py` & `pynecone-0.1.32a0/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/media/image.py` & `pynecone-0.1.32a0/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.32a0/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/navigation/link.py` & `pynecone-0.1.32a0/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.32a0/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/overlay/__init__.py` & `pynecone-0.1.32a0/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.32a0/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/overlay/drawer.py` & `pynecone-0.1.32a0/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/overlay/menu.py` & `pynecone-0.1.32a0/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/overlay/modal.py` & `pynecone-0.1.32a0/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/overlay/popover.py` & `pynecone-0.1.32a0/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.32a0/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.32a0/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/tags/tag.py` & `pynecone-0.1.32a0/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/tags/tagless.py` & `pynecone-0.1.32a0/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/components/typography/markdown.py` & `pynecone-0.1.32a0/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/config.py` & `pynecone-0.1.32a0/pynecone/config.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/constants.py` & `pynecone-0.1.32a0/pynecone/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 SITEMAP_CONFIG_FILE = os.path.join(WEB_DIR, "next-sitemap.config.js")
 # The node modules directory.
 NODE_MODULES = "node_modules"
 # The package lock file.
 PACKAGE_LOCK = "package-lock.json"
 # The pcversion app file.
 PCVERSION_APP_FILE = os.path.join(WEB_DIR, "pynecone.json")
-
+ENV_JSON = os.path.join(WEB_DIR, "env.json")
 
 # Commands to run the app.
 # The frontend default port.
 FRONTEND_PORT = "3000"
 # The backend default port.
 BACKEND_PORT = "8000"
 # The backend api url.
```

### Comparing `pynecone-0.1.31a1/pynecone/el/constants/html.py` & `pynecone-0.1.32a0/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/el/constants/pynecone.py` & `pynecone-0.1.32a0/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/el/constants/react.py` & `pynecone-0.1.32a0/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/el/element.py` & `pynecone-0.1.32a0/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/el/elements/__init__.py` & `pynecone-0.1.32a0/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/el/precompile.py` & `pynecone-0.1.32a0/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/event.py` & `pynecone-0.1.32a0/pynecone/event.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.32a0/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/middleware/middleware.py` & `pynecone-0.1.32a0/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/model.py` & `pynecone-0.1.32a0/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/pc.py` & `pynecone-0.1.32a0/pynecone/pc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Pynecone CLI to create, run, and deploy apps."""
 
 import os
 import platform
+import threading
 from pathlib import Path
 
 import httpx
 import typer
 
 from pynecone import constants
 from pynecone.config import get_config
@@ -79,15 +80,15 @@
         console.print(
             "[yellow][WARNING] We strongly advise you to use Windows Subsystem for Linux (WSL) for optimal performance when using Pynecone. Due to compatibility issues with one of our dependencies, Bun, you may experience slower performance on Windows. By using WSL, you can expect to see a significant speed increase."
         )
 
     frontend_port = get_config().port if port is None else port
     backend_port = get_config().backend_port if backend_port is None else backend_port
 
-    # If --no-frontend-only and no --backend-only, then turn on frontend and backend both
+    # If no --frontend-only and no --backend-only, then turn on frontend and backend both
     if not frontend and not backend:
         frontend = True
         backend = True
 
     # If something is running on the ports, ask the user if they want to kill or change it.
     if frontend and processes.is_process_on_port(frontend_port):
         frontend_port = processes.change_or_terminate_port(frontend_port, "frontend")
@@ -121,24 +122,23 @@
         frontend_cmd, backend_cmd = exec.run_frontend_prod, exec.run_backend_prod
     assert frontend_cmd and backend_cmd, "Invalid env"
 
     # Post a telemetry event.
     telemetry.send(f"run-{env.value}", get_config().telemetry_enabled)
 
     # Run the frontend and backend.
-    try:
-        if frontend:
-            frontend_cmd(app.app, Path.cwd(), frontend_port)
-        if backend:
-            backend_cmd(app.__name__, port=int(backend_port), loglevel=loglevel)
-    finally:
-        if frontend:
-            processes.kill_process_on_port(frontend_port)
-        if backend:
-            processes.kill_process_on_port(backend_port)
+    # try:
+    if backend:
+        threading.Thread(
+            target=backend_cmd, args=(app.__name__, backend_port, loglevel)
+        ).start()
+    if frontend:
+        threading.Thread(
+            target=frontend_cmd, args=(app.app, Path.cwd(), frontend_port)
+        ).start()
 
 
 @cli.command()
 def deploy(dry_run: bool = typer.Option(False, help="Whether to run a dry run.")):
     """Deploy the app to the Pynecone hosting service."""
     # Get the app config.
     config = get_config()
```

### Comparing `pynecone-0.1.31a1/pynecone/route.py` & `pynecone-0.1.32a0/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/state.py` & `pynecone-0.1.32a0/pynecone/state.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/style.py` & `pynecone-0.1.32a0/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/utils/build.py` & `pynecone-0.1.32a0/pynecone/utils/build.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,53 +3,62 @@
 from __future__ import annotations
 
 import json
 import os
 import random
 import subprocess
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Optional,
-)
+from typing import TYPE_CHECKING, Optional, Union
+
+from rich.progress import Progress
 
 from pynecone import constants
 from pynecone.config import get_config
 from pynecone.utils import path_ops, prerequisites
 
 if TYPE_CHECKING:
     from pynecone.app import App
 
 
-def update_json_file(file_path, key, value):
+def update_json_file(file_path: str, update_dict: dict[str, Union[int, str]]):
     """Update the contents of a json file.
 
     Args:
         file_path: the path to the JSON file.
-        key: object key to update.
-        value: value of key.
+        update_dict: object to update json.
     """
-    with open(file_path) as f:  # type: ignore
-        json_object = json.load(f)
-        json_object[key] = value
-    with open(file_path, "w") as f:
+    fp = Path(file_path)
+    # create file if it doesn't exist
+    fp.touch(exist_ok=True)
+    # create an empty json object if file is empty
+    fp.write_text("{}") if fp.stat().st_size == 0 else None
+
+    with open(fp) as f:  # type: ignore
+        json_object: dict = json.load(f)
+        json_object.update(update_dict)
+    with open(fp, "w") as f:
         json.dump(json_object, f, ensure_ascii=False)
 
 
 def set_pynecone_project_hash():
     """Write the hash of the Pynecone project to a PCVERSION_APP_FILE."""
     update_json_file(
-        constants.PCVERSION_APP_FILE, "project_hash", random.getrandbits(128)
+        constants.PCVERSION_APP_FILE, {"project_hash": random.getrandbits(128)}
     )
 
 
-def set_pynecone_upload_endpoint():
+def set_environment_variables():
     """Write the upload url to a PCVERSION_APP_FILE."""
     update_json_file(
-        constants.PCVERSION_APP_FILE, "uploadUrl", constants.Endpoint.UPLOAD.get_url()
+        constants.ENV_JSON,
+        {
+            "uploadUrl": constants.Endpoint.UPLOAD.get_url(),
+            "eventUrl": constants.Endpoint.EVENT.get_url(),
+            "pingUrl": constants.Endpoint.PING.get_url(),
+        },
     )
 
 
 def generate_sitemap(deploy_url: str):
     """Generate the sitemap config file.
 
     Args:
@@ -71,38 +80,71 @@
 
 def export_app(
     app: App,
     backend: bool = True,
     frontend: bool = True,
     zip: bool = False,
     deploy_url: Optional[str] = None,
+    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Zip up the app for deployment.
 
     Args:
         app: The app.
         backend: Whether to zip up the backend app.
         frontend: Whether to zip up the frontend app.
         zip: Whether to zip the app.
         deploy_url: The URL of the deployed app.
+        loglevel: The log level to use.
     """
-    # Force compile the app.
-    app.compile(force_compile=True)
-
     # Remove the static folder.
     path_ops.rm(constants.WEB_STATIC_DIR)
 
     # Generate the sitemap file.
     if deploy_url is not None:
         generate_sitemap(deploy_url)
 
-    # Export the Next app.
-    subprocess.run(
-        [prerequisites.get_package_manager(), "run", "export"], cwd=constants.WEB_DIR
-    )
+    # Create a progress object
+    progress = Progress()
+
+    # Add a single task to the progress object
+    task = progress.add_task("Building app... ", total=500)
+
+    # Start the progress bar
+    with progress:
+        # Run the subprocess command
+        export_process = subprocess.Popen(
+            [prerequisites.get_package_manager(), "run", "export"],
+            cwd=constants.WEB_DIR,
+            env=os.environ,
+            stderr=subprocess.STDOUT,
+            stdout=subprocess.PIPE,  # Redirect stdout to a pipe
+            universal_newlines=True,  # Set universal_newlines to True for text mode
+        )
+
+        if export_process.stdout:
+            for line in iter(export_process.stdout.readline, ""):
+                if "Linting and checking " in line:
+                    progress.update(task, advance=100)
+                elif "Compiled successfully" in line:
+                    progress.update(task, advance=100)
+                elif "Route (pages)" in line:
+                    progress.update(task, advance=100)
+                elif "automatically rendered as static HTML" in line:
+                    progress.update(task, advance=100)
+                elif "Export successful" in line:
+                    print("DOOE")
+                    progress.update(task, completed=500)
+                    break  # Exit the loop if the completion message is found
+                elif loglevel == constants.LogLevel.DEBUG:
+                    print(line, end="")
+
+        # Wait for the subprocess to complete
+        export_process.wait()
+        print("Export process completed.")
 
     # Zip up the app.
     if zip:
         if os.name == "posix":
             posix_export(backend, frontend)
         if os.name == "nt":
             nt_export(backend, frontend)
@@ -156,16 +198,16 @@
     # Copy asset files to public folder.
     path_ops.mkdir(str(root / constants.WEB_ASSETS_DIR))
     path_ops.cp(
         src=str(root / constants.APP_ASSETS_DIR),
         dest=str(root / constants.WEB_ASSETS_DIR),
     )
 
-    # set the upload url in pynecone.json file
-    set_pynecone_upload_endpoint()
+    # set the environment variables in client(env.json)
+    set_environment_variables()
 
     # Disable the Next telemetry.
     if disable_telemetry:
         subprocess.Popen(
             [
                 prerequisites.get_package_manager(),
                 "run",
```

### Comparing `pynecone-0.1.31a1/pynecone/utils/console.py` & `pynecone-0.1.32a0/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/utils/exec.py` & `pynecone-0.1.32a0/pynecone/utils/exec.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Everything regarding execution of the built app."""
 
 from __future__ import annotations
 
 import os
 import platform
 import subprocess
+from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING
 
-import uvicorn
+from rich import print
 
 from pynecone import constants
 from pynecone.config import get_config
 from pynecone.utils import console, prerequisites, processes
 from pynecone.utils.build import export_app, setup_backend, setup_frontend
 from pynecone.utils.watch import AssetFolderWatch
 
@@ -26,68 +27,111 @@
     Args:
         root: root path of the project.
     """
     asset_watch = AssetFolderWatch(root)
     asset_watch.start()
 
 
-def run_frontend(app: App, root: Path, port: str):
+def run_process_and_launch_url(
+    run_command: list[str],
+    root: Path,
+    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
+):
+    """Run the process and launch the URL.
+
+    Args:
+        run_command: The command to run.
+        root: root path of the project.
+        loglevel: The log level to use.
+    """
+    process = subprocess.Popen(
+        run_command,
+        cwd=constants.WEB_DIR,
+        env=os.environ,
+        stderr=subprocess.STDOUT,
+        stdout=subprocess.PIPE,
+        universal_newlines=True,
+    )
+
+    current_time = datetime.now()
+    if process.stdout:
+        for line in process.stdout:
+            if "ready started server on" in line:
+                url = line.split("url: ")[-1].strip()
+                print(f"App running at: [bold green]{url}")
+            if (
+                "Fast Refresh" in line
+                and (datetime.now() - current_time).total_seconds() > 1
+            ):
+                print(
+                    f"[yellow][Updating App][/yellow] Applying changes and refreshing. Time: {current_time}"
+                )
+                current_time = datetime.now()
+            elif loglevel == constants.LogLevel.DEBUG:
+                print(line, end="")
+
+
+def run_frontend(
+    app: App,
+    root: Path,
+    port: str,
+    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
+):
     """Run the frontend.
 
     Args:
         app: The app.
         root: root path of the project.
         port: port of the app.
+        loglevel: The log level to use.
     """
     # validate bun version
     prerequisites.validate_and_install_bun(initialize=False)
 
     # Set up the frontend.
     setup_frontend(root)
 
-    # start watching asset folder
+    # Start watching asset folder.
     start_watching_assets_folder(root)
 
-    # Compile the frontend.
-    app.compile(force_compile=True)
-
     # Run the frontend in development mode.
     console.rule("[bold green]App Running")
     os.environ["PORT"] = get_config().port if port is None else port
-
-    # Run the frontend in development mode.
-    subprocess.Popen(
-        [prerequisites.get_package_manager(), "run", "dev"],
-        cwd=constants.WEB_DIR,
-        env=os.environ,
+    run_process_and_launch_url(
+        [prerequisites.get_package_manager(), "run", "dev"], root, loglevel
     )
 
 
-def run_frontend_prod(app: App, root: Path, port: str):
+def run_frontend_prod(
+    app: App,
+    root: Path,
+    port: str,
+    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
+):
     """Run the frontend.
 
     Args:
         app: The app.
         root: root path of the project.
         port: port of the app.
+        loglevel: The log level to use.
     """
     # Set up the frontend.
     setup_frontend(root)
 
     # Export the app.
-    export_app(app)
+    export_app(app, loglevel=loglevel)
 
     # Set the port.
     os.environ["PORT"] = get_config().port if port is None else port
 
     # Run the frontend in production mode.
-    subprocess.Popen(
-        [prerequisites.get_package_manager(), "run", "prod"],
-        cwd=constants.WEB_DIR,
-        env=os.environ,
+    console.rule("[bold green]App Running")
+    run_process_and_launch_url(
+        [prerequisites.get_package_manager(), "run", "prod"], root, loglevel
     )
 
 
 def run_backend(
     app_name: str, port: int, loglevel: constants.LogLevel = constants.LogLevel.ERROR
 ):
     """Run the backend.
@@ -95,21 +139,31 @@
     Args:
         app_name: The app name.
         port: The app port
         loglevel: The log level.
     """
     setup_backend()
 
-    uvicorn.run(
+    cmd = [
+        "uvicorn",
         f"{app_name}:{constants.APP_VAR}.{constants.API_VAR}",
-        host=constants.BACKEND_HOST,
-        port=port,
-        log_level=loglevel,
-        reload=True,
-    )
+        "--host",
+        constants.BACKEND_HOST,
+        "--port",
+        str(port),
+        "--log-level",
+        loglevel,
+        "--reload",
+    ]
+    process = subprocess.Popen(cmd)
+
+    try:
+        process.wait()
+    except KeyboardInterrupt:
+        process.terminate()
 
 
 def run_backend_prod(
     app_name: str, port: int, loglevel: constants.LogLevel = constants.LogLevel.ERROR
 ):
     """Run the backend.
```

### Comparing `pynecone-0.1.31a1/pynecone/utils/format.py` & `pynecone-0.1.32a0/pynecone/utils/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,8 +443,8 @@
 
     Args:
         obj: The object to be serialized.
 
     Returns:
         A string
     """
-    return json.dumps(obj, ensure_ascii=False)
+    return json.dumps(obj, ensure_ascii=False, default=list)
```

### Comparing `pynecone-0.1.31a1/pynecone/utils/imports.py` & `pynecone-0.1.32a0/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/utils/path_ops.py` & `pynecone-0.1.32a0/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/utils/prerequisites.py` & `pynecone-0.1.32a0/pynecone/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/utils/processes.py` & `pynecone-0.1.32a0/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/utils/telemetry.py` & `pynecone-0.1.32a0/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/utils/types.py` & `pynecone-0.1.32a0/pynecone/utils/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pynecone.base import Base
 
 # Union of generic types.
 GenericType = Union[Type, _GenericAlias]
 
 # Valid state var types.
-PrimitiveType = Union[int, float, bool, str, list, dict, tuple]
+PrimitiveType = Union[int, float, bool, str, list, dict, set, tuple]
 StateVar = Union[PrimitiveType, Base, None]
 
 
 def get_args(alias: _GenericAlias) -> Tuple[Type, ...]:
     """Get the arguments of a type alias.
 
     Args:
```

### Comparing `pynecone-0.1.31a1/pynecone/utils/watch.py` & `pynecone-0.1.32a0/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.31a1/pynecone/vars.py` & `pynecone-0.1.32a0/pynecone/vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         # Indexing is only supported for lists, dicts, and dataframes.
         if not (
             types._issubclass(self.type_, Union[List, Dict])
             or types.is_dataframe(self.type_)
         ):
             if self.type_ == Any:
                 raise TypeError(
-                    f"Could not index into var of type Any. (If you are trying to index into a state var, add a type annotation to the var.)"
+                    f"Could not index into var of type Any. (If you are trying to index into a state var, add the correct type annotation to the var.)"
                 )
             raise TypeError(
                 f"Var {self.name} of type {self.type_} does not support indexing."
             )
 
         # The type of the indexed var.
         type_ = Any
```

### Comparing `pynecone-0.1.31a1/pyproject.toml` & `pynecone-0.1.32a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.31a1"
+version = "0.1.32a0"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.31a1/PKG-INFO` & `pynecone-0.1.32a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.31a1
+Version: 0.1.32a0
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

