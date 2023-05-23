# Comparing `tmp/zndraw-0.1.8.tar.gz` & `tmp/zndraw-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zndraw-0.1.8.tar", max compression
+gzip compressed data, was "zndraw-0.2.0a1.tar", max compression
```

## Comparing `zndraw-0.1.8.tar` & `zndraw-0.2.0a1.tar`

### file list

```diff
@@ -1,1025 +1,1132 @@
--rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.1.8/LICENSE
--rw-r--r--   0        0        0     2020 2023-05-23 11:12:28.775564 zndraw-0.1.8/README.md
--rw-r--r--   0        0        0      834 2023-05-23 11:13:08.035137 zndraw-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      166 2023-04-26 21:59:54.873628 zndraw-0.1.8/zndraw/__init__.py
--rw-r--r--   0        0        0     3933 2023-05-04 14:56:20.539772 zndraw-0.1.8/zndraw/analyse.py
--rw-r--r--   0        0        0     4741 2023-05-23 11:12:28.775564 zndraw-0.1.8/zndraw/app.py
--rw-r--r--   0        0        0     2092 2023-05-02 08:43:51.521509 zndraw-0.1.8/zndraw/cli.py
--rw-r--r--   0        0        0     2695 2023-05-23 11:12:28.775564 zndraw-0.1.8/zndraw/examples/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-22 20:55:05.579300 zndraw-0.1.8/zndraw/io.py
--rw-r--r--   0        0        0      878 2023-05-02 08:43:51.521509 zndraw-0.1.8/zndraw/main.py
--rw-r--r--   0        0        0     4887 2023-05-23 11:12:28.775564 zndraw-0.1.8/zndraw/shared.py
--rw-r--r--   0        0        0     3655 2023-05-23 09:54:59.686413 zndraw-0.1.8/zndraw/static/World/components/draw.js
--rw-r--r--   0        0        0     9533 2023-04-17 10:14:40.724969 zndraw-0.1.8/zndraw/static/favion-192x192.png
--rw-r--r--   0        0        0     5183 2023-05-23 11:12:28.775564 zndraw-0.1.8/zndraw/static/main.css
--rw-r--r--   0        0        0    19182 2023-05-23 11:12:28.785564 zndraw-0.1.8/zndraw/static/main.js
--rw-r--r--   0        0        0     2980 2023-05-23 11:12:28.785564 zndraw-0.1.8/zndraw/static/modules/data.js
--rw-r--r--   0        0        0     2893 2023-05-23 11:12:28.785564 zndraw-0.1.8/zndraw/static/modules/draw.js
--rw-r--r--   0        0        0     1704 2023-05-23 11:12:28.785564 zndraw-0.1.8/zndraw/static/modules/keypress.js
--rw-r--r--   0        0        0     4344 2023-05-23 11:12:28.785564 zndraw-0.1.8/zndraw/static/modules/methods.js
--rw-r--r--   0        0        0    11591 2023-05-23 11:12:28.785564 zndraw-0.1.8/zndraw/static/modules/particles.js
--rw-r--r--   0        0        0     2779 2023-05-23 11:12:28.785564 zndraw-0.1.8/zndraw/static/modules/schemaforms.js
--rw-r--r--   0        0        0     1600 2023-05-22 13:00:16.953583 zndraw-0.1.8/zndraw/static/node_modules/.package-lock.json
--rw-r--r--   0        0        0     1082 2023-05-22 13:00:13.053626 zndraw-0.1.8/zndraw/static/node_modules/@popperjs/core/LICENSE.md
--rw-r--r--   0        0        0    13561 2023-05-22 13:00:13.053626 zndraw-0.1.8/zndraw/static/node_modules/@popperjs/core/README.md
--rw-r--r--   0        0        0       23 2023-05-22 13:00:13.053626 zndraw-0.1.8/zndraw/static/node_modules/@popperjs/core/index.d.ts
--rw-r--r--   0        0        0     4230 2023-05-22 13:00:13.053626 zndraw-0.1.8/zndraw/static/node_modules/@popperjs/core/package.json
--rw-r--r--   0        0        0     1131 2023-05-22 13:00:13.213624 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/LICENSE
--rw-r--r--   0        0        0    13659 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/README.md
--rw-r--r--   0        0        0     1901 2023-05-22 13:00:13.253624 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/alert.js
--rw-r--r--   0        0        0     1930 2023-05-22 13:00:13.263623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/base-component.js
--rw-r--r--   0        0        0     1626 2023-05-22 13:00:13.283623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/button.js
--rw-r--r--   0        0        0    11820 2023-05-22 13:00:13.283623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/carousel.js
--rw-r--r--   0        0        0     7669 2023-05-22 13:00:13.283623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/collapse.js
--rw-r--r--   0        0        0     1405 2023-05-22 13:00:13.293623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dom/data.js
--rw-r--r--   0        0        0     8450 2023-05-22 13:00:13.293623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dom/event-handler.js
--rw-r--r--   0        0        0     1668 2023-05-22 13:00:13.443621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dom/manipulator.js
--rw-r--r--   0        0        0     1968 2023-05-22 13:00:13.463621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dom/selector-engine.js
--rw-r--r--   0        0        0    13257 2023-05-22 13:00:13.293623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dropdown.js
--rw-r--r--   0        0        0     9629 2023-05-22 13:00:13.453621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/modal.js
--rw-r--r--   0        0        0     6804 2023-05-22 13:00:13.453621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/offcanvas.js
--rw-r--r--   0        0        0     1874 2023-05-22 13:00:13.453621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/popover.js
--rw-r--r--   0        0        0     8448 2023-05-22 13:00:13.463621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/scrollspy.js
--rw-r--r--   0        0        0     8756 2023-05-22 13:00:13.463621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/tab.js
--rw-r--r--   0        0        0     5037 2023-05-22 13:00:13.463621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/toast.js
--rw-r--r--   0        0        0    16188 2023-05-22 13:00:13.473621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/tooltip.js
--rw-r--r--   0        0        0     3126 2023-05-22 13:00:13.263623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/backdrop.js
--rw-r--r--   0        0        0     1072 2023-05-22 13:00:13.283623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/component-functions.js
--rw-r--r--   0        0        0     1818 2023-05-22 13:00:13.283623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/config.js
--rw-r--r--   0        0        0     2519 2023-05-22 13:00:13.293623 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/focustrap.js
--rw-r--r--   0        0        0     8436 2023-05-22 13:00:13.443621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/index.js
--rw-r--r--   0        0        0     3253 2023-05-22 13:00:13.453621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/sanitizer.js
--rw-r--r--   0        0        0     3755 2023-05-22 13:00:13.453621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/scrollbar.js
--rw-r--r--   0        0        0     3410 2023-05-22 13:00:13.463621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/swipe.js
--rw-r--r--   0        0        0     3630 2023-05-22 13:00:13.463621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/template-factory.js
--rw-r--r--   0        0        0     9330 2023-05-22 13:00:13.473621 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/package.json
--rw-r--r--   0        0        0     4790 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_accordion.scss
--rw-r--r--   0        0        0     2126 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_alert.scss
--rw-r--r--   0        0        0     1118 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_badge.scss
--rw-r--r--   0        0        0     1751 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_breadcrumb.scss
--rw-r--r--   0        0        0     3073 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_button-group.scss
--rw-r--r--   0        0        0     6685 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_buttons.scss
--rw-r--r--   0        0        0     6736 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_card.scss
--rw-r--r--   0        0        0     5580 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_carousel.scss
--rw-r--r--   0        0        0     1127 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_close.scss
--rw-r--r--   0        0        0     1201 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_containers.scss
--rw-r--r--   0        0        0     8018 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_dropdown.scss
--rw-r--r--   0        0        0      256 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_forms.scss
--rw-r--r--   0        0        0    10554 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_functions.scss
--rw-r--r--   0        0        0      575 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_grid.scss
--rw-r--r--   0        0        0      294 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_helpers.scss
--rw-r--r--   0        0        0     1158 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_images.scss
--rw-r--r--   0        0        0     6475 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_list-group.scss
--rw-r--r--   0        0        0     1648 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_maps.scss
--rw-r--r--   0        0        0      899 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_mixins.scss
--rw-r--r--   0        0        0     7762 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_modal.scss
--rw-r--r--   0        0        0     4665 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_nav.scss
--rw-r--r--   0        0        0     8936 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_navbar.scss
--rw-r--r--   0        0        0     4555 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_offcanvas.scss
--rw-r--r--   0        0        0     3940 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_pagination.scss
--rw-r--r--   0        0        0      859 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_placeholders.scss
--rw-r--r--   0        0        0     6907 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_popover.scss
--rw-r--r--   0        0        0     1875 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_progress.scss
--rw-r--r--   0        0        0    12311 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_reboot.scss
--rw-r--r--   0        0        0     2395 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_root.scss
--rw-r--r--   0        0        0     2429 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_spinners.scss
--rw-r--r--   0        0        0     4358 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_tables.scss
--rw-r--r--   0        0        0     2490 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_toasts.scss
--rw-r--r--   0        0        0     3939 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_tooltip.scss
--rw-r--r--   0        0        0      425 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_transitions.scss
--rw-r--r--   0        0        0     1420 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_type.scss
--rw-r--r--   0        0        0    14817 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_utilities.scss
--rw-r--r--   0        0        0    68610 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_variables.scss
--rw-r--r--   0        0        0     1198 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/bootstrap-grid.scss
--rw-r--r--   0        0        0      163 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/bootstrap-reboot.scss
--rw-r--r--   0        0        0      280 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/bootstrap-utilities.scss
--rw-r--r--   0        0        0      912 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/bootstrap.scss
--rw-r--r--   0        0        0     2030 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_floating-labels.scss
--rw-r--r--   0        0        0     4287 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_form-check.scss
--rw-r--r--   0        0        0     5695 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_form-control.scss
--rw-r--r--   0        0        0     2796 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_form-range.scss
--rw-r--r--   0        0        0     2316 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_form-select.scss
--rw-r--r--   0        0        0      219 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_form-text.scss
--rw-r--r--   0        0        0     3835 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_input-group.scss
--rw-r--r--   0        0        0     1142 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_labels.scss
--rw-r--r--   0        0        0      478 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_validation.scss
--rw-r--r--   0        0        0       37 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_clearfix.scss
--rw-r--r--   0        0        0      454 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_color-bg.scss
--rw-r--r--   0        0        0      450 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_colored-links.scss
--rw-r--r--   0        0        0      621 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_position.scss
--rw-r--r--   0        0        0      399 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_ratio.scss
--rw-r--r--   0        0        0      245 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_stacks.scss
--rw-r--r--   0        0        0      223 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_stretched-link.scss
--rw-r--r--   0        0        0       73 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_text-truncation.scss
--rw-r--r--   0        0        0      136 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_visually-hidden.scss
--rw-r--r--   0        0        0      147 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_vr.scss
--rw-r--r--   0        0        0      393 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_alert.scss
--rw-r--r--   0        0        0      328 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_backdrop.scss
--rw-r--r--   0        0        0      263 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_banner.scss
--rw-r--r--   0        0        0     2031 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_border-radius.scss
--rw-r--r--   0        0        0      398 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_box-shadow.scss
--rw-r--r--   0        0        0     4580 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_breakpoints.scss
--rw-r--r--   0        0        0     3220 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_buttons.scss
--rw-r--r--   0        0        0     1473 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_caret.scss
--rw-r--r--   0        0        0      147 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_clearfix.scss
--rw-r--r--   0        0        0      167 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_color-scheme.scss
--rw-r--r--   0        0        0      410 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_container.scss
--rw-r--r--   0        0        0      613 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_deprecate.scss
--rw-r--r--   0        0        0     4122 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_forms.scss
--rw-r--r--   0        0        0     1956 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_gradients.scss
--rw-r--r--   0        0        0     4726 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_grid.scss
--rw-r--r--   0        0        0      395 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_image.scss
--rw-r--r--   0        0        0      509 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_list-group.scss
--rw-r--r--   0        0        0      168 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_lists.scss
--rw-r--r--   0        0        0      387 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_pagination.scss
--rw-r--r--   0        0        0      495 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_reset-text.scss
--rw-r--r--   0        0        0      202 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_resize.scss
--rw-r--r--   0        0        0     1101 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_table-variants.scss
--rw-r--r--   0        0        0      168 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_text-truncate.scss
--rw-r--r--   0        0        0      661 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_transition.scss
--rw-r--r--   0        0        0     3380 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_utilities.scss
--rw-r--r--   0        0        0     1012 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_visually-hidden.scss
--rw-r--r--   0        0        0     1737 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/utilities/_api.scss
--rw-r--r--   0        0        0    10029 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/vendor/_rfs.scss
--rw-r--r--   0        0        0     1078 2023-05-22 13:00:13.093625 zndraw-0.1.8/zndraw/static/node_modules/plotly.js-dist/LICENSE
--rw-r--r--   0        0        0     1356 2023-05-22 13:00:13.443621 zndraw-0.1.8/zndraw/static/node_modules/plotly.js-dist/README.md
--rw-r--r--   0        0        0      521 2023-05-22 13:00:13.443621 zndraw-0.1.8/zndraw/static/node_modules/plotly.js-dist/package.json
--rw-r--r--   0        0        0  8528210 2023-05-22 13:00:13.373622 zndraw-0.1.8/zndraw/static/node_modules/plotly.js-dist/plotly.js
--rw-r--r--   0        0        0     1081 2023-05-22 13:00:13.453621 zndraw-0.1.8/zndraw/static/node_modules/three/LICENSE
--rw-r--r--   0        0        0     2989 2023-05-22 13:00:14.073615 zndraw-0.1.8/zndraw/static/node_modules/three/README.md
--rw-r--r--   0        0        0     2006 2023-05-22 13:00:13.453621 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/LICENSE
--rw-r--r--   0        0        0      334 2023-05-22 13:00:14.073615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/README.md
--rw-r--r--   0        0        0    10695 2023-05-22 13:00:13.453621 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/NOTICE
--rw-r--r--   0        0        0      692 2023-05-22 13:00:14.073615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/README.txt
--rw-r--r--   0        0        0   329885 2023-05-22 13:00:14.033615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_bold.typeface.json
--rw-r--r--   0        0        0   190569 2023-05-22 13:00:14.033615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_mono_regular.typeface.json
--rw-r--r--   0        0        0   319895 2023-05-22 13:00:14.043615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_regular.typeface.json
--rw-r--r--   0        0        0   485403 2023-05-22 13:00:14.043615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_serif_bold.typeface.json
--rw-r--r--   0        0        0   477058 2023-05-22 13:00:14.053615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_serif_regular.typeface.json
--rw-r--r--   0        0        0   649318 2023-05-22 13:00:14.053615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/gentilis_bold.typeface.json
--rw-r--r--   0        0        0   627529 2023-05-22 13:00:14.063615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/gentilis_regular.typeface.json
--rw-r--r--   0        0        0    61632 2023-05-22 13:00:14.063615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/helvetiker_bold.typeface.json
--rw-r--r--   0        0        0    63182 2023-05-22 13:00:14.063615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/helvetiker_regular.typeface.json
--rw-r--r--   0        0        0   112249 2023-05-22 13:00:14.063615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/optimer_bold.typeface.json
--rw-r--r--   0        0        0   110666 2023-05-22 13:00:14.063615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/optimer_regular.typeface.json
--rw-r--r--   0        0        0      188 2023-05-22 13:00:14.073615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/ttf/README.md
--rw-r--r--   0        0        0    18068 2023-05-22 13:00:14.073615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/ttf/kenpixel.ttf
--rw-r--r--   0        0        0     2556 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/animation/AnimationClipCreator.js
--rw-r--r--   0        0        0     9855 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/animation/CCDIKSolver.js
--rw-r--r--   0        0        0    25130 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/animation/MMDAnimationHelper.js
--rw-r--r--   0        0        0    28135 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/animation/MMDPhysics.js
--rw-r--r--   0        0        0     6106 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/cameras/CinematicCamera.js
--rw-r--r--   0        0        0     1702 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/capabilities/WebGL.js
--rw-r--r--   0        0        0      859 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/capabilities/WebGPU.js
--rw-r--r--   0        0        0    80030 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/ArcballControls.js
--rw-r--r--   0        0        0     4592 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/DragControls.js
--rw-r--r--   0        0        0     6764 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/FirstPersonControls.js
--rw-r--r--   0        0        0     7072 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/FlyControls.js
--rw-r--r--   0        0        0      863 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/MapControls.js
--rw-r--r--   0        0        0    25214 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/OrbitControls.js
--rw-r--r--   0        0        0     3347 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/PointerLockControls.js
--rw-r--r--   0        0        0    17409 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/TrackballControls.js
--rw-r--r--   0        0        0    40287 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/TransformControls.js
--rw-r--r--   0        0        0     9291 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/csm/CSM.js
--rw-r--r--   0        0        0     2741 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/csm/CSMFrustum.js
--rw-r--r--   0        0        0     5832 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/csm/CSMHelper.js
--rw-r--r--   0        0        0     8262 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/csm/CSMShader.js
--rw-r--r--   0        0        0     7326 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/curves/CurveExtras.js
--rw-r--r--   0        0        0     1878 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/curves/NURBSCurve.js
--rw-r--r--   0        0        0     1296 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/curves/NURBSSurface.js
--rw-r--r--   0        0        0     7861 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/curves/NURBSUtils.js
--rw-r--r--   0        0        0     3932 2023-05-22 13:00:13.553620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/AnaglyphEffect.js
--rw-r--r--   0        0        0     6077 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/AsciiEffect.js
--rw-r--r--   0        0        0    12953 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/OutlineEffect.js
--rw-r--r--   0        0        0     2348 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/ParallaxBarrierEffect.js
--rw-r--r--   0        0        0     3549 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/PeppersGhostEffect.js
--rw-r--r--   0        0        0     1179 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/StereoEffect.js
--rw-r--r--   0        0        0     1335 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/environments/DebugEnvironment.js
--rw-r--r--   0        0        0     3606 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/environments/RoomEnvironment.js
--rw-r--r--   0        0        0    19279 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/ColladaExporter.js
--rw-r--r--   0        0        0     6594 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/DRACOExporter.js
--rw-r--r--   0        0        0    10602 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/EXRExporter.js
--rw-r--r--   0        0        0    72734 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/GLTFExporter.js
--rw-r--r--   0        0        0     6633 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/KTX2Exporter.js
--rw-r--r--   0        0        0     4052 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/MMDExporter.js
--rw-r--r--   0        0        0     5370 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/OBJExporter.js
--rw-r--r--   0        0        0    12001 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/PLYExporter.js
--rw-r--r--   0        0        0     3890 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/STLExporter.js
--rw-r--r--   0        0        0    16113 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/USDZExporter.js
--rw-r--r--   0        0        0     1968 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/BoxLineGeometry.js
--rw-r--r--   0        0        0     1035 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/ConvexGeometry.js
--rw-r--r--   0        0        0     8506 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/DecalGeometry.js
--rw-r--r--   0        0        0    32742 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/LightningStrike.js
--rw-r--r--   0        0        0     5472 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/ParametricGeometries.js
--rw-r--r--   0        0        0     2478 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/ParametricGeometry.js
--rw-r--r--   0        0        0     4625 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/RoundedBoxGeometry.js
--rw-r--r--   0        0        0    19498 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/TeapotGeometry.js
--rw-r--r--   0        0        0     1308 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/TextGeometry.js
--rw-r--r--   0        0        0     2818 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/LightProbeHelper.js
--rw-r--r--   0        0        0     1976 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/OctreeHelper.js
--rw-r--r--   0        0        0     2712 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/PositionalAudioHelper.js
--rw-r--r--   0        0        0     2051 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/RectAreaLightHelper.js
--rw-r--r--   0        0        0     1811 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/VertexNormalsHelper.js
--rw-r--r--   0        0        0     1659 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/VertexTangentsHelper.js
--rw-r--r--   0        0        0     8059 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/ViewHelper.js
--rw-r--r--   0        0        0    12655 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/interactive/HTMLMesh.js
--rw-r--r--   0        0        0     2996 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/interactive/InteractiveGroup.js
--rw-r--r--   0        0        0     6139 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/interactive/SelectionBox.js
--rw-r--r--   0        0        0     2430 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/interactive/SelectionHelper.js
--rw-r--r--   0        0        0   393768 2023-05-22 13:00:13.553620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/ammo.wasm.js
--rw-r--r--   0        0        0   651386 2023-05-22 13:00:14.073615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/ammo.wasm.wasm
--rw-r--r--   0        0        0     1448 2023-05-22 13:00:14.073615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/basis/README.md
--rw-r--r--   0        0        0    62337 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/basis/basis_transcoder.js
--rw-r--r--   0        0        0   499935 2023-05-22 13:00:14.083614 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/basis/basis_transcoder.wasm
--rw-r--r--   0        0        0   157440 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/chevrotain.module.min.js
--rw-r--r--   0        0        0     1501 2023-05-22 13:00:14.073615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/README.md
--rw-r--r--   0        0        0   719410 2023-05-22 13:00:13.663619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_decoder.js
--rw-r--r--   0        0        0   285747 2023-05-22 13:00:14.083614 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_decoder.wasm
--rw-r--r--   0        0        0   928718 2023-05-22 13:00:13.683619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_encoder.js
--rw-r--r--   0        0        0    58763 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_wasm_wrapper.js
--rw-r--r--   0        0        0   512465 2023-05-22 13:00:13.673619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_decoder.js
--rw-r--r--   0        0        0   192420 2023-05-22 13:00:14.093614 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_decoder.wasm
--rwxr-xr-x   0        0        0   954360 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_encoder.js
--rw-r--r--   0        0        0    58456 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_wasm_wrapper.js
--rw-r--r--   0        0        0    45516 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/ecsy.module.js
--rw-r--r--   0        0        0    83291 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/fflate.module.js
--rw-r--r--   0        0        0    18676 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/ktx-parse.module.js
--rw-r--r--   0        0        0    29526 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/lil-gui.module.min.js
--rw-r--r--   0        0        0   476927 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/lottie_canvas.module.js
--rw-r--r--   0        0        0    24850 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/meshopt_decoder.module.js
--rw-r--r--   0        0        0    48525 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/mikktspace.module.js
--rw-r--r--   0        0        0   158598 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/mmdparser.module.js
--rw-r--r--   0        0        0    13492 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/motion-controllers.module.js
--rw-r--r--   0        0        0   469356 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/opentype.module.js
--rw-r--r--   0        0        0     3951 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/potpack.module.js
--rw-r--r--   0        0        0   134655 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.js
--rw-r--r--   0        0        0   134252 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.module.js
--rw-r--r--   0        0        0  2803968 2023-05-22 13:00:14.113614 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.wasm
--rw-r--r--   0        0        0     3514 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/stats.module.js
--rw-r--r--   0        0        0    23045 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/tween.module.js
--rw-r--r--   0        0        0   104667 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/utif.module.js
--rw-r--r--   0        0        0    39754 2023-05-22 13:00:14.033615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/zstddec.module.js
--rw-r--r--   0        0        0      387 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lights/IESSpotLight.js
--rw-r--r--   0        0        0     5597 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lights/LightProbeGenerator.js
--rw-r--r--   0        0        0   313854 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lights/RectAreaLightUniformsLib.js
--rw-r--r--   0        0        0      433 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/Line2.js
--rw-r--r--   0        0        0     1458 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/LineGeometry.js
--rw-r--r--   0        0        0    12422 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/LineMaterial.js
--rw-r--r--   0        0        0     9330 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/LineSegments2.js
--rw-r--r--   0        0        0     4632 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/LineSegmentsGeometry.js
--rw-r--r--   0        0        0     1577 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/Wireframe.js
--rw-r--r--   0        0        0      419 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/WireframeGeometry2.js
--rw-r--r--   0        0        0    31227 2023-05-22 13:00:13.493621 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/3DMLoader.js
--rw-r--r--   0        0        0    34478 2023-05-22 13:00:13.493621 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/3MFLoader.js
--rw-r--r--   0        0        0    10621 2023-05-22 13:00:13.533620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/AMFLoader.js
--rw-r--r--   0        0        0     9019 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/BVHLoader.js
--rw-r--r--   0        0        0    83853 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/ColladaLoader.js
--rw-r--r--   0        0        0     6153 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/DDSLoader.js
--rw-r--r--   0        0        0    13508 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/DRACOLoader.js
--rw-r--r--   0        0        0    54975 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/EXRLoader.js
--rw-r--r--   0        0        0    97556 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/FBXLoader.js
--rw-r--r--   0        0        0     3204 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/FontLoader.js
--rw-r--r--   0        0        0     5409 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/GCodeLoader.js
--rw-r--r--   0        0        0   102783 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/GLTFLoader.js
--rw-r--r--   0        0        0     2183 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/HDRCubeTextureLoader.js
--rw-r--r--   0        0        0     7096 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/IESLoader.js
--rw-r--r--   0        0        0     2211 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/KMZLoader.js
--rw-r--r--   0        0        0    19830 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/KTX2Loader.js
--rw-r--r--   0        0        0     6450 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/KTXLoader.js
--rw-r--r--   0        0        0    57006 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LDrawLoader.js
--rw-r--r--   0        0        0     3907 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LUT3dlLoader.js
--rw-r--r--   0        0        0     3441 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LUTCubeLoader.js
--rw-r--r--   0        0        0    23543 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LWOLoader.js
--rw-r--r--   0        0        0    19405 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LogLuvLoader.js
--rw-r--r--   0        0        0     1486 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LottieLoader.js
--rw-r--r--   0        0        0    12372 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MD2Loader.js
--rw-r--r--   0        0        0     2304 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MDDLoader.js
--rw-r--r--   0        0        0    51619 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MMDLoader.js
--rw-r--r--   0        0        0    10580 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MTLLoader.js
--rw-r--r--   0        0        0    14996 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MaterialXLoader.js
--rw-r--r--   0        0        0    13679 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/NRRDLoader.js
--rw-r--r--   0        0        0    21175 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/OBJLoader.js
--rw-r--r--   0        0        0    12080 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PCDLoader.js
--rw-r--r--   0        0        0     6781 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PDBLoader.js
--rw-r--r--   0        0        0    15666 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PLYLoader.js
--rw-r--r--   0        0        0     5741 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PRWMLoader.js
--rw-r--r--   0        0        0     4718 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PVRLoader.js
--rw-r--r--   0        0        0    11793 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/RGBELoader.js
--rw-r--r--   0        0        0    28278 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/RGBMLoader.js
--rw-r--r--   0        0        0     9694 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/STLLoader.js
--rw-r--r--   0        0        0    69560 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/SVGLoader.js
--rw-r--r--   0        0        0    24660 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TDSLoader.js
--rw-r--r--   0        0        0    11138 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TGALoader.js
--rw-r--r--   0        0        0      572 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TIFFLoader.js
--rw-r--r--   0        0        0     4212 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TTFLoader.js
--rw-r--r--   0        0        0    14505 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TiltLoader.js
--rw-r--r--   0        0        0    11483 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/USDZLoader.js
--rw-r--r--   0        0        0     8785 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/VOXLoader.js
--rw-r--r--   0        0        0    72146 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/VRMLLoader.js
--rw-r--r--   0        0        0    27300 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/VTKLoader.js
--rw-r--r--   0        0        0     1795 2023-05-22 13:00:14.033615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/XYZLoader.js
--rw-r--r--   0        0        0    26644 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/IFFParser.js
--rw-r--r--   0        0        0    10137 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/LWO2Parser.js
--rw-r--r--   0        0        0     9269 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/LWO3Parser.js
--rw-r--r--   0        0        0     9751 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/materials/MeshGouraudMaterial.js
--rw-r--r--   0        0        0     2522 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/Capsule.js
--rw-r--r--   0        0        0      723 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/ColorConverter.js
--rw-r--r--   0        0        0    21832 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/ConvexHull.js
--rw-r--r--   0        0        0     2564 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/ImprovedNoise.js
--rw-r--r--   0        0        0     3642 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/Lut.js
--rw-r--r--   0        0        0     4260 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/MeshSurfaceSampler.js
--rw-r--r--   0        0        0    10227 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/OBB.js
--rw-r--r--   0        0        0     9208 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/Octree.js
--rw-r--r--   0        0        0    14351 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/SimplexNoise.js
--rw-r--r--   0        0        0    13577 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/ConvexObjectBreaker.js
--rw-r--r--   0        0        0    12137 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/GPUComputationRenderer.js
--rw-r--r--   0        0        0     1188 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/Gyroscope.js
--rw-r--r--   0        0        0     5216 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/MD2Character.js
--rw-r--r--   0        0        0    11980 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/MD2CharacterComplex.js
--rw-r--r--   0        0        0     1107 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/MorphAnimMesh.js
--rw-r--r--   0        0        0     5459 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/MorphBlendMesh.js
--rw-r--r--   0        0        0    11076 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/ProgressiveLightMap.js
--rw-r--r--   0        0        0    13795 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/RollerCoaster.js
--rw-r--r--   0        0        0     4673 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/TubePainter.js
--rw-r--r--   0        0        0    13500 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/Volume.js
--rw-r--r--   0        0        0     6177 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/VolumeSlice.js
--rw-r--r--   0        0        0     9107 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/modifiers/CurveModifier.js
--rw-r--r--   0        0        0     5296 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/modifiers/EdgeSplitModifier.js
--rw-r--r--   0        0        0    10082 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/modifiers/SimplifyModifier.js
--rw-r--r--   0        0        0     6159 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/modifiers/TessellateModifier.js
--rw-r--r--   0        0        0    11752 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/Nodes.js
--rw-r--r--   0        0        0     2365 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/BitangentNode.js
--rw-r--r--   0        0        0      648 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/BufferNode.js
--rw-r--r--   0        0        0     1583 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/CameraNode.js
--rw-r--r--   0        0        0     2173 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/CubeTextureNode.js
--rw-r--r--   0        0        0     1252 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ExtendedMaterialNode.js
--rw-r--r--   0        0        0     1434 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/InstanceNode.js
--rw-r--r--   0        0        0     6340 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/MaterialNode.js
--rw-r--r--   0        0        0      916 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/MaterialReferenceNode.js
--rw-r--r--   0        0        0      903 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ModelNode.js
--rw-r--r--   0        0        0      785 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ModelViewProjectionNode.js
--rw-r--r--   0        0        0     2276 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/NormalNode.js
--rw-r--r--   0        0        0     3428 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/Object3DNode.js
--rw-r--r--   0        0        0      429 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/PointUVNode.js
--rw-r--r--   0        0        0     2586 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/PositionNode.js
--rw-r--r--   0        0        0     1273 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ReferenceNode.js
--rw-r--r--   0        0        0      733 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ReflectVectorNode.js
--rw-r--r--   0        0        0     3114 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/SkinningNode.js
--rw-r--r--   0        0        0      628 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/StorageBufferNode.js
--rw-r--r--   0        0        0     2280 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/TangentNode.js
--rw-r--r--   0        0        0     3209 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/TextureNode.js
--rw-r--r--   0        0        0      718 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/UVNode.js
--rw-r--r--   0        0        0      644 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/UserDataNode.js
--rw-r--r--   0        0        0     1155 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/CodeNode.js
--rw-r--r--   0        0        0      637 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/ExpressionNode.js
--rw-r--r--   0        0        0     1812 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/FunctionCallNode.js
--rw-r--r--   0        0        0     2006 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/FunctionNode.js
--rw-r--r--   0        0        0     7789 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/ScriptableNode.js
--rw-r--r--   0        0        0     3227 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/ScriptableValueNode.js
--rw-r--r--   0        0        0      389 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/ArrayUniformNode.js
--rw-r--r--   0        0        0     1973 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/AttributeNode.js
--rw-r--r--   0        0        0      745 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/BypassNode.js
--rw-r--r--   0        0        0      768 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/CacheNode.js
--rw-r--r--   0        0        0      538 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/ConstNode.js
--rw-r--r--   0        0        0     1025 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/ContextNode.js
--rw-r--r--   0        0        0     1447 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/InputNode.js
--rw-r--r--   0        0        0      433 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/InstanceIndexNode.js
--rw-r--r--   0        0        0      401 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/LightingModel.js
--rw-r--r--   0        0        0     7371 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/Node.js
--rw-r--r--   0        0        0      163 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeAttribute.js
--rw-r--r--   0        0        0    17154 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeBuilder.js
--rw-r--r--   0        0        0      274 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeCache.js
--rw-r--r--   0        0        0      217 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeCode.js
--rw-r--r--   0        0        0     2049 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeFrame.js
--rw-r--r--   0        0        0      330 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeFunction.js
--rw-r--r--   0        0        0      311 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeFunctionInput.js
--rw-r--r--   0        0        0     1161 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeKeywords.js
--rw-r--r--   0        0        0      127 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeParser.js
--rw-r--r--   0        0        0      340 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeUniform.js
--rw-r--r--   0        0        0     3668 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeUtils.js
--rw-r--r--   0        0        0      145 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeVar.js
--rw-r--r--   0        0        0      229 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeVarying.js
--rw-r--r--   0        0        0     1214 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/PropertyNode.js
--rw-r--r--   0        0        0     1595 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/StackNode.js
--rw-r--r--   0        0        0     1273 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/TempNode.js
--rw-r--r--   0        0        0     1324 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/UniformNode.js
--rw-r--r--   0        0        0     1383 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/VarNode.js
--rw-r--r--   0        0        0     1354 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/VaryingNode.js
--rw-r--r--   0        0        0      612 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/constants.js
--rw-r--r--   0        0        0     2586 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/BlendModeNode.js
--rw-r--r--   0        0        0     2750 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ColorAdjustmentNode.js
--rw-r--r--   0        0        0     2027 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ColorSpaceNode.js
--rw-r--r--   0        0        0      505 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/FrontFacingNode.js
--rw-r--r--   0        0        0     2606 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/NormalMapNode.js
--rw-r--r--   0        0        0      615 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/PosterizeNode.js
--rw-r--r--   0        0        0     3616 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ToneMappingNode.js
--rw-r--r--   0        0        0     2581 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportNode.js
--rw-r--r--   0        0        0      695 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportSharedTextureNode.js
--rw-r--r--   0        0        0     1248 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportTextureNode.js
--rw-r--r--   0        0        0      745 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogExp2Node.js
--rw-r--r--   0        0        0      568 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogNode.js
--rw-r--r--   0        0        0      722 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogRangeNode.js
--rw-r--r--   0        0        0     1005 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_BlinnPhong.js
--rw-r--r--   0        0        0     1145 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_GGX.js
--rw-r--r--   0        0        0      231 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_Lambert.js
--rw-r--r--   0        0        0      973 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/DFGApprox.js
--rw-r--r--   0        0        0      573 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/D_GGX.js
--rw-r--r--   0        0        0      588 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/F_Schlick.js
--rw-r--r--   0        0        0      726 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/V_GGX_SmithCorrelated.js
--rw-r--r--   0        0        0     1231 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/PhongLightingModel.js
--rw-r--r--   0        0        0     3444 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/PhysicalLightingModel.js
--rw-r--r--   0        0        0      389 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/material/getGeometryRoughness.js
--rw-r--r--   0        0        0      541 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/material/getRoughness.js
--rw-r--r--   0        0        0     3103 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/geometry/RangeNode.js
--rw-r--r--   0        0        0     1325 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/gpgpu/ComputeNode.js
--rw-r--r--   0        0        0      440 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/AONode.js
--rw-r--r--   0        0        0      503 2023-05-22 13:00:13.533620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/AmbientLightNode.js
--rw-r--r--   0        0        0     3286 2023-05-22 13:00:13.553620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/AnalyticLightNode.js
--rw-r--r--   0        0        0      981 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/DirectionalLightNode.js
--rw-r--r--   0        0        0     3068 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/EnvironmentNode.js
--rw-r--r--   0        0        0     1358 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/HemisphereLightNode.js
--rw-r--r--   0        0        0      866 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/IESSpotLightNode.js
--rw-r--r--   0        0        0     1025 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightNode.js
--rw-r--r--   0        0        0      663 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightUtils.js
--rw-r--r--   0        0        0     2660 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightingContextNode.js
--rw-r--r--   0        0        0      268 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightingNode.js
--rw-r--r--   0        0        0     2337 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightsNode.js
--rw-r--r--   0        0        0     1737 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/PointLightNode.js
--rw-r--r--   0        0        0     2394 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/SpotLightNode.js
--rw-r--r--   0        0        0     1732 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeLoader.js
--rw-r--r--   0        0        0      918 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeMaterialLoader.js
--rw-r--r--   0        0        0     1097 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeObjectLoader.js
--rw-r--r--   0        0        0      768 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/LineBasicNodeMaterial.js
--rw-r--r--   0        0        0      891 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/Materials.js
--rw-r--r--   0        0        0      744 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshBasicNodeMaterial.js
--rw-r--r--   0        0        0     1139 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshNormalNodeMaterial.js
--rw-r--r--   0        0        0     1623 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshPhongNodeMaterial.js
--rw-r--r--   0        0        0     1843 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshPhysicalNodeMaterial.js
--rw-r--r--   0        0        0     2245 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshStandardNodeMaterial.js
--rw-r--r--   0        0        0     9200 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/NodeMaterial.js
--rw-r--r--   0        0        0      977 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/PointsNodeMaterial.js
--rw-r--r--   0        0        0     2634 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/SpriteNodeMaterial.js
--rw-r--r--   0        0        0    10562 2023-05-22 13:00:14.073615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/DISCLAIMER.md
--rw-r--r--   0        0        0     4232 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/MaterialXNodes.js
--rw-r--r--   0        0        0     2113 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/math/CondNode.js
--rw-r--r--   0        0        0    10373 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/math/MathNode.js
--rw-r--r--   0        0        0     6210 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/math/OperatorNode.js
--rw-r--r--   0        0        0     2894 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/GLSLNodeFunction.js
--rw-r--r--   0        0        0      254 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/GLSLNodeParser.js
--rw-r--r--   0        0        0     1932 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/WGSLNodeFunction.js
--rw-r--r--   0        0        0      254 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/WGSLNodeParser.js
--rw-r--r--   0        0        0      814 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/procedural/CheckerNode.js
--rw-r--r--   0        0        0    10299 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/shadernode/ShaderNode.js
--rw-r--r--   0        0        0      594 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/ArrayElementNode.js
--rw-r--r--   0        0        0     1004 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/ConvertNode.js
--rw-r--r--   0        0        0      576 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/DiscardNode.js
--rw-r--r--   0        0        0      772 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/EquirectUVNode.js
--rw-r--r--   0        0        0      946 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/JoinNode.js
--rw-r--r--   0        0        0      771 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/MatcapUVNode.js
--rw-r--r--   0        0        0      919 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/MaxMipLevelNode.js
--rw-r--r--   0        0        0     1569 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/OscNode.js
--rw-r--r--   0        0        0     1122 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/PackingNode.js
--rw-r--r--   0        0        0      967 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/RemapNode.js
--rw-r--r--   0        0        0     1014 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/RotateUVNode.js
--rw-r--r--   0        0        0      962 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SpecularMIPLevelNode.js
--rw-r--r--   0        0        0     1842 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SplitNode.js
--rw-r--r--   0        0        0      944 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SpriteSheetUVNode.js
--rw-r--r--   0        0        0     1858 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/TimerNode.js
--rw-r--r--   0        0        0     1967 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/TriplanarTexturesNode.js
--rw-r--r--   0        0        0     3420 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/GroundProjectedSkybox.js
--rw-r--r--   0        0        0     8427 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Lensflare.js
--rw-r--r--   0        0        0     7502 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/LightningStorm.js
--rw-r--r--   0        0        0    37944 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/MarchingCubes.js
--rw-r--r--   0        0        0     7294 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Reflector.js
--rw-r--r--   0        0        0    10319 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/ReflectorForSSRPass.js
--rw-r--r--   0        0        0     8419 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Refractor.js
--rw-r--r--   0        0        0     2030 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/ShadowMesh.js
--rw-r--r--   0        0        0     6841 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Sky.js
--rw-r--r--   0        0        0    11125 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Water.js
--rw-r--r--   0        0        0     8395 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Water2.js
--rw-r--r--   0        0        0      645 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/offscreen/jank.js
--rw-r--r--   0        0        0      188 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/offscreen/offscreen.js
--rw-r--r--   0        0        0     2078 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/offscreen/scene.js
--rw-r--r--   0        0        0     6769 2023-05-22 13:00:13.553620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/physics/AmmoPhysics.js
--rw-r--r--   0        0        0     4912 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/physics/RapierPhysics.js
--rw-r--r--   0        0        0     8906 2023-05-22 13:00:13.493621 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/AdaptiveToneMappingPass.js
--rw-r--r--   0        0        0     2186 2023-05-22 13:00:13.503621 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/AfterimagePass.js
--rw-r--r--   0        0        0     3836 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/BloomPass.js
--rw-r--r--   0        0        0     3388 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/BokehPass.js
--rw-r--r--   0        0        0      875 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/ClearPass.js
--rw-r--r--   0        0        0     1940 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/CubeTexturePass.js
--rw-r--r--   0        0        0     1346 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/DotScreenPass.js
--rw-r--r--   0        0        0     4549 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/EffectComposer.js
--rw-r--r--   0        0        0     1456 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/FilmPass.js
--rw-r--r--   0        0        0     3076 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/GlitchPass.js
--rw-r--r--   0        0        0     1522 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/HalftonePass.js
--rw-r--r--   0        0        0     3209 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/LUTPass.js
--rw-r--r--   0        0        0     2120 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/MaskPass.js
--rw-r--r--   0        0        0    20231 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/OutlinePass.js
--rw-r--r--   0        0        0     1603 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/Pass.js
--rw-r--r--   0        0        0     1734 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/RenderPass.js
--rw-r--r--   0        0        0     6102 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/RenderPixelatedPass.js
--rw-r--r--   0        0        0    14008 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SAOPass.js
--rw-r--r--   0        0        0    49430 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SMAAPass.js
--rw-r--r--   0        0        0     6246 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSAARenderPass.js
--rw-r--r--   0        0        0    12016 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSAOPass.js
--rw-r--r--   0        0        0    18496 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSRPass.js
--rw-r--r--   0        0        0     1355 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SavePass.js
--rw-r--r--   0        0        0     1505 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/ShaderPass.js
--rw-r--r--   0        0        0     4605 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/TAARenderPass.js
--rw-r--r--   0        0        0     1316 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/TexturePass.js
--rw-r--r--   0        0        0    12256 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/UnrealBloomPass.js
--rw-r--r--   0        0        0     4407 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/CSS2DRenderer.js
--rw-r--r--   0        0        0     7865 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/CSS3DRenderer.js
--rw-r--r--   0        0        0    19380 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/Projector.js
--rw-r--r--   0        0        0    12465 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/SVGRenderer.js
--rw-r--r--   0        0        0      383 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/SlotNode.js
--rw-r--r--   0        0        0    16860 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/WebGLNodeBuilder.js
--rw-r--r--   0        0        0     1017 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/WebGLNodes.js
--rw-r--r--   0        0        0      802 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUAnimation.js
--rw-r--r--   0        0        0     3444 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUAttributes.js
--rw-r--r--   0        0        0     4642 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBackground.js
--rw-r--r--   0        0        0      265 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBinding.js
--rw-r--r--   0        0        0     5849 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBindings.js
--rw-r--r--   0        0        0      661 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBuffer.js
--rw-r--r--   0        0        0      665 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBufferUtils.js
--rw-r--r--   0        0        0     1358 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUComputePipelines.js
--rw-r--r--   0        0        0     4103 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUGeometries.js
--rw-r--r--   0        0        0     1054 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUInfo.js
--rw-r--r--   0        0        0      324 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUProgrammableStage.js
--rw-r--r--   0        0        0      468 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUProperties.js
--rw-r--r--   0        0        0     3800 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderLists.js
--rw-r--r--   0        0        0      849 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderObject.js
--rw-r--r--   0        0        0     1005 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderObjects.js
--rw-r--r--   0        0        0    16177 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderPipeline.js
--rw-r--r--   0        0        0     7560 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderPipelines.js
--rw-r--r--   0        0        0      746 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderStates.js
--rw-r--r--   0        0        0      289 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderTarget.js
--rw-r--r--   0        0        0    26892 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderer.js
--rw-r--r--   0        0        0     1406 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUSampledTexture.js
--rw-r--r--   0        0        0      463 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUSampler.js
--rw-r--r--   0        0        0      417 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUStorageBuffer.js
--rw-r--r--   0        0        0      634 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextureRenderer.js
--rw-r--r--   0        0        0     4747 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextureUtils.js
--rw-r--r--   0        0        0    29302 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextures.js
--rw-r--r--   0        0        0     2017 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniform.js
--rw-r--r--   0        0        0      357 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniformBuffer.js
--rw-r--r--   0        0        0     5397 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniformsGroup.js
--rw-r--r--   0        0        0     1670 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUtils.js
--rw-r--r--   0        0        0     1076 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUWeakMap.js
--rw-r--r--   0        0        0     7838 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/constants.js
--rw-r--r--   0        0        0    17770 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeBuilder.js
--rw-r--r--   0        0        0      637 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeSampledTexture.js
--rw-r--r--   0        0        0      304 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeSampler.js
--rw-r--r--   0        0        0     1872 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeUniform.js
--rw-r--r--   0        0        0     6826 2023-05-22 13:00:14.013615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodes.js
--rw-r--r--   0        0        0     1871 2023-05-22 13:00:13.493621 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ACESFilmicToneMappingShader.js
--rw-r--r--   0        0        0      875 2023-05-22 13:00:13.503621 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/AfterimageShader.js
--rw-r--r--   0        0        0      328 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BasicShader.js
--rw-r--r--   0        0        0     1182 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BleachBypassShader.js
--rw-r--r--   0        0        0      751 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BlendShader.js
--rw-r--r--   0        0        0     5746 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BokehShader.js
--rw-r--r--   0        0        0     9557 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BokehShader2.js
--rw-r--r--   0        0        0     1030 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BrightnessContrastShader.js
--rw-r--r--   0        0        0      789 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ColorCorrectionShader.js
--rw-r--r--   0        0        0      678 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ColorifyShader.js
--rw-r--r--   0        0        0     1780 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ConvolutionShader.js
--rw-r--r--   0        0        0      546 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/CopyShader.js
--rw-r--r--   0        0        0      891 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/DOFMipMapShader.js
--rw-r--r--   0        0        0     3670 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/DepthLimitedBlurShader.js
--rw-r--r--   0        0        0     2574 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/DigitalGlitch.js
--rw-r--r--   0        0        0     1177 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/DotScreenShader.js
--rw-r--r--   0        0        0     8473 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/FXAAShader.js
--rw-r--r--   0        0        0     2338 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/FilmShader.js
--rw-r--r--   0        0        0     2282 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/FocusShader.js
--rw-r--r--   0        0        0     2944 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/FreiChenShader.js
--rw-r--r--   0        0        0      558 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/GammaCorrectionShader.js
--rw-r--r--   0        0        0     6695 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/GodRaysShader.js
--rw-r--r--   0        0        0     8558 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/HalftoneShader.js
--rw-r--r--   0        0        0     1420 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/HorizontalBlurShader.js
--rw-r--r--   0        0        0     1548 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/HorizontalTiltShiftShader.js
--rw-r--r--   0        0        0     1449 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/HueSaturationShader.js
--rw-r--r--   0        0        0      989 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/KaleidoShader.js
--rw-r--r--   0        0        0     1156 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/LuminosityHighPassShader.js
--rw-r--r--   0        0        0      596 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/LuminosityShader.js
--rw-r--r--   0        0        0     3252 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/MMDToonShader.js
--rw-r--r--   0        0        0      890 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/MirrorShader.js
--rw-r--r--   0        0        0      968 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/NormalMapShader.js
--rw-r--r--   0        0        0     1089 2023-05-22 13:00:13.873617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/RGBShiftShader.js
--rw-r--r--   0        0        0     5160 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SAOShader.js
--rw-r--r--   0        0        0    14545 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SMAAShader.js
--rw-r--r--   0        0        0     6315 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SSAOShader.js
--rw-r--r--   0        0        0     9333 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SSRShader.js
--rw-r--r--   0        0        0      913 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SepiaShader.js
--rw-r--r--   0        0        0     2321 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SobelOperatorShader.js
--rw-r--r--   0        0        0     2908 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SubsurfaceScatteringShader.js
--rw-r--r--   0        0        0      835 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/TechnicolorShader.js
--rw-r--r--   0        0        0     1601 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ToneMapShader.js
--rw-r--r--   0        0        0     6634 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ToonShader.js
--rw-r--r--   0        0        0     1248 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/TriangleBlurShader.js
--rw-r--r--   0        0        0      676 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/UnpackDepthRGBAShader.js
--rw-r--r--   0        0        0     2970 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VelocityShader.js
--rw-r--r--   0        0        0     1416 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VerticalBlurShader.js
--rw-r--r--   0        0        0     1544 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VerticalTiltShiftShader.js
--rw-r--r--   0        0        0      867 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VignetteShader.js
--rw-r--r--   0        0        0     9745 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VolumeShader.js
--rw-r--r--   0        0        0     1706 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/WaterRefractionShader.js
--rw-r--r--   0        0        0      876 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/textures/FlakesTexture.js
--rw-r--r--   0        0        0    31105 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/BufferGeometryUtils.js
--rw-r--r--   0        0        0     2850 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/CameraUtils.js
--rw-r--r--   0        0        0     2470 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/GPUStatsPanel.js
--rw-r--r--   0        0        0    14687 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/GeometryCompressionUtils.js
--rw-r--r--   0        0        0     5113 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/GeometryUtils.js
--rw-r--r--   0        0        0     5808 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/LDrawUtils.js
--rw-r--r--   0        0        0     3950 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/PackedPhongMaterial.js
--rw-r--r--   0        0        0     5511 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/SceneUtils.js
--rw-r--r--   0        0        0     5595 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/ShadowMapViewer.js
--rw-r--r--   0        0        0     8007 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/SkeletonUtils.js
--rw-r--r--   0        0        0     3097 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/UVsDebug.js
--rw-r--r--   0        0        0     1712 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/WorkerPool.js
--rw-r--r--   0        0        0     4352 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/ARButton.js
--rw-r--r--   0        0        0     1756 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/OculusHandModel.js
--rw-r--r--   0        0        0     9461 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/OculusHandPointerModel.js
--rw-r--r--   0        0        0     1018 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/Text2D.js
--rw-r--r--   0        0        0     4222 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/VRButton.js
--rw-r--r--   0        0        0     3585 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRButton.js
--rw-r--r--   0        0        0     6990 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRControllerModelFactory.js
--rw-r--r--   0        0        0     5308 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XREstimatedLight.js
--rw-r--r--   0        0        0     2398 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandMeshModel.js
--rw-r--r--   0        0        0     1841 2023-05-22 13:00:14.033615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandModelFactory.js
--rw-r--r--   0        0        0     2277 2023-05-22 13:00:14.033615 zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandPrimitiveModel.js
--rw-r--r--   0        0        0     3780 2023-05-22 13:00:14.063615 zndraw-0.1.8/zndraw/static/node_modules/three/package.json
--rw-r--r--   0        0        0     7074 2023-05-22 13:00:13.933616 zndraw-0.1.8/zndraw/static/node_modules/three/src/Three.Legacy.js
--rw-r--r--   0        0        0     9631 2023-05-22 13:00:13.933616 zndraw-0.1.8/zndraw/static/node_modules/three/src/Three.js
--rw-r--r--   0        0        0    12606 2023-05-22 13:00:13.553620 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationAction.js
--rw-r--r--   0        0        0     9535 2023-05-22 13:00:13.553620 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationClip.js
--rw-r--r--   0        0        0    16463 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationMixer.js
--rw-r--r--   0        0        0     9230 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationObjectGroup.js
--rw-r--r--   0        0        0     8231 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationUtils.js
--rw-r--r--   0        0        0     9273 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/KeyframeTrack.js
--rw-r--r--   0        0        0    16404 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/PropertyBinding.js
--rw-r--r--   0        0        0     6825 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/PropertyMixer.js
--rw-r--r--   0        0        0      757 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/tracks/BooleanKeyframeTrack.js
--rw-r--r--   0        0        0      445 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/tracks/ColorKeyframeTrack.js
--rw-r--r--   0        0        0      311 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/tracks/NumberKeyframeTrack.js
--rw-r--r--   0        0        0      755 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/tracks/QuaternionKeyframeTrack.js
--rw-r--r--   0        0        0      575 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/tracks/StringKeyframeTrack.js
--rw-r--r--   0        0        0      312 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/tracks/VectorKeyframeTrack.js
--rw-r--r--   0        0        0     6016 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/audio/Audio.js
--rw-r--r--   0        0        0      591 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/audio/AudioAnalyser.js
--rw-r--r--   0        0        0      284 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/audio/AudioContext.js
--rw-r--r--   0        0        0     2893 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/audio/AudioListener.js
--rw-r--r--   0        0        0     2578 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/audio/PositionalAudio.js
--rw-r--r--   0        0        0      236 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/ArrayCamera.js
--rw-r--r--   0        0        0     1209 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/Camera.js
--rw-r--r--   0        0        0     2871 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/CubeCamera.js
--rwxr-xr-x   0        0        0     2730 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/OrthographicCamera.js
--rw-r--r--   0        0        0     5273 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/PerspectiveCamera.js
--rw-r--r--   0        0        0     2694 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/StereoCamera.js
--rw-r--r--   0        0        0     7137 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/src/constants.js
--rw-r--r--   0        0        0    10577 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/BufferAttribute.js
--rw-r--r--   0        0        0    20961 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/BufferGeometry.js
--rw-r--r--   0        0        0      890 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/Clock.js
--rw-r--r--   0        0        0     1479 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/EventDispatcher.js
--rw-r--r--   0        0        0      725 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/GLBufferAttribute.js
--rw-r--r--   0        0        0      631 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InstancedBufferAttribute.js
--rw-r--r--   0        0        0      562 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InstancedBufferGeometry.js
--rw-r--r--   0        0        0      747 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InstancedInterleavedBuffer.js
--rw-r--r--   0        0        0     2388 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InterleavedBuffer.js
--rw-r--r--   0        0        0     5853 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InterleavedBufferAttribute.js
--rw-r--r--   0        0        0      577 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/Layers.js
--rw-r--r--   0        0        0    17943 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/Object3D.js
--rw-r--r--   0        0        0     2234 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/Raycaster.js
--rw-r--r--   0        0        0      199 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/Uniform.js
--rw-r--r--   0        0        0     1179 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/core/UniformsGroup.js
--rw-r--r--   0        0        0     3482 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/DataUtils.js
--rw-r--r--   0        0        0    17687 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/Earcut.js
--rw-r--r--   0        0        0     2496 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/ImageUtils.js
--rw-r--r--   0        0        0    21807 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/PMREMGenerator.js
--rw-r--r--   0        0        0     1516 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/ShapeUtils.js
--rw-r--r--   0        0        0     8025 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/Curve.js
--rw-r--r--   0        0        0     4640 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/CurvePath.js
--rw-r--r--   0        0        0     1223 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/Interpolations.js
--rw-r--r--   0        0        0     3562 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/Path.js
--rw-r--r--   0        0        0     1419 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/Shape.js
--rw-r--r--   0        0        0     5801 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/ShapePath.js
--rw-r--r--   0        0        0      317 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/ArcCurve.js
--rw-r--r--   0        0        0     5479 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/CatmullRomCurve3.js
--rw-r--r--   0        0        0     1315 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/CubicBezierCurve.js
--rw-r--r--   0        0        0     1364 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/CubicBezierCurve3.js
--rw-r--r--   0        0        0      540 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/Curves.js
--rw-r--r--   0        0        0     2753 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/EllipseCurve.js
--rw-r--r--   0        0        0     1318 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/LineCurve.js
--rw-r--r--   0        0        0     1318 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/LineCurve3.js
--rw-r--r--   0        0        0     1189 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/QuadraticBezierCurve.js
--rw-r--r--   0        0        0     1236 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/QuadraticBezierCurve3.js
--rw-r--r--   0        0        0     1678 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/SplineCurve.js
--rw-r--r--   0        0        0     4339 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/BoxGeometry.js
--rw-r--r--   0        0        0      760 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/CapsuleGeometry.js
--rw-r--r--   0        0        0     1960 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/CircleGeometry.js
--rw-r--r--   0        0        0      810 2023-05-22 13:00:13.633619 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/ConeGeometry.js
--rw-r--r--   0        0        0     5865 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/CylinderGeometry.js
--rw-r--r--   0        0        0     1351 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/DodecahedronGeometry.js
--rw-r--r--   0        0        0     4116 2023-05-22 13:00:13.693619 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/EdgesGeometry.js
--rw-r--r--   0        0        0    18337 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/ExtrudeGeometry.js
--rw-r--r--   0        0        0      797 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/Geometries.js
--rw-r--r--   0        0        0      896 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/IcosahedronGeometry.js
--rw-r--r--   0        0        0     3934 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/LatheGeometry.js
--rw-r--r--   0        0        0      641 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/OctahedronGeometry.js
--rw-r--r--   0        0        0     1999 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/PlaneGeometry.js
--rw-r--r--   0        0        0     6436 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/PolyhedronGeometry.js
--rw-r--r--   0        0        0     2760 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/RingGeometry.js
--rw-r--r--   0        0        0     3687 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/ShapeGeometry.js
--rw-r--r--   0        0        0     3129 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/SphereGeometry.js
--rw-r--r--   0        0        0      590 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/TetrahedronGeometry.js
--rw-r--r--   0        0        0     2607 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/TorusGeometry.js
--rw-r--r--   0        0        0     4255 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/TorusKnotGeometry.js
--rw-r--r--   0        0        0     4364 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/TubeGeometry.js
--rw-r--r--   0        0        0     3004 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/WireframeGeometry.js
--rw-r--r--   0        0        0     2740 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/ArrowHelper.js
--rw-r--r--   0        0        0     1486 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/AxesHelper.js
--rw-r--r--   0        0        0     1287 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/Box3Helper.js
--rw-r--r--   0        0        0     2481 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/BoxHelper.js
--rw-r--r--   0        0        0     8392 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/CameraHelper.js
--rw-r--r--   0        0        0     2243 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/DirectionalLightHelper.js
--rw-r--r--   0        0        0     1477 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/GridHelper.js
--rw-r--r--   0        0        0     2047 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/HemisphereLightHelper.js
--rw-r--r--   0        0        0     1737 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/PlaneHelper.js
--rw-r--r--   0        0        0     1724 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/PointLightHelper.js
--rw-r--r--   0        0        0     2096 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/PolarGridHelper.js
--rw-r--r--   0        0        0     2854 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/SkeletonHelper.js
--rw-r--r--   0        0        0     2012 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/SpotLightHelper.js
--rw-r--r--   0        0        0      233 2023-05-22 13:00:13.523621 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/AmbientLight.js
--rw-r--r--   0        0        0      517 2023-05-22 13:00:13.533620 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/AmbientLightProbe.js
--rw-r--r--   0        0        0      703 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/DirectionalLight.js
--rw-r--r--   0        0        0      337 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/DirectionalLightShadow.js
--rw-r--r--   0        0        0      605 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/HemisphereLight.js
--rw-r--r--   0        0        0      879 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/HemisphereLightProbe.js
--rw-r--r--   0        0        0     1168 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/Light.js
--rw-r--r--   0        0        0      679 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/LightProbe.js
--rw-r--r--   0        0        0     2638 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/LightShadow.js
--rw-r--r--   0        0        0     1026 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/PointLight.js
--rw-r--r--   0        0        0     2566 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/PointLightShadow.js
--rw-r--r--   0        0        0      926 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/RectAreaLight.js
--rw-r--r--   0        0        0     1366 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/SpotLight.js
--rw-r--r--   0        0        0      925 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/SpotLightShadow.js
--rw-r--r--   0        0        0     1009 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/AnimationLoader.js
--rw-r--r--   0        0        0     1178 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/AudioLoader.js
--rw-r--r--   0        0        0     5596 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/BufferGeometryLoader.js
--rw-r--r--   0        0        0      503 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/Cache.js
--rw-r--r--   0        0        0     2666 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/CompressedTextureLoader.js
--rw-r--r--   0        0        0      870 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/CubeTextureLoader.js
--rw-r--r--   0        0        0     2626 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/DataTextureLoader.js
--rw-r--r--   0        0        0     5554 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/FileLoader.js
--rw-r--r--   0        0        0     1777 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/ImageBitmapLoader.js
--rw-r--r--   0        0        0     1505 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/ImageLoader.js
--rw-r--r--   0        0        0     1019 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/Loader.js
--rw-r--r--   0        0        0     1308 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/LoaderUtils.js
--rw-r--r--   0        0        0     2033 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/LoadingManager.js
--rw-r--r--   0        0        0    13513 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/MaterialLoader.js
--rw-r--r--   0        0        0    24955 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/ObjectLoader.js
--rw-r--r--   0        0        0      679 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/TextureLoader.js
--rw-r--r--   0        0        0      727 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/LineBasicMaterial.js
--rw-r--r--   0        0        0      524 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/LineDashedMaterial.js
--rw-r--r--   0        0        0    14310 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/Material.js
--rw-r--r--   0        0        0     1428 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/Materials.js
--rw-r--r--   0        0        0     1612 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshBasicMaterial.js
--rw-r--r--   0        0        0      977 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshDepthMaterial.js
--rw-r--r--   0        0        0      699 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshDistanceMaterial.js
--rw-r--r--   0        0        0     2602 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshLambertMaterial.js
--rw-r--r--   0        0        0     1528 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshMatcapMaterial.js
--rw-r--r--   0        0        0     1270 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshNormalMaterial.js
--rw-r--r--   0        0        0     2736 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshPhongMaterial.js
--rw-r--r--   0        0        0     3909 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshPhysicalMaterial.js
--rw-r--r--   0        0        0     2723 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshStandardMaterial.js
--rw-r--r--   0        0        0     2249 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshToonMaterial.js
--rw-r--r--   0        0        0      719 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/PointsMaterial.js
--rw-r--r--   0        0        0      268 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/RawShaderMaterial.js
--rw-r--r--   0        0        0     4004 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/ShaderMaterial.js
--rw-r--r--   0        0        0      513 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/ShadowMaterial.js
--rw-r--r--   0        0        0      761 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/SpriteMaterial.js
--rw-r--r--   0        0        0     3215 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Box2.js
--rw-r--r--   0        0        0    11131 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Box3.js
--rw-r--r--   0        0        0    13676 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Color.js
--rw-r--r--   0        0        0     3481 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/ColorManagement.js
--rw-r--r--   0        0        0      953 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Cylindrical.js
--rw-r--r--   0        0        0     4760 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Euler.js
--rw-r--r--   0        0        0     3449 2023-05-22 13:00:13.723618 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Frustum.js
--rw-r--r--   0        0        0     4271 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Interpolant.js
--rw-r--r--   0        0        0     1776 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Line3.js
--rw-r--r--   0        0        0     8286 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/MathUtils.js
--rw-r--r--   0        0        0     5805 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Matrix3.js
--rw-r--r--   0        0        0    18553 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Matrix4.js
--rw-r--r--   0        0        0     3649 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Plane.js
--rw-r--r--   0        0        0    12518 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Quaternion.js
--rw-r--r--   0        0        0     9979 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Ray.js
--rw-r--r--   0        0        0     3657 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Sphere.js
--rw-r--r--   0        0        0     1355 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Spherical.js
--rw-r--r--   0        0        0     4498 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/SphericalHarmonics3.js
--rw-r--r--   0        0        0     7069 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Triangle.js
--rw-r--r--   0        0        0     5787 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Vector2.js
--rw-r--r--   0        0        0    11022 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Vector3.js
--rw-r--r--   0        0        0    10233 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Vector4.js
--rw-r--r--   0        0        0     2966 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/interpolants/CubicInterpolant.js
--rw-r--r--   0        0        0      482 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/interpolants/DiscreteInterpolant.js
--rw-r--r--   0        0        0      704 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/interpolants/LinearInterpolant.js
--rw-r--r--   0        0        0      789 2023-05-22 13:00:13.863617 zndraw-0.1.8/zndraw/static/node_modules/three/src/math/interpolants/QuaternionLinearInterpolant.js
--rw-r--r--   0        0        0      180 2023-05-22 13:00:13.593620 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Bone.js
--rw-r--r--   0        0        0      184 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Group.js
--rw-r--r--   0        0        0     4172 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/InstancedMesh.js
--rw-r--r--   0        0        0     3173 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/LOD.js
--rw-r--r--   0        0        0     5669 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Line.js
--rw-r--r--   0        0        0      218 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/LineLoop.js
--rw-r--r--   0        0        0     1249 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/LineSegments.js
--rw-r--r--   0        0        0    10318 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Mesh.js
--rw-r--r--   0        0        0     3937 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Points.js
--rw-r--r--   0        0        0     5243 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Skeleton.js
--rw-r--r--   0        0        0     4867 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/SkinnedMesh.js
--rw-r--r--   0        0        0     4796 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Sprite.js
--rw-r--r--   0        0        0      178 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGL1Renderer.js
--rw-r--r--   0        0        0      470 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGL3DRenderTarget.js
--rw-r--r--   0        0        0      488 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGLArrayRenderTarget.js
--rw-r--r--   0        0        0     4441 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGLCubeRenderTarget.js
--rw-r--r--   0        0        0     1686 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGLMultipleRenderTargets.js
--rw-r--r--   0        0        0     3407 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGLRenderTarget.js
--rw-r--r--   0        0        0    62065 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGLRenderer.js
--rw-r--r--   0        0        0      116 2023-05-22 13:00:13.513621 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/alphamap_fragment.glsl.js
--rw-r--r--   0        0        0       88 2023-05-22 13:00:13.513621 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/alphamap_pars_fragment.glsl.js
--rw-r--r--   0        0        0      104 2023-05-22 13:00:13.513621 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/alphatest_fragment.glsl.js
--rw-r--r--   0        0        0       84 2023-05-22 13:00:13.523621 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/alphatest_pars_fragment.glsl.js
--rw-r--r--   0        0        0      532 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/aomap_fragment.glsl.js
--rw-r--r--   0        0        0      113 2023-05-22 13:00:13.563620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/aomap_pars_fragment.glsl.js
--rw-r--r--   0        0        0       67 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/begin_vertex.glsl.js
--rw-r--r--   0        0        0      138 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/beginnormal_vertex.glsl.js
--rw-r--r--   0        0        0      845 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/bsdfs.glsl.js
--rw-r--r--   0        0        0     1137 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/bumpmap_pars_fragment.glsl.js
--rw-r--r--   0        0        0      100 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clearcoat_normal_fragment_begin.glsl.js
--rw-r--r--   0        0        0      262 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clearcoat_normal_fragment_maps.glsl.js
--rw-r--r--   0        0        0      299 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clearcoat_pars_fragment.glsl.js
--rw-r--r--   0        0        0      630 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_fragment.glsl.js
--rw-r--r--   0        0        0      150 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_pars_fragment.glsl.js
--rw-r--r--   0        0        0       96 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_pars_vertex.glsl.js
--rw-r--r--   0        0        0      102 2023-05-22 13:00:13.613620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_vertex.glsl.js
--rw-r--r--   0        0        0      153 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/color_fragment.glsl.js
--rw-r--r--   0        0        0      143 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/color_pars_fragment.glsl.js
--rw-r--r--   0        0        0      178 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/color_pars_vertex.glsl.js
--rw-r--r--   0        0        0      297 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/color_vertex.glsl.js
--rw-r--r--   0        0        0     3881 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/common.glsl.js
--rw-r--r--   0        0        0     4004 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/cube_uv_reflection_fragment.glsl.js
--rw-r--r--   0        0        0       90 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/default_fragment.glsl.js
--rw-r--r--   0        0        0      121 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/default_vertex.glsl.js
--rw-r--r--   0        0        0      705 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/defaultnormal_vertex.glsl.js
--rw-r--r--   0        0        0      169 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/displacementmap_pars_vertex.glsl.js
--rw-r--r--   0        0        0      205 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/displacementmap_vertex.glsl.js
--rw-r--r--   0        0        0      107 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/dithering_fragment.glsl.js
--rw-r--r--   0        0        0      608 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/dithering_pars_fragment.glsl.js
--rw-r--r--   0        0        0      172 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/emissivemap_fragment.glsl.js
--rw-r--r--   0        0        0       94 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/emissivemap_pars_fragment.glsl.js
--rw-r--r--   0        0        0       82 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/encodings_fragment.glsl.js
--rw-r--r--   0        0        0      293 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/encodings_pars_fragment.glsl.js
--rw-r--r--   0        0        0      216 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_common_pars_fragment.glsl.js
--rw-r--r--   0        0        0     1242 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_fragment.glsl.js
--rw-r--r--   0        0        0      345 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_pars_fragment.glsl.js
--rw-r--r--   0        0        0      320 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_pars_vertex.glsl.js
--rw-r--r--   0        0        0     1027 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_physical_pars_fragment.glsl.js
--rw-r--r--   0        0        0      647 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_vertex.glsl.js
--rw-r--r--   0        0        0      303 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/fog_fragment.glsl.js
--rw-r--r--   0        0        0      218 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/fog_pars_fragment.glsl.js
--rw-r--r--   0        0        0       80 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/fog_pars_vertex.glsl.js
--rw-r--r--   0        0        0       83 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/fog_vertex.glsl.js
--rw-r--r--   0        0        0      512 2023-05-22 13:00:13.733618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/gradientmap_pars_fragment.glsl.js
--rw-r--r--   0        0        0     3632 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/iridescence_fragment.glsl.js
--rw-r--r--   0        0        0      191 2023-05-22 13:00:13.743618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/iridescence_pars_fragment.glsl.js
--rw-r--r--   0        0        0      239 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lightmap_fragment.glsl.js
--rw-r--r--   0        0        0      122 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lightmap_pars_fragment.glsl.js
--rw-r--r--   0        0        0     5799 2023-05-22 13:00:13.753618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_begin.glsl.js
--rw-r--r--   0        0        0      293 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_end.glsl.js
--rw-r--r--   0        0        0      721 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_maps.glsl.js
--rw-r--r--   0        0        0      144 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_lambert_fragment.glsl.js
--rw-r--r--   0        0        0      873 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_lambert_pars_fragment.glsl.js
--rw-r--r--   0        0        0     5466 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_pars_begin.glsl.js
--rw-r--r--   0        0        0      222 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_phong_fragment.glsl.js
--rw-r--r--   0        0        0     1146 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_phong_pars_fragment.glsl.js
--rw-r--r--   0        0        0     3038 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_physical_fragment.glsl.js
--rw-r--r--   0        0        0    16313 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_physical_pars_fragment.glsl.js
--rw-r--r--   0        0        0       95 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_toon_fragment.glsl.js
--rw-r--r--   0        0        0      811 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_toon_pars_fragment.glsl.js
--rw-r--r--   0        0        0      315 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/logdepthbuf_fragment.glsl.js
--rw-r--r--   0        0        0      192 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/logdepthbuf_pars_fragment.glsl.js
--rw-r--r--   0        0        0      200 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/logdepthbuf_pars_vertex.glsl.js
--rw-r--r--   0        0        0      393 2023-05-22 13:00:13.773618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/logdepthbuf_vertex.glsl.js
--rw-r--r--   0        0        0       97 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/map_fragment.glsl.js
--rw-r--r--   0        0        0       78 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/map_pars_fragment.glsl.js
--rw-r--r--   0        0        0      381 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/map_particle_fragment.glsl.js
--rw-r--r--   0        0        0      292 2023-05-22 13:00:13.783618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/map_particle_pars_fragment.glsl.js
--rw-r--r--   0        0        0      294 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/metalnessmap_fragment.glsl.js
--rw-r--r--   0        0        0       96 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/metalnessmap_pars_fragment.glsl.js
--rw-r--r--   0        0        0      861 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphcolor_vertex.glsl.js
--rw-r--r--   0        0        0      936 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphnormal_vertex.glsl.js
--rw-r--r--   0        0        0      832 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphtarget_pars_vertex.glsl.js
--rw-r--r--   0        0        0     1215 2023-05-22 13:00:13.813617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphtarget_vertex.glsl.js
--rw-r--r--   0        0        0     1132 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_fragment_begin.glsl.js
--rw-r--r--   0        0        0      642 2023-05-22 13:00:13.823617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_fragment_maps.glsl.js
--rw-r--r--   0        0        0      165 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_pars_fragment.glsl.js
--rw-r--r--   0        0        0      165 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_pars_vertex.glsl.js
--rw-r--r--   0        0        0      303 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_vertex.glsl.js
--rw-r--r--   0        0        0      942 2023-05-22 13:00:13.833617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normalmap_pars_fragment.glsl.js
--rw-r--r--   0        0        0      261 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/output_fragment.glsl.js
--rw-r--r--   0        0        0     2171 2023-05-22 13:00:13.843617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/packing.glsl.js
--rw-r--r--   0        0        0      223 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/premultiplied_alpha_fragment.glsl.js
--rw-r--r--   0        0        0      239 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/project_vertex.glsl.js
--rw-r--r--   0        0        0      294 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/roughnessmap_fragment.glsl.js
--rw-r--r--   0        0        0       96 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/roughnessmap_pars_fragment.glsl.js
--rw-r--r--   0        0        0     9965 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_pars_fragment.glsl.js
--rw-r--r--   0        0        0     1368 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_pars_vertex.glsl.js
--rw-r--r--   0        0        0     1798 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_vertex.glsl.js
--rw-r--r--   0        0        0     1509 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmask_pars_fragment.glsl.js
--rw-r--r--   0        0        0      247 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinbase_vertex.glsl.js
--rw-r--r--   0        0        0      795 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinning_pars_vertex.glsl.js
--rw-r--r--   0        0        0      400 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinning_vertex.glsl.js
--rw-r--r--   0        0        0      481 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinnormal_vertex.glsl.js
--rw-r--r--   0        0        0      221 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/specularmap_fragment.glsl.js
--rw-r--r--   0        0        0       94 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/specularmap_pars_fragment.glsl.js
--rw-r--r--   0        0        0      120 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/tonemapping_fragment.glsl.js
--rw-r--r--   0        0        0     2018 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/tonemapping_pars_fragment.glsl.js
--rw-r--r--   0        0        0     1099 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/transmission_fragment.glsl.js
--rw-r--r--   0        0        0     5804 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/transmission_pars_fragment.glsl.js
--rw-r--r--   0        0        0     1530 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_pars_fragment.glsl.js
--rw-r--r--   0        0        0     2355 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_pars_vertex.glsl.js
--rw-r--r--   0        0        0     2606 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_vertex.glsl.js
--rw-r--r--   0        0        0      357 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/worldpos_vertex.glsl.js
--rw-r--r--   0        0        0    15020 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk.js
--rw-r--r--   0        0        0      497 2023-05-22 13:00:13.573620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/background.glsl.js
--rw-r--r--   0        0        0     1079 2023-05-22 13:00:13.583620 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/backgroundCube.glsl.js
--rw-r--r--   0        0        0      653 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/cube.glsl.js
--rw-r--r--   0        0        0     2069 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/depth.glsl.js
--rw-r--r--   0        0        0     1500 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/distanceRGBA.glsl.js
--rw-r--r--   0        0        0      567 2023-05-22 13:00:13.703619 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/equirect.glsl.js
--rw-r--r--   0        0        0     1522 2023-05-22 13:00:13.763618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/linedashed.glsl.js
--rw-r--r--   0        0        0     2561 2023-05-22 13:00:13.793618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshbasic.glsl.js
--rw-r--r--   0        0        0     3032 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshlambert.glsl.js
--rw-r--r--   0        0        0     2532 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshmatcap.glsl.js
--rw-r--r--   0        0        0     1718 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshnormal.glsl.js
--rw-r--r--   0        0        0     3138 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshphong.glsl.js
--rw-r--r--   0        0        0     5169 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshphysical.glsl.js
--rw-r--r--   0        0        0     2832 2023-05-22 13:00:13.803618 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshtoon.glsl.js
--rw-r--r--   0        0        0     1660 2023-05-22 13:00:13.853617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/points.glsl.js
--rw-r--r--   0        0        0     1128 2023-05-22 13:00:13.893617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/shadow.glsl.js
--rw-r--r--   0        0        0     1896 2023-05-22 13:00:13.913616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/sprite.glsl.js
--rw-r--r--   0        0        0     1206 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/vsm.glsl.js
--rw-r--r--   0        0        0     8167 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib.js
--rw-r--r--   0        0        0     4406 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/UniformsLib.js
--rw-r--r--   0        0        0     1666 2023-05-22 13:00:13.963616 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/UniformsUtils.js
--rw-r--r--   0        0        0      767 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLAnimation.js
--rw-r--r--   0        0        0     3453 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLAttributes.js
--rw-r--r--   0        0        0     6412 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBackground.js
--rw-r--r--   0        0        0    13419 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBindingStates.js
--rw-r--r--   0        0        0     1050 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBufferRenderer.js
--rw-r--r--   0        0        0     3167 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCapabilities.js
--rw-r--r--   0        0        0     3372 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLClipping.js
--rw-r--r--   0        0        0     1956 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCubeMaps.js
--rw-r--r--   0        0        0     2755 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCubeUVMaps.js
--rw-r--r--   0        0        0     2217 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLExtensions.js
--rw-r--r--   0        0        0     3623 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLGeometries.js
--rw-r--r--   0        0        0     1281 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLIndexedBufferRenderer.js
--rw-r--r--   0        0        0     1044 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLInfo.js
--rw-r--r--   0        0        0    13387 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLLights.js
--rw-r--r--   0        0        0    12823 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLMaterials.js
--rw-r--r--   0        0        0     7750 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLMorphtargets.js
--rw-r--r--   0        0        0     1290 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLObjects.js
--rw-r--r--   0        0        0    28100 2023-05-22 13:00:13.993615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLProgram.js
--rw-r--r--   0        0        0    19534 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLPrograms.js
--rw-r--r--   0        0        0      560 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLProperties.js
--rw-r--r--   0        0        0     4054 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLRenderLists.js
--rw-r--r--   0        0        0     1687 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLRenderStates.js
--rw-r--r--   0        0        0      196 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShader.js
--rw-r--r--   0        0        0     1975 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShaderCache.js
--rw-r--r--   0        0        0    10649 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShadowMap.js
--rw-r--r--   0        0        0    25232 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLState.js
--rw-r--r--   0        0        0    56653 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLTextures.js
--rw-r--r--   0        0        0    20325 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUniforms.js
--rw-r--r--   0        0        0     8558 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUniformsGroups.js
--rw-r--r--   0        0        0     9973 2023-05-22 13:00:14.003615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUtils.js
--rw-r--r--   0        0        0     6520 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webxr/WebXRController.js
--rw-r--r--   0        0        0    19550 2023-05-22 13:00:14.023615 zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webxr/WebXRManager.js
--rw-r--r--   0        0        0      442 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/src/scenes/Fog.js
--rw-r--r--   0        0        0      427 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/src/scenes/FogExp2.js
--rw-r--r--   0        0        0     1785 2023-05-22 13:00:13.883617 zndraw-0.1.8/zndraw/static/node_modules/three/src/scenes/Scene.js
--rw-r--r--   0        0        0      361 2023-05-22 13:00:13.603620 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/CanvasTexture.js
--rw-r--r--   0        0        0      434 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/CompressedArrayTexture.js
--rw-r--r--   0        0        0      703 2023-05-22 13:00:13.623619 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/CompressedTexture.js
--rw-r--r--   0        0        0      642 2023-05-22 13:00:13.643619 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/CubeTexture.js
--rw-r--r--   0        0        0      793 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/Data3DTexture.js
--rw-r--r--   0        0        0      544 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/DataArrayTexture.js
--rw-r--r--   0        0        0      603 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/DataTexture.js
--rw-r--r--   0        0        0     1109 2023-05-22 13:00:13.653619 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/DepthTexture.js
--rw-r--r--   0        0        0      436 2023-05-22 13:00:13.713619 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/FramebufferTexture.js
--rw-r--r--   0        0        0     1843 2023-05-22 13:00:13.903617 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/Source.js
--rw-r--r--   0        0        0     6777 2023-05-22 13:00:13.923616 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/Texture.js
--rw-r--r--   0        0        0     1111 2023-05-22 13:00:13.983615 zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/VideoTexture.js
--rw-r--r--   0        0        0     1404 2023-05-22 13:00:13.973616 zndraw-0.1.8/zndraw/static/node_modules/three/src/utils.js
--rw-r--r--   0        0        0    18257 2023-05-23 11:12:28.795564 zndraw-0.1.8/zndraw/templates/index.html
--rw-r--r--   0        0        0       68 2023-04-27 11:21:12.206714 zndraw-0.1.8/zndraw/tools/__init__.py
--rw-r--r--   0        0        0      699 2023-05-23 11:12:28.795564 zndraw-0.1.8/zndraw/tools/data.py
--rw-r--r--   0        0        0      856 2023-04-27 11:21:12.206714 zndraw-0.1.8/zndraw/tools/select.py
--rw-r--r--   0        0        0     2991 1970-01-01 00:00:00.000000 zndraw-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-04-12 16:10:14.508402 zndraw-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0     2219 2023-05-15 11:14:00.799165 zndraw-0.2.0a1/README.md
+-rw-r--r--   0        0        0      882 2023-05-17 07:28:24.211480 zndraw-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-04-26 21:59:54.873628 zndraw-0.2.0a1/zndraw/__init__.py
+-rw-r--r--   0        0        0     3933 2023-05-04 14:56:20.539772 zndraw-0.2.0a1/zndraw/analyse.py
+-rw-r--r--   0        0        0     4986 2023-05-16 16:14:57.211667 zndraw-0.2.0a1/zndraw/app.py
+-rw-r--r--   0        0        0     2092 2023-05-02 08:43:51.521509 zndraw-0.2.0a1/zndraw/cli.py
+-rw-r--r--   0        0        0     2695 2023-05-03 13:11:03.981013 zndraw-0.2.0a1/zndraw/examples/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-22 20:55:05.579300 zndraw-0.2.0a1/zndraw/io.py
+-rw-r--r--   0        0        0      878 2023-05-02 08:43:51.521509 zndraw-0.2.0a1/zndraw/main.py
+-rw-r--r--   0        0        0     4926 2023-05-15 16:29:00.984885 zndraw-0.2.0a1/zndraw/shared.py
+-rw-r--r--   0        0        0      198 2023-05-15 11:35:24.785385 zndraw-0.2.0a1/zndraw/static/.eslintrc.json
+-rw-r--r--   0        0        0       14 2023-05-15 09:14:27.397718 zndraw-0.2.0a1/zndraw/static/.gitignore
+-rw-r--r--   0        0        0        3 2023-05-15 11:35:10.225541 zndraw-0.2.0a1/zndraw/static/.prettierrc.json
+-rw-r--r--   0        0        0     7473 2023-05-17 07:08:03.024411 zndraw-0.2.0a1/zndraw/static/UI/UI.js
+-rw-r--r--   0        0        0     2988 2023-05-16 16:01:27.100288 zndraw-0.2.0a1/zndraw/static/UI/schemaforms.js
+-rw-r--r--   0        0        0     1876 2023-05-17 07:01:07.738799 zndraw-0.2.0a1/zndraw/static/World/World.js
+-rw-r--r--   0        0        0      459 2023-05-15 16:19:43.360961 zndraw-0.2.0a1/zndraw/static/World/components/camera.js
+-rw-r--r--   0        0        0      277 2023-05-15 16:20:32.780422 zndraw-0.2.0a1/zndraw/static/World/components/lights.js
+-rw-r--r--   0        0        0     8525 2023-05-17 07:08:06.084378 zndraw-0.2.0a1/zndraw/static/World/components/particles.js
+-rw-r--r--   0        0        0      179 2023-05-15 11:35:24.965383 zndraw-0.2.0a1/zndraw/static/World/components/scene.js
+-rw-r--r--   0        0        0     1116 2023-05-16 12:28:19.648433 zndraw-0.2.0a1/zndraw/static/World/systems/Loop.js
+-rw-r--r--   0        0        0      659 2023-05-15 11:35:25.025382 zndraw-0.2.0a1/zndraw/static/World/systems/Resizer.js
+-rw-r--r--   0        0        0     2673 2023-05-16 15:59:54.061278 zndraw-0.2.0a1/zndraw/static/World/systems/Stream.js
+-rw-r--r--   0        0        0      915 2023-05-16 11:19:21.993438 zndraw-0.2.0a1/zndraw/static/World/systems/controls.js
+-rw-r--r--   0        0        0      177 2023-05-15 11:35:25.005382 zndraw-0.2.0a1/zndraw/static/World/systems/renderer.js
+-rw-r--r--   0        0        0      797 2023-05-16 09:51:00.991320 zndraw-0.2.0a1/zndraw/static/World/systems/select.js
+-rw-r--r--   0        0        0     9533 2023-04-17 10:14:40.724969 zndraw-0.2.0a1/zndraw/static/favion-192x192.png
+-rw-r--r--   0        0        0     5036 2023-05-15 11:35:24.835384 zndraw-0.2.0a1/zndraw/static/main.css
+-rw-r--r--   0        0        0     1811 2023-05-16 15:59:54.061278 zndraw-0.2.0a1/zndraw/static/main.js
+-rw-r--r--   0        0        0      917 2023-05-17 07:27:50.641837 zndraw-0.2.0a1/zndraw/static/node_modules/.package-lock.json
+-rw-r--r--   0        0        0     1131 2023-05-17 07:27:49.151852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/LICENSE
+-rw-r--r--   0        0        0    13659 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/README.md
+-rw-r--r--   0        0        0    71861 2023-05-17 07:27:49.151852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   210357 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    53265 2023-05-17 07:27:49.151852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   131395 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    71935 2023-05-17 07:27:49.151852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   210361 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    53340 2023-05-17 07:27:49.151852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   131472 2023-05-17 07:27:49.221851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0     7965 2023-05-17 07:27:49.151852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   110875 2023-05-17 07:27:49.221851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0     6490 2023-05-17 07:27:49.151852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    40331 2023-05-17 07:27:49.221851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0     7958 2023-05-17 07:27:49.151852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   110888 2023-05-17 07:27:49.221851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0     6562 2023-05-17 07:27:49.151852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    48693 2023-05-17 07:27:49.221851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0    76347 2023-05-17 07:27:49.161852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   212450 2023-05-17 07:27:49.231851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    58266 2023-05-17 07:27:49.161852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   131956 2023-05-17 07:27:49.231851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0    76214 2023-05-17 07:27:49.161852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   212393 2023-05-17 07:27:49.231851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    58194 2023-05-17 07:27:49.161852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   131791 2023-05-17 07:27:49.231851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   237950 2023-05-17 07:27:49.161852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0        0        0   608300 2023-05-17 07:27:49.251851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0        0        0   194901 2023-05-17 07:27:49.161852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0        0        0   522639 2023-05-17 07:27:49.261851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   237528 2023-05-17 07:27:49.171852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   608144 2023-05-17 07:27:49.271851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   195007 2023-05-17 07:27:49.171852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   767483 2023-05-17 07:27:49.381850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207989 2023-05-17 07:27:49.181852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   451770 2023-05-17 07:27:49.241851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80420 2023-05-17 07:27:49.181852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   333078 2023-05-17 07:27:49.241851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   136215 2023-05-17 07:27:49.181852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   308207 2023-05-17 07:27:49.251851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73978 2023-05-17 07:27:49.181852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   221179 2023-05-17 07:27:49.251851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145543 2023-05-17 07:27:49.181852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0        0        0   309348 2023-05-17 07:27:49.261851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60404 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0        0        0   216913 2023-05-17 07:27:49.261851 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/dist/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     3140 2023-05-17 07:27:49.171852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/alert.js
+-rw-r--r--   0        0        0     4294 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/alert.js.map
+-rw-r--r--   0        0        0     3224 2023-05-17 07:27:49.181852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/base-component.js
+-rw-r--r--   0        0        0     4602 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/base-component.js.map
+-rw-r--r--   0        0        0     2756 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/button.js
+-rw-r--r--   0        0        0     3466 2023-05-17 07:27:49.381850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/button.js.map
+-rw-r--r--   0        0        0    14281 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/carousel.js
+-rw-r--r--   0        0        0    27442 2023-05-17 07:27:49.381850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/carousel.js.map
+-rw-r--r--   0        0        0     9455 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/collapse.js
+-rw-r--r--   0        0        0    18212 2023-05-17 07:27:49.381850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/collapse.js.map
+-rw-r--r--   0        0        0     2119 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dom/data.js
+-rw-r--r--   0        0        0     3047 2023-05-17 07:27:49.391850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dom/data.js.map
+-rw-r--r--   0        0        0     9578 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dom/event-handler.js
+-rw-r--r--   0        0        0    19800 2023-05-17 07:27:49.391850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dom/event-handler.js.map
+-rw-r--r--   0        0        0     2438 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dom/manipulator.js
+-rw-r--r--   0        0        0     4319 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dom/manipulator.js.map
+-rw-r--r--   0        0        0     2700 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dom/selector-engine.js
+-rw-r--r--   0        0        0     4619 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dom/selector-engine.js.map
+-rw-r--r--   0        0        0    16199 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dropdown.js
+-rw-r--r--   0        0        0    29448 2023-05-17 07:27:49.391850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/dropdown.js.map
+-rw-r--r--   0        0        0    12194 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/modal.js
+-rw-r--r--   0        0        0    22634 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/modal.js.map
+-rw-r--r--   0        0        0     9166 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/offcanvas.js
+-rw-r--r--   0        0        0    16142 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/offcanvas.js.map
+-rw-r--r--   0        0        0     2883 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/popover.js
+-rw-r--r--   0        0        0     4053 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/popover.js.map
+-rw-r--r--   0        0        0    10303 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/scrollspy.js
+-rw-r--r--   0        0        0    18973 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/scrollspy.js.map
+-rw-r--r--   0        0        0    10647 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/tab.js
+-rw-r--r--   0        0        0    19947 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/tab.js.map
+-rw-r--r--   0        0        0     6632 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/toast.js
+-rw-r--r--   0        0        0    12018 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/toast.js.map
+-rw-r--r--   0        0        0    19225 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/tooltip.js
+-rw-r--r--   0        0        0    37599 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/tooltip.js.map
+-rw-r--r--   0        0        0     4413 2023-05-17 07:27:49.171852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/backdrop.js
+-rw-r--r--   0        0        0     7172 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/backdrop.js.map
+-rw-r--r--   0        0        0     2174 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/component-functions.js
+-rw-r--r--   0        0        0     2310 2023-05-17 07:27:49.381850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/component-functions.js.map
+-rw-r--r--   0        0        0     2808 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/config.js
+-rw-r--r--   0        0        0     4073 2023-05-17 07:27:49.391850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/config.js.map
+-rw-r--r--   0        0        0     3913 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/focustrap.js
+-rw-r--r--   0        0        0     5891 2023-05-17 07:27:49.391850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/focustrap.js.map
+-rw-r--r--   0        0        0    10248 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/index.js
+-rw-r--r--   0        0        0    18675 2023-05-17 07:27:49.391850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/index.js.map
+-rw-r--r--   0        0        0     4253 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/sanitizer.js
+-rw-r--r--   0        0        0     7572 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/sanitizer.js.map
+-rw-r--r--   0        0        0     5031 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/scrollbar.js
+-rw-r--r--   0        0        0     8041 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/scrollbar.js.map
+-rw-r--r--   0        0        0     4733 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/swipe.js
+-rw-r--r--   0        0        0     8335 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/swipe.js.map
+-rw-r--r--   0        0        0     4980 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/template-factory.js
+-rw-r--r--   0        0        0     8655 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/dist/util/template-factory.js.map
+-rw-r--r--   0        0        0     1901 2023-05-17 07:27:49.171852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/alert.js
+-rw-r--r--   0        0        0     1930 2023-05-17 07:27:49.181852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/base-component.js
+-rw-r--r--   0        0        0     1626 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/button.js
+-rw-r--r--   0        0        0    11820 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/carousel.js
+-rw-r--r--   0        0        0     7669 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/collapse.js
+-rw-r--r--   0        0        0     1405 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dom/data.js
+-rw-r--r--   0        0        0     8450 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dom/event-handler.js
+-rw-r--r--   0        0        0     1668 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dom/manipulator.js
+-rw-r--r--   0        0        0     1968 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dom/selector-engine.js
+-rw-r--r--   0        0        0    13257 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dropdown.js
+-rw-r--r--   0        0        0     9629 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/modal.js
+-rw-r--r--   0        0        0     6804 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/offcanvas.js
+-rw-r--r--   0        0        0     1874 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/popover.js
+-rw-r--r--   0        0        0     8448 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/scrollspy.js
+-rw-r--r--   0        0        0     8756 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/tab.js
+-rw-r--r--   0        0        0     5037 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/toast.js
+-rw-r--r--   0        0        0    16188 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/tooltip.js
+-rw-r--r--   0        0        0     3126 2023-05-17 07:27:49.181852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/backdrop.js
+-rw-r--r--   0        0        0     1072 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/component-functions.js
+-rw-r--r--   0        0        0     1818 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/config.js
+-rw-r--r--   0        0        0     2519 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/focustrap.js
+-rw-r--r--   0        0        0     8436 2023-05-17 07:27:49.191852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/index.js
+-rw-r--r--   0        0        0     3253 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/sanitizer.js
+-rw-r--r--   0        0        0     3755 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/scrollbar.js
+-rw-r--r--   0        0        0     3410 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/swipe.js
+-rw-r--r--   0        0        0     3630 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/template-factory.js
+-rw-r--r--   0        0        0     9330 2023-05-17 07:27:49.211852 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/package.json
+-rw-r--r--   0        0        0     4790 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_accordion.scss
+-rw-r--r--   0        0        0     2126 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_alert.scss
+-rw-r--r--   0        0        0     1118 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_badge.scss
+-rw-r--r--   0        0        0     1751 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_breadcrumb.scss
+-rw-r--r--   0        0        0     3073 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_button-group.scss
+-rw-r--r--   0        0        0     6685 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_buttons.scss
+-rw-r--r--   0        0        0     6736 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_card.scss
+-rw-r--r--   0        0        0     5580 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_carousel.scss
+-rw-r--r--   0        0        0     1127 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_close.scss
+-rw-r--r--   0        0        0     1201 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_containers.scss
+-rw-r--r--   0        0        0     8018 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_dropdown.scss
+-rw-r--r--   0        0        0      256 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_forms.scss
+-rw-r--r--   0        0        0    10554 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_functions.scss
+-rw-r--r--   0        0        0      575 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_grid.scss
+-rw-r--r--   0        0        0      294 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_helpers.scss
+-rw-r--r--   0        0        0     1158 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_images.scss
+-rw-r--r--   0        0        0     6475 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_list-group.scss
+-rw-r--r--   0        0        0     1648 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_maps.scss
+-rw-r--r--   0        0        0      899 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_mixins.scss
+-rw-r--r--   0        0        0     7762 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_modal.scss
+-rw-r--r--   0        0        0     4665 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_nav.scss
+-rw-r--r--   0        0        0     8936 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_navbar.scss
+-rw-r--r--   0        0        0     4555 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_offcanvas.scss
+-rw-r--r--   0        0        0     3940 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_pagination.scss
+-rw-r--r--   0        0        0      859 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_placeholders.scss
+-rw-r--r--   0        0        0     6907 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_popover.scss
+-rw-r--r--   0        0        0     1875 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_progress.scss
+-rw-r--r--   0        0        0    12311 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_reboot.scss
+-rw-r--r--   0        0        0     2395 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_root.scss
+-rw-r--r--   0        0        0     2429 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_spinners.scss
+-rw-r--r--   0        0        0     4358 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_tables.scss
+-rw-r--r--   0        0        0     2490 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_toasts.scss
+-rw-r--r--   0        0        0     3939 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_tooltip.scss
+-rw-r--r--   0        0        0      425 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_transitions.scss
+-rw-r--r--   0        0        0     1420 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_type.scss
+-rw-r--r--   0        0        0    14817 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_utilities.scss
+-rw-r--r--   0        0        0    68610 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_variables.scss
+-rw-r--r--   0        0        0     1198 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/bootstrap-grid.scss
+-rw-r--r--   0        0        0      163 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/bootstrap-reboot.scss
+-rw-r--r--   0        0        0      280 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/bootstrap-utilities.scss
+-rw-r--r--   0        0        0      912 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/bootstrap.scss
+-rw-r--r--   0        0        0     2030 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_floating-labels.scss
+-rw-r--r--   0        0        0     4287 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_form-check.scss
+-rw-r--r--   0        0        0     5695 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_form-control.scss
+-rw-r--r--   0        0        0     2796 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_form-range.scss
+-rw-r--r--   0        0        0     2316 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_form-select.scss
+-rw-r--r--   0        0        0      219 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_form-text.scss
+-rw-r--r--   0        0        0     3835 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_input-group.scss
+-rw-r--r--   0        0        0     1142 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_labels.scss
+-rw-r--r--   0        0        0      478 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_validation.scss
+-rw-r--r--   0        0        0       37 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_clearfix.scss
+-rw-r--r--   0        0        0      454 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_color-bg.scss
+-rw-r--r--   0        0        0      450 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_colored-links.scss
+-rw-r--r--   0        0        0      621 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_position.scss
+-rw-r--r--   0        0        0      399 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_ratio.scss
+-rw-r--r--   0        0        0      245 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_stacks.scss
+-rw-r--r--   0        0        0      223 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_stretched-link.scss
+-rw-r--r--   0        0        0       73 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_text-truncation.scss
+-rw-r--r--   0        0        0      136 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_visually-hidden.scss
+-rw-r--r--   0        0        0      147 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_vr.scss
+-rw-r--r--   0        0        0      393 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_alert.scss
+-rw-r--r--   0        0        0      328 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_backdrop.scss
+-rw-r--r--   0        0        0      263 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_banner.scss
+-rw-r--r--   0        0        0     2031 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_border-radius.scss
+-rw-r--r--   0        0        0      398 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_box-shadow.scss
+-rw-r--r--   0        0        0     4580 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_breakpoints.scss
+-rw-r--r--   0        0        0     3220 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_buttons.scss
+-rw-r--r--   0        0        0     1473 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_caret.scss
+-rw-r--r--   0        0        0      147 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_clearfix.scss
+-rw-r--r--   0        0        0      167 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_color-scheme.scss
+-rw-r--r--   0        0        0      410 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_container.scss
+-rw-r--r--   0        0        0      613 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_deprecate.scss
+-rw-r--r--   0        0        0     4122 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_forms.scss
+-rw-r--r--   0        0        0     1956 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_gradients.scss
+-rw-r--r--   0        0        0     4726 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_grid.scss
+-rw-r--r--   0        0        0      395 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_image.scss
+-rw-r--r--   0        0        0      509 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_list-group.scss
+-rw-r--r--   0        0        0      168 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_lists.scss
+-rw-r--r--   0        0        0      387 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_pagination.scss
+-rw-r--r--   0        0        0      495 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_reset-text.scss
+-rw-r--r--   0        0        0      202 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_resize.scss
+-rw-r--r--   0        0        0     1101 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_table-variants.scss
+-rw-r--r--   0        0        0      168 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_text-truncate.scss
+-rw-r--r--   0        0        0      661 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_transition.scss
+-rw-r--r--   0        0        0     3380 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_utilities.scss
+-rw-r--r--   0        0        0     1012 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_visually-hidden.scss
+-rw-r--r--   0        0        0     1737 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/utilities/_api.scss
+-rw-r--r--   0        0        0    10029 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/vendor/_rfs.scss
+-rw-r--r--   0        0        0     1081 2023-05-17 07:27:49.381850 zndraw-0.2.0a1/zndraw/static/node_modules/three/LICENSE
+-rw-r--r--   0        0        0     2989 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/README.md
+-rw-r--r--   0        0        0  1219553 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/three/build/three.cjs
+-rw-r--r--   0        0        0  1250474 2023-05-17 07:27:50.461838 zndraw-0.2.0a1/zndraw/static/node_modules/three/build/three.js
+-rw-r--r--   0        0        0   633338 2023-05-17 07:27:50.461838 zndraw-0.2.0a1/zndraw/static/node_modules/three/build/three.min.js
+-rw-r--r--   0        0        0  1208839 2023-05-17 07:27:50.481838 zndraw-0.2.0a1/zndraw/static/node_modules/three/build/three.module.js
+-rw-r--r--   0        0        0   634410 2023-05-17 07:27:50.481838 zndraw-0.2.0a1/zndraw/static/node_modules/three/build/three.module.min.js
+-rw-r--r--   0        0        0     2006 2023-05-17 07:27:49.381850 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/LICENSE
+-rw-r--r--   0        0        0      334 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/README.md
+-rw-r--r--   0        0        0    10695 2023-05-17 07:27:49.391850 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/NOTICE
+-rw-r--r--   0        0        0      692 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/README.txt
+-rw-r--r--   0        0        0   329885 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_bold.typeface.json
+-rw-r--r--   0        0        0   190569 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_mono_regular.typeface.json
+-rw-r--r--   0        0        0   319895 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_regular.typeface.json
+-rw-r--r--   0        0        0   485403 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_serif_bold.typeface.json
+-rw-r--r--   0        0        0   477058 2023-05-17 07:27:50.571837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_serif_regular.typeface.json
+-rw-r--r--   0        0        0   649318 2023-05-17 07:27:50.571837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/gentilis_bold.typeface.json
+-rw-r--r--   0        0        0   627529 2023-05-17 07:27:50.581837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/gentilis_regular.typeface.json
+-rw-r--r--   0        0        0    61632 2023-05-17 07:27:50.581837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/helvetiker_bold.typeface.json
+-rw-r--r--   0        0        0    63182 2023-05-17 07:27:50.581837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/helvetiker_regular.typeface.json
+-rw-r--r--   0        0        0   112249 2023-05-17 07:27:50.581837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/optimer_bold.typeface.json
+-rw-r--r--   0        0        0   110666 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/optimer_regular.typeface.json
+-rw-r--r--   0        0        0      188 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/ttf/README.md
+-rw-r--r--   0        0        0    18068 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/ttf/kenpixel.ttf
+-rw-r--r--   0        0        0     2556 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/animation/AnimationClipCreator.js
+-rw-r--r--   0        0        0     9855 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/animation/CCDIKSolver.js
+-rw-r--r--   0        0        0    25130 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/animation/MMDAnimationHelper.js
+-rw-r--r--   0        0        0    28135 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/animation/MMDPhysics.js
+-rw-r--r--   0        0        0     6106 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/cameras/CinematicCamera.js
+-rw-r--r--   0        0        0     1702 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/capabilities/WebGL.js
+-rw-r--r--   0        0        0      859 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/capabilities/WebGPU.js
+-rw-r--r--   0        0        0    80030 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/ArcballControls.js
+-rw-r--r--   0        0        0     4592 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/DragControls.js
+-rw-r--r--   0        0        0     6764 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/FirstPersonControls.js
+-rw-r--r--   0        0        0     7072 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/FlyControls.js
+-rw-r--r--   0        0        0      863 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/MapControls.js
+-rw-r--r--   0        0        0    25214 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/OrbitControls.js
+-rw-r--r--   0        0        0     3347 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/PointerLockControls.js
+-rw-r--r--   0        0        0    17409 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/TrackballControls.js
+-rw-r--r--   0        0        0    40287 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/TransformControls.js
+-rw-r--r--   0        0        0     9291 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/csm/CSM.js
+-rw-r--r--   0        0        0     2741 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/csm/CSMFrustum.js
+-rw-r--r--   0        0        0     5832 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/csm/CSMHelper.js
+-rw-r--r--   0        0        0     8262 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/csm/CSMShader.js
+-rw-r--r--   0        0        0     7326 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/curves/CurveExtras.js
+-rw-r--r--   0        0        0     1878 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/curves/NURBSCurve.js
+-rw-r--r--   0        0        0     1296 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/curves/NURBSSurface.js
+-rw-r--r--   0        0        0     7861 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/curves/NURBSUtils.js
+-rw-r--r--   0        0        0     3932 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/AnaglyphEffect.js
+-rw-r--r--   0        0        0     6077 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/AsciiEffect.js
+-rw-r--r--   0        0        0    12953 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/OutlineEffect.js
+-rw-r--r--   0        0        0     2348 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/ParallaxBarrierEffect.js
+-rw-r--r--   0        0        0     3549 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/PeppersGhostEffect.js
+-rw-r--r--   0        0        0     1179 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/StereoEffect.js
+-rw-r--r--   0        0        0     1335 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/environments/DebugEnvironment.js
+-rw-r--r--   0        0        0     3606 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/environments/RoomEnvironment.js
+-rw-r--r--   0        0        0    19279 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/ColladaExporter.js
+-rw-r--r--   0        0        0     6594 2023-05-17 07:27:49.551848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/DRACOExporter.js
+-rw-r--r--   0        0        0    10602 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/EXRExporter.js
+-rw-r--r--   0        0        0    72734 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/GLTFExporter.js
+-rw-r--r--   0        0        0     6633 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/KTX2Exporter.js
+-rw-r--r--   0        0        0     4052 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/MMDExporter.js
+-rw-r--r--   0        0        0     5370 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/OBJExporter.js
+-rw-r--r--   0        0        0    12001 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/PLYExporter.js
+-rw-r--r--   0        0        0     3890 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/STLExporter.js
+-rw-r--r--   0        0        0    16113 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/USDZExporter.js
+-rw-r--r--   0        0        0     1968 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/BoxLineGeometry.js
+-rw-r--r--   0        0        0     1035 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/ConvexGeometry.js
+-rw-r--r--   0        0        0     8506 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/DecalGeometry.js
+-rw-r--r--   0        0        0    32742 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/LightningStrike.js
+-rw-r--r--   0        0        0     5472 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/ParametricGeometries.js
+-rw-r--r--   0        0        0     2478 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/ParametricGeometry.js
+-rw-r--r--   0        0        0     4625 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/RoundedBoxGeometry.js
+-rw-r--r--   0        0        0    19498 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/TeapotGeometry.js
+-rw-r--r--   0        0        0     1308 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/TextGeometry.js
+-rw-r--r--   0        0        0     2818 2023-05-17 07:27:50.361839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/LightProbeHelper.js
+-rw-r--r--   0        0        0     1976 2023-05-17 07:27:50.361839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/OctreeHelper.js
+-rw-r--r--   0        0        0     2712 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/PositionalAudioHelper.js
+-rw-r--r--   0        0        0     2051 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/RectAreaLightHelper.js
+-rw-r--r--   0        0        0     1811 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/VertexNormalsHelper.js
+-rw-r--r--   0        0        0     1659 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/VertexTangentsHelper.js
+-rw-r--r--   0        0        0     8059 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/ViewHelper.js
+-rw-r--r--   0        0        0    12655 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/interactive/HTMLMesh.js
+-rw-r--r--   0        0        0     2996 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/interactive/InteractiveGroup.js
+-rw-r--r--   0        0        0     6139 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/interactive/SelectionBox.js
+-rw-r--r--   0        0        0     2430 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/interactive/SelectionHelper.js
+-rw-r--r--   0        0        0   393768 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/ammo.wasm.js
+-rw-r--r--   0        0        0   651386 2023-05-17 07:27:50.601837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/ammo.wasm.wasm
+-rw-r--r--   0        0        0     1448 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/basis/README.md
+-rw-r--r--   0        0        0    62337 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/basis/basis_transcoder.js
+-rw-r--r--   0        0        0   499935 2023-05-17 07:27:50.601837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/basis/basis_transcoder.wasm
+-rw-r--r--   0        0        0   157440 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/chevrotain.module.min.js
+-rw-r--r--   0        0        0     1501 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/README.md
+-rw-r--r--   0        0        0   719410 2023-05-17 07:27:49.531848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_decoder.js
+-rw-r--r--   0        0        0   285747 2023-05-17 07:27:50.601837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_decoder.wasm
+-rw-r--r--   0        0        0   928718 2023-05-17 07:27:49.541848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_encoder.js
+-rw-r--r--   0        0        0    58763 2023-05-17 07:27:49.551848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_wasm_wrapper.js
+-rw-r--r--   0        0        0   512465 2023-05-17 07:27:49.531848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_decoder.js
+-rw-r--r--   0        0        0   192420 2023-05-17 07:27:50.611837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_decoder.wasm
+-rwxr-xr-x   0        0        0   954360 2023-05-17 07:27:49.551848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_encoder.js
+-rw-r--r--   0        0        0    58456 2023-05-17 07:27:49.551848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_wasm_wrapper.js
+-rw-r--r--   0        0        0    45516 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/ecsy.module.js
+-rw-r--r--   0        0        0    83291 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/fflate.module.js
+-rw-r--r--   0        0        0    18676 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/ktx-parse.module.js
+-rw-r--r--   0        0        0    29526 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/lil-gui.module.min.js
+-rw-r--r--   0        0        0   476927 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/lottie_canvas.module.js
+-rw-r--r--   0        0        0    24850 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/meshopt_decoder.module.js
+-rw-r--r--   0        0        0    48525 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/mikktspace.module.js
+-rw-r--r--   0        0        0   158598 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/mmdparser.module.js
+-rw-r--r--   0        0        0    13492 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/motion-controllers.module.js
+-rw-r--r--   0        0        0   469356 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/opentype.module.js
+-rw-r--r--   0        0        0     3951 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/potpack.module.js
+-rw-r--r--   0        0        0   134655 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.js
+-rw-r--r--   0        0        0   134252 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.module.js
+-rw-r--r--   0        0        0  2803968 2023-05-17 07:27:50.631837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.wasm
+-rw-r--r--   0        0        0     3514 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/stats.module.js
+-rw-r--r--   0        0        0    23045 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/tween.module.js
+-rw-r--r--   0        0        0   104667 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/utif.module.js
+-rw-r--r--   0        0        0    39754 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/zstddec.module.js
+-rw-r--r--   0        0        0      387 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lights/IESSpotLight.js
+-rw-r--r--   0        0        0     5597 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lights/LightProbeGenerator.js
+-rw-r--r--   0        0        0   313854 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lights/RectAreaLightUniformsLib.js
+-rw-r--r--   0        0        0      433 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/Line2.js
+-rw-r--r--   0        0        0     1458 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/LineGeometry.js
+-rw-r--r--   0        0        0    12422 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/LineMaterial.js
+-rw-r--r--   0        0        0     9330 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/LineSegments2.js
+-rw-r--r--   0        0        0     4632 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/LineSegmentsGeometry.js
+-rw-r--r--   0        0        0     1577 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/Wireframe.js
+-rw-r--r--   0        0        0      419 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/WireframeGeometry2.js
+-rw-r--r--   0        0        0    31227 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/3DMLoader.js
+-rw-r--r--   0        0        0    34478 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/3MFLoader.js
+-rw-r--r--   0        0        0    10621 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/AMFLoader.js
+-rw-r--r--   0        0        0     9019 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/BVHLoader.js
+-rw-r--r--   0        0        0    83853 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/ColladaLoader.js
+-rw-r--r--   0        0        0     6153 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/DDSLoader.js
+-rw-r--r--   0        0        0    13508 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/DRACOLoader.js
+-rw-r--r--   0        0        0    54975 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/EXRLoader.js
+-rw-r--r--   0        0        0    97556 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/FBXLoader.js
+-rw-r--r--   0        0        0     3204 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/FontLoader.js
+-rw-r--r--   0        0        0     5409 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/GCodeLoader.js
+-rw-r--r--   0        0        0   102783 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/GLTFLoader.js
+-rw-r--r--   0        0        0     2183 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/HDRCubeTextureLoader.js
+-rw-r--r--   0        0        0     7096 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/IESLoader.js
+-rw-r--r--   0        0        0     2211 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/KMZLoader.js
+-rw-r--r--   0        0        0    19830 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/KTX2Loader.js
+-rw-r--r--   0        0        0     6450 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/KTXLoader.js
+-rw-r--r--   0        0        0    57006 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LDrawLoader.js
+-rw-r--r--   0        0        0     3907 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LUT3dlLoader.js
+-rw-r--r--   0        0        0     3441 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LUTCubeLoader.js
+-rw-r--r--   0        0        0    23543 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LWOLoader.js
+-rw-r--r--   0        0        0    19405 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LogLuvLoader.js
+-rw-r--r--   0        0        0     1486 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LottieLoader.js
+-rw-r--r--   0        0        0    12372 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MD2Loader.js
+-rw-r--r--   0        0        0     2304 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MDDLoader.js
+-rw-r--r--   0        0        0    51619 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MMDLoader.js
+-rw-r--r--   0        0        0    10580 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MTLLoader.js
+-rw-r--r--   0        0        0    14996 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MaterialXLoader.js
+-rw-r--r--   0        0        0    13679 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/NRRDLoader.js
+-rw-r--r--   0        0        0    21175 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/OBJLoader.js
+-rw-r--r--   0        0        0    12080 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PCDLoader.js
+-rw-r--r--   0        0        0     6781 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PDBLoader.js
+-rw-r--r--   0        0        0    15666 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PLYLoader.js
+-rw-r--r--   0        0        0     5741 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PRWMLoader.js
+-rw-r--r--   0        0        0     4718 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PVRLoader.js
+-rw-r--r--   0        0        0    11793 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/RGBELoader.js
+-rw-r--r--   0        0        0    28278 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/RGBMLoader.js
+-rw-r--r--   0        0        0     9694 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/STLLoader.js
+-rw-r--r--   0        0        0    69560 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/SVGLoader.js
+-rw-r--r--   0        0        0    24660 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TDSLoader.js
+-rw-r--r--   0        0        0    11138 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TGALoader.js
+-rw-r--r--   0        0        0      572 2023-05-17 07:27:50.481838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TIFFLoader.js
+-rw-r--r--   0        0        0     4212 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TTFLoader.js
+-rw-r--r--   0        0        0    14505 2023-05-17 07:27:50.481838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TiltLoader.js
+-rw-r--r--   0        0        0    11483 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/USDZLoader.js
+-rw-r--r--   0        0        0     8785 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/VOXLoader.js
+-rw-r--r--   0        0        0    72146 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/VRMLLoader.js
+-rw-r--r--   0        0        0    27300 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/VTKLoader.js
+-rw-r--r--   0        0        0     1795 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/XYZLoader.js
+-rw-r--r--   0        0        0    26644 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/IFFParser.js
+-rw-r--r--   0        0        0    10137 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/LWO2Parser.js
+-rw-r--r--   0        0        0     9269 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/LWO3Parser.js
+-rw-r--r--   0        0        0     9751 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/materials/MeshGouraudMaterial.js
+-rw-r--r--   0        0        0     2522 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/Capsule.js
+-rw-r--r--   0        0        0      723 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/ColorConverter.js
+-rw-r--r--   0        0        0    21832 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/ConvexHull.js
+-rw-r--r--   0        0        0     2564 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/ImprovedNoise.js
+-rw-r--r--   0        0        0     3642 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/Lut.js
+-rw-r--r--   0        0        0     4260 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/MeshSurfaceSampler.js
+-rw-r--r--   0        0        0    10227 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/OBB.js
+-rw-r--r--   0        0        0     9208 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/Octree.js
+-rw-r--r--   0        0        0    14351 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/SimplexNoise.js
+-rw-r--r--   0        0        0    13577 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/ConvexObjectBreaker.js
+-rw-r--r--   0        0        0    12137 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/GPUComputationRenderer.js
+-rw-r--r--   0        0        0     1188 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/Gyroscope.js
+-rw-r--r--   0        0        0     5216 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/MD2Character.js
+-rw-r--r--   0        0        0    11980 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/MD2CharacterComplex.js
+-rw-r--r--   0        0        0     1107 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/MorphAnimMesh.js
+-rw-r--r--   0        0        0     5459 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/MorphBlendMesh.js
+-rw-r--r--   0        0        0    11076 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/ProgressiveLightMap.js
+-rw-r--r--   0        0        0    13795 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/RollerCoaster.js
+-rw-r--r--   0        0        0     4673 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/TubePainter.js
+-rw-r--r--   0        0        0    13500 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/Volume.js
+-rw-r--r--   0        0        0     6177 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/VolumeSlice.js
+-rw-r--r--   0        0        0     9107 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/modifiers/CurveModifier.js
+-rw-r--r--   0        0        0     5296 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/modifiers/EdgeSplitModifier.js
+-rw-r--r--   0        0        0    10082 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/modifiers/SimplifyModifier.js
+-rw-r--r--   0        0        0     6159 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/modifiers/TessellateModifier.js
+-rw-r--r--   0        0        0    11752 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/Nodes.js
+-rw-r--r--   0        0        0     2365 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/BitangentNode.js
+-rw-r--r--   0        0        0      648 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/BufferNode.js
+-rw-r--r--   0        0        0     1583 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/CameraNode.js
+-rw-r--r--   0        0        0     2173 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/CubeTextureNode.js
+-rw-r--r--   0        0        0     1252 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ExtendedMaterialNode.js
+-rw-r--r--   0        0        0     1434 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/InstanceNode.js
+-rw-r--r--   0        0        0     6340 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/MaterialNode.js
+-rw-r--r--   0        0        0      916 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/MaterialReferenceNode.js
+-rw-r--r--   0        0        0      903 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ModelNode.js
+-rw-r--r--   0        0        0      785 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ModelViewProjectionNode.js
+-rw-r--r--   0        0        0     2276 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/NormalNode.js
+-rw-r--r--   0        0        0     3428 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/Object3DNode.js
+-rw-r--r--   0        0        0      429 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/PointUVNode.js
+-rw-r--r--   0        0        0     2586 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/PositionNode.js
+-rw-r--r--   0        0        0     1273 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ReferenceNode.js
+-rw-r--r--   0        0        0      733 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ReflectVectorNode.js
+-rw-r--r--   0        0        0     3114 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/SkinningNode.js
+-rw-r--r--   0        0        0      628 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/StorageBufferNode.js
+-rw-r--r--   0        0        0     2280 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/TangentNode.js
+-rw-r--r--   0        0        0     3209 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/TextureNode.js
+-rw-r--r--   0        0        0      718 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/UVNode.js
+-rw-r--r--   0        0        0      644 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/UserDataNode.js
+-rw-r--r--   0        0        0     1155 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/CodeNode.js
+-rw-r--r--   0        0        0      637 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/ExpressionNode.js
+-rw-r--r--   0        0        0     1812 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/FunctionCallNode.js
+-rw-r--r--   0        0        0     2006 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/FunctionNode.js
+-rw-r--r--   0        0        0     7789 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/ScriptableNode.js
+-rw-r--r--   0        0        0     3227 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/ScriptableValueNode.js
+-rw-r--r--   0        0        0      389 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/ArrayUniformNode.js
+-rw-r--r--   0        0        0     1973 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/AttributeNode.js
+-rw-r--r--   0        0        0      745 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/BypassNode.js
+-rw-r--r--   0        0        0      768 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/CacheNode.js
+-rw-r--r--   0        0        0      538 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/ConstNode.js
+-rw-r--r--   0        0        0     1025 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/ContextNode.js
+-rw-r--r--   0        0        0     1447 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/InputNode.js
+-rw-r--r--   0        0        0      433 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/InstanceIndexNode.js
+-rw-r--r--   0        0        0      401 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/LightingModel.js
+-rw-r--r--   0        0        0     7371 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/Node.js
+-rw-r--r--   0        0        0      163 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeAttribute.js
+-rw-r--r--   0        0        0    17154 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeBuilder.js
+-rw-r--r--   0        0        0      274 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeCache.js
+-rw-r--r--   0        0        0      217 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeCode.js
+-rw-r--r--   0        0        0     2049 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeFrame.js
+-rw-r--r--   0        0        0      330 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeFunction.js
+-rw-r--r--   0        0        0      311 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeFunctionInput.js
+-rw-r--r--   0        0        0     1161 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeKeywords.js
+-rw-r--r--   0        0        0      127 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeParser.js
+-rw-r--r--   0        0        0      340 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeUniform.js
+-rw-r--r--   0        0        0     3668 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeUtils.js
+-rw-r--r--   0        0        0      145 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeVar.js
+-rw-r--r--   0        0        0      229 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeVarying.js
+-rw-r--r--   0        0        0     1214 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/PropertyNode.js
+-rw-r--r--   0        0        0     1595 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/StackNode.js
+-rw-r--r--   0        0        0     1273 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/TempNode.js
+-rw-r--r--   0        0        0     1324 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/UniformNode.js
+-rw-r--r--   0        0        0     1383 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/VarNode.js
+-rw-r--r--   0        0        0     1354 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/VaryingNode.js
+-rw-r--r--   0        0        0      612 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/constants.js
+-rw-r--r--   0        0        0     2586 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/BlendModeNode.js
+-rw-r--r--   0        0        0     2750 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ColorAdjustmentNode.js
+-rw-r--r--   0        0        0     2027 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ColorSpaceNode.js
+-rw-r--r--   0        0        0      505 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/FrontFacingNode.js
+-rw-r--r--   0        0        0     2606 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/NormalMapNode.js
+-rw-r--r--   0        0        0      615 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/PosterizeNode.js
+-rw-r--r--   0        0        0     3616 2023-05-17 07:27:50.481838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ToneMappingNode.js
+-rw-r--r--   0        0        0     2581 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportNode.js
+-rw-r--r--   0        0        0      695 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportSharedTextureNode.js
+-rw-r--r--   0        0        0     1248 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportTextureNode.js
+-rw-r--r--   0        0        0      745 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogExp2Node.js
+-rw-r--r--   0        0        0      568 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogNode.js
+-rw-r--r--   0        0        0      722 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogRangeNode.js
+-rw-r--r--   0        0        0     1005 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_BlinnPhong.js
+-rw-r--r--   0        0        0     1145 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_GGX.js
+-rw-r--r--   0        0        0      231 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_Lambert.js
+-rw-r--r--   0        0        0      973 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/DFGApprox.js
+-rw-r--r--   0        0        0      573 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/D_GGX.js
+-rw-r--r--   0        0        0      588 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/F_Schlick.js
+-rw-r--r--   0        0        0      726 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/V_GGX_SmithCorrelated.js
+-rw-r--r--   0        0        0     1231 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/PhongLightingModel.js
+-rw-r--r--   0        0        0     3444 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/PhysicalLightingModel.js
+-rw-r--r--   0        0        0      389 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/material/getGeometryRoughness.js
+-rw-r--r--   0        0        0      541 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/material/getRoughness.js
+-rw-r--r--   0        0        0     3103 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/geometry/RangeNode.js
+-rw-r--r--   0        0        0     1325 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/gpgpu/ComputeNode.js
+-rw-r--r--   0        0        0      440 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/AONode.js
+-rw-r--r--   0        0        0      503 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/AmbientLightNode.js
+-rw-r--r--   0        0        0     3286 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/AnalyticLightNode.js
+-rw-r--r--   0        0        0      981 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/DirectionalLightNode.js
+-rw-r--r--   0        0        0     3068 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/EnvironmentNode.js
+-rw-r--r--   0        0        0     1358 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/HemisphereLightNode.js
+-rw-r--r--   0        0        0      866 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/IESSpotLightNode.js
+-rw-r--r--   0        0        0     1025 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightNode.js
+-rw-r--r--   0        0        0      663 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightUtils.js
+-rw-r--r--   0        0        0     2660 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightingContextNode.js
+-rw-r--r--   0        0        0      268 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightingNode.js
+-rw-r--r--   0        0        0     2337 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightsNode.js
+-rw-r--r--   0        0        0     1737 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/PointLightNode.js
+-rw-r--r--   0        0        0     2394 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/SpotLightNode.js
+-rw-r--r--   0        0        0     1732 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeLoader.js
+-rw-r--r--   0        0        0      918 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeMaterialLoader.js
+-rw-r--r--   0        0        0     1097 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeObjectLoader.js
+-rw-r--r--   0        0        0      768 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/LineBasicNodeMaterial.js
+-rw-r--r--   0        0        0      891 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/Materials.js
+-rw-r--r--   0        0        0      744 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshBasicNodeMaterial.js
+-rw-r--r--   0        0        0     1139 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshNormalNodeMaterial.js
+-rw-r--r--   0        0        0     1623 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshPhongNodeMaterial.js
+-rw-r--r--   0        0        0     1843 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshPhysicalNodeMaterial.js
+-rw-r--r--   0        0        0     2245 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshStandardNodeMaterial.js
+-rw-r--r--   0        0        0     9200 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/NodeMaterial.js
+-rw-r--r--   0        0        0      977 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/PointsNodeMaterial.js
+-rw-r--r--   0        0        0     2634 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/SpriteNodeMaterial.js
+-rw-r--r--   0        0        0    10562 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/DISCLAIMER.md
+-rw-r--r--   0        0        0     4232 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/MaterialXNodes.js
+-rw-r--r--   0        0        0     1688 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/lib/mx_hsv.js
+-rw-r--r--   0        0        0    19096 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/lib/mx_noise.js
+-rw-r--r--   0        0        0      925 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/lib/mx_transform_color.js
+-rw-r--r--   0        0        0     2113 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/math/CondNode.js
+-rw-r--r--   0        0        0    10373 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/math/MathNode.js
+-rw-r--r--   0        0        0     6210 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/math/OperatorNode.js
+-rw-r--r--   0        0        0     2894 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/GLSLNodeFunction.js
+-rw-r--r--   0        0        0      254 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/GLSLNodeParser.js
+-rw-r--r--   0        0        0     1932 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/WGSLNodeFunction.js
+-rw-r--r--   0        0        0      254 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/WGSLNodeParser.js
+-rw-r--r--   0        0        0      814 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/procedural/CheckerNode.js
+-rw-r--r--   0        0        0    10299 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/shadernode/ShaderNode.js
+-rw-r--r--   0        0        0      594 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/ArrayElementNode.js
+-rw-r--r--   0        0        0     1004 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/ConvertNode.js
+-rw-r--r--   0        0        0      576 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/DiscardNode.js
+-rw-r--r--   0        0        0      772 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/EquirectUVNode.js
+-rw-r--r--   0        0        0      946 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/JoinNode.js
+-rw-r--r--   0        0        0      771 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/MatcapUVNode.js
+-rw-r--r--   0        0        0      919 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/MaxMipLevelNode.js
+-rw-r--r--   0        0        0     1569 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/OscNode.js
+-rw-r--r--   0        0        0     1122 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/PackingNode.js
+-rw-r--r--   0        0        0      967 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/RemapNode.js
+-rw-r--r--   0        0        0     1014 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/RotateUVNode.js
+-rw-r--r--   0        0        0      962 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SpecularMIPLevelNode.js
+-rw-r--r--   0        0        0     1842 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SplitNode.js
+-rw-r--r--   0        0        0      944 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SpriteSheetUVNode.js
+-rw-r--r--   0        0        0     1858 2023-05-17 07:27:50.481838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/TimerNode.js
+-rw-r--r--   0        0        0     1967 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/TriplanarTexturesNode.js
+-rw-r--r--   0        0        0     3420 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/GroundProjectedSkybox.js
+-rw-r--r--   0        0        0     8427 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Lensflare.js
+-rw-r--r--   0        0        0     7502 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/LightningStorm.js
+-rw-r--r--   0        0        0    37944 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/MarchingCubes.js
+-rw-r--r--   0        0        0     7294 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Reflector.js
+-rw-r--r--   0        0        0    10319 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/ReflectorForSSRPass.js
+-rw-r--r--   0        0        0     8419 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Refractor.js
+-rw-r--r--   0        0        0     2030 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/ShadowMesh.js
+-rw-r--r--   0        0        0     6841 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Sky.js
+-rw-r--r--   0        0        0    11125 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Water.js
+-rw-r--r--   0        0        0     8395 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Water2.js
+-rw-r--r--   0        0        0      645 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/offscreen/jank.js
+-rw-r--r--   0        0        0      188 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/offscreen/offscreen.js
+-rw-r--r--   0        0        0     2078 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/offscreen/scene.js
+-rw-r--r--   0        0        0     6769 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/physics/AmmoPhysics.js
+-rw-r--r--   0        0        0     4912 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/physics/RapierPhysics.js
+-rw-r--r--   0        0        0     8906 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/AdaptiveToneMappingPass.js
+-rw-r--r--   0        0        0     2186 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/AfterimagePass.js
+-rw-r--r--   0        0        0     3836 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/BloomPass.js
+-rw-r--r--   0        0        0     3388 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/BokehPass.js
+-rw-r--r--   0        0        0      875 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/ClearPass.js
+-rw-r--r--   0        0        0     1940 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/CubeTexturePass.js
+-rw-r--r--   0        0        0     1346 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/DotScreenPass.js
+-rw-r--r--   0        0        0     4549 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/EffectComposer.js
+-rw-r--r--   0        0        0     1456 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/FilmPass.js
+-rw-r--r--   0        0        0     3076 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/GlitchPass.js
+-rw-r--r--   0        0        0     1522 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/HalftonePass.js
+-rw-r--r--   0        0        0     3209 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/LUTPass.js
+-rw-r--r--   0        0        0     2120 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/MaskPass.js
+-rw-r--r--   0        0        0    20231 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/OutlinePass.js
+-rw-r--r--   0        0        0     1603 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/Pass.js
+-rw-r--r--   0        0        0     1734 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/RenderPass.js
+-rw-r--r--   0        0        0     6102 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/RenderPixelatedPass.js
+-rw-r--r--   0        0        0    14008 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SAOPass.js
+-rw-r--r--   0        0        0    49430 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SMAAPass.js
+-rw-r--r--   0        0        0     6246 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSAARenderPass.js
+-rw-r--r--   0        0        0    12016 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSAOPass.js
+-rw-r--r--   0        0        0    18496 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSRPass.js
+-rw-r--r--   0        0        0     1355 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SavePass.js
+-rw-r--r--   0        0        0     1505 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/ShaderPass.js
+-rw-r--r--   0        0        0     4605 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/TAARenderPass.js
+-rw-r--r--   0        0        0     1316 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/TexturePass.js
+-rw-r--r--   0        0        0    12256 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/UnrealBloomPass.js
+-rw-r--r--   0        0        0     4407 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/CSS2DRenderer.js
+-rw-r--r--   0        0        0     7865 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/CSS3DRenderer.js
+-rw-r--r--   0        0        0    19380 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/Projector.js
+-rw-r--r--   0        0        0    12465 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/SVGRenderer.js
+-rw-r--r--   0        0        0      383 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/SlotNode.js
+-rw-r--r--   0        0        0    16860 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/WebGLNodeBuilder.js
+-rw-r--r--   0        0        0     1017 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/WebGLNodes.js
+-rw-r--r--   0        0        0      802 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUAnimation.js
+-rw-r--r--   0        0        0     3444 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUAttributes.js
+-rw-r--r--   0        0        0     4642 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBackground.js
+-rw-r--r--   0        0        0      265 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBinding.js
+-rw-r--r--   0        0        0     5849 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBindings.js
+-rw-r--r--   0        0        0      661 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBuffer.js
+-rw-r--r--   0        0        0      665 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBufferUtils.js
+-rw-r--r--   0        0        0     1358 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUComputePipelines.js
+-rw-r--r--   0        0        0     4103 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUGeometries.js
+-rw-r--r--   0        0        0     1054 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUInfo.js
+-rw-r--r--   0        0        0      324 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUProgrammableStage.js
+-rw-r--r--   0        0        0      468 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUProperties.js
+-rw-r--r--   0        0        0     3800 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderLists.js
+-rw-r--r--   0        0        0      849 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderObject.js
+-rw-r--r--   0        0        0     1005 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderObjects.js
+-rw-r--r--   0        0        0    16177 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderPipeline.js
+-rw-r--r--   0        0        0     7560 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderPipelines.js
+-rw-r--r--   0        0        0      746 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderStates.js
+-rw-r--r--   0        0        0      289 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderTarget.js
+-rw-r--r--   0        0        0    26892 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderer.js
+-rw-r--r--   0        0        0     1406 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUSampledTexture.js
+-rw-r--r--   0        0        0      463 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUSampler.js
+-rw-r--r--   0        0        0      417 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUStorageBuffer.js
+-rw-r--r--   0        0        0      634 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextureRenderer.js
+-rw-r--r--   0        0        0     4747 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextureUtils.js
+-rw-r--r--   0        0        0    29302 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextures.js
+-rw-r--r--   0        0        0     2017 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniform.js
+-rw-r--r--   0        0        0      357 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniformBuffer.js
+-rw-r--r--   0        0        0     5397 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniformsGroup.js
+-rw-r--r--   0        0        0     1670 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUtils.js
+-rw-r--r--   0        0        0     1076 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUWeakMap.js
+-rw-r--r--   0        0        0     7838 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/constants.js
+-rw-r--r--   0        0        0    17770 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeBuilder.js
+-rw-r--r--   0        0        0      637 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeSampledTexture.js
+-rw-r--r--   0        0        0      304 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeSampler.js
+-rw-r--r--   0        0        0     1872 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeUniform.js
+-rw-r--r--   0        0        0     6826 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodes.js
+-rw-r--r--   0        0        0     1871 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ACESFilmicToneMappingShader.js
+-rw-r--r--   0        0        0      875 2023-05-17 07:27:49.401850 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/AfterimageShader.js
+-rw-r--r--   0        0        0      328 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BasicShader.js
+-rw-r--r--   0        0        0     1182 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BleachBypassShader.js
+-rw-r--r--   0        0        0      751 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BlendShader.js
+-rw-r--r--   0        0        0     5746 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BokehShader.js
+-rw-r--r--   0        0        0     9557 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BokehShader2.js
+-rw-r--r--   0        0        0     1030 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BrightnessContrastShader.js
+-rw-r--r--   0        0        0      789 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ColorCorrectionShader.js
+-rw-r--r--   0        0        0      678 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ColorifyShader.js
+-rw-r--r--   0        0        0     1780 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ConvolutionShader.js
+-rw-r--r--   0        0        0      546 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/CopyShader.js
+-rw-r--r--   0        0        0      891 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/DOFMipMapShader.js
+-rw-r--r--   0        0        0     3670 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/DepthLimitedBlurShader.js
+-rw-r--r--   0        0        0     2574 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/DigitalGlitch.js
+-rw-r--r--   0        0        0     1177 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/DotScreenShader.js
+-rw-r--r--   0        0        0     8473 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/FXAAShader.js
+-rw-r--r--   0        0        0     2338 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/FilmShader.js
+-rw-r--r--   0        0        0     2282 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/FocusShader.js
+-rw-r--r--   0        0        0     2944 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/FreiChenShader.js
+-rw-r--r--   0        0        0      558 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/GammaCorrectionShader.js
+-rw-r--r--   0        0        0     6695 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/GodRaysShader.js
+-rw-r--r--   0        0        0     8558 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/HalftoneShader.js
+-rw-r--r--   0        0        0     1420 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/HorizontalBlurShader.js
+-rw-r--r--   0        0        0     1548 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/HorizontalTiltShiftShader.js
+-rw-r--r--   0        0        0     1449 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/HueSaturationShader.js
+-rw-r--r--   0        0        0      989 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/KaleidoShader.js
+-rw-r--r--   0        0        0     1156 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/LuminosityHighPassShader.js
+-rw-r--r--   0        0        0      596 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/LuminosityShader.js
+-rw-r--r--   0        0        0     3252 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/MMDToonShader.js
+-rw-r--r--   0        0        0      890 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/MirrorShader.js
+-rw-r--r--   0        0        0      968 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/NormalMapShader.js
+-rw-r--r--   0        0        0     1089 2023-05-17 07:27:50.401839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/RGBShiftShader.js
+-rw-r--r--   0        0        0     5160 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SAOShader.js
+-rw-r--r--   0        0        0    14545 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SMAAShader.js
+-rw-r--r--   0        0        0     6315 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SSAOShader.js
+-rw-r--r--   0        0        0     9333 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SSRShader.js
+-rw-r--r--   0        0        0      913 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SepiaShader.js
+-rw-r--r--   0        0        0     2321 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SobelOperatorShader.js
+-rw-r--r--   0        0        0     2908 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SubsurfaceScatteringShader.js
+-rw-r--r--   0        0        0      835 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/TechnicolorShader.js
+-rw-r--r--   0        0        0     1601 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ToneMapShader.js
+-rw-r--r--   0        0        0     6634 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ToonShader.js
+-rw-r--r--   0        0        0     1248 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/TriangleBlurShader.js
+-rw-r--r--   0        0        0      676 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/UnpackDepthRGBAShader.js
+-rw-r--r--   0        0        0     2970 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VelocityShader.js
+-rw-r--r--   0        0        0     1416 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VerticalBlurShader.js
+-rw-r--r--   0        0        0     1544 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VerticalTiltShiftShader.js
+-rw-r--r--   0        0        0      867 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VignetteShader.js
+-rw-r--r--   0        0        0     9745 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VolumeShader.js
+-rw-r--r--   0        0        0     1706 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/WaterRefractionShader.js
+-rw-r--r--   0        0        0      876 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/textures/FlakesTexture.js
+-rw-r--r--   0        0        0    31105 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/BufferGeometryUtils.js
+-rw-r--r--   0        0        0     2850 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/CameraUtils.js
+-rw-r--r--   0        0        0     2470 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/GPUStatsPanel.js
+-rw-r--r--   0        0        0    14687 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/GeometryCompressionUtils.js
+-rw-r--r--   0        0        0     5113 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/GeometryUtils.js
+-rw-r--r--   0        0        0     5808 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/LDrawUtils.js
+-rw-r--r--   0        0        0     3950 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/PackedPhongMaterial.js
+-rw-r--r--   0        0        0     5511 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/SceneUtils.js
+-rw-r--r--   0        0        0     5595 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/ShadowMapViewer.js
+-rw-r--r--   0        0        0     8007 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/SkeletonUtils.js
+-rw-r--r--   0        0        0     3097 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/UVsDebug.js
+-rw-r--r--   0        0        0     1712 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/WorkerPool.js
+-rw-r--r--   0        0        0     4352 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/ARButton.js
+-rw-r--r--   0        0        0     1756 2023-05-17 07:27:50.361839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/OculusHandModel.js
+-rw-r--r--   0        0        0     9461 2023-05-17 07:27:50.361839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/OculusHandPointerModel.js
+-rw-r--r--   0        0        0     1018 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/Text2D.js
+-rw-r--r--   0        0        0     4222 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/VRButton.js
+-rw-r--r--   0        0        0     3585 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRButton.js
+-rw-r--r--   0        0        0     6990 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRControllerModelFactory.js
+-rw-r--r--   0        0        0     5308 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XREstimatedLight.js
+-rw-r--r--   0        0        0     2398 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandMeshModel.js
+-rw-r--r--   0        0        0     1841 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandModelFactory.js
+-rw-r--r--   0        0        0     2277 2023-05-17 07:27:50.561837 zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandPrimitiveModel.js
+-rw-r--r--   0        0        0     3780 2023-05-17 07:27:50.591837 zndraw-0.2.0a1/zndraw/static/node_modules/three/package.json
+-rw-r--r--   0        0        0     7074 2023-05-17 07:27:50.461838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/Three.Legacy.js
+-rw-r--r--   0        0        0     9631 2023-05-17 07:27:50.461838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/Three.js
+-rw-r--r--   0        0        0    12606 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationAction.js
+-rw-r--r--   0        0        0     9535 2023-05-17 07:27:49.421849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationClip.js
+-rw-r--r--   0        0        0    16463 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationMixer.js
+-rw-r--r--   0        0        0     9230 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationObjectGroup.js
+-rw-r--r--   0        0        0     8231 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationUtils.js
+-rw-r--r--   0        0        0     9273 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/KeyframeTrack.js
+-rw-r--r--   0        0        0    16404 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/PropertyBinding.js
+-rw-r--r--   0        0        0     6825 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/PropertyMixer.js
+-rw-r--r--   0        0        0      757 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/tracks/BooleanKeyframeTrack.js
+-rw-r--r--   0        0        0      445 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/tracks/ColorKeyframeTrack.js
+-rw-r--r--   0        0        0      311 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/tracks/NumberKeyframeTrack.js
+-rw-r--r--   0        0        0      755 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/tracks/QuaternionKeyframeTrack.js
+-rw-r--r--   0        0        0      575 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/tracks/StringKeyframeTrack.js
+-rw-r--r--   0        0        0      312 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/tracks/VectorKeyframeTrack.js
+-rw-r--r--   0        0        0     6016 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/audio/Audio.js
+-rw-r--r--   0        0        0      591 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/audio/AudioAnalyser.js
+-rw-r--r--   0        0        0      284 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/audio/AudioContext.js
+-rw-r--r--   0        0        0     2893 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/audio/AudioListener.js
+-rw-r--r--   0        0        0     2578 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/audio/PositionalAudio.js
+-rw-r--r--   0        0        0      236 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/ArrayCamera.js
+-rw-r--r--   0        0        0     1209 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/Camera.js
+-rw-r--r--   0        0        0     2871 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/CubeCamera.js
+-rwxr-xr-x   0        0        0     2730 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/OrthographicCamera.js
+-rw-r--r--   0        0        0     5273 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/PerspectiveCamera.js
+-rw-r--r--   0        0        0     2694 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/StereoCamera.js
+-rw-r--r--   0        0        0     7137 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/constants.js
+-rw-r--r--   0        0        0    10577 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/BufferAttribute.js
+-rw-r--r--   0        0        0    20961 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/BufferGeometry.js
+-rw-r--r--   0        0        0      890 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/Clock.js
+-rw-r--r--   0        0        0     1479 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/EventDispatcher.js
+-rw-r--r--   0        0        0      725 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/GLBufferAttribute.js
+-rw-r--r--   0        0        0      631 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InstancedBufferAttribute.js
+-rw-r--r--   0        0        0      562 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InstancedBufferGeometry.js
+-rw-r--r--   0        0        0      747 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InstancedInterleavedBuffer.js
+-rw-r--r--   0        0        0     2388 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InterleavedBuffer.js
+-rw-r--r--   0        0        0     5853 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InterleavedBufferAttribute.js
+-rw-r--r--   0        0        0      577 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/Layers.js
+-rw-r--r--   0        0        0    17943 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/Object3D.js
+-rw-r--r--   0        0        0     2234 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/Raycaster.js
+-rw-r--r--   0        0        0      199 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/Uniform.js
+-rw-r--r--   0        0        0     1179 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/UniformsGroup.js
+-rw-r--r--   0        0        0     3482 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/DataUtils.js
+-rw-r--r--   0        0        0    17687 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/Earcut.js
+-rw-r--r--   0        0        0     2496 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/ImageUtils.js
+-rw-r--r--   0        0        0    21807 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/PMREMGenerator.js
+-rw-r--r--   0        0        0     1516 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/ShapeUtils.js
+-rw-r--r--   0        0        0     8025 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/Curve.js
+-rw-r--r--   0        0        0     4640 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/CurvePath.js
+-rw-r--r--   0        0        0     1223 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/Interpolations.js
+-rw-r--r--   0        0        0     3562 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/Path.js
+-rw-r--r--   0        0        0     1419 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/Shape.js
+-rw-r--r--   0        0        0     5801 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/ShapePath.js
+-rw-r--r--   0        0        0      317 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/ArcCurve.js
+-rw-r--r--   0        0        0     5479 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/CatmullRomCurve3.js
+-rw-r--r--   0        0        0     1315 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/CubicBezierCurve.js
+-rw-r--r--   0        0        0     1364 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/CubicBezierCurve3.js
+-rw-r--r--   0        0        0      540 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/Curves.js
+-rw-r--r--   0        0        0     2753 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/EllipseCurve.js
+-rw-r--r--   0        0        0     1318 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/LineCurve.js
+-rw-r--r--   0        0        0     1318 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/LineCurve3.js
+-rw-r--r--   0        0        0     1189 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/QuadraticBezierCurve.js
+-rw-r--r--   0        0        0     1236 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/QuadraticBezierCurve3.js
+-rw-r--r--   0        0        0     1678 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/SplineCurve.js
+-rw-r--r--   0        0        0     4339 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/BoxGeometry.js
+-rw-r--r--   0        0        0      760 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/CapsuleGeometry.js
+-rw-r--r--   0        0        0     1960 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/CircleGeometry.js
+-rw-r--r--   0        0        0      810 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/ConeGeometry.js
+-rw-r--r--   0        0        0     5865 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/CylinderGeometry.js
+-rw-r--r--   0        0        0     1351 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/DodecahedronGeometry.js
+-rw-r--r--   0        0        0     4116 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/EdgesGeometry.js
+-rw-r--r--   0        0        0    18337 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/ExtrudeGeometry.js
+-rw-r--r--   0        0        0      797 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/Geometries.js
+-rw-r--r--   0        0        0      896 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/IcosahedronGeometry.js
+-rw-r--r--   0        0        0     3934 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/LatheGeometry.js
+-rw-r--r--   0        0        0      641 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/OctahedronGeometry.js
+-rw-r--r--   0        0        0     1999 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/PlaneGeometry.js
+-rw-r--r--   0        0        0     6436 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/PolyhedronGeometry.js
+-rw-r--r--   0        0        0     2760 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/RingGeometry.js
+-rw-r--r--   0        0        0     3687 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/ShapeGeometry.js
+-rw-r--r--   0        0        0     3129 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/SphereGeometry.js
+-rw-r--r--   0        0        0      590 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/TetrahedronGeometry.js
+-rw-r--r--   0        0        0     2607 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/TorusGeometry.js
+-rw-r--r--   0        0        0     4255 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/TorusKnotGeometry.js
+-rw-r--r--   0        0        0     4364 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/TubeGeometry.js
+-rw-r--r--   0        0        0     3004 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/WireframeGeometry.js
+-rw-r--r--   0        0        0     2740 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/ArrowHelper.js
+-rw-r--r--   0        0        0     1486 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/AxesHelper.js
+-rw-r--r--   0        0        0     1287 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/Box3Helper.js
+-rw-r--r--   0        0        0     2481 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/BoxHelper.js
+-rw-r--r--   0        0        0     8392 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/CameraHelper.js
+-rw-r--r--   0        0        0     2243 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/DirectionalLightHelper.js
+-rw-r--r--   0        0        0     1477 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/GridHelper.js
+-rw-r--r--   0        0        0     2047 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/HemisphereLightHelper.js
+-rw-r--r--   0        0        0     1737 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/PlaneHelper.js
+-rw-r--r--   0        0        0     1724 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/PointLightHelper.js
+-rw-r--r--   0        0        0     2096 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/PolarGridHelper.js
+-rw-r--r--   0        0        0     2854 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/SkeletonHelper.js
+-rw-r--r--   0        0        0     2012 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/SpotLightHelper.js
+-rw-r--r--   0        0        0      233 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/AmbientLight.js
+-rw-r--r--   0        0        0      517 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/AmbientLightProbe.js
+-rw-r--r--   0        0        0      703 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/DirectionalLight.js
+-rw-r--r--   0        0        0      337 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/DirectionalLightShadow.js
+-rw-r--r--   0        0        0      605 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/HemisphereLight.js
+-rw-r--r--   0        0        0      879 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/HemisphereLightProbe.js
+-rw-r--r--   0        0        0     1168 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/Light.js
+-rw-r--r--   0        0        0      679 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/LightProbe.js
+-rw-r--r--   0        0        0     2638 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/LightShadow.js
+-rw-r--r--   0        0        0     1026 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/PointLight.js
+-rw-r--r--   0        0        0     2566 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/PointLightShadow.js
+-rw-r--r--   0        0        0      926 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/RectAreaLight.js
+-rw-r--r--   0        0        0     1366 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/SpotLight.js
+-rw-r--r--   0        0        0      925 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/SpotLightShadow.js
+-rw-r--r--   0        0        0     1009 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/AnimationLoader.js
+-rw-r--r--   0        0        0     1178 2023-05-17 07:27:49.441849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/AudioLoader.js
+-rw-r--r--   0        0        0     5596 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/BufferGeometryLoader.js
+-rw-r--r--   0        0        0      503 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/Cache.js
+-rw-r--r--   0        0        0     2666 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/CompressedTextureLoader.js
+-rw-r--r--   0        0        0      870 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/CubeTextureLoader.js
+-rw-r--r--   0        0        0     2626 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/DataTextureLoader.js
+-rw-r--r--   0        0        0     5554 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/FileLoader.js
+-rw-r--r--   0        0        0     1777 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/ImageBitmapLoader.js
+-rw-r--r--   0        0        0     1505 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/ImageLoader.js
+-rw-r--r--   0        0        0     1019 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/Loader.js
+-rw-r--r--   0        0        0     1308 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/LoaderUtils.js
+-rw-r--r--   0        0        0     2033 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/LoadingManager.js
+-rw-r--r--   0        0        0    13513 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/MaterialLoader.js
+-rw-r--r--   0        0        0    24955 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/ObjectLoader.js
+-rw-r--r--   0        0        0      679 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/TextureLoader.js
+-rw-r--r--   0        0        0      727 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/LineBasicMaterial.js
+-rw-r--r--   0        0        0      524 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/LineDashedMaterial.js
+-rw-r--r--   0        0        0    14310 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/Material.js
+-rw-r--r--   0        0        0     1428 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/Materials.js
+-rw-r--r--   0        0        0     1612 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshBasicMaterial.js
+-rw-r--r--   0        0        0      977 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshDepthMaterial.js
+-rw-r--r--   0        0        0      699 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshDistanceMaterial.js
+-rw-r--r--   0        0        0     2602 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshLambertMaterial.js
+-rw-r--r--   0        0        0     1528 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshMatcapMaterial.js
+-rw-r--r--   0        0        0     1270 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshNormalMaterial.js
+-rw-r--r--   0        0        0     2736 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshPhongMaterial.js
+-rw-r--r--   0        0        0     3909 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshPhysicalMaterial.js
+-rw-r--r--   0        0        0     2723 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshStandardMaterial.js
+-rw-r--r--   0        0        0     2249 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshToonMaterial.js
+-rw-r--r--   0        0        0      719 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/PointsMaterial.js
+-rw-r--r--   0        0        0      268 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/RawShaderMaterial.js
+-rw-r--r--   0        0        0     4004 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/ShaderMaterial.js
+-rw-r--r--   0        0        0      513 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/ShadowMaterial.js
+-rw-r--r--   0        0        0      761 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/SpriteMaterial.js
+-rw-r--r--   0        0        0     3215 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Box2.js
+-rw-r--r--   0        0        0    11131 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Box3.js
+-rw-r--r--   0        0        0    13676 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Color.js
+-rw-r--r--   0        0        0     3481 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/ColorManagement.js
+-rw-r--r--   0        0        0      953 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Cylindrical.js
+-rw-r--r--   0        0        0     4760 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Euler.js
+-rw-r--r--   0        0        0     3449 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Frustum.js
+-rw-r--r--   0        0        0     4271 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Interpolant.js
+-rw-r--r--   0        0        0     1776 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Line3.js
+-rw-r--r--   0        0        0     8286 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/MathUtils.js
+-rw-r--r--   0        0        0     5805 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Matrix3.js
+-rw-r--r--   0        0        0    18553 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Matrix4.js
+-rw-r--r--   0        0        0     3649 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Plane.js
+-rw-r--r--   0        0        0    12518 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Quaternion.js
+-rw-r--r--   0        0        0     9979 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Ray.js
+-rw-r--r--   0        0        0     3657 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Sphere.js
+-rw-r--r--   0        0        0     1355 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Spherical.js
+-rw-r--r--   0        0        0     4498 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/SphericalHarmonics3.js
+-rw-r--r--   0        0        0     7069 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Triangle.js
+-rw-r--r--   0        0        0     5787 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Vector2.js
+-rw-r--r--   0        0        0    11022 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Vector3.js
+-rw-r--r--   0        0        0    10233 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Vector4.js
+-rw-r--r--   0        0        0     2966 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/interpolants/CubicInterpolant.js
+-rw-r--r--   0        0        0      482 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/interpolants/DiscreteInterpolant.js
+-rw-r--r--   0        0        0      704 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/interpolants/LinearInterpolant.js
+-rw-r--r--   0        0        0      789 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/interpolants/QuaternionLinearInterpolant.js
+-rw-r--r--   0        0        0      180 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Bone.js
+-rw-r--r--   0        0        0      184 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Group.js
+-rw-r--r--   0        0        0     4172 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/InstancedMesh.js
+-rw-r--r--   0        0        0     3173 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/LOD.js
+-rw-r--r--   0        0        0     5669 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Line.js
+-rw-r--r--   0        0        0      218 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/LineLoop.js
+-rw-r--r--   0        0        0     1249 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/LineSegments.js
+-rw-r--r--   0        0        0    10318 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Mesh.js
+-rw-r--r--   0        0        0     3937 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Points.js
+-rw-r--r--   0        0        0     5243 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Skeleton.js
+-rw-r--r--   0        0        0     4867 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/SkinnedMesh.js
+-rw-r--r--   0        0        0     4796 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Sprite.js
+-rw-r--r--   0        0        0      178 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGL1Renderer.js
+-rw-r--r--   0        0        0      470 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGL3DRenderTarget.js
+-rw-r--r--   0        0        0      488 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGLArrayRenderTarget.js
+-rw-r--r--   0        0        0     4441 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGLCubeRenderTarget.js
+-rw-r--r--   0        0        0     1686 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGLMultipleRenderTargets.js
+-rw-r--r--   0        0        0     3407 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGLRenderTarget.js
+-rw-r--r--   0        0        0    62065 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGLRenderer.js
+-rw-r--r--   0        0        0      116 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/alphamap_fragment.glsl.js
+-rw-r--r--   0        0        0       88 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/alphamap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      104 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/alphatest_fragment.glsl.js
+-rw-r--r--   0        0        0       84 2023-05-17 07:27:49.411849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/alphatest_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      532 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/aomap_fragment.glsl.js
+-rw-r--r--   0        0        0      113 2023-05-17 07:27:49.431849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/aomap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0       67 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/begin_vertex.glsl.js
+-rw-r--r--   0        0        0      138 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/beginnormal_vertex.glsl.js
+-rw-r--r--   0        0        0      845 2023-05-17 07:27:49.461849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/bsdfs.glsl.js
+-rw-r--r--   0        0        0     1137 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/bumpmap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      100 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clearcoat_normal_fragment_begin.glsl.js
+-rw-r--r--   0        0        0      262 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clearcoat_normal_fragment_maps.glsl.js
+-rw-r--r--   0        0        0      299 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clearcoat_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      630 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_fragment.glsl.js
+-rw-r--r--   0        0        0      150 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_pars_fragment.glsl.js
+-rw-r--r--   0        0        0       96 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_pars_vertex.glsl.js
+-rw-r--r--   0        0        0      102 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_vertex.glsl.js
+-rw-r--r--   0        0        0      153 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/color_fragment.glsl.js
+-rw-r--r--   0        0        0      143 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/color_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      178 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/color_pars_vertex.glsl.js
+-rw-r--r--   0        0        0      297 2023-05-17 07:27:49.481849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/color_vertex.glsl.js
+-rw-r--r--   0        0        0     3881 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/common.glsl.js
+-rw-r--r--   0        0        0     4004 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/cube_uv_reflection_fragment.glsl.js
+-rw-r--r--   0        0        0       90 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/default_fragment.glsl.js
+-rw-r--r--   0        0        0      121 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/default_vertex.glsl.js
+-rw-r--r--   0        0        0      705 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/defaultnormal_vertex.glsl.js
+-rw-r--r--   0        0        0      169 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/displacementmap_pars_vertex.glsl.js
+-rw-r--r--   0        0        0      205 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/displacementmap_vertex.glsl.js
+-rw-r--r--   0        0        0      107 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/dithering_fragment.glsl.js
+-rw-r--r--   0        0        0      608 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/dithering_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      172 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/emissivemap_fragment.glsl.js
+-rw-r--r--   0        0        0       94 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/emissivemap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0       82 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/encodings_fragment.glsl.js
+-rw-r--r--   0        0        0      293 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/encodings_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      216 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_common_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     1242 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_fragment.glsl.js
+-rw-r--r--   0        0        0      345 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      320 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_pars_vertex.glsl.js
+-rw-r--r--   0        0        0     1027 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_physical_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      647 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_vertex.glsl.js
+-rw-r--r--   0        0        0      303 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/fog_fragment.glsl.js
+-rw-r--r--   0        0        0      218 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/fog_pars_fragment.glsl.js
+-rw-r--r--   0        0        0       80 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/fog_pars_vertex.glsl.js
+-rw-r--r--   0        0        0       83 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/fog_vertex.glsl.js
+-rw-r--r--   0        0        0      512 2023-05-17 07:27:49.591848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/gradientmap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     3632 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/iridescence_fragment.glsl.js
+-rw-r--r--   0        0        0      191 2023-05-17 07:27:49.601848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/iridescence_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      239 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lightmap_fragment.glsl.js
+-rw-r--r--   0        0        0      122 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lightmap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     5799 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_begin.glsl.js
+-rw-r--r--   0        0        0      293 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_end.glsl.js
+-rw-r--r--   0        0        0      721 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_maps.glsl.js
+-rw-r--r--   0        0        0      144 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_lambert_fragment.glsl.js
+-rw-r--r--   0        0        0      873 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_lambert_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     5466 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_pars_begin.glsl.js
+-rw-r--r--   0        0        0      222 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_phong_fragment.glsl.js
+-rw-r--r--   0        0        0     1146 2023-05-17 07:27:49.611847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_phong_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     3038 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_physical_fragment.glsl.js
+-rw-r--r--   0        0        0    16313 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_physical_pars_fragment.glsl.js
+-rw-r--r--   0        0        0       95 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_toon_fragment.glsl.js
+-rw-r--r--   0        0        0      811 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_toon_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      315 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/logdepthbuf_fragment.glsl.js
+-rw-r--r--   0        0        0      192 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/logdepthbuf_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      200 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/logdepthbuf_pars_vertex.glsl.js
+-rw-r--r--   0        0        0      393 2023-05-17 07:27:49.631847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/logdepthbuf_vertex.glsl.js
+-rw-r--r--   0        0        0       97 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/map_fragment.glsl.js
+-rw-r--r--   0        0        0       78 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/map_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      381 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/map_particle_fragment.glsl.js
+-rw-r--r--   0        0        0      292 2023-05-17 07:27:49.641847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/map_particle_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      294 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/metalnessmap_fragment.glsl.js
+-rw-r--r--   0        0        0       96 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/metalnessmap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      861 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphcolor_vertex.glsl.js
+-rw-r--r--   0        0        0      936 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphnormal_vertex.glsl.js
+-rw-r--r--   0        0        0      832 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphtarget_pars_vertex.glsl.js
+-rw-r--r--   0        0        0     1215 2023-05-17 07:27:49.661847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphtarget_vertex.glsl.js
+-rw-r--r--   0        0        0     1132 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_fragment_begin.glsl.js
+-rw-r--r--   0        0        0      642 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_fragment_maps.glsl.js
+-rw-r--r--   0        0        0      165 2023-05-17 07:27:49.671847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      165 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_pars_vertex.glsl.js
+-rw-r--r--   0        0        0      303 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_vertex.glsl.js
+-rw-r--r--   0        0        0      942 2023-05-17 07:27:49.681846 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normalmap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      261 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/output_fragment.glsl.js
+-rw-r--r--   0        0        0     2171 2023-05-17 07:27:50.371839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/packing.glsl.js
+-rw-r--r--   0        0        0      223 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/premultiplied_alpha_fragment.glsl.js
+-rw-r--r--   0        0        0      239 2023-05-17 07:27:50.391839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/project_vertex.glsl.js
+-rw-r--r--   0        0        0      294 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/roughnessmap_fragment.glsl.js
+-rw-r--r--   0        0        0       96 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/roughnessmap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     9965 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     1368 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_pars_vertex.glsl.js
+-rw-r--r--   0        0        0     1798 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_vertex.glsl.js
+-rw-r--r--   0        0        0     1509 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmask_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      247 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinbase_vertex.glsl.js
+-rw-r--r--   0        0        0      795 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinning_pars_vertex.glsl.js
+-rw-r--r--   0        0        0      400 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinning_vertex.glsl.js
+-rw-r--r--   0        0        0      481 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinnormal_vertex.glsl.js
+-rw-r--r--   0        0        0      221 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/specularmap_fragment.glsl.js
+-rw-r--r--   0        0        0       94 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/specularmap_pars_fragment.glsl.js
+-rw-r--r--   0        0        0      120 2023-05-17 07:27:50.481838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/tonemapping_fragment.glsl.js
+-rw-r--r--   0        0        0     2018 2023-05-17 07:27:50.481838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/tonemapping_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     1099 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/transmission_fragment.glsl.js
+-rw-r--r--   0        0        0     5804 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/transmission_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     1530 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_pars_fragment.glsl.js
+-rw-r--r--   0        0        0     2355 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_pars_vertex.glsl.js
+-rw-r--r--   0        0        0     2606 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_vertex.glsl.js
+-rw-r--r--   0        0        0      357 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/worldpos_vertex.glsl.js
+-rw-r--r--   0        0        0    15020 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk.js
+-rw-r--r--   0        0        0      497 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/background.glsl.js
+-rw-r--r--   0        0        0     1079 2023-05-17 07:27:49.451849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/backgroundCube.glsl.js
+-rw-r--r--   0        0        0      653 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/cube.glsl.js
+-rw-r--r--   0        0        0     2069 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/depth.glsl.js
+-rw-r--r--   0        0        0     1500 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/distanceRGBA.glsl.js
+-rw-r--r--   0        0        0      567 2023-05-17 07:27:49.561848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/equirect.glsl.js
+-rw-r--r--   0        0        0     1522 2023-05-17 07:27:49.621847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/linedashed.glsl.js
+-rw-r--r--   0        0        0     2561 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshbasic.glsl.js
+-rw-r--r--   0        0        0     3032 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshlambert.glsl.js
+-rw-r--r--   0        0        0     2532 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshmatcap.glsl.js
+-rw-r--r--   0        0        0     1718 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshnormal.glsl.js
+-rw-r--r--   0        0        0     3138 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshphong.glsl.js
+-rw-r--r--   0        0        0     5169 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshphysical.glsl.js
+-rw-r--r--   0        0        0     2832 2023-05-17 07:27:49.651847 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshtoon.glsl.js
+-rw-r--r--   0        0        0     1660 2023-05-17 07:27:50.381839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/points.glsl.js
+-rw-r--r--   0        0        0     1128 2023-05-17 07:27:50.421839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/shadow.glsl.js
+-rw-r--r--   0        0        0     1896 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/sprite.glsl.js
+-rw-r--r--   0        0        0     1206 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/vsm.glsl.js
+-rw-r--r--   0        0        0     8167 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib.js
+-rw-r--r--   0        0        0     4406 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/UniformsLib.js
+-rw-r--r--   0        0        0     1666 2023-05-17 07:27:50.491838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/UniformsUtils.js
+-rw-r--r--   0        0        0      767 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLAnimation.js
+-rw-r--r--   0        0        0     3453 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLAttributes.js
+-rw-r--r--   0        0        0     6412 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBackground.js
+-rw-r--r--   0        0        0    13419 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBindingStates.js
+-rw-r--r--   0        0        0     1050 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBufferRenderer.js
+-rw-r--r--   0        0        0     3167 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCapabilities.js
+-rw-r--r--   0        0        0     3372 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLClipping.js
+-rw-r--r--   0        0        0     1956 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCubeMaps.js
+-rw-r--r--   0        0        0     2755 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCubeUVMaps.js
+-rw-r--r--   0        0        0     2217 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLExtensions.js
+-rw-r--r--   0        0        0     3623 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLGeometries.js
+-rw-r--r--   0        0        0     1281 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLIndexedBufferRenderer.js
+-rw-r--r--   0        0        0     1044 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLInfo.js
+-rw-r--r--   0        0        0    13387 2023-05-17 07:27:50.511838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLLights.js
+-rw-r--r--   0        0        0    12823 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLMaterials.js
+-rw-r--r--   0        0        0     7750 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLMorphtargets.js
+-rw-r--r--   0        0        0     1290 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLObjects.js
+-rw-r--r--   0        0        0    28100 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLProgram.js
+-rw-r--r--   0        0        0    19534 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLPrograms.js
+-rw-r--r--   0        0        0      560 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLProperties.js
+-rw-r--r--   0        0        0     4054 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLRenderLists.js
+-rw-r--r--   0        0        0     1687 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLRenderStates.js
+-rw-r--r--   0        0        0      196 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShader.js
+-rw-r--r--   0        0        0     1975 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShaderCache.js
+-rw-r--r--   0        0        0    10649 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShadowMap.js
+-rw-r--r--   0        0        0    25232 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLState.js
+-rw-r--r--   0        0        0    56653 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLTextures.js
+-rw-r--r--   0        0        0    20325 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUniforms.js
+-rw-r--r--   0        0        0     8558 2023-05-17 07:27:50.521838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUniformsGroups.js
+-rw-r--r--   0        0        0     9973 2023-05-17 07:27:50.531838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUtils.js
+-rw-r--r--   0        0        0     6520 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webxr/WebXRController.js
+-rw-r--r--   0        0        0    19550 2023-05-17 07:27:50.541838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webxr/WebXRManager.js
+-rw-r--r--   0        0        0      442 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/scenes/Fog.js
+-rw-r--r--   0        0        0      427 2023-05-17 07:27:49.571848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/scenes/FogExp2.js
+-rw-r--r--   0        0        0     1785 2023-05-17 07:27:50.411839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/scenes/Scene.js
+-rw-r--r--   0        0        0      361 2023-05-17 07:27:49.471849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/CanvasTexture.js
+-rw-r--r--   0        0        0      434 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/CompressedArrayTexture.js
+-rw-r--r--   0        0        0      703 2023-05-17 07:27:49.491849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/CompressedTexture.js
+-rw-r--r--   0        0        0      642 2023-05-17 07:27:49.501849 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/CubeTexture.js
+-rw-r--r--   0        0        0      793 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/Data3DTexture.js
+-rw-r--r--   0        0        0      544 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/DataArrayTexture.js
+-rw-r--r--   0        0        0      603 2023-05-17 07:27:49.511848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/DataTexture.js
+-rw-r--r--   0        0        0     1109 2023-05-17 07:27:49.521848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/DepthTexture.js
+-rw-r--r--   0        0        0      436 2023-05-17 07:27:49.581848 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/FramebufferTexture.js
+-rw-r--r--   0        0        0     1843 2023-05-17 07:27:50.431839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/Source.js
+-rw-r--r--   0        0        0     6777 2023-05-17 07:27:50.441839 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/Texture.js
+-rw-r--r--   0        0        0     1111 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/VideoTexture.js
+-rw-r--r--   0        0        0     1404 2023-05-17 07:27:50.501838 zndraw-0.2.0a1/zndraw/static/node_modules/three/src/utils.js
+-rw-r--r--   0        0        0     1561 2023-05-17 07:27:50.641837 zndraw-0.2.0a1/zndraw/static/package-lock.json
+-rw-r--r--   0        0        0       79 2023-05-15 11:39:37.682661 zndraw-0.2.0a1/zndraw/static/package.json
+-rw-r--r--   0        0        0    17715 2023-05-16 15:59:54.061278 zndraw-0.2.0a1/zndraw/templates/index.html
+-rw-r--r--   0        0        0       68 2023-04-27 11:21:12.206714 zndraw-0.2.0a1/zndraw/tools/__init__.py
+-rw-r--r--   0        0        0     1825 2023-05-15 16:15:51.883487 zndraw-0.2.0a1/zndraw/tools/data.py
+-rw-r--r--   0        0        0      856 2023-04-27 11:21:12.206714 zndraw-0.2.0a1/zndraw/tools/select.py
+-rw-r--r--   0        0        0     3192 1970-01-01 00:00:00.000000 zndraw-0.2.0a1/PKG-INFO
```

### Comparing `zndraw-0.1.8/LICENSE` & `zndraw-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/README.md` & `zndraw-0.2.0a1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,67 @@
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 [![PyPI version](https://badge.fury.io/py/zndraw.svg)](https://badge.fury.io/py/zndraw)
 !['Threejs](https://img.shields.io/badge/threejs-black?style=for-the-badge&logo=three.js&logoColor=white)
 
-
 # ZnDraw
 
-Install via ``pip install zndraw`` or ``pip install zndraw[webview]`` to open zndraw in a dedicated window.
+Install via `pip install zndraw` or `pip install zndraw[webview]` to open zndraw
+in a dedicated window.
 
 ## CLI
 
-You can use ZnDraw with the CLI ``zndraw atoms.xyz``.
-For a full list of arguments use `zndraw --help`.
+You can use ZnDraw with the CLI `zndraw atoms.xyz`. For a full list of arguments
+use `zndraw --help`.
 
-ZnDraw is designed to work with your Python scripts.
-To interface you can inherit from `zndraw.examples.UpdateScene` or follow this base class:
+ZnDraw is designed to work with your Python scripts. To interface you can
+inherit from `zndraw.examples.UpdateScene` or follow this base class:
 
 ```python
 import abc
 from pydantic import BaseModel
 
 class UpdateScene(BaseModel, abc.ABC):
     @abc.abstractmethod
     def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         pass
 ```
 
-The ``run`` method expects as inputs
-- atom_ids: list[int], the ids of the currently selected atoms
-- atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where selected.
+The `run` method expects as inputs
+
+- atom_ids: list\[int\], the ids of the currently selected atoms
+- atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where
+  selected.
 - kwargs: dict could be additional information from the scene
 
 and as an output:
-- list[ase.Atoms], a list of ase Atoms objects to display.
 
+- list\[ase.Atoms\], a list of ase Atoms objects to display.
 
-You can define the parameters using `pydantic.Field` which will be displayed in the UI.
+You can define the parameters using `pydantic.Field` which will be displayed in
+the UI.
 
 ```python
 class MyUpdateCls(UpdateScene):
     steps: int = Field(100, le=1000, ge=1)
     x: float = Field(0.5, le=5, ge=0)
     symbol: str = Field("same")
 ```
 
-To add your method click on the `+` on the right side of the window.
-Your should be able to add your method from the working directory via `module.MyUpdateCls` as long
-as it can be imported via `from module import MyUpdateCls`.
+To add your method click on the `+` on the right side of the window. Your should
+be able to add your method from the working directory via `module.MyUpdateCls`
+as long as it can be imported via `from module import MyUpdateCls`.
 
 ![ZnDraw UI](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
 
 ![ZnDraw UI2](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_protein.png "ZnDraw UI2")
 
 ![ZnDraw UI3](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_draw.png "ZnDraw UI3")
+
+# Development
+
+ZnDraw is developed using https://python-poetry.org/. Furthermore, the
+javascript packages have to be installed using https://www.npmjs.com/.
+
+```bash
+cd zndraw/static/
+npm install
+```
```

### Comparing `zndraw-0.1.8/pyproject.toml` & `zndraw-0.2.0a1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "zndraw"
-version = "0.1.8"
+version = "0.2.0a1"
 description = ""
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
+include = ["zndraw/static/node_modules/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ase = "^3.22.1"
 networkx = "^3.1"
 typer = {extras = ["all"], version = "^0.7.0"}
 flask = "^2.2.3"
```

### Comparing `zndraw-0.1.8/zndraw/analyse.py` & `zndraw-0.2.0a1/zndraw/analyse.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/app.py` & `zndraw-0.2.0a1/zndraw/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import json
 import uuid
 
 import networkx as nx
 import numpy as np
-from flask import Flask, render_template, request, session
+import tqdm
+from flask import (Flask, Response, render_template, request, session,
+                   stream_with_context)
 
 from zndraw import io, shared, tools
 
 app = Flask(__name__)
 app.secret_key = str(uuid.uuid4())
 
 
 @app.route("/")
 def index():
     """Render the main ZnDraw page."""
     session["key"] = str(uuid.uuid4())  # TODO use session key e.g. for atoms cache
+    session["step"] = 0
     return render_template("index.html", config=shared.config.dict())
 
 
 @app.route("/config", methods=["POST", "GET"])
 def config():
     """Get the zndraw configuration."""
     if request.method == "POST":
@@ -26,34 +30,14 @@
             setattr(shared.config, key, value)
     return {
         **shared.config.dict(),
         "total_frames": len(shared.config._atoms_cache) - 1,
     }
 
 
-@app.route("/graph", methods=["POST"])
-def get_graph():
-    step = request.json
-    try:
-        atoms = shared.config.get_atoms(step=int(step))
-        graph = io.get_graph(atoms)
-        return {
-            "nodes": [{**graph.nodes[idx], "id": idx} for idx in graph.nodes],
-            "edges": list(graph.edges),
-            "box": atoms.get_cell().diagonal().tolist(),
-        }
-    except KeyError:
-        return {}
-
-
-@app.route("/data", methods=["POST"])
-def positions_step():
-    return tools.data.serialize_atoms(request.json["start"], request.json["stop"])
-
-
 @app.route("/select", methods=["POST"])
 def select() -> list[int]:
     """Update the selected atoms."""
     step = request.json["step"]
     method = request.json["method"]
     try:
         selected_ids = [int(x) for x in request.json["selected_ids"]]
@@ -91,15 +75,16 @@
 @app.route("/update", methods=["POST"])
 def update_scene():
     """Update the scene with the selected atoms."""
     modifier = request.json["modifier"]
     modifier_kwargs = request.json["modifier_kwargs"]
     selected_ids = list(sorted(request.json["selected_ids"]))
     step = request.json["step"]
-    points = np.array([[x["x"], x["y"], x["z"]] for x in request.json["points"]])
+    # points = np.array([[x["x"], x["y"], x["z"]] for x in request.json["points"]])
+    points = None
     shared.config.run_modifier(
         modifier, selected_ids, step, modifier_kwargs, points=points
     )
     return {}
 
 
 @app.route("/add_analysis", methods=["POST"])
@@ -153,7 +138,29 @@
 def download():
     """Download the current atoms."""
     from flask import send_file
 
     b = shared.config.export_atoms()
     b.seek(0)
     return send_file(b, download_name="traj.h5", as_attachment=True)
+
+
+@app.route("/frame-set", methods=["POST"])
+def frame_set():
+    session["step"] = request.json["step"]
+    print(f"Setting step to {session['step']}")
+    return {}
+
+
+@app.route("/frame-stream")
+def frame_stream():
+    def generate(step):
+        for idx in tqdm.tqdm(range(step, step + 100), desc=f"Streaming from {step}"):
+            try:
+                data = {idx: tools.data.serialize_frame(idx)}
+                yield f"data: {json.dumps(data)}\n\n"
+            except KeyError:
+                print(f"Can not load step {idx}")
+                break
+        yield f"data: {json.dumps({})} \nretry: 10\n\n"
+
+    return Response(generate(session["step"]), mimetype="text/event-stream")
```

### Comparing `zndraw-0.1.8/zndraw/cli.py` & `zndraw-0.2.0a1/zndraw/cli.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/examples/__init__.py` & `zndraw-0.2.0a1/zndraw/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/io.py` & `zndraw-0.2.0a1/zndraw/io.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/main.py` & `zndraw-0.2.0a1/zndraw/main.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/shared.py` & `zndraw-0.2.0a1/zndraw/shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     bond_size: float = Field(1.0, description="Bond Size")
     sphere_size: float = Field(1.0, description="Sphere Size")
     resolution: int = Field(10, description="Resolution")
     max_fps: int = Field(100, description="Maximum Frames Per Second")
     frames_per_post: int = Field(100, description="Frames per JS POST request")
     active_update_function: str = Field(None, description="Active Update Function")
     material: str = Field("MeshPhongMaterial", description="Material")
+    material_wireframe: bool = Field(False, description="Material Wireframe")
     antialias: bool = Field(True, description="Antialias")
     continuous_loading: bool = Field(
         False, description="Continuous Loading of the trajectory"
     )
     analysis_functions: typing.List[str] = _ANALYSIS_FUNCTIONS
     modify_functions: typing.List[str] = _MODIFY_FUNCTIONS
     selection_functions: typing.List[str] = _SELECTION_FUNCTIONS
@@ -128,20 +129,19 @@
         return list(self._atoms_cache.values())
 
     def load_atoms(self, step: int = 999999999):
         """Load the atoms up to a given step."""
         # TODO ZnH5MD
         if self._modifier_applied:
             return  # We don't want to load any further from file at this point
+        print("Loading atoms")
         if pathlib.Path(self.file).suffix == ".h5":
             # We load all at once here
             self._atoms_cache.update(
-                dict(enumerate(znh5md.ASEH5MD(self.file).get_atoms_list()[: step + 1]))
+                dict(enumerate(znh5md.ASEH5MD(self.file).get_atoms_list()))
             )
         else:
             for idx, atoms in enumerate(tqdm.tqdm(ase.io.iread(self.file))):
                 self._atoms_cache[idx] = atoms
-                if idx == step:
-                    break
 
 
 config: Config = None
```

### Comparing `zndraw-0.1.8/zndraw/static/favion-192x192.png` & `zndraw-0.2.0a1/zndraw/static/favion-192x192.png`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/main.css` & `zndraw-0.2.0a1/zndraw/static/main.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,271 +1,272 @@
 :root {
-    --spinner-size: 60px;
+  --spinner-size: 60px;
 }
 
-
 body {
-    margin: 0;
-    /* overflow: hidden;  don't show scrolling bars */
-}
-
-canvas {
-    position: absolute;
-    top: 0;
-    left: 0;
-    width: 100%;
-    height: 100%;
-    z-index: -100;
+  /* remove margins and scroll bars */
+  margin: 0;
+  overflow: hidden;
+}
+
+#scene-container {
+  /* tell our scene container to take up the full page */
+  position: absolute;
+  width: 100%;
+  height: 100%;
+
+  /*
+    Set the container's background color to the same as the scene's
+    background to prevent flashing on load
+  */
+  background-color: rgb(255, 255, 255);
 }
 
 .atom-spinner,
 .atom-spinner * {
-    box-sizing: border-box;
+  box-sizing: border-box;
 }
 
 .atom-spinner {
-    height: var(--spinner-size);
-    width: var(--spinner-size);
-    overflow: hidden;
-    position: absolute;
-    bottom: 50%;
-    left: 50%;
-    z-index: 100;
-    display: block;
+  height: var(--spinner-size);
+  width: var(--spinner-size);
+  overflow: hidden;
+  position: absolute;
+  bottom: 50%;
+  left: 50%;
+  z-index: 100;
+  display: block;
 }
 
 .atom-spinner .spinner-inner {
-    position: relative;
-    display: block;
-    height: 100%;
-    width: 100%;
+  position: relative;
+  display: block;
+  height: 100%;
+  width: 100%;
 }
 
 .atom-spinner .spinner-circle {
-    display: block;
-    position: absolute;
-    color: #ffa500;
-    font-size: calc(var(--spinner-size) * 0.24);
-    top: 50%;
-    left: 50%;
-    transform: translate(-50%, -50%);
+  display: block;
+  position: absolute;
+  color: #ffa500;
+  font-size: calc(var(--spinner-size) * 0.24);
+  top: 50%;
+  left: 50%;
+  transform: translate(-50%, -50%);
 }
 
 .atom-spinner .spinner-line {
-    position: absolute;
-    width: 100%;
-    height: 100%;
-    border-radius: 50%;
-    animation-duration: 1s;
-    border-left-width: calc(var(--spinner-size) / 25);
-    border-top-width: calc(var(--spinner-size) / 25);
-    border-left-color: #ffa500;
-    border-left-style: solid;
-    border-top-style: solid;
-    border-top-color: transparent;
+  position: absolute;
+  width: 100%;
+  height: 100%;
+  border-radius: 50%;
+  animation-duration: 1s;
+  border-left-width: calc(var(--spinner-size) / 25);
+  border-top-width: calc(var(--spinner-size) / 25);
+  border-left-color: #ffa500;
+  border-left-style: solid;
+  border-top-style: solid;
+  border-top-color: transparent;
 }
 
 .atom-spinner .spinner-line:nth-child(1) {
-    animation: atom-spinner-animation-1 1s linear infinite;
-    transform: rotateZ(120deg) rotateX(66deg) rotateZ(0deg);
+  animation: atom-spinner-animation-1 1s linear infinite;
+  transform: rotateZ(120deg) rotateX(66deg) rotateZ(0deg);
 }
 
 .atom-spinner .spinner-line:nth-child(2) {
-    animation: atom-spinner-animation-2 1s linear infinite;
-    transform: rotateZ(240deg) rotateX(66deg) rotateZ(0deg);
+  animation: atom-spinner-animation-2 1s linear infinite;
+  transform: rotateZ(240deg) rotateX(66deg) rotateZ(0deg);
 }
 
 .atom-spinner .spinner-line:nth-child(3) {
-    animation: atom-spinner-animation-3 1s linear infinite;
-    transform: rotateZ(360deg) rotateX(66deg) rotateZ(0deg);
+  animation: atom-spinner-animation-3 1s linear infinite;
+  transform: rotateZ(360deg) rotateX(66deg) rotateZ(0deg);
 }
 
 @keyframes atom-spinner-animation-1 {
-    100% {
-        transform: rotateZ(120deg) rotateX(66deg) rotateZ(360deg);
-    }
+  100% {
+    transform: rotateZ(120deg) rotateX(66deg) rotateZ(360deg);
+  }
 }
 
 @keyframes atom-spinner-animation-2 {
-    100% {
-        transform: rotateZ(240deg) rotateX(66deg) rotateZ(360deg);
-    }
+  100% {
+    transform: rotateZ(240deg) rotateX(66deg) rotateZ(360deg);
+  }
 }
 
 @keyframes atom-spinner-animation-3 {
-    100% {
-        transform: rotateZ(360deg) rotateX(66deg) rotateZ(360deg);
-    }
+  100% {
+    transform: rotateZ(360deg) rotateX(66deg) rotateZ(360deg);
+  }
 }
 
-
 #greyOut {
-    pointer-events: none;
-    display: block;
-    position: fixed;
-    top: 0;
-    bottom: 0;
-    left: 0;
-    right: 0;
-    width: 100%;
-    height: 100%;
-    background-color: black;
-    opacity: 0.05;
-    z-index: 1;
-    text-align: center;
+  pointer-events: none;
+  display: block;
+  position: fixed;
+  top: 0;
+  bottom: 0;
+  left: 0;
+  right: 0;
+  width: 100%;
+  height: 100%;
+  background-color: black;
+  opacity: 0.05;
+  z-index: 1;
+  text-align: center;
 }
 
 #info {
-    position: absolute;
-    bottom: 10px;
-    text-align: center;
-    width: 100%;
-    z-index: 100;
-    display: block;
-    opacity: 0.5;
+  position: absolute;
+  bottom: 10px;
+  text-align: center;
+  width: 100%;
+  z-index: 100;
+  display: block;
+  opacity: 0.5;
 }
 
 #infoBox {
-    position: absolute;
-    bottom: 1%;
-    left: 69%;
-    right: 1%;
-    width: 30%;
-    z-index: 100;
-    display: block;
-    background-color: rgb(235, 235, 235);
-    opacity: 0.8;
+  position: absolute;
+  bottom: 1%;
+  left: 69%;
+  right: 1%;
+  width: 30%;
+  z-index: 100;
+  display: block;
+  background-color: rgb(235, 235, 235);
+  opacity: 0.8;
 }
 
 #helpBox {
-    position: absolute;
-    top: 20%;
-    display: block;
-    left: 10%;
-    right: 10%;
-    width: 80%;
+  position: absolute;
+  top: 20%;
+  display: block;
+  left: 10%;
+  right: 10%;
+  width: 80%;
 }
 
 .canvasControl {
-    opacity: 0.95;
+  opacity: 0.95;
 }
 
-
 .frame-slider {
-    -webkit-appearance: none;
-    position: fixed;
-    width: 100%;
-    z-index: 100;
-    overflow: hidden;
-    bottom: -6px;
-    display: block;
-    left: 0;
-    transition: bottom .1s ease;
-    height: 12px;
-    width: 100%;
+  -webkit-appearance: none;
+  position: fixed;
+  width: 100%;
+  z-index: 100;
+  overflow: hidden;
+  bottom: -6px;
+  display: block;
+  left: 0;
+  transition: bottom 0.1s ease;
+  height: 12px;
+  width: 100%;
 }
 
 .frame-slider:focus {
-    outline: none;
+  outline: none;
 }
 
 .frame-slider::-webkit-slider-runnable-track {
-    width: 100%;
-    height: 12px;
-    cursor: pointer;
-    animate: 0.2s;
-    box-shadow: 0px 0px 0px #000000;
-    background: #EEEEEE;
-    border-radius: 0px;
-    border: 0px solid #000000;
+  width: 100%;
+  height: 12px;
+  cursor: pointer;
+  animate: 0.2s;
+  box-shadow: 0px 0px 0px #000000;
+  background: #eeeeee;
+  border-radius: 0px;
+  border: 0px solid #000000;
 }
 
 .frame-slider::-webkit-slider-thumb {
-    box-shadow: 0px 0px 0px #000000;
-    border: 0px solid #000000;
-    height: 12px;
-    width: 30px;
-    border-radius: 0px;
-    background: #314159;
-    cursor: pointer;
-    -webkit-appearance: none;
-    margin-top: 0px;
+  box-shadow: 0px 0px 0px #000000;
+  border: 0px solid #000000;
+  height: 12px;
+  width: 30px;
+  border-radius: 0px;
+  background: #314159;
+  cursor: pointer;
+  -webkit-appearance: none;
+  margin-top: 0px;
 }
 
 .frame-slider:focus::-webkit-slider-runnable-track {
-    background: #EEEEEE;
+  background: #eeeeee;
 }
 
 .frame-slider::-moz-range-track {
-    width: 100%;
-    height: 12px;
-    cursor: pointer;
-    animate: 0.2s;
-    box-shadow: 0px 0px 0px #000000;
-    background: #EEEEEE;
-    border-radius: 0px;
-    border: 0px solid #000000;
+  width: 100%;
+  height: 12px;
+  cursor: pointer;
+  animate: 0.2s;
+  box-shadow: 0px 0px 0px #000000;
+  background: #eeeeee;
+  border-radius: 0px;
+  border: 0px solid #000000;
 }
 
 .frame-slider::-moz-range-thumb {
-    box-shadow: 0px 0px 0px #000000;
-    border: 0px solid #000000;
-    height: 12px;
-    width: 30px;
-    border-radius: 0px;
-    background: #314159;
-    cursor: pointer;
+  box-shadow: 0px 0px 0px #000000;
+  border: 0px solid #000000;
+  height: 12px;
+  width: 30px;
+  border-radius: 0px;
+  background: #314159;
+  cursor: pointer;
 }
 
 .frame-slider::-ms-track {
-    width: 100%;
-    height: 12px;
-    cursor: pointer;
-    animate: 0.2s;
-    background: transparent;
-    border-color: transparent;
-    color: transparent;
+  width: 100%;
+  height: 12px;
+  cursor: pointer;
+  animate: 0.2s;
+  background: transparent;
+  border-color: transparent;
+  color: transparent;
 }
 
 .frame-slider::-ms-fill-lower {
-    background: #EEEEEE;
-    border: 0px solid #000000;
-    border-radius: 0px;
-    box-shadow: 0px 0px 0px #000000;
+  background: #eeeeee;
+  border: 0px solid #000000;
+  border-radius: 0px;
+  box-shadow: 0px 0px 0px #000000;
 }
 
 .frame-slider::-ms-fill-upper {
-    background: #EEEEEE;
-    border: 0px solid #000000;
-    border-radius: 0px;
-    box-shadow: 0px 0px 0px #000000;
+  background: #eeeeee;
+  border: 0px solid #000000;
+  border-radius: 0px;
+  box-shadow: 0px 0px 0px #000000;
 }
 
 .frame-slider::-ms-thumb {
-    margin-top: 1px;
-    box-shadow: 0px 0px 0px #000000;
-    border: 0px solid #000000;
-    height: 12px;
-    width: 30px;
-    border-radius: 0px;
-    background: #314159;
-    cursor: pointer;
+  margin-top: 1px;
+  box-shadow: 0px 0px 0px #000000;
+  border: 0px solid #000000;
+  height: 12px;
+  width: 30px;
+  border-radius: 0px;
+  background: #314159;
+  cursor: pointer;
 }
 
 .frame-slider:focus::-ms-fill-lower {
-    background: #EEEEEE;
+  background: #eeeeee;
 }
 
 .frame-slider:focus::-ms-fill-upper {
-    background: #EEEEEE;
+  background: #eeeeee;
 }
 
-
 .offcanvas-border {
-    content: '';
-    background-color: #00000000;
-    position: absolute;
-    left: 400px;
-    width: 4px;
-    height: 100%;
-    cursor: ew-resize;
+  content: "";
+  background-color: #00000000;
+  position: absolute;
+  left: 400px;
+  width: 4px;
+  height: 100%;
+  cursor: ew-resize;
 }
```

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/.package-lock.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/.package-lock.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'packages'": "{delete: ['node_modules/@popperjs/core', 'node_modules/plotly.js-dist']}"}*

```diff
@@ -1,21 +1,11 @@
 {
     "lockfileVersion": 2,
     "name": "static",
     "packages": {
-        "node_modules/@popperjs/core": {
-            "funding": {
-                "type": "opencollective",
-                "url": "https://opencollective.com/popperjs"
-            },
-            "integrity": "sha512-Cr4OjIkipTtcXKjAsm8agyleBuDHvxzeBoa1v543lbv1YaIwQjESsVcmjiWiPEbC1FIeHOG/Op9kdCmAmiS3Kw==",
-            "peer": true,
-            "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.7.tgz",
-            "version": "2.11.7"
-        },
         "node_modules/bootstrap": {
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/twbs"
                 },
                 {
@@ -26,19 +16,14 @@
             "integrity": "sha512-cEKPM+fwb3cT8NzQZYEu4HilJ3anCrWqh3CHAok1p9jXqMPsPTBhU25fBckEJHJ/p+tTxTFTsFQGM+gaHpi3QQ==",
             "peerDependencies": {
                 "@popperjs/core": "^2.11.6"
             },
             "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.2.3.tgz",
             "version": "5.2.3"
         },
-        "node_modules/plotly.js-dist": {
-            "integrity": "sha512-+P4ouT5yPvPagFxNzTkAl0rraSWyjXIKPIXogBSzqfzVjbnapyoAK14sOh6X6+HPZlzOuh4/nGd+F+w7Te6KRA==",
-            "resolved": "https://registry.npmjs.org/plotly.js-dist/-/plotly.js-dist-2.23.2.tgz",
-            "version": "2.23.2"
-        },
         "node_modules/three": {
             "integrity": "sha512-Ff9zIpSfkkqcBcpdiFo2f35vA9ZucO+N8TNacJOqaEE6DrB0eufItVMib8bK8Pcju/ZNT6a7blE1GhTpkdsILw==",
             "resolved": "https://registry.npmjs.org/three/-/three-0.152.2.tgz",
             "version": "0.152.2"
         }
     },
     "requires": true
```

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/@popperjs/core/LICENSE.md` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-The MIT License (MIT)
+The MIT License
 
-Copyright (c) 2019 Federico Zivolo
+Copyright © 2010-2023 three.js authors
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/LICENSE` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/README.md` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/README.md`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/alert.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/alert.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/base-component.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/base-component.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/button.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/button.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/carousel.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/carousel.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/collapse.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/collapse.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dom/data.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dom/data.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dom/event-handler.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dom/event-handler.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dom/manipulator.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dom/manipulator.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dom/selector-engine.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dom/selector-engine.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/dropdown.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/dropdown.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/modal.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/modal.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/offcanvas.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/offcanvas.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/popover.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/popover.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/scrollspy.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/scrollspy.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/tab.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/tab.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/toast.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/toast.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/tooltip.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/tooltip.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/backdrop.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/backdrop.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/component-functions.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/component-functions.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/config.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/config.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/focustrap.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/focustrap.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/index.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/index.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/sanitizer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/sanitizer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/scrollbar.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/scrollbar.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/swipe.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/swipe.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/js/src/util/template-factory.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/js/src/util/template-factory.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/package.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_accordion.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_alert.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_badge.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_breadcrumb.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_button-group.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_buttons.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_card.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_carousel.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_close.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_containers.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_dropdown.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_functions.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_grid.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_images.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_list-group.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_maps.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_mixins.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_modal.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_nav.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_navbar.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_offcanvas.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_pagination.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_placeholders.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_popover.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_progress.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_reboot.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_root.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_spinners.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_tables.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_toasts.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_tooltip.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_type.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_utilities.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/_variables.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/bootstrap-grid.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/bootstrap.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_floating-labels.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_form-check.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_form-control.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_form-range.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_form-select.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_input-group.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/forms/_labels.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/helpers/_position.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_border-radius.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_breakpoints.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_buttons.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_caret.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_deprecate.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_forms.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_gradients.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_grid.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_table-variants.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_transition.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_utilities.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/mixins/_visually-hidden.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/utilities/_api.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/bootstrap/scss/vendor/_rfs.scss` & `zndraw-0.2.0a1/zndraw/static/node_modules/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/README.md` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/README.md`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/LICENSE` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/NOTICE` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/NOTICE`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/README.txt` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/README.txt`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_bold.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_bold.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_mono_regular.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_mono_regular.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_regular.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_sans_regular.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_serif_bold.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_serif_bold.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/droid/droid_serif_regular.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/droid/droid_serif_regular.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/gentilis_bold.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/gentilis_bold.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/gentilis_regular.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/gentilis_regular.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/helvetiker_bold.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/helvetiker_bold.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/helvetiker_regular.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/helvetiker_regular.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/optimer_bold.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/optimer_bold.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/optimer_regular.typeface.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/optimer_regular.typeface.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/fonts/ttf/kenpixel.ttf` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/fonts/ttf/kenpixel.ttf`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/animation/AnimationClipCreator.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/animation/AnimationClipCreator.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/animation/CCDIKSolver.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/animation/CCDIKSolver.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/animation/MMDAnimationHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/animation/MMDAnimationHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/animation/MMDPhysics.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/animation/MMDPhysics.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/cameras/CinematicCamera.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/cameras/CinematicCamera.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/capabilities/WebGL.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/capabilities/WebGL.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/capabilities/WebGPU.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/capabilities/WebGPU.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/ArcballControls.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/ArcballControls.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/DragControls.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/DragControls.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/FirstPersonControls.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/FirstPersonControls.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/FlyControls.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/FlyControls.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/MapControls.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/MapControls.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/OrbitControls.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/OrbitControls.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/PointerLockControls.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/PointerLockControls.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/TrackballControls.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/TrackballControls.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/controls/TransformControls.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/controls/TransformControls.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/csm/CSM.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/csm/CSM.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/csm/CSMFrustum.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/csm/CSMFrustum.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/csm/CSMHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/csm/CSMHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/csm/CSMShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/csm/CSMShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/curves/CurveExtras.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/curves/CurveExtras.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/curves/NURBSCurve.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/curves/NURBSCurve.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/curves/NURBSSurface.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/curves/NURBSSurface.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/curves/NURBSUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/curves/NURBSUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/AnaglyphEffect.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/AnaglyphEffect.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/AsciiEffect.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/AsciiEffect.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/OutlineEffect.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/OutlineEffect.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/ParallaxBarrierEffect.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/ParallaxBarrierEffect.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/PeppersGhostEffect.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/PeppersGhostEffect.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/effects/StereoEffect.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/effects/StereoEffect.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/environments/DebugEnvironment.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/environments/DebugEnvironment.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/environments/RoomEnvironment.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/environments/RoomEnvironment.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/ColladaExporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/ColladaExporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/DRACOExporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/DRACOExporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/EXRExporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/EXRExporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/GLTFExporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/GLTFExporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/KTX2Exporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/KTX2Exporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/MMDExporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/MMDExporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/OBJExporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/OBJExporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/PLYExporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/PLYExporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/STLExporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/STLExporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/exporters/USDZExporter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/exporters/USDZExporter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/BoxLineGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/BoxLineGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/ConvexGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/ConvexGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/DecalGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/DecalGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/LightningStrike.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/LightningStrike.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/ParametricGeometries.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/ParametricGeometries.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/ParametricGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/ParametricGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/RoundedBoxGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/RoundedBoxGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/TeapotGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/TeapotGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/geometries/TextGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/geometries/TextGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/LightProbeHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/LightProbeHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/OctreeHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/OctreeHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/PositionalAudioHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/PositionalAudioHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/RectAreaLightHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/RectAreaLightHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/VertexNormalsHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/VertexNormalsHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/VertexTangentsHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/VertexTangentsHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/helpers/ViewHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/helpers/ViewHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/interactive/HTMLMesh.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/interactive/HTMLMesh.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/interactive/InteractiveGroup.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/interactive/InteractiveGroup.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/interactive/SelectionBox.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/interactive/SelectionBox.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/interactive/SelectionHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/interactive/SelectionHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/ammo.wasm.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/ammo.wasm.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/ammo.wasm.wasm` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/ammo.wasm.wasm`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/basis/README.md` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/basis/README.md`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/basis/basis_transcoder.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/basis/basis_transcoder.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/basis/basis_transcoder.wasm` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/basis/basis_transcoder.wasm`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/chevrotain.module.min.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/chevrotain.module.min.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/README.md` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/README.md`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_decoder.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_decoder.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_decoder.wasm` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_decoder.wasm`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_encoder.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_encoder.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_wasm_wrapper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/draco_wasm_wrapper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_decoder.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_decoder.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_decoder.wasm` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_decoder.wasm`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_encoder.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_encoder.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_wasm_wrapper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/draco/gltf/draco_wasm_wrapper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/ecsy.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/ecsy.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/fflate.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/fflate.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/ktx-parse.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/ktx-parse.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/lil-gui.module.min.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/lil-gui.module.min.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/lottie_canvas.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/lottie_canvas.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/meshopt_decoder.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/meshopt_decoder.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/mikktspace.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/mikktspace.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/mmdparser.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/mmdparser.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/motion-controllers.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/motion-controllers.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/opentype.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/opentype.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/potpack.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/potpack.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.wasm` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/rhino3dm/rhino3dm.wasm`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/stats.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/stats.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/tween.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/tween.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/utif.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/utif.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/libs/zstddec.module.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/libs/zstddec.module.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lights/LightProbeGenerator.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lights/LightProbeGenerator.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lights/RectAreaLightUniformsLib.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lights/RectAreaLightUniformsLib.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/LineGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/LineGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/LineMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/LineMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/LineSegments2.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/LineSegments2.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/LineSegmentsGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/LineSegmentsGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/lines/Wireframe.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/lines/Wireframe.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/3DMLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/3DMLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/3MFLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/3MFLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/AMFLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/AMFLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/BVHLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/BVHLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/ColladaLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/ColladaLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/DDSLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/DDSLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/DRACOLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/DRACOLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/EXRLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/EXRLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/FBXLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/FBXLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/FontLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/FontLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/GCodeLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/GCodeLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/GLTFLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/GLTFLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/HDRCubeTextureLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/HDRCubeTextureLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/IESLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/IESLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/KMZLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/KMZLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/KTX2Loader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/KTX2Loader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/KTXLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/KTXLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LDrawLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LDrawLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LUT3dlLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LUT3dlLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LUTCubeLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LUTCubeLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LWOLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LWOLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LogLuvLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LogLuvLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/LottieLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/LottieLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MD2Loader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MD2Loader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MDDLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MDDLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MMDLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MMDLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MTLLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MTLLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/MaterialXLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/MaterialXLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/NRRDLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/NRRDLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/OBJLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/OBJLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PCDLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PCDLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PDBLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PDBLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PLYLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PLYLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PRWMLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PRWMLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/PVRLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/PVRLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/RGBELoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/RGBELoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/RGBMLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/RGBMLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/STLLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/STLLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/SVGLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/SVGLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TDSLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TDSLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TGALoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TGALoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TIFFLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TIFFLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TTFLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TTFLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/TiltLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/TiltLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/USDZLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/USDZLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/VOXLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/VOXLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/VRMLLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/VRMLLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/VTKLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/VTKLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/XYZLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/XYZLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/IFFParser.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/IFFParser.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/LWO2Parser.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/LWO2Parser.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/LWO3Parser.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/loaders/lwo/LWO3Parser.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/materials/MeshGouraudMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/materials/MeshGouraudMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/Capsule.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/Capsule.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/ColorConverter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/ColorConverter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/ConvexHull.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/ConvexHull.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/ImprovedNoise.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/ImprovedNoise.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/Lut.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/Lut.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/MeshSurfaceSampler.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/MeshSurfaceSampler.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/OBB.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/OBB.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/Octree.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/Octree.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/math/SimplexNoise.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/math/SimplexNoise.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/ConvexObjectBreaker.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/ConvexObjectBreaker.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/GPUComputationRenderer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/GPUComputationRenderer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/Gyroscope.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/Gyroscope.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/MD2Character.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/MD2Character.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/MD2CharacterComplex.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/MD2CharacterComplex.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/MorphAnimMesh.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/MorphAnimMesh.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/MorphBlendMesh.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/MorphBlendMesh.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/ProgressiveLightMap.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/ProgressiveLightMap.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/RollerCoaster.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/RollerCoaster.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/TubePainter.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/TubePainter.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/Volume.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/Volume.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/misc/VolumeSlice.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/misc/VolumeSlice.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/modifiers/CurveModifier.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/modifiers/CurveModifier.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/modifiers/EdgeSplitModifier.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/modifiers/EdgeSplitModifier.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/modifiers/SimplifyModifier.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/modifiers/SimplifyModifier.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/modifiers/TessellateModifier.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/modifiers/TessellateModifier.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/Nodes.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/Nodes.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/BitangentNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/BitangentNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/BufferNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/BufferNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/CameraNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/CameraNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/CubeTextureNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/CubeTextureNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ExtendedMaterialNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ExtendedMaterialNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/InstanceNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/InstanceNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/MaterialNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/MaterialNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/MaterialReferenceNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/MaterialReferenceNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ModelNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ModelNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ModelViewProjectionNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ModelViewProjectionNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/NormalNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/NormalNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/Object3DNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/Object3DNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/PositionNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/PositionNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ReferenceNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ReferenceNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ReflectVectorNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/ReflectVectorNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/SkinningNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/SkinningNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/StorageBufferNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/StorageBufferNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/TangentNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/TangentNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/TextureNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/TextureNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/UVNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/UVNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/UserDataNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/accessors/UserDataNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/CodeNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/CodeNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/ExpressionNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/ExpressionNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/FunctionCallNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/FunctionCallNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/FunctionNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/FunctionNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/ScriptableNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/ScriptableNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/code/ScriptableValueNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/code/ScriptableValueNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/AttributeNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/AttributeNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/BypassNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/BypassNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/CacheNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/CacheNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/ConstNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/ConstNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/ContextNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/ContextNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/InputNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/InputNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/Node.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/Node.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeBuilder.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeBuilder.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeFrame.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeFrame.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeKeywords.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeKeywords.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/NodeUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/PropertyNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/PropertyNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/StackNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/StackNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/TempNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/TempNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/UniformNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/UniformNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/VarNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/VarNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/VaryingNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/VaryingNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/core/constants.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/core/constants.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/BlendModeNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/BlendModeNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ColorAdjustmentNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ColorAdjustmentNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ColorSpaceNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ColorSpaceNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/NormalMapNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/NormalMapNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/PosterizeNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/PosterizeNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ToneMappingNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ToneMappingNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportSharedTextureNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportSharedTextureNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportTextureNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/display/ViewportTextureNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogExp2Node.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogExp2Node.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogRangeNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/fog/FogRangeNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_BlinnPhong.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_BlinnPhong.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_GGX.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/BRDF_GGX.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/DFGApprox.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/DFGApprox.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/D_GGX.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/D_GGX.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/F_Schlick.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/F_Schlick.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/V_GGX_SmithCorrelated.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/BSDF/V_GGX_SmithCorrelated.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/PhongLightingModel.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/PhongLightingModel.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/PhysicalLightingModel.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/PhysicalLightingModel.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/functions/material/getRoughness.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/functions/material/getRoughness.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/geometry/RangeNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/geometry/RangeNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/gpgpu/ComputeNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/gpgpu/ComputeNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/AnalyticLightNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/AnalyticLightNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/DirectionalLightNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/DirectionalLightNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/EnvironmentNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/EnvironmentNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/HemisphereLightNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/HemisphereLightNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/IESSpotLightNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/IESSpotLightNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightingContextNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightingContextNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightsNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/LightsNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/PointLightNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/PointLightNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/SpotLightNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/lighting/SpotLightNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeMaterialLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeMaterialLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeObjectLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/loaders/NodeObjectLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/LineBasicNodeMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/LineBasicNodeMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/Materials.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/Materials.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshBasicNodeMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshBasicNodeMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshNormalNodeMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshNormalNodeMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshPhongNodeMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshPhongNodeMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshPhysicalNodeMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshPhysicalNodeMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshStandardNodeMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/MeshStandardNodeMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/NodeMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/NodeMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/PointsNodeMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/PointsNodeMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materials/SpriteNodeMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materials/SpriteNodeMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/DISCLAIMER.md` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/MaterialXNodes.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/materialx/MaterialXNodes.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/math/CondNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/math/CondNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/math/MathNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/math/MathNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/math/OperatorNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/math/OperatorNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/GLSLNodeFunction.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/GLSLNodeFunction.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/WGSLNodeFunction.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/parsers/WGSLNodeFunction.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/procedural/CheckerNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/procedural/CheckerNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/shadernode/ShaderNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/shadernode/ShaderNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/ArrayElementNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/ArrayElementNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/ConvertNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/ConvertNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/DiscardNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/DiscardNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/EquirectUVNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/EquirectUVNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/JoinNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/JoinNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/MatcapUVNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/MatcapUVNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/MaxMipLevelNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/MaxMipLevelNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/OscNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/OscNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/PackingNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/PackingNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/RemapNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/RemapNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/RotateUVNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/RotateUVNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SpecularMIPLevelNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SpecularMIPLevelNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SplitNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SplitNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SpriteSheetUVNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/SpriteSheetUVNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/TimerNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/TimerNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/nodes/utils/TriplanarTexturesNode.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/nodes/utils/TriplanarTexturesNode.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/GroundProjectedSkybox.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/GroundProjectedSkybox.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Lensflare.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Lensflare.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/LightningStorm.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/LightningStorm.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/MarchingCubes.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/MarchingCubes.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Reflector.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Reflector.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/ReflectorForSSRPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/ReflectorForSSRPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Refractor.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Refractor.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/ShadowMesh.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/ShadowMesh.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Sky.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Sky.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Water.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Water.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/objects/Water2.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/objects/Water2.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/offscreen/jank.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/offscreen/jank.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/offscreen/scene.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/offscreen/scene.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/physics/AmmoPhysics.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/physics/AmmoPhysics.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/physics/RapierPhysics.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/physics/RapierPhysics.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/AdaptiveToneMappingPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/AdaptiveToneMappingPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/AfterimagePass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/AfterimagePass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/BloomPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/BloomPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/BokehPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/BokehPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/ClearPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/ClearPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/CubeTexturePass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/CubeTexturePass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/DotScreenPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/DotScreenPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/EffectComposer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/EffectComposer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/FilmPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/FilmPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/GlitchPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/GlitchPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/HalftonePass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/HalftonePass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/LUTPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/LUTPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/MaskPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/MaskPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/OutlinePass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/OutlinePass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/Pass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/Pass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/RenderPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/RenderPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/RenderPixelatedPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/RenderPixelatedPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SAOPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SAOPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SMAAPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SMAAPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSAARenderPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSAARenderPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSAOPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSAOPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSRPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SSRPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/SavePass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/SavePass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/ShaderPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/ShaderPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/TAARenderPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/TAARenderPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/TexturePass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/TexturePass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/postprocessing/UnrealBloomPass.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/postprocessing/UnrealBloomPass.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/CSS2DRenderer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/CSS2DRenderer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/CSS3DRenderer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/CSS3DRenderer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/Projector.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/Projector.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/SVGRenderer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/SVGRenderer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/WebGLNodeBuilder.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/WebGLNodeBuilder.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/WebGLNodes.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgl/nodes/WebGLNodes.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUAnimation.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUAnimation.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUAttributes.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUAttributes.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBackground.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBackground.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBindings.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBindings.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBuffer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBuffer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBufferUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUBufferUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUComputePipelines.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUComputePipelines.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUGeometries.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUGeometries.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUInfo.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUInfo.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderLists.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderLists.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderObject.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderObject.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderObjects.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderObjects.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderPipeline.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderPipeline.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderPipelines.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderPipelines.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderStates.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderStates.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPURenderer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUSampledTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUSampledTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextureRenderer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextureRenderer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextureUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextureUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextures.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUTextures.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniform.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniform.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniformsGroup.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUniformsGroup.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUWeakMap.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/WebGPUWeakMap.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/constants.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/constants.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeBuilder.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeBuilder.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeSampledTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeSampledTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeUniform.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodeUniform.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodes.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/renderers/webgpu/nodes/WebGPUNodes.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ACESFilmicToneMappingShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ACESFilmicToneMappingShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/AfterimageShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/AfterimageShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BleachBypassShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BleachBypassShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BlendShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BlendShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BokehShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BokehShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BokehShader2.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BokehShader2.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/BrightnessContrastShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/BrightnessContrastShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ColorCorrectionShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ColorCorrectionShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ColorifyShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ColorifyShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ConvolutionShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ConvolutionShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/CopyShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/CopyShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/DOFMipMapShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/DOFMipMapShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/DepthLimitedBlurShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/DepthLimitedBlurShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/DigitalGlitch.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/DigitalGlitch.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/DotScreenShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/DotScreenShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/FXAAShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/FXAAShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/FilmShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/FilmShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/FocusShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/FocusShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/FreiChenShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/FreiChenShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/GammaCorrectionShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/GammaCorrectionShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/GodRaysShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/GodRaysShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/HalftoneShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/HalftoneShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/HorizontalBlurShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/HorizontalBlurShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/HorizontalTiltShiftShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/HorizontalTiltShiftShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/HueSaturationShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/HueSaturationShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/KaleidoShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/KaleidoShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/LuminosityHighPassShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/LuminosityHighPassShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/LuminosityShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/LuminosityShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/MMDToonShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/MMDToonShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/MirrorShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/MirrorShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/NormalMapShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/NormalMapShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/RGBShiftShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/RGBShiftShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SAOShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SAOShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SMAAShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SMAAShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SSAOShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SSAOShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SSRShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SSRShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SepiaShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SepiaShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SobelOperatorShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SobelOperatorShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/SubsurfaceScatteringShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/SubsurfaceScatteringShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/TechnicolorShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/TechnicolorShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ToneMapShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ToneMapShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/ToonShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/ToonShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/TriangleBlurShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/TriangleBlurShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/UnpackDepthRGBAShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/UnpackDepthRGBAShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VelocityShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VelocityShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VerticalBlurShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VerticalBlurShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VerticalTiltShiftShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VerticalTiltShiftShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VignetteShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VignetteShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/VolumeShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/VolumeShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/shaders/WaterRefractionShader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/shaders/WaterRefractionShader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/textures/FlakesTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/textures/FlakesTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/BufferGeometryUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/BufferGeometryUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/CameraUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/CameraUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/GPUStatsPanel.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/GPUStatsPanel.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/GeometryCompressionUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/GeometryCompressionUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/GeometryUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/GeometryUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/LDrawUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/LDrawUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/PackedPhongMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/PackedPhongMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/SceneUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/SceneUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/ShadowMapViewer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/ShadowMapViewer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/SkeletonUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/SkeletonUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/UVsDebug.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/UVsDebug.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/utils/WorkerPool.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/utils/WorkerPool.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/ARButton.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/ARButton.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/OculusHandModel.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/OculusHandModel.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/OculusHandPointerModel.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/OculusHandPointerModel.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/Text2D.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/Text2D.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/VRButton.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/VRButton.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRButton.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRButton.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRControllerModelFactory.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRControllerModelFactory.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XREstimatedLight.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XREstimatedLight.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandMeshModel.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandMeshModel.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandModelFactory.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandModelFactory.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandPrimitiveModel.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/examples/jsm/webxr/XRHandPrimitiveModel.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/package.json` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/package.json`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/Three.Legacy.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/Three.Legacy.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/Three.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/Three.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationAction.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationAction.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationClip.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationClip.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationMixer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationMixer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationObjectGroup.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationObjectGroup.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/AnimationUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/AnimationUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/KeyframeTrack.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/KeyframeTrack.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/PropertyBinding.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/PropertyBinding.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/PropertyMixer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/PropertyMixer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/tracks/BooleanKeyframeTrack.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/tracks/BooleanKeyframeTrack.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/tracks/QuaternionKeyframeTrack.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/tracks/QuaternionKeyframeTrack.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/animation/tracks/StringKeyframeTrack.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/animation/tracks/StringKeyframeTrack.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/audio/Audio.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/audio/Audio.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/audio/AudioAnalyser.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/audio/AudioAnalyser.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/audio/AudioListener.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/audio/AudioListener.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/audio/PositionalAudio.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/audio/PositionalAudio.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/Camera.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/Camera.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/CubeCamera.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/CubeCamera.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/OrthographicCamera.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/OrthographicCamera.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/PerspectiveCamera.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/PerspectiveCamera.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/cameras/StereoCamera.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/cameras/StereoCamera.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/constants.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/constants.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/BufferAttribute.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/BufferAttribute.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/BufferGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/BufferGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/Clock.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/Clock.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/EventDispatcher.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/EventDispatcher.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/GLBufferAttribute.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/GLBufferAttribute.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InstancedBufferAttribute.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InstancedBufferAttribute.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InstancedBufferGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InstancedBufferGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InstancedInterleavedBuffer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InstancedInterleavedBuffer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InterleavedBuffer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InterleavedBuffer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/InterleavedBufferAttribute.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/InterleavedBufferAttribute.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/Layers.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/Layers.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/Object3D.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/Object3D.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/Raycaster.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/Raycaster.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/core/UniformsGroup.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/core/UniformsGroup.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/DataUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/DataUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/Earcut.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/Earcut.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/ImageUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/ImageUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/PMREMGenerator.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/PMREMGenerator.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/ShapeUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/ShapeUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/Curve.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/Curve.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/CurvePath.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/CurvePath.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/Interpolations.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/Interpolations.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/Path.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/Path.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/Shape.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/Shape.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/core/ShapePath.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/core/ShapePath.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/CatmullRomCurve3.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/CatmullRomCurve3.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/CubicBezierCurve.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/CubicBezierCurve.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/CubicBezierCurve3.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/CubicBezierCurve3.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/Curves.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/Curves.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/EllipseCurve.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/EllipseCurve.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/LineCurve.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/LineCurve.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/LineCurve3.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/LineCurve3.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/QuadraticBezierCurve.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/QuadraticBezierCurve.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/QuadraticBezierCurve3.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/QuadraticBezierCurve3.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/extras/curves/SplineCurve.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/extras/curves/SplineCurve.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/BoxGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/BoxGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/CapsuleGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/CapsuleGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/CircleGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/CircleGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/ConeGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/ConeGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/CylinderGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/CylinderGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/DodecahedronGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/DodecahedronGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/EdgesGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/EdgesGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/ExtrudeGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/ExtrudeGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/Geometries.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/Geometries.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/IcosahedronGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/IcosahedronGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/LatheGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/LatheGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/OctahedronGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/OctahedronGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/PlaneGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/PlaneGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/PolyhedronGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/PolyhedronGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/RingGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/RingGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/ShapeGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/ShapeGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/SphereGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/SphereGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/TetrahedronGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/TetrahedronGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/TorusGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/TorusGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/TorusKnotGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/TorusKnotGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/TubeGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/TubeGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/geometries/WireframeGeometry.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/geometries/WireframeGeometry.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/ArrowHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/ArrowHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/AxesHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/AxesHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/Box3Helper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/Box3Helper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/BoxHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/BoxHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/CameraHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/CameraHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/DirectionalLightHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/DirectionalLightHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/GridHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/GridHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/HemisphereLightHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/HemisphereLightHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/PlaneHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/PlaneHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/PointLightHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/PointLightHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/PolarGridHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/PolarGridHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/SkeletonHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/SkeletonHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/helpers/SpotLightHelper.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/helpers/SpotLightHelper.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/AmbientLightProbe.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/AmbientLightProbe.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/DirectionalLight.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/DirectionalLight.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/HemisphereLight.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/HemisphereLight.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/HemisphereLightProbe.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/HemisphereLightProbe.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/Light.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/Light.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/LightProbe.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/LightProbe.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/LightShadow.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/LightShadow.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/PointLight.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/PointLight.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/PointLightShadow.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/PointLightShadow.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/RectAreaLight.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/RectAreaLight.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/SpotLight.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/SpotLight.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/lights/SpotLightShadow.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/lights/SpotLightShadow.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/AnimationLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/AnimationLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/AudioLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/AudioLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/BufferGeometryLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/BufferGeometryLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/CompressedTextureLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/CompressedTextureLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/CubeTextureLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/CubeTextureLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/DataTextureLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/DataTextureLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/FileLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/FileLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/ImageBitmapLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/ImageBitmapLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/ImageLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/ImageLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/Loader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/Loader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/LoaderUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/LoaderUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/LoadingManager.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/LoadingManager.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/MaterialLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/MaterialLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/ObjectLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/ObjectLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/loaders/TextureLoader.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/loaders/TextureLoader.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/LineBasicMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/LineBasicMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/LineDashedMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/LineDashedMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/Material.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/Material.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/Materials.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/Materials.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshBasicMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshBasicMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshDepthMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshDepthMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshDistanceMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshDistanceMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshLambertMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshLambertMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshMatcapMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshMatcapMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshNormalMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshNormalMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshPhongMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshPhongMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshPhysicalMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshPhysicalMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshStandardMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshStandardMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/MeshToonMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/MeshToonMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/PointsMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/PointsMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/ShaderMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/ShaderMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/ShadowMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/ShadowMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/materials/SpriteMaterial.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/materials/SpriteMaterial.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Box2.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Box2.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Box3.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Box3.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Color.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Color.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/ColorManagement.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/ColorManagement.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Cylindrical.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Cylindrical.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Euler.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Euler.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Frustum.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Frustum.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Interpolant.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Interpolant.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Line3.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Line3.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/MathUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/MathUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Matrix3.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Matrix3.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Matrix4.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Matrix4.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Plane.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Plane.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Quaternion.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Quaternion.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Ray.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Ray.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Sphere.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Sphere.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Spherical.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Spherical.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/SphericalHarmonics3.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/SphericalHarmonics3.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Triangle.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Triangle.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Vector2.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Vector2.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Vector3.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Vector3.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/Vector4.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/Vector4.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/interpolants/CubicInterpolant.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/interpolants/CubicInterpolant.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/interpolants/LinearInterpolant.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/interpolants/LinearInterpolant.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/math/interpolants/QuaternionLinearInterpolant.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/math/interpolants/QuaternionLinearInterpolant.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/InstancedMesh.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/InstancedMesh.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/LOD.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/LOD.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Line.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Line.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/LineSegments.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/LineSegments.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Mesh.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Mesh.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Points.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Points.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Skeleton.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Skeleton.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/SkinnedMesh.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/SkinnedMesh.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/objects/Sprite.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/objects/Sprite.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGLCubeRenderTarget.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGLCubeRenderTarget.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGLMultipleRenderTargets.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGLMultipleRenderTargets.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGLRenderTarget.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGLRenderTarget.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/WebGLRenderer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/WebGLRenderer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/aomap_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/aomap_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/bsdfs.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/bsdfs.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/bumpmap_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/bumpmap_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/clipping_planes_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/common.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/common.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/cube_uv_reflection_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/cube_uv_reflection_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/defaultnormal_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/defaultnormal_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/dithering_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/dithering_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_physical_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_physical_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/envmap_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/gradientmap_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/gradientmap_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/iridescence_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/iridescence_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_begin.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_begin.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_maps.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_fragment_maps.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_lambert_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_lambert_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_pars_begin.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_pars_begin.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_phong_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_phong_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_physical_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_physical_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_physical_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_physical_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_toon_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/lights_toon_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphcolor_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphcolor_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphnormal_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphnormal_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphtarget_pars_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphtarget_pars_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphtarget_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/morphtarget_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_fragment_begin.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_fragment_begin.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_fragment_maps.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normal_fragment_maps.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normalmap_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/normalmap_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/packing.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/packing.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_pars_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_pars_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmap_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmask_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/shadowmask_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinning_pars_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/skinning_pars_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/tonemapping_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/tonemapping_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/transmission_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/transmission_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/transmission_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/transmission_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_pars_fragment.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_pars_fragment.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_pars_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_pars_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_vertex.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk/uv_vertex.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderChunk.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/backgroundCube.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/backgroundCube.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/cube.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/cube.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/depth.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/depth.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/distanceRGBA.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/distanceRGBA.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/equirect.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/equirect.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/linedashed.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/linedashed.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshbasic.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshbasic.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshlambert.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshlambert.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshmatcap.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshmatcap.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshnormal.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshnormal.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshphong.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshphong.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshphysical.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshphysical.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshtoon.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/meshtoon.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/points.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/points.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/shadow.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/shadow.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/sprite.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/sprite.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/vsm.glsl.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib/vsm.glsl.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/ShaderLib.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/UniformsLib.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/UniformsLib.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/shaders/UniformsUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/shaders/UniformsUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLAnimation.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLAnimation.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLAttributes.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLAttributes.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBackground.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBackground.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBindingStates.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBindingStates.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBufferRenderer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLBufferRenderer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCapabilities.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCapabilities.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLClipping.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLClipping.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCubeMaps.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCubeMaps.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCubeUVMaps.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLCubeUVMaps.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLExtensions.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLExtensions.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLGeometries.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLGeometries.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLIndexedBufferRenderer.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLIndexedBufferRenderer.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLInfo.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLInfo.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLLights.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLLights.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLMaterials.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLMaterials.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLMorphtargets.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLMorphtargets.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLObjects.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLObjects.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLProgram.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLProgram.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLPrograms.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLPrograms.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLProperties.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLProperties.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLRenderLists.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLRenderLists.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLRenderStates.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLRenderStates.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShaderCache.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShaderCache.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShadowMap.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLShadowMap.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLState.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLState.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLTextures.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLTextures.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUniforms.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUniforms.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUniformsGroups.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUniformsGroups.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUtils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webgl/WebGLUtils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webxr/WebXRController.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webxr/WebXRController.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/renderers/webxr/WebXRManager.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/renderers/webxr/WebXRManager.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/scenes/Scene.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/scenes/Scene.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/CompressedTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/CompressedTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/CubeTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/CubeTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/Data3DTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/Data3DTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/DataArrayTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/DataArrayTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/DataTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/DataTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/DepthTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/DepthTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/Source.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/Source.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/Texture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/Texture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/textures/VideoTexture.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/textures/VideoTexture.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/static/node_modules/three/src/utils.js` & `zndraw-0.2.0a1/zndraw/static/node_modules/three/src/utils.js`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/zndraw/templates/index.html` & `zndraw-0.2.0a1/zndraw/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 <!DOCTYPE html>
-<html>
+<html lang="en">
 
-
-<head lang="en">
+<head>
   <meta charset="utf-8">
   <title>ZnDraw</title>
   <link rel="icon" type="image/x-icon" href="{{ url_for('static', filename='favion-192x192.png') }}">
-  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet"
-    integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
-  <link rel="stylesheet" href="{{ url_for('static', filename='main.css') }}">
-  <script async src="https://unpkg.com/es-module-shims@1.6.3/dist/es-module-shims.js"></script>
   <script type="importmap">
-  {
-    "imports": {
-      "three": "https://unpkg.com/three@0.151.3/build/three.module.js",
-      "three/addons/": "https://unpkg.com/three@0.151.3/examples/jsm/",
-      "./modules/": "{{ url_for('static', filename='/modules/') }}"
-    }
-  }
-</script>
-  <script src="https://cdnjs.cloudflare.com/ajax/libs/plotly.js/2.21.0/plotly.min.js"
-    integrity="sha512-oalOW03buJpcBKtaooDOM2XrfQXI4ifCNBaFgYfY6UCQBGCFPsiwsrQVdAnENOJwjwEwLiVAgy3Ljyt7cN2LJw=="
-    crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+      {
+        "imports": {
+          "three": "{{ url_for('static', filename='/node_modules/three/build/three.module.js') }}",
+          "three/": "{{ url_for('static', filename='/node_modules/three/') }}"
+        }
+      }
+    </script>
+  <link rel="stylesheet" href="{{ url_for('static', filename='main.css') }}">
+  <!-- Bootstrap -->
+  <link rel="stylesheet" href="{{ url_for('static', filename='node_modules/bootstrap/dist/css/bootstrap.min.css') }}">
 </head>
 
 <body>
+  <script src="{{ url_for('static', filename='node_modules/bootstrap/dist/js/bootstrap.min.js') }}"></script>
   <script type="module" src="{{ url_for('static', filename='main.js') }}"></script>
 
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
-    integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe"
-    crossorigin="anonymous"></script>
+  <div id="scene-container"></div>
 
   <!-- Loading Spinner -->
   <div class="atom-spinner" , id="atom-spinner">
     <div class="spinner-inner">
       <div class="spinner-line"></div>
       <div class="spinner-line"></div>
       <div class="spinner-line"></div>
@@ -64,15 +57,16 @@
             <button class="btn btn-outline-secondary" type="button" data-bs-toggle="offcanvas"
               data-bs-target="#particleCanvas" aria-controls="particleCanvas" onclick="document.activeElement.blur();">
               Particles
             </button>
           </li>
           <li class="nav-item mx-1">
             <button class="btn btn-outline-secondary" type="button" data-bs-toggle="offcanvas"
-              data-bs-target="#interactionCanvas" aria-controls="interactionCanvas" onclick="document.activeElement.blur();">
+              data-bs-target="#interactionCanvas" aria-controls="interactionCanvas"
+              onclick="document.activeElement.blur();">
               Interaction
             </button>
           </li>
           <li class="nav-item mx-1">
             <button class="btn btn-outline-secondary" type="button" data-bs-toggle="offcanvas"
               data-bs-target="#sceneCanvas" aria-controls="sceneCanvas" onclick="document.activeElement.blur();">
               Scene
@@ -132,15 +126,15 @@
           }}</label>
         <input type="range" class="form-range" id="sphereRadius" min="0.1" max="4" step="0.1"
           value="{{ config['sphere_size'] }}">
       </div>
       <div class="mb-3">
         <label for="bondDiameter" class="form-label" id="bondDiameterLabel">Bond diameter: {{ config['bond_size']
           }}</label>
-        <input type="range" class="form-range" id="bondDiameter" min="0.1" max="2.0" step="0.1"
+        <input type="range" class="form-range" id="bondDiameter" min="0" max="2.0" step="0.1"
           value="{{ config['bond_size'] }}">
       </div>
       <div class="mb-3">
         <label for="resolution" class="form-label" id="resolutionLabel">Resolution: {{ config['resolution'] }}</label>
         <input type="range" class="form-range" id="resolution" min="1" max="20" step="1"
           value="{{ config['resolution'] }}">
       </div>
@@ -373,16 +367,15 @@
         <div class="modal-header">
           <h5 class="modal-title">Add Analysis</h5>
           <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
         </div>
         <div class="modal-body">
           <div class="mb-3">
             <label for="addAnalysisImport" class="form-label">Path to modifier <code>class</code></label>
-            <input type="email" class="form-control" id="addAnalysisImport"
-              aria-describedby="addAnalysisImportHelp">
+            <input type="email" class="form-control" id="addAnalysisImport" aria-describedby="addAnalysisImportHelp">
             <div id="addAnalysisImportHelp" class="form-text">The input should be <code>module.cls</code> such
               that
               <code> from module import cls</code> works.
             </div>
           </div>
         </div>
         <div class="modal-footer">
@@ -392,11 +385,10 @@
       </div>
     </div>
   </div>
 
   <!-- Progress Bar -->
   <div id="info"></div>
   <input id="frame-slider" class="frame-slider" type="range" value="0" min="0" max="100">
-
 </body>
 
-</html>
+</html>
```

### Comparing `zndraw-0.1.8/zndraw/tools/select.py` & `zndraw-0.2.0a1/zndraw/tools/select.py`

 * *Files identical despite different names*

### Comparing `zndraw-0.1.8/PKG-INFO` & `zndraw-0.2.0a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zndraw
-Version: 0.1.8
+Version: 0.2.0a1
 Summary: 
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -25,58 +25,71 @@
 Project-URL: repository, https://github.com/zincware/ZnDraw
 Description-Content-Type: text/markdown
 
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 [![PyPI version](https://badge.fury.io/py/zndraw.svg)](https://badge.fury.io/py/zndraw)
 !['Threejs](https://img.shields.io/badge/threejs-black?style=for-the-badge&logo=three.js&logoColor=white)
 
-
 # ZnDraw
 
-Install via ``pip install zndraw`` or ``pip install zndraw[webview]`` to open zndraw in a dedicated window.
+Install via `pip install zndraw` or `pip install zndraw[webview]` to open zndraw
+in a dedicated window.
 
 ## CLI
 
-You can use ZnDraw with the CLI ``zndraw atoms.xyz``.
-For a full list of arguments use `zndraw --help`.
+You can use ZnDraw with the CLI `zndraw atoms.xyz`. For a full list of arguments
+use `zndraw --help`.
 
-ZnDraw is designed to work with your Python scripts.
-To interface you can inherit from `zndraw.examples.UpdateScene` or follow this base class:
+ZnDraw is designed to work with your Python scripts. To interface you can
+inherit from `zndraw.examples.UpdateScene` or follow this base class:
 
 ```python
 import abc
 from pydantic import BaseModel
 
 class UpdateScene(BaseModel, abc.ABC):
     @abc.abstractmethod
     def run(self, atom_ids: list[int], atoms: ase.Atoms, **kwargs) -> list[ase.Atoms]:
         pass
 ```
 
-The ``run`` method expects as inputs
-- atom_ids: list[int], the ids of the currently selected atoms
-- atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where selected.
+The `run` method expects as inputs
+
+- atom_ids: list\[int\], the ids of the currently selected atoms
+- atoms: ase.Atoms, the configuration as `ase.Atoms` file where atom_ids where
+  selected.
 - kwargs: dict could be additional information from the scene
 
 and as an output:
-- list[ase.Atoms], a list of ase Atoms objects to display.
 
+- list\[ase.Atoms\], a list of ase Atoms objects to display.
 
-You can define the parameters using `pydantic.Field` which will be displayed in the UI.
+You can define the parameters using `pydantic.Field` which will be displayed in
+the UI.
 
 ```python
 class MyUpdateCls(UpdateScene):
     steps: int = Field(100, le=1000, ge=1)
     x: float = Field(0.5, le=5, ge=0)
     symbol: str = Field("same")
 ```
 
-To add your method click on the `+` on the right side of the window.
-Your should be able to add your method from the working directory via `module.MyUpdateCls` as long
-as it can be imported via `from module import MyUpdateCls`.
+To add your method click on the `+` on the right side of the window. Your should
+be able to add your method from the working directory via `module.MyUpdateCls`
+as long as it can be imported via `from module import MyUpdateCls`.
 
 ![ZnDraw UI](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_ui.png "ZnDraw UI")
 
 ![ZnDraw UI2](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_protein.png "ZnDraw UI2")
 
 ![ZnDraw UI3](https://raw.githubusercontent.com/zincware/ZnDraw/main/misc/zndraw_draw.png "ZnDraw UI3")
 
+# Development
+
+ZnDraw is developed using https://python-poetry.org/. Furthermore, the
+javascript packages have to be installed using https://www.npmjs.com/.
+
+```bash
+cd zndraw/static/
+npm install
+```
+
```

