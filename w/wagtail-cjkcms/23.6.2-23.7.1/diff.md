# Comparing `tmp/wagtail-cjkcms-23.6.2.tar.gz` & `tmp/wagtail-cjkcms-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cjkcms-23.6.2.tar", last modified: Mon Jun  5 13:56:33 2023, max compression
+gzip compressed data, was "wagtail-cjkcms-23.7.1.tar", last modified: Sun Jul  2 19:17:52 2023, max compression
```

## Comparing `wagtail-cjkcms-23.6.2.tar` & `wagtail-cjkcms-23.7.1.tar`

### file list

```diff
@@ -1,267 +1,272 @@
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/
--rw-r--r--   0 grze      (1000) grze      (1000)     7412 2023-06-05 13:55:53.000000 wagtail-cjkcms-23.6.2/CHANGELOG.md
--rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/LICENSE
--rw-r--r--   0 grze      (1000) grze      (1000)      239 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/MANIFEST.in
--rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     1688 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/
--rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-06-05 13:54:14.000000 wagtail-cjkcms-23.6.2/cjkcms/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/api/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/api/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/api/mailchimp.py
--rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/apps.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/bin/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/bin/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/bin/cjkcms.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     3166 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)    10455 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/base_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     8476 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/content_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9251 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/html_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/layout_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/blocks/searchable_html_block.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/draftail/
--rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/draftail/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/draftail/draftail_extensions.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/draftail/draftail_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/fields.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.202377 wagtail-cjkcms-23.6.2/cjkcms/finders/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/finders/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/finders/oembed.py
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/forms.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/image_formats.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.182377 wagtail-cjkcms-23.6.2/cjkcms/management/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/management/commands/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/clear-embeds.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/import-csv.py
--rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-collections.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-navbar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-website.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
--rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1334 2023-05-31 15:55:06.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
--rw-r--r--   0 grze      (1000) grze      (1000)      685 2023-06-04 21:40:37.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/0009_navbar_language.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/migrations/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/models/
--rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-05-31 15:50:31.000000 wagtail-cjkcms-23.6.2/cjkcms/models/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      335 2023-05-31 16:04:59.000000 wagtail-cjkcms-23.6.2/cjkcms/models/admin_sidebar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/models/cms_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/models/integration_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    19637 2023-05-31 15:57:04.000000 wagtail-cjkcms-23.6.2/cjkcms/models/page_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    13532 2023-06-05 10:56:37.000000 wagtail-cjkcms-23.6.2/cjkcms/models/snippet_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    18513 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/models/wagtailsettings_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/search_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9500 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/settings.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.192377 wagtail-cjkcms-23.6.2/cjkcms/static/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.192377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/
--rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css
--rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json
--rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.212377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/
--rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
--rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/
--rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-admin.css
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-06-04 21:08:12.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-editor.css
--rw-r--r--   0 grze      (1000) grze      (1000)     4375 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-front.css
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.192377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/avatars/
--rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/avatars/default.png
--rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/avatars/default.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/icons/quote.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/
--rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
--rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/
--rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/js/
--rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/js/cjkcms-editor.js
--rw-r--r--   0 grze      (1000) grze      (1000)     5780 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/js/cjkcms-front.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/cookieconsent.css
--rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/cookieconsent.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/templates/
--rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/404.html
--rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/500.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.222377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/accordion_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/article_block_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/base_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/base_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/button_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_blurb.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_head.html
--rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_img.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_landing1.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_landing2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/carousel_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/column_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/document_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/download_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/embed_video_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/external_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/grid_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/h1_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/h2_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/h3_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/hero_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/modal_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/page_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
--rw-r--r--   0 grze      (1000) grze      (1000)      397 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
--rw-r--r--   0 grze      (1000) grze      (1000)      300 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1065 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_form.html
--rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pricelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
--rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/rich_text_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/table_block.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/cookieconsent/languages.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/
--rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/date.html
--rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/datetime.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/
--rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/time.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/align-left.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/check-square-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/columns.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/desktop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/font.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/google.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/hashtag.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/header.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/list-alt.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/map.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/newspaper-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/recycle.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/stop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/th-large.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/universal-access.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/usd.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/window-maximize.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/window-minimize.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/classifier_nav.html
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/codered_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/form_honeypot.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/pagination.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.242377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/stream_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/
--rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_index_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1705 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_page.search.html
--rw-r--r--   0 grze      (1000) grze      (1000)     7931 2023-06-05 10:34:33.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/base.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/form_page_landing.html
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/home_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/search_result.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2462 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/stream_form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      838 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/web_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      623 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/web_page_notitle.html
--rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/robots.txt
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1943 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/footer.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2712 2023-06-05 10:52:40.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar_search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/tracking_g3.html
--rw-r--r--   0 grze      (1000) grze      (1000)      831 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/widgets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1384 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.192377 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      839 2023-06-04 21:09:36.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/struct.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/shared/
--rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.252377 wagtail-cjkcms-23.6.2/cjkcms/templatetags/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/auth_extras.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6785 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/cjkcms_tags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/friendly_loader.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/templatetags/txtutils_tags.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/cjkcms/tests/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4226 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_articlepages.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4639 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_search_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_settings.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3511 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_templatetags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/tests/test_webpage.py
--rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/utils.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/views.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6557 2023-05-31 16:27:47.000000 wagtail-cjkcms-23.6.2/cjkcms/wagtail_hooks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/cjkcms/widgets.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/docs/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/docs/how-to/
--rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/how-to/oembed_finder.md
--rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/installation.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/docs/management_commands/
--rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/management_commands/clear-embeds.md
--rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/management_commands/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/management_commands/init-collections.md
--rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/quick-start.md
--rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/requirements.txt
--rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/docs/why-another-cms.md
--rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/pyproject.toml
--rw-r--r--   0 grze      (1000) grze      (1000)     1555 2023-06-05 13:56:33.282377 wagtail-cjkcms-23.6.2/setup.cfg
--rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.6.2/setup.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-06-05 13:56:33.262377 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/
--rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     9533 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/SOURCES.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/dependency_links.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/entry_points.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       79 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/requires.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-06-05 13:56:33.000000 wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/top_level.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/
+-rw-r--r--   0 grze      (1000) grze      (1000)     7683 2023-07-02 11:52:15.000000 wagtail-cjkcms-23.7.1/CHANGELOG.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/LICENSE
+-rw-r--r--   0 grze      (1000) grze      (1000)      239 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/MANIFEST.in
+-rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     1688 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-07-02 17:54:21.000000 wagtail-cjkcms-23.7.1/cjkcms/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/api/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/api/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/api/mailchimp.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/apps.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/bin/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/bin/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/bin/cjkcms.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3223 2023-07-02 10:36:27.000000 wagtail-cjkcms-23.7.1/cjkcms/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    10539 2023-07-02 10:10:41.000000 wagtail-cjkcms-23.7.1/cjkcms/blocks/base_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     8757 2023-07-02 10:38:05.000000 wagtail-cjkcms-23.7.1/cjkcms/blocks/content_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9537 2023-07-02 19:16:58.000000 wagtail-cjkcms-23.7.1/cjkcms/blocks/html_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/blocks/layout_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/blocks/searchable_html_block.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/draftail/
+-rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/draftail/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/draftail/draftail_extensions.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/draftail/draftail_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/fields.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/finders/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/finders/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/finders/oembed.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/forms.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/image_formats.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.026487 wagtail-cjkcms-23.7.1/cjkcms/management/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/management/commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/management/commands/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/management/commands/clear-embeds.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/management/commands/import-csv.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/management/commands/init-collections.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/management/commands/init-navbar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/management/commands/init-website.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1334 2023-05-31 15:55:06.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      685 2023-06-04 21:40:37.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0009_navbar_language.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3479 2023-07-02 11:44:17.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0010_filmstrip_filmpanel.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1393 2023-07-02 17:30:25.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-05-31 15:50:31.000000 wagtail-cjkcms-23.7.1/cjkcms/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      335 2023-05-31 16:04:59.000000 wagtail-cjkcms-23.7.1/cjkcms/models/admin_sidebar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/models/cms_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/models/integration_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    23735 2023-07-02 18:11:25.000000 wagtail-cjkcms-23.7.1/cjkcms/models/page_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    15369 2023-07-02 11:08:25.000000 wagtail-cjkcms-23.7.1/cjkcms/models/snippet_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    18513 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/models/wagtailsettings_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/search_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9541 2023-07-02 17:18:42.000000 wagtail-cjkcms-23.7.1/cjkcms/settings.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.026487 wagtail-cjkcms-23.7.1/cjkcms/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.026487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/
+-rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json
+-rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/fonts/
+-rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
+-rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/css/cjkcms-admin.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-06-04 21:08:12.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/css/cjkcms-editor.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     4614 2023-07-02 11:08:20.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/css/cjkcms-front.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.026487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/avatars/
+-rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/avatars/default.png
+-rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/avatars/default.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/icons/quote.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/logos/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/patterns/
+-rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/js/cjkcms-editor.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     5565 2023-07-02 11:07:19.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/js/cjkcms-front.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/static/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cookieconsent/cookieconsent.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/static/cookieconsent/cookieconsent.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/templates/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/404.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/500.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/accordion_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/article_block_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/base_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/base_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/button_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_blurb.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_head.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_img.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_landing1.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_landing2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/carousel_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/column_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/document_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/download_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/embed_video_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/external_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1484 2023-07-02 12:08:07.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/film_strip_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/grid_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/h1_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/h2_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/h3_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/hero_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/image_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/image_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/modal_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/page_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      823 2023-07-02 18:57:37.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-02 17:20:14.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1065 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pricelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/quote_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/rich_text_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/table_block.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/cookieconsent/languages.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/
+-rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/date.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/datetime.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.046487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/mailchimp/
+-rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/time.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/align-left.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/check-square-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/columns.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/desktop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/font.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/google.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/hashtag.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/header.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/list-alt.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/map.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/newspaper-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/recycle.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/stop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/th-large.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/universal-access.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/usd.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/window-maximize.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/window-minimize.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/classifier_nav.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/codered_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/form_honeypot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/pagination.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/stream_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/article_index_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2031 2023-07-02 17:41:05.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/article_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/article_page.search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     8658 2023-07-02 18:34:26.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/base.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/form_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-07-02 17:27:50.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/form_page.mini.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/form_page_landing.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/home_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      491 2023-07-02 12:27:06.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/page.mini.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/search_result.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2462 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/stream_form_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-07-02 17:46:00.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/web_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-02 17:29:59.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/robots.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1943 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/footer.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2712 2023-06-05 10:52:40.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/navbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/navbar_search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/tracking_g3.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      832 2023-07-02 11:03:38.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/widgets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1444 2023-07-02 10:12:54.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.036487 wagtail-cjkcms-23.7.1/cjkcms/templates/wagtailadmin/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/templates/wagtailadmin/block_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      839 2023-06-04 21:09:36.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/wagtailadmin/block_forms/struct.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/templates/wagtailadmin/shared/
+-rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/templatetags/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templatetags/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templatetags/auth_extras.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6785 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templatetags/cjkcms_tags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templatetags/friendly_loader.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templatetags/gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/templatetags/txtutils_tags.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/cjkcms/tests/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/tests/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4226 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/tests/test_articlepages.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/tests/test_gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4639 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/tests/test_search_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/tests/test_settings.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3511 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/tests/test_templatetags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/tests/test_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/tests/test_webpage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/utils.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/views.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6557 2023-05-31 16:27:47.000000 wagtail-cjkcms-23.7.1/cjkcms/wagtail_hooks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/cjkcms/widgets.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/docs/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/docs/how-to/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/docs/how-to/oembed_finder.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/docs/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/docs/installation.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/docs/management_commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/docs/management_commands/clear-embeds.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/docs/management_commands/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/docs/management_commands/init-collections.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/docs/quick-start.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/docs/requirements.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/docs/why-another-cms.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/pyproject.toml
+-rw-r--r--   0 grze      (1000) grze      (1000)     1555 2023-07-02 19:17:52.066487 wagtail-cjkcms-23.7.1/setup.cfg
+-rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.1/setup.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-02 19:17:52.056487 wagtail-cjkcms-23.7.1/wagtail_cjkcms.egg-info/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-07-02 19:17:51.000000 wagtail-cjkcms-23.7.1/wagtail_cjkcms.egg-info/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     9797 2023-07-02 19:17:52.000000 wagtail-cjkcms-23.7.1/wagtail_cjkcms.egg-info/SOURCES.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-07-02 19:17:51.000000 wagtail-cjkcms-23.7.1/wagtail_cjkcms.egg-info/dependency_links.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-07-02 19:17:51.000000 wagtail-cjkcms-23.7.1/wagtail_cjkcms.egg-info/entry_points.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       79 2023-07-02 19:17:51.000000 wagtail-cjkcms-23.7.1/wagtail_cjkcms.egg-info/requires.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-07-02 19:17:51.000000 wagtail-cjkcms-23.7.1/wagtail_cjkcms.egg-info/top_level.txt
```

### Comparing `wagtail-cjkcms-23.6.2/CHANGELOG.md` & `wagtail-cjkcms-23.7.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -182,7 +182,14 @@
 - Basic compatibility with Wagtail 5.0
 - Due to wagtail-seo and wagtail-cache not being compatible with Wagtail 5.0, they were replaced with forked versions downloadable from github. This is a temporary solution until the original packages are updated.
 
 # 23.6.2 (2023-06-05)
 - Added new project template with webpack support (untested as of yet)
 - Modified the navbar model to support multilingual websites: new column "language" allows setting navbar
 visibility to all languages or just one selected.
+
+# 23.7.1 (2023-07-02)
+- Split requirements into prod and dev
+- Classifier bug fixes copied from codered #51d8838
+- Implemented filmstrip block as per codered #849f1f4
+- Implemented related pages feature as per codered #a130c53;
+- Added ButtonLink title in collapsed view
```

### Comparing `wagtail-cjkcms-23.6.2/LICENSE` & `wagtail-cjkcms-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/PKG-INFO` & `wagtail-cjkcms-23.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.6.2
+Version: 23.7.1
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.x site. Based on Codered CRX.
 Home-page: https://github.com/cjkpl/wagtail-cjkcms
 Author: Grzegorz Krol
 Author-email: gk@cjk.pl
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail-cjkcms-23.6.2/README.md` & `wagtail-cjkcms-23.7.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/api/mailchimp.py` & `wagtail-cjkcms-23.7.1/cjkcms/api/mailchimp.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/bin/cjkcms.py` & `wagtail-cjkcms-23.7.1/cjkcms/bin/cjkcms.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/blocks/__init__.py` & `wagtail-cjkcms-23.7.1/cjkcms/blocks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     TableBlock,
     SearchableHTMLBlock,
 )
 from .content_blocks import (  # noqa
     AccordionBlock,
     CardBlock,
     CarouselBlock,
+    FilmStripBlock,
     ImageGalleryBlock,
     ModalBlock,
     NavDocumentLinkWithSubLinkBlock,
     NavExternalLinkWithSubLinkBlock,
     NavPageLinkWithSubLinkBlock,
     PriceListBlock,
     ReusableContentBlock,
@@ -63,14 +64,15 @@
     ("page_preview", PagePreviewBlock()),
 ]
 
 CONTENT_STREAMBLOCKS = HTML_STREAMBLOCKS + [
     ("accordion", AccordionBlock()),
     ("card", CardBlock()),
     ("carousel", CarouselBlock()),
+    ("filmstrip", FilmStripBlock()),
     ("image_gallery", ImageGalleryBlock()),
     ("modal", ModalBlock(HTML_STREAMBLOCKS)),
     ("pricelist", PriceListBlock()),
     ("reusable_content", ReusableContentBlock()),
 ]
 
 NAVIGATION_STREAMBLOCKS = [
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/blocks/base_blocks.py` & `wagtail-cjkcms-23.7.1/cjkcms/blocks/base_blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         )
 
     def to_python(self, value):
         """
         Convert the serialized value back into a python object.
         """
         if isinstance(value, int):
-            return self.target_model.objects.get(pk=value)  # type: ignore
+            try:
+                return self.target_model.objects.get(pk=value)
+            except self.target_model.DoesNotExist:
+                return None
         return value
 
     def get_prep_value(self, value):
         """
         Serialize the model in a form suitable for wagtail's JSON-ish streamfield
         """
         return value.pk if isinstance(value, self.target_model) else value
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/blocks/content_blocks.py` & `wagtail-cjkcms-23.7.1/cjkcms/blocks/content_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,27 @@
     class Meta:
         icon = "image"
         label = _("Carousel")
         label_format = _("Carousel")
         template = "cjkcms/blocks/carousel_block.html"
 
 
+class FilmStripBlock(BaseBlock):
+    """
+    Enables choosing a Film Strip Snippet.
+    """
+
+    film_strip = SnippetChooserBlock("cjkcms.FilmStrip")
+
+    class Meta:
+        icon = "image"
+        label = _("Film Strip")
+        template = "cjkcms/blocks/film_strip_block.html"
+
+
 class ImageGalleryBlock(BaseBlock):
     """
     Show a collection of images with interactive previews that expand to
     full size images in a modal.
     """
 
     collection = CollectionChooserBlock(
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/blocks/html_blocks.py` & `wagtail-cjkcms-23.7.1/cjkcms/blocks/html_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     A link styled as a button.
     """
 
     class Meta:
         template = "cjkcms/blocks/button_block.html"
         icon = "hand-pointer-o"
         label = _("Button Link")
+        label_format = "{button_title} (Button Link)"
         value_class = LinkStructValue
 
 
 class DownloadBlock(ButtonMixin, BaseBlock):
     """
     Link to a file that can be downloaded.
     """
@@ -176,26 +177,31 @@
 
 
 class PageListBlock(BaseBlock):
     """
     Renders a preview of selected pages.
     """
 
+    # default miniview template, overridden by individual page models
+    miniview_template = "cjkcms/pages/page.mini.html"
+
     indexed_by = blocks.PageChooserBlock(
         required=False,
         label=_("Parent page"),
         help_text=_(
             "Preview of pages that are children of the selected page (default to own parent). Uses ordering specified in the page’s LAYOUT tab."  # noqa
         ),
     )
     classified_by = ClassifierTermChooserBlock(
         required=False,
         label=_("Classified as"),
         help_text=_("Only show pages that are classified with this term."),
     )
+
+    # DEPRECATED - replaced with mini-views
     show_preview = blocks.BooleanBlock(
         required=False,
         default=False,
         label=_("Show body preview"),
     )
     show_dates = blocks.BooleanBlock(
         required=False,
@@ -295,14 +301,15 @@
                 previous_page = item
             if (index == current_index + 1) and (index < page_count):
                 next_page = item
 
         context["previous_page"] = previous_page
         context["next_page"] = next_page
         context["pages"] = pages_limited
+        context["miniview_template"] = self.miniview_template
         return context
 
 
 class PagePreviewBlock(BaseBlock):
     """
     Renders a preview of a specific page.
     """
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/blocks/layout_blocks.py` & `wagtail-cjkcms-23.7.1/cjkcms/blocks/layout_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/draftail/draftail_extensions.py` & `wagtail-cjkcms-23.7.1/cjkcms/draftail/draftail_extensions.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/draftail/draftail_icons.py` & `wagtail-cjkcms-23.7.1/cjkcms/draftail/draftail_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/fields.py` & `wagtail-cjkcms-23.7.1/cjkcms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/finders/oembed.py` & `wagtail-cjkcms-23.7.1/cjkcms/finders/oembed.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/image_formats.py` & `wagtail-cjkcms-23.7.1/cjkcms/image_formats.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/management/commands/import-csv.py` & `wagtail-cjkcms-23.7.1/cjkcms/management/commands/import-csv.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-collections.py` & `wagtail-cjkcms-23.7.1/cjkcms/management/commands/init-collections.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-navbar.py` & `wagtail-cjkcms-23.7.1/cjkcms/management/commands/init-navbar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/management/commands/init-website.py` & `wagtail-cjkcms-23.7.1/cjkcms/management/commands/init-website.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/migrations/0001_initial.py` & `wagtail-cjkcms-23.7.1/cjkcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py` & `wagtail-cjkcms-23.7.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py` & `wagtail-cjkcms-23.7.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py` & `wagtail-cjkcms-23.7.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py` & `wagtail-cjkcms-23.7.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py` & `wagtail-cjkcms-23.7.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py` & `wagtail-cjkcms-23.7.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py` & `wagtail-cjkcms-23.7.1/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/migrations/0009_navbar_language.py` & `wagtail-cjkcms-23.7.1/cjkcms/migrations/0009_navbar_language.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/models/cms_models.py` & `wagtail-cjkcms-23.7.1/cjkcms/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/models/integration_models.py` & `wagtail-cjkcms-23.7.1/cjkcms/models/integration_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/models/page_models.py` & `wagtail-cjkcms-23.7.1/cjkcms/models/page_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Base and abstract pages used in Cjk CMS.
 
 Based on CODEREDCMS
 """
 
 import logging
 from datetime import datetime
-from typing import Optional, TYPE_CHECKING
+from typing import Optional, TYPE_CHECKING, Union
 
 # import geocoder
 from django import forms
 from django.conf import settings
 from django.core.paginator import Paginator, InvalidPage, EmptyPage, PageNotAnInteger
 from django.db import models
 from django.utils.translation import gettext_lazy as _
@@ -71,18 +71,18 @@
             CJKCMS_PAGE_MODELS.append(cls)
 
 
 class CjkcmsTag(TaggedItemBase):
     class Meta:
         verbose_name = _("CMS Tag")
 
-    content_object = ParentalKey("cjkcms.CjkcmsPage", related_name="tagged_items")
+    content_object = ParentalKey("cjkcms.CjkcmsPage", related_name="tagged_items")  # type: ignore  # noqa: E501
 
 
-class CjkcmsPage(WagtailCacheMixin, SeoMixin, Page, metaclass=CjkcmsPageMeta):  # type: ignore
+class CjkcmsPage(WagtailCacheMixin, SeoMixin, Page, metaclass=CjkcmsPageMeta):
     """
     General use page with caching, templating, and SEO functionality.
     All pages should inherit from this.
     """
 
     class Meta:
         verbose_name = _("CjkCMS Page")
@@ -91,15 +91,19 @@
     is_creatable = False
 
     # Templates
     # The page will render the following templates under certain conditions:
     #
     # template = ''
     # ajax_template = ''
-    # search_template = ''
+    # Template used in site search results.
+    search_template = "cjkcms/pages/search_result.html"
+
+    # Template used for related pages, Latest Pages block, and Page Preview block.
+    miniview_template = "cjkcms/pages/page.mini.html"
 
     ###############
     # Content fields
     ###############
 
     cover_image = models.ForeignKey(
         get_image_model_string(),
@@ -162,20 +166,55 @@
     index_classifiers = ParentalManyToManyField(
         "cjkcms.Classifier",
         blank=True,
         verbose_name=_("Filter child pages by"),
         help_text=_("Enable filtering child pages by these classifiers."),
     )
 
+    #####################
+    # Related Page Fields
+    #####################
+
+    # Subclasses can override this to query on a specific
+    # page model. By default sibling pages are used.
+    related_query_pagemodel = None
+
+    # Subclasses can override this to enabled related pages by default.
+    related_show_default = False
+
+    related_show = models.BooleanField(
+        default=related_show_default,
+        verbose_name=_("Show list of related pages"),
+    )
+
+    related_num = models.PositiveIntegerField(
+        default=3,
+        verbose_name=_("Number of related pages to show"),
+    )
+
+    related_classifier_term = models.ForeignKey(
+        "cjkcms.ClassifierTerm",
+        blank=True,
+        null=True,
+        on_delete=models.SET_NULL,
+        related_name="+",
+        verbose_name=_("Preferred related classifier term"),
+        help_text=_(
+            "When getting related pages, pages with this term will be "
+            "weighted over other classifier terms. By default, pages with "
+            "the greatest number of classifiers in common are ranked highest."
+        ),
+    )
+
     ###############
     # Layout fields
     ###############
 
     custom_template = models.CharField(
-        blank=True, max_length=255, choices=None, verbose_name=_("Template")
+        blank=True, max_length=255, choices=None, verbose_name=_("Template")  # type: ignore  # noqa: E501
     )
 
     ###############
     # SEO overrides
     ###############
 
     seo_image_sources = [
@@ -241,14 +280,22 @@
                 FieldPanel("index_num_per_page"),
                 FieldPanel("index_order_by_classifier"),
                 FieldPanel("index_order_by"),
                 FieldPanel("index_classifiers", widget=forms.CheckboxSelectMultiple()),
             ],
             heading=_("Show Child Pages"),
         ),
+        MultiFieldPanel(
+            [
+                FieldPanel("related_show"),
+                FieldPanel("related_num"),
+                FieldPanel("related_classifier_term"),
+            ],
+            heading=_("Related Pages"),
+        ),
     ]
 
     promote_panels = SeoMixin.seo_meta_panels + SeoMixin.seo_struct_panels
 
     integration_panels = []
 
     def __init__(self, *args, **kwargs):
@@ -263,14 +310,15 @@
         ) + cms_settings.CJKCMS_FRONTEND_TEMPLATES_PAGES.get(klassname, [])
 
         self._meta.get_field("index_order_by").choices = self.index_order_by_choices  # type: ignore
         self._meta.get_field("custom_template").choices = template_choices  # type: ignore
         if not self.id:  # type: ignore
             self.index_order_by = self.index_order_by_default
             self.index_show_subpages = self.index_show_subpages_default
+            self.related_show = self.related_show_default
 
     @classmethod
     def get_panels(cls):  # sourcery skip: instance-method-first-arg-name
         panels = [
             ObjectList(
                 cls.content_panels
                 + cls.body_content_panels
@@ -380,20 +428,68 @@
 
         # Order the query.
         if order:
             query = query.order_by(*order)
 
         return query
 
+    def get_related_pages(self) -> models.QuerySet:
+        """
+        Returns a queryset of sibling pages, or the model type
+        defined by `self.related_query_pagemodel`. Ordered by number
+        of shared classifier terms.
+        """
+
+        # Get our related query model, and queryset.
+        if self.related_query_pagemodel:
+            if isinstance(self.related_query_pagemodel, Union[str, models.Model]):
+                querymodel = resolve_model_string(
+                    self.related_query_pagemodel, self._meta.app_label
+                )
+                r_qs = querymodel.objects.all().live()  # type: ignore
+            else:
+                raise AttributeError(
+                    f"The related_querymodel should be a model or str."
+                    f" The related_querymodel of {self} is {type(self.related_querymodel)}"  # type: ignore  # noqa: E501
+                )
+        else:
+            r_qs = self.get_parent().specific.get_index_children()  # type: ignore
+
+        # Exclude self to avoid infinite recursion.
+        r_qs = r_qs.exclude(pk=self.pk)
+
+        order_by = []
+
+        # If we have a preferred classifier term, order by that.
+        if self.related_classifier_term:
+            p_ct_q = models.Q(classifier_terms=self.related_classifier_term)
+            r_qs = r_qs.annotate(p_ct=p_ct_q)
+            order_by.append("-p_ct")
+
+        # If this page has a classifier, then order by number of
+        # shared classifier terms.
+        if self.classifier_terms.exists():
+            r_ct_q = models.Q(classifier_terms__in=self.classifier_terms.all())
+            r_qs = r_qs.annotate(r_ct=models.Count("classifier_terms", r_ct_q))
+            order_by.append("-r_ct")
+
+        # Order the related pages, then add distinct to deal with
+        # annotating based on a many to many.
+        if order_by:
+            r_qs = r_qs.order_by(*order_by).distinct()
+
+        return r_qs[: self.related_num]
+
     def get_context(self, request, *args, **kwargs):
         """
         Add child pages and paginated child pages to context.
         """
         context = super().get_context(request)
 
+        # Show list of child pages.
         if self.index_show_subpages:
             # Get child pages
             all_children = self.get_index_children()
             # Filter by classifier terms if applicable
             if len(request.GET) > 0 and self.index_classifiers.exists():
                 # Look up comma separated ClassifierTerm slugs i.e. `/?c=term1-slug,term2-slug`
                 terms = []
@@ -413,28 +509,38 @@
                         try:
                             for term in selected_terms:
                                 all_children = all_children.filter(
                                     classifier_terms=term
                                 )
                         except AttributeError:
                             logger.warning(
-                                "Tried to filter by ClassifierTerm, but <%s.%s ('%s')>.get_index_children() did not return a queryset or is not a queryset of CjkcmsPage models.",  # noqa
+                                (
+                                    "Tried to filter by ClassifierTerm, "
+                                    "but <%s.%s ('%s')>.get_index_children() "
+                                    "did not return a queryset or is not a "
+                                    "queryset of CoderedPage models."
+                                ),
                                 self._meta.app_label,
                                 self.__class__.__name__,
                                 self.title,
                             )
             paginator = Paginator(all_children, self.index_num_per_page)
             pagenum = request.GET.get("p", 1)
             try:
                 paged_children = paginator.page(pagenum)
             except (PageNotAnInteger, EmptyPage, InvalidPage) as e:  # noqa
                 paged_children = paginator.page(1)
 
             context["index_paginated"] = paged_children
             context["index_children"] = all_children
+
+        # Show a list of related pages.
+        if self.related_show:
+            context["related_pages"] = self.get_related_pages()
+
         return context
 
 
 ###############################################################################
 # Abstract pages providing pre-built common website functionality, suitable for subclassing.
 # These are abstract so subclasses can override fields if desired.
 ###############################################################################
@@ -480,14 +586,18 @@
 
     class Meta:
         verbose_name = _("CMS Article")
         abstract = True
 
     template = "cjkcms/pages/article_page.html"
 
+    search_template = "cjkcms/pages/article_page.search.html"
+
+    related_show_default = True
+
     # Override body to provide simpler content
     body = StreamField(CONTENT_STREAMBLOCKS, null=True, blank=True, use_json_field=True)
 
     caption = models.CharField(
         max_length=255,
         blank=True,
         verbose_name=_("Caption"),
@@ -525,15 +635,15 @@
 
     @property
     def seo_published_at(self) -> datetime:
         """
         Override of method in SeoMixin.
         Gets published date.
         """
-        return self.date_display or self.first_published_at
+        return self.date_display or self.first_published_at  # type: ignore
 
     @property
     def seo_description(self) -> str:
         """
         Override of method in SeoMixin.
         Gets the description using a fallback.
         """
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/models/snippet_models.py` & `wagtail-cjkcms-23.7.1/cjkcms/models/snippet_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     HTML_STREAMBLOCKS,
     LAYOUT_STREAMBLOCKS,
     NAVIGATION_STREAMBLOCKS,
 )
 from cjkcms.settings import cms_settings
 from django.conf import settings
 from cjkcms.fields import CjkcmsStreamField
+from wagtail_color_panel.fields import ColorField
+from wagtail_color_panel.edit_handlers import NativeColorPanel
 
 
 @register_snippet
 class Carousel(ClusterableModel):
     """
     Model that represents a Carousel. Can be modified through the snippets UI.
     Selected through Page StreamField bodies by the CarouselSnippetChooser in
@@ -102,15 +104,15 @@
     class Meta:
         verbose_name = _("Carousel Slide")
 
     carousel = ParentalKey(
         Carousel,
         related_name="carousel_slides",
         verbose_name=_("Carousel"),
-    )
+    )  # type: ignore
     image = models.ForeignKey(
         get_image_model_string(),
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
         related_name="+",
         verbose_name=_("Image"),
@@ -153,15 +155,15 @@
         verbose_name_plural = _("Classifiers")
         ordering = ["name"]
 
     slug = models.SlugField(
         allow_unicode=True,
         unique=True,
         verbose_name=_("Slug"),
-    )
+    )  # type: ignore
     name = models.CharField(
         max_length=255,
         verbose_name=_("Name"),
     )
 
     panels = [FieldPanel("name"), InlinePanel("terms", label=_("Classifier Terms"))]
 
@@ -192,20 +194,20 @@
         verbose_name = _("Classifier Term")
         verbose_name_plural = _("Classifier Terms")
 
     classifier = ParentalKey(
         Classifier,
         related_name="terms",
         verbose_name=_("Classifier"),
-    )
+    )  # type: ignore
     slug = models.SlugField(
         allow_unicode=True,
         unique=True,
         verbose_name=_("Slug"),
-    )
+    )  # type: ignore
     name = models.CharField(
         max_length=255,
         verbose_name=_("Name"),
     )
 
     panels = [
         FieldPanel("name"),
@@ -226,14 +228,84 @@
         return super().save(*args, **kwargs)
 
     def __str__(self):
         return "{0} > {1}".format(self.classifier.name, self.name)
 
 
 @register_snippet
+class FilmStrip(ClusterableModel):
+    class Meta:
+        verbose_name = _("Film Strip")
+
+    name = models.CharField(
+        max_length=255,
+        verbose_name=_("Name"),
+    )
+
+    panels = [
+        FieldPanel("name"),
+        InlinePanel("film_panels", label=_("Panels")),
+    ]
+
+    def __str__(self):
+        return self.name
+
+
+class FilmPanel(Orderable, models.Model):
+    class Meta:
+        verbose_name = _("Film Panel")
+
+    film_strip = ParentalKey(
+        FilmStrip,
+        related_name="film_panels",
+        verbose_name=_("Film Panel"),
+    )  # type: ignore
+    background_image = models.ForeignKey(
+        get_image_model_string(),
+        null=True,
+        blank=True,
+        on_delete=models.SET_NULL,
+        related_name="+",
+        verbose_name=_("Background image"),
+    )
+    background_color = ColorField(
+        blank=True,
+        verbose_name=_("Background color"),
+    )
+    foreground_color = ColorField(
+        blank=True,
+        verbose_name=_("Text color"),
+    )
+    custom_css_class = models.CharField(
+        max_length=255,
+        blank=True,
+        verbose_name=_("Custom CSS class"),
+    )
+    custom_id = models.CharField(
+        max_length=255,
+        blank=True,
+        verbose_name=_("Custom ID"),
+    )
+    content = CjkcmsStreamField(
+        HTML_STREAMBLOCKS,
+        blank=True,
+        use_json_field=True,
+    )
+
+    panels = [
+        FieldPanel("background_image"),
+        NativeColorPanel("background_color"),
+        NativeColorPanel("foreground_color"),
+        FieldPanel("custom_css_class"),
+        FieldPanel("custom_id"),
+        FieldPanel("content"),
+    ]
+
+
+@register_snippet
 class Navbar(models.Model):
     """
     Snippet for site navigation bars (header, main menu, etc.)
     """
 
     class Meta:
         verbose_name = _("Navigation Bar")
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/models/wagtailsettings_models.py` & `wagtail-cjkcms-23.7.1/cjkcms/models/wagtailsettings_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/settings.py` & `wagtail-cjkcms-23.7.1/cjkcms/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.conf import settings
 
 
 class _DefaultSettings:
-
     CJKCMS_FONT_URL = "https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap"  # noqa
 
     CJKCMS_FONT_FAMILY = "Roboto, sans-serif"
 
     CJKCMS_BRAND_LOGO_LONG = "cjkcms/images/logos/cms-logo-long.svg"
     CJKCMS_BRAND_LOGO_SQUARE = "cjkcms/images/logos/cms-logo-square.svg"
     CJKCMS_FRONTEND_BTN_SIZE_DEFAULT = ""
@@ -135,14 +134,15 @@
                 "Card deck - separate cards of equal size",
             ),
             (
                 "cjkcms/blocks/cardgrid_columns.html",
                 "Card masonry - fluid brick pattern",
             ),
         ],
+        # DEPRECATED
         "pagelistblock": [
             ("cjkcms/blocks/pagelist_block.html", "General, simple list"),
             (
                 "cjkcms/blocks/pagelist_list_group.html",
                 "General, list group navigation panel",
             ),
             (
@@ -159,14 +159,15 @@
                 "Article, card deck - separate cards of equal size",
             ),
             (
                 "cjkcms/blocks/pagelist_article_card_columns.html",
                 "Article, card masonry - fluid brick pattern",
             ),
         ],
+        # DEPRECATED
         "pagepreviewblock": [
             ("cjkcms/blocks/pagepreview_card.html", "Card"),
         ],
         "quoteblock": [
             ("cjkcms/blocks/quote_block.html", "Simple blockquote"),
             ("cjkcms/blocks/quote_block_leftbar.html", "Quote with left bar"),
             ("cjkcms/blocks/quote_block_start_end_quote.html", "With start/end quote"),
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.css` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.json` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/bootstrap-icons.scss` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-admin.css` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/css/cjkcms-admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-editor.css` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/css/cjkcms-editor.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/css/cjkcms-front.css` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/css/cjkcms-front.css`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,31 @@
 }
 
 .richtext-image.full-width {
   width: 100%;
   height: auto;
 }
 
+.cms-filmstrip-container {
+  overflow: hidden;
+}
+
+@media (hover: none) {
+  .cms-filmstrip-container {
+    overflow-x: scroll;
+  }
+}
+
+.cms-filmstrip-panel {
+  min-width: 300px;
+  min-height: 300px;
+  padding: 40px;
+  text-align: center;
+}
+
 .modal-lightbox {
   max-width: 100vw;
   text-align: center;
 }
 
 .modal-lightbox img {
   max-height: 90vh;
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/avatars/default.png` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/avatars/default.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/icons/quote.svg` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern1.jpg` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern2.jpg` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cjkcms/images/patterns/pattern3.jpg` & `wagtail-cjkcms-23.7.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/cookieconsent.css` & `wagtail-cjkcms-23.7.1/cjkcms/static/cookieconsent/cookieconsent.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/static/cookieconsent/cookieconsent.js` & `wagtail-cjkcms-23.7.1/cjkcms/static/cookieconsent/cookieconsent.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/404.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/404.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/500.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/500.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/accordion_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/article_block_card.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/article_masonry_card.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/base_link_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/button_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_blurb.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_foot.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_head.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_head_foot.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_horizontal.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_horizontal2.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_img.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_landing1.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_landing1.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/card_landing2.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/card_landing2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/carousel_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/download_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/hero_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_gallery_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/image_link_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/modal_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_card.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pagepreview_form.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/blocks/table_block.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/cookieconsent/languages.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/cookieconsent/languages.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/check-square-o.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/check-square-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/font.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/font.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/hashtag.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/hashtag.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/header.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/header.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/list-alt.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/list-alt.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/puzzle-piece.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/recycle.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/recycle.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/universal-access.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/universal-access.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/icons/usd.svg` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/icons/usd.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/classifier_nav.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/pagination.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_index_page.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_page.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/article_page.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 {% extends "cjkcms/pages/web_page.html" %}
 {% load wagtailadmin_tags wagtailcore_tags wagtailimages_tags cjkcms_tags %}
 
 {% block content %}
     <article class="cjkcms-article {%if self.cover_image %}has-img{% endif %}">
+        {% block article_cover_image %}
         {% if self.cover_image %}
         {% image self.cover_image fill-2000x1000 as cover_image %}
         <img src="{{cover_image.url}}" class="w-100" />
         {% endif %}
+        {% endblock article_cover_image %}
         <div class="container">
+            {% block article_header %}
             <div class="article-header">
                 <h1 {% if not self.cover_image %}class="mt-5"{% endif %}>{{ self.title }}</h1>
                 {% if self.caption %}
                 <p class="lead">{{self.caption}}</p>
                 {% endif %}
                 <p>
                     {% if settings.cjkcms.LayoutSettings.articles_show_author %}
@@ -24,13 +27,19 @@
                     {% endif %}
                     {% if settings.cjkcms.LayoutSettings.articles_date_format %}
                     <span class="article-date">{{ self.seo_published_at|date:settings.cjkcms.LayoutSettings.articles_date_format }}</span>
                     {% endif %}
                 </p>
                 <hr>
             </div>
+            {% endblock article_header %}
+            {% block article_body %}
             <div class="article-body">
                 {% include_block self.body with settings=settings %}
             </div>
+            {% endblock article_body %}
         </div>
+        {% block related_content %}
+        {{ block.super }}
+        {% endblock %}
     </article>
 {% endblock %}
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/article_page.search.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/base.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -68,65 +68,82 @@
                 {% include "cjkcms/snippets/tracking_g4.html" %}
             {% endif %}
         {% endblock %}
     </head>
 {% endblock base_head %}
 
     <body class="cjkcms-{{page.content_type.model}} {% if page.get_parent %}parent-page-{{page.get_parent.id}}{% endif %} {% block body_class %}{% endblock %}" id="page-{{page.id}}">
-
         {% include "cjkcms/includes/cjkcms_banner.html" %}
 
         {% wagtailuserbar %}
 
         {% block navbar %}{% endblock %}
+
         <div id="content">
             {% block content %}
                 {% block messages %}
                     {% if messages %}
                         <div class="container">
                         {% for message in messages %}
                             <div class="alert alert-{{ message.tags|map_to_bootstrap_alert }}" role="alert">{{ message }}</div>
                         {% endfor %}
                         </div>
                     {% endif %}
                 {% endblock %}
                 {% block content_pre_body %}{% endblock %}
 
                 {% block content_body %}
-                {% include_block page.body with settings=settings %}
+
+                    {% for block in page.body %}
+                    {{ page }}
+                        {% include_block block with settings=settings %}
+                    {% endfor %}
                 {% endblock %}
 
                 {% block content_post_body %}{% endblock %}
 
                 {% block index_filters %}
-                {% if page.index_show_subpages and page.index_classifiers.exists %}
-                    {% include "cjkcms/includes/classifier_dropdowns.html" with formclass="form-inline" %}
-                {% endif %}
+                <div class="container">
+                    {% if page.index_show_subpages and page.index_classifiers.exists %}
+                    {% include "cjkcms/includes/classifier_dropdowns.html" with formclass="d-flex" formid="filter" %}
+                    {% endif %}
+                </div>
                 {% endblock %}
 
                 {% block index_content %}
                 {% if page.index_show_subpages %}
-                    <ul>
-                    {% for child in index_paginated %}
-                        <li><a href="{% pageurl child %}">{{child.title}}</a></li>
-                    {% endfor %}
-                    </ul>
+                    <div class="container">
+                        <div class="row">
+                        {% for child in index_paginated %}
+                        <div class="col-sm-6 col-lg-4">
+                            {% include child.miniview_template with page=child %}
+                        </div>
+                        {% endfor %}
+                        </div>
+                    </div>
                     {% include "cjkcms/includes/pagination.html" with items=index_paginated %}
                 {% endif %}
-                {% endblock %}
+                {% endblock index_content %}
 
-            {% endblock %}
-        </div>
+                {% block related_content %}
+                {% if page.related_show %}
+                <div class="container">
+                  <h2 class="text-center my-5">{% trans "Related" %}</h2>
+                  <div class="row">
+                    {% for rp in related_pages %}
+                    <div class="col-sm-6 col-lg-4">
+                      {% include rp.miniview_template with page=rp %}
+                    </div>
+                    {% endfor %}
+                  </div>
+                </div>
+                {% endif %}
+                {% endblock related_content %}
 
-        <div id="content-walls">
-            {% block content_walls %}
-                {% for content_wall in content_walls %}
-                    {% include_block content_wall with settings=settings %}
-                {% endfor %}
-            {% endblock %}
+            {% endblock content %}
         </div>
 
         {% block footer %}{% endblock %}
 
         {% block required_scripts %}
 
         {% endblock %}
```

#### html2text {}

```diff
@@ -41,28 +41,32 @@
 {% include "cjkcms/includes/cjkcms_banner.html" %} {% wagtailuserbar %} {%
 block navbar %}{% endblock %}
 {% block content %} {% block messages %} {% if messages %}
 {% for message in messages %}
 {{ message }}
 {% endfor %}
 {% endif %} {% endblock %} {% block content_pre_body %}{% endblock %} {% block
-content_body %} {% include_block page.body with settings=settings %} {%
-endblock %} {% block content_post_body %}{% endblock %} {% block index_filters
-%} {% if page.index_show_subpages and page.index_classifiers.exists %} {%
-include "cjkcms/includes/classifier_dropdowns.html" with formclass="form-
-inline" %} {% endif %} {% endblock %} {% block index_content %} {% if
-page.index_show_subpages %}
-    * {% for child in index_paginated %}
-    * {{child.title}}
-    * {% endfor %}
+content_body %} {% for block in page.body %} {{ page }} {% include_block block
+with settings=settings %} {% endfor %} {% endblock %} {% block
+content_post_body %}{% endblock %} {% block index_filters %}
+{% if page.index_show_subpages and page.index_classifiers.exists %} {% include
+"cjkcms/includes/classifier_dropdowns.html" with formclass="d-flex"
+formid="filter" %} {% endif %}
+{% endblock %} {% block index_content %} {% if page.index_show_subpages %}
+{% for child in index_paginated %}
+{% include child.miniview_template with page=child %}
+{% endfor %}
 {% include "cjkcms/includes/pagination.html" with items=index_paginated %} {%
-endif %} {% endblock %} {% endblock %}
-{% block content_walls %} {% for content_wall in content_walls %} {%
-include_block content_wall with settings=settings %} {% endfor %} {% endblock
-%}
+endif %} {% endblock index_content %} {% block related_content %} {% if
+page.related_show %}
+***** {% trans "Related" %} *****
+{% for rp in related_pages %}
+{% include rp.miniview_template with page=rp %}
+{% endfor %}
+{% endif %} {% endblock related_content %} {% endblock content %}
 {% block footer %}{% endblock %} {% block required_scripts %} {% endblock %} {%
 block frontend_scripts %} {% include "cjkcms/snippets/frontend_scripts.html" %}
 {% endblock %} {% block cjkcms_scripts %}
  {% endblock %} {% block custom_scripts %} {# Leave blank for client sites to
 implement. #} {#
  #} {% endblock %} {% block cookie_consent_scripts %} {% if
 settings.cjkcms.AnalyticsSettings.cookie_consent %}
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/form_page.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/form_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/search.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/search_result.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/search_result.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/pages/stream_form_page.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/pages/stream_form_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/frontend_assets.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/frontend_scripts.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/navbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/snippets/tracking_g4.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,13 @@
   function gtag(){dataLayer.push(arguments);}
   gtag('js', new Date());
 
   gtag('config', '{{settings.cjkcms.AnalyticsSettings.g4_tracking_id}}');
 </script>
 
 <script data-cookiecategory="analytics">
-  cr_track_clicks = {{settings.cjkcms.AnalyticsSettings.ga_track_button_clicks|yesno:"true,false"}};
+  cms_track_clicks = {{settings.cjkcms.AnalyticsSettings.ga_track_button_clicks|yesno:"true,false"}};
   window.dataLayer = window.dataLayer || [];
   function gtag(){dataLayer.push(arguments);}
   gtag('js', new Date());
   gtag('config', '{{settings.cjkcms.AnalyticsSettings.ga_tracking_id}}');
 </script>
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 {% if widget.optgroups %}
     {% with id=widget.attrs.id %}
     <div class="field-row {{ widget.attrs.class }}" {% if id %}id="{{ id }}"{% endif %}>
     {% for group, options, index in widget.optgroups %}
         {% if group %}
         <div class="field-col col4">
         <ul class="cjkcms-checkbox-group">
-            <li><strong>{{ group }}</strong>
+            <li><label class="w-field__label">{{ group }}</label>
         {% endif %}
         <ul{% if id %} id="{{ id }}_{{ index }}"{% endif %}>
         {% for option in options %}
         <li>{% include option.template_name with widget=option %}</li>
         {% endfor %}
         </ul>
         {% if group %}
         </li></ul></div>
         {% endif %}
         {% if forloop.counter|divisibleby:3 %}
-        <div class="clearfix"></div>
+        <div style="clear:both;"></div>
         {% endif %}
     {% endfor %}
+    <div style="clear:both;"></div>
     </div>
     {% endwith %}
 {% else %}
     {% load i18n %}
     <div class="cjkcms-callout">
         <div class="cjkcms-big-icon icon icon-snippet"></div>
         <h3>
```

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/block_forms/struct.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/wagtailadmin/block_forms/struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html` & `wagtail-cjkcms-23.7.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templatetags/cjkcms_tags.py` & `wagtail-cjkcms-23.7.1/cjkcms/templatetags/cjkcms_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templatetags/friendly_loader.py` & `wagtail-cjkcms-23.7.1/cjkcms/templatetags/friendly_loader.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templatetags/gravatar.py` & `wagtail-cjkcms-23.7.1/cjkcms/templatetags/gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/templatetags/txtutils_tags.py` & `wagtail-cjkcms-23.7.1/cjkcms/templatetags/txtutils_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/tests/test_articlepages.py` & `wagtail-cjkcms-23.7.1/cjkcms/tests/test_articlepages.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/tests/test_gravatar.py` & `wagtail-cjkcms-23.7.1/cjkcms/tests/test_gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/tests/test_search_blocks.py` & `wagtail-cjkcms-23.7.1/cjkcms/tests/test_search_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/tests/test_settings.py` & `wagtail-cjkcms-23.7.1/cjkcms/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/tests/test_templatetags.py` & `wagtail-cjkcms-23.7.1/cjkcms/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/tests/test_urls.py` & `wagtail-cjkcms-23.7.1/cjkcms/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/tests/test_webpage.py` & `wagtail-cjkcms-23.7.1/cjkcms/tests/test_webpage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/utils.py` & `wagtail-cjkcms-23.7.1/cjkcms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/views.py` & `wagtail-cjkcms-23.7.1/cjkcms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/wagtail_hooks.py` & `wagtail-cjkcms-23.7.1/cjkcms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/cjkcms/widgets.py` & `wagtail-cjkcms-23.7.1/cjkcms/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/docs/how-to/oembed_finder.md` & `wagtail-cjkcms-23.7.1/docs/how-to/oembed_finder.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/docs/index.md` & `wagtail-cjkcms-23.7.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/docs/installation.md` & `wagtail-cjkcms-23.7.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/docs/quick-start.md` & `wagtail-cjkcms-23.7.1/docs/quick-start.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/docs/why-another-cms.md` & `wagtail-cjkcms-23.7.1/docs/why-another-cms.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/setup.cfg` & `wagtail-cjkcms-23.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/PKG-INFO` & `wagtail-cjkcms-23.7.1/wagtail_cjkcms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.6.2
+Version: 23.7.1
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.x site. Based on Codered CRX.
 Home-page: https://github.com/cjkpl/wagtail-cjkcms
 Author: Grzegorz Krol
 Author-email: gk@cjk.pl
 License: BSD-3-Clause  # Example license
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail-cjkcms-23.6.2/wagtail_cjkcms.egg-info/SOURCES.txt` & `wagtail-cjkcms-23.7.1/wagtail_cjkcms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
 cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
 cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
 cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
 cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
 cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
 cjkcms/migrations/0009_navbar_language.py
+cjkcms/migrations/0010_filmstrip_filmpanel.py
+cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py
 cjkcms/migrations/__init__.py
 cjkcms/models/__init__.py
 cjkcms/models/admin_sidebar.py
 cjkcms/models/cms_models.py
 cjkcms/models/integration_models.py
 cjkcms/models/page_models.py
 cjkcms/models/snippet_models.py
@@ -100,14 +102,15 @@
 cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
 cjkcms/templates/cjkcms/blocks/carousel_block.html
 cjkcms/templates/cjkcms/blocks/column_block.html
 cjkcms/templates/cjkcms/blocks/document_link_block.html
 cjkcms/templates/cjkcms/blocks/download_block.html
 cjkcms/templates/cjkcms/blocks/embed_video_block.html
 cjkcms/templates/cjkcms/blocks/external_link_block.html
+cjkcms/templates/cjkcms/blocks/film_strip_block.html
 cjkcms/templates/cjkcms/blocks/grid_block.html
 cjkcms/templates/cjkcms/blocks/h1_block.html
 cjkcms/templates/cjkcms/blocks/h2_block.html
 cjkcms/templates/cjkcms/blocks/h3_block.html
 cjkcms/templates/cjkcms/blocks/hero_block.html
 cjkcms/templates/cjkcms/blocks/image_block.html
 cjkcms/templates/cjkcms/blocks/image_gallery_block.html
@@ -167,16 +170,18 @@
 cjkcms/templates/cjkcms/includes/pagination.html
 cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
 cjkcms/templates/cjkcms/pages/article_index_page.html
 cjkcms/templates/cjkcms/pages/article_page.html
 cjkcms/templates/cjkcms/pages/article_page.search.html
 cjkcms/templates/cjkcms/pages/base.html
 cjkcms/templates/cjkcms/pages/form_page.html
+cjkcms/templates/cjkcms/pages/form_page.mini.html
 cjkcms/templates/cjkcms/pages/form_page_landing.html
 cjkcms/templates/cjkcms/pages/home_page.html
+cjkcms/templates/cjkcms/pages/page.mini.html
 cjkcms/templates/cjkcms/pages/search.html
 cjkcms/templates/cjkcms/pages/search_result.html
 cjkcms/templates/cjkcms/pages/stream_form_page.html
 cjkcms/templates/cjkcms/pages/web_page.html
 cjkcms/templates/cjkcms/pages/web_page_notitle.html
 cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
 cjkcms/templates/cjkcms/snippets/footer.html
```

