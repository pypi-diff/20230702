# Comparing `tmp/gs-netsuite-api-1.1.3.tar.gz` & `tmp/gs-netsuite-api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs-netsuite-api-1.1.3.tar", last modified: Wed Jun 28 06:02:29 2023, max compression
+gzip compressed data, was "gs-netsuite-api-1.2.0.tar", last modified: Sun Jul  2 17:09:26 2023, max compression
```

## Comparing `gs-netsuite-api-1.1.3.tar` & `gs-netsuite-api-1.2.0.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.348637 gs-netsuite-api-1.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     1910 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.328637 gs-netsuite-api-1.1.3/.idea/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.idea/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.idea/GitlabLint.xml
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.idea/misc.xml
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.idea/vcs.xml
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.local-antora-playbook.yml
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/.ruff
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-28 06:02:29.348637 gs-netsuite-api-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/README.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.328637 gs-netsuite-api-1.1.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/docs/antora.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.324637 gs-netsuite-api-1.1.3/docs/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.328637 gs-netsuite-api-1.1.3/docs/modules/ROOT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.324637 gs-netsuite-api-1.1.3/docs/modules/ROOT/examples/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/docs/modules/ROOT/nav.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.332637 gs-netsuite-api-1.1.3/docs/modules/ROOT/pages/
--rw-rw-rw-   0 root         (0) root         (0)     3361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/docs/modules/ROOT/pages/api.adoc
--rw-rw-rw-   0 root         (0) root         (0)     2996 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/docs/modules/ROOT/pages/convertion.adoc
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/docs/modules/ROOT/pages/index.adoc
--rw-rw-rw-   0 root         (0) root         (0)     2206 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/docs/modules/ROOT/pages/types.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.332637 gs-netsuite-api-1.1.3/example/
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/example/sample_item_fulfillment_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1311 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/example/sample_item_receipt_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/example/sample_product_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/example/sample_purchase_api.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2023-06-28 05:51:00.000000 gs-netsuite-api-1.1.3/example/sample_relationship_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2023-06-27 05:06:56.000000 gs-netsuite-api-1.1.3/example/sample_sale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 14:42:03.000000 gs-netsuite-api-1.1.3/netsuite-api.iml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.324637 gs-netsuite-api-1.1.3/output/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.324637 gs-netsuite-api-1.1.3/output/wsdl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.332637 gs-netsuite-api-1.1.3/output/wsdl/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   133803 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/wsdl/v2022_2_0/netsuite.wsdl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.328637 gs-netsuite-api-1.1.3/output/xsd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.324637 gs-netsuite-api-1.1.3/output/xsd/activities/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.332637 gs-netsuite-api-1.1.3/output/xsd/activities/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    38231 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/activities/v2022_2_0/scheduling.xsd
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/activities/v2022_2_0/schedulingTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.324637 gs-netsuite-api-1.1.3/output/xsd/documents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.332637 gs-netsuite-api-1.1.3/output/xsd/documents/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)     8963 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/documents/v2022_2_0/fileCabinet.xsd
--rw-rw-rw-   0 root         (0) root         (0)     4282 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.324637 gs-netsuite-api-1.1.3/output/xsd/general/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.336637 gs-netsuite-api-1.1.3/output/xsd/general/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    14530 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/general/v2022_2_0/communication.xsd
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/general/v2022_2_0/communicationTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.324637 gs-netsuite-api-1.1.3/output/xsd/lists/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.340637 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   424972 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/accounting.xsd
--rw-rw-rw-   0 root         (0) root         (0)    40848 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/accountingTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    11949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/employeeTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    31010 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/employees.xsd
--rw-rw-rw-   0 root         (0) root         (0)    27949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/marketing.xsd
--rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/marketingTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     7100 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/relationshipTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)   102099 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/relationships.xsd
--rw-rw-rw-   0 root         (0) root         (0)    16989 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/supplyChain.xsd
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    29653 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/support.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2906 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/supportTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/website.xsd
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/websiteTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.328637 gs-netsuite-api-1.1.3/output/xsd/platform/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.340637 gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   744517 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/common.xsd
--rw-rw-rw-   0 root         (0) root         (0)    59244 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/commonTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    47859 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/core.xsd
--rw-rw-rw-   0 root         (0) root         (0)    37883 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/coreTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    72361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/faultTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     3764 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/faults.xsd
--rw-rw-rw-   0 root         (0) root         (0)    28339 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/messages.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.328637 gs-netsuite-api-1.1.3/output/xsd/setup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.340637 gs-netsuite-api-1.1.3/output/xsd/setup/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   102180 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/setup/v2022_2_0/customization.xsd
--rw-rw-rw-   0 root         (0) root         (0)     4880 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/setup/v2022_2_0/customizationTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.328637 gs-netsuite-api-1.1.3/output/xsd/transactions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.344637 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    13345 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/bank.xsd
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/bankTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/customerTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    75538 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/customers.xsd
--rw-rw-rw-   0 root         (0) root         (0)    10022 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/demandPlanning.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2094 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/employeeTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    43650 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/employees.xsd
--rw-rw-rw-   0 root         (0) root         (0)     5844 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/financial.xsd
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/financialTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    23444 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/general.xsd
--rw-rw-rw-   0 root         (0) root         (0)    49374 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/inventory.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     1983 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    64002 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/purchases.xsd
--rw-rw-rw-   0 root         (0) root         (0)    32740 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/saleTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)   141383 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/sales.xsd
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-06-22 14:42:03.000000 gs-netsuite-api-1.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 06:02:29.348637 gs-netsuite-api-1.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.328637 gs-netsuite-api-1.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.348637 gs-netsuite-api-1.1.3/src/gs_netsuite_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-28 06:02:29.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    27401 2023-06-28 05:48:05.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api/api.py.adoc
--rw-rw-rw-   0 root         (0) root         (0)     4389 2023-06-28 05:48:05.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)     4296 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api/ns_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:02:29.348637 gs-netsuite-api-1.1.3/src/gs_netsuite_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-28 06:02:29.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3270 2023-06-28 06:02:29.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 06:02:29.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-28 06:02:29.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-28 06:02:29.000000 gs-netsuite-api-1.1.3/src/gs_netsuite_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3862 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.3/wsdldownloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.903235 gs-netsuite-api-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-02 17:00:02.000000 gs-netsuite-api-1.2.0/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/.idea/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/.idea/GitlabLint.xml
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/.idea/vcs.xml
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/.local-antora-playbook.yml
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/.ruff
+-rw-r--r--   0 root         (0) root         (0)      186 2023-07-02 17:09:26.903235 gs-netsuite-api-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/README.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/docs/antora.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.883235 gs-netsuite-api-1.2.0/docs/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/docs/modules/ROOT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.883235 gs-netsuite-api-1.2.0/docs/modules/ROOT/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/docs/modules/ROOT/nav.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/docs/modules/ROOT/pages/
+-rw-rw-rw-   0 root         (0) root         (0)     3361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/docs/modules/ROOT/pages/api.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2353 2023-07-02 15:12:18.000000 gs-netsuite-api-1.2.0/docs/modules/ROOT/pages/convertion.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/docs/modules/ROOT/pages/index.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2206 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/docs/modules/ROOT/pages/types.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/example/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-07-02 17:04:11.000000 gs-netsuite-api-1.2.0/example/sample_customer_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.0/example/sample_item_fulfillment_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.0/example/sample_item_receipt_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.0/example/sample_product_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1819 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.0/example/sample_purchase_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-02 15:19:42.000000 gs-netsuite-api-1.2.0/example/sample_sale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-02 17:04:11.000000 gs-netsuite-api-1.2.0/example/sample_vendor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 14:42:03.000000 gs-netsuite-api-1.2.0/netsuite-api.iml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.883235 gs-netsuite-api-1.2.0/output/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.883235 gs-netsuite-api-1.2.0/output/wsdl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/output/wsdl/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   133803 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/wsdl/v2022_2_0/netsuite.wsdl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/output/xsd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.883235 gs-netsuite-api-1.2.0/output/xsd/activities/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.891235 gs-netsuite-api-1.2.0/output/xsd/activities/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    38231 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/activities/v2022_2_0/scheduling.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/activities/v2022_2_0/schedulingTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.883235 gs-netsuite-api-1.2.0/output/xsd/documents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.891235 gs-netsuite-api-1.2.0/output/xsd/documents/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)     8963 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/documents/v2022_2_0/fileCabinet.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     4282 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.883235 gs-netsuite-api-1.2.0/output/xsd/general/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.891235 gs-netsuite-api-1.2.0/output/xsd/general/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    14530 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/general/v2022_2_0/communication.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/general/v2022_2_0/communicationTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/output/xsd/lists/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.895235 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   424972 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/accounting.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    40848 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/accountingTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/employeeTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    31010 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/employees.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    27949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/marketing.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/marketingTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     7100 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/relationshipTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)   102099 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/relationships.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    16989 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/supplyChain.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    29653 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/support.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2906 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/supportTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/website.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/websiteTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/output/xsd/platform/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.895235 gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   744517 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/common.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    59244 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/commonTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    47859 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/core.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    37883 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/coreTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    72361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/faultTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     3764 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/faults.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    28339 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/messages.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/output/xsd/setup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.895235 gs-netsuite-api-1.2.0/output/xsd/setup/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   102180 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/setup/v2022_2_0/customization.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     4880 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/setup/v2022_2_0/customizationTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/output/xsd/transactions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.899235 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    13345 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/bank.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/bankTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/customerTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    75538 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/customers.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    10022 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/demandPlanning.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/employeeTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    43650 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/employees.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     5844 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/financial.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/financialTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    23444 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/general.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    49374 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/inventory.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    64002 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/purchases.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    32740 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/saleTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)   141383 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/sales.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-06-22 14:42:03.000000 gs-netsuite-api-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 17:09:26.903235 gs-netsuite-api-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.887235 gs-netsuite-api-1.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.903235 gs-netsuite-api-1.2.0/src/gs_netsuite_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-02 17:09:26.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    27681 2023-07-02 17:04:11.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-22 14:37:57.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api/api.py.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     4606 2023-07-02 17:04:11.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3856 2023-07-02 15:24:56.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api/ns_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:09:26.903235 gs-netsuite-api-1.2.0/src/gs_netsuite_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-07-02 17:09:26.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3295 2023-07-02 17:09:26.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 17:09:26.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-07-02 17:09:26.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-02 17:09:26.000000 gs-netsuite-api-1.2.0/src/gs_netsuite_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3864 2023-07-02 15:28:33.000000 gs-netsuite-api-1.2.0/wsdldownloader.py
```

### Comparing `gs-netsuite-api-1.1.3/.gitignore` & `gs-netsuite-api-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/.pre-commit-config.yaml` & `gs-netsuite-api-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/README.adoc` & `gs-netsuite-api-1.2.0/README.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/docs/modules/ROOT/pages/api.adoc` & `gs-netsuite-api-1.2.0/docs/modules/ROOT/pages/api.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/docs/modules/ROOT/pages/convertion.adoc` & `gs-netsuite-api-1.2.0/docs/modules/ROOT/pages/convertion.adoc`

 * *Files 16% similar despite different names*

```diff
@@ -58,29 +58,12 @@
 
 
 == Les RecordRef
 
 Dans certain `xsd` vous aurez le type `platformCore:RecordRef`.
 Vous pouvez le convertir simplement en `data_types.RecordRef` graçe à sa fonction `data_types.RecordRef#from_rec_named`
 
-== Les customs field
+== Les custom fields
 
 Dans NetSuite chaque ressource peut avoir des `customField` dans un champs qui s'appelle `customFieldList`.
-Dans le package `ns_utils` il existe la fonction `extract_custom_field`
+Dans la classe `RecordRef` il existe la fonction `extract_custom_field`
 qui permet de simplement extraire la valeur en fonction du custom field recherché.
-
-A utilise4r comme suit
-
-[,python]
-----
-from ns_utls import extract_custom_field
-def convert_record(self, record) -> DataClass:
-    return DataClass(
-        field_from_custom=extract_custom_field(record, "custom_field_name"),<1>
-        int_field_from_custom=extract_custom_field(record, "custom_field_str_int_name", converter=int),<2>
-        ...
-    )
-----
-<1> Extraction du field `custom_field_name` de record en respectant le type dans la ressource NetSuite.
-<2> Extraction du field `custom_field_str_int_name` de record en forçant le type avec le converter.
-
-IMPORTANT: Si le converteur `raise` une erreur, celle ci ne sera pas géré.
```

### Comparing `gs-netsuite-api-1.1.3/docs/modules/ROOT/pages/index.adoc` & `gs-netsuite-api-1.2.0/docs/modules/ROOT/pages/index.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/docs/modules/ROOT/pages/types.adoc` & `gs-netsuite-api-1.2.0/docs/modules/ROOT/pages/types.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/example/sample_item_fulfillment_api.py` & `gs-netsuite-api-1.2.0/example/sample_item_fulfillment_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import dataclasses
 import datetime
+import logging
 from pprint import pprint
 
-import logging
-from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 from gs_netsuite_api.api import ItemFulFillmentAPI
-
+from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 
 logging.root.setLevel(logging.INFO)
 logging.root.addHandler(logging.StreamHandler())
 
 # Question sur les datas
 
 if __name__ == "__main__":
```

### Comparing `gs-netsuite-api-1.1.3/example/sample_item_receipt_api.py` & `gs-netsuite-api-1.2.0/example/sample_item_receipt_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import dataclasses
 import datetime
+import logging
 from pprint import pprint
 
-import logging
-from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 from gs_netsuite_api.api import ItemReceiptAPI
-
+from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 
 logging.root.setLevel(logging.INFO)
 logging.root.addHandler(logging.StreamHandler())
 
 # Question sur les datas
 
 if __name__ == "__main__":
```

### Comparing `gs-netsuite-api-1.1.3/example/sample_product_api.py` & `gs-netsuite-api-1.2.0/example/sample_product_api.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 import datetime
-from pprint import pprint
 import logging
+from pprint import pprint
 
-from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 from gs_netsuite_api.api import ProductAPI
+from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 
 logging.root.setLevel(logging.DEBUG)
 logging.root.addHandler(logging.StreamHandler())
 
 if __name__ == "__main__":
     # Existe d'autre methode pour avoir un NetSuiteCredential
     cred = NetSuiteCredential.from_env_file("./auth_netsuite.env")
```

### Comparing `gs-netsuite-api-1.1.3/example/sample_purchase_api.py` & `gs-netsuite-api-1.2.0/example/sample_purchase_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+import logging
 from pprint import pprint
 
-import logging
-from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 from gs_netsuite_api.api import PurchaseAPI
-
+from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 
 logging.root.setLevel(logging.INFO)
 logging.root.addHandler(logging.StreamHandler())
 
 # Question sur les datas
 # Le champs tax2Total c'est quoi ?
 # custbody_stc_tax_after_discount ?
```

### Comparing `gs-netsuite-api-1.1.3/example/sample_relationship_api.py` & `gs-netsuite-api-1.2.0/example/sample_vendor_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from pprint import pprint
 
-from gs_netsuite_api.api import RelationShipAPI
+from gs_netsuite_api.api import VendorAPI
 from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 
 logging.root.setLevel(logging.DEBUG)
 logging.root.addHandler(logging.StreamHandler())
 
 
 if __name__ == "__main__":
     # Existe d'autre methode pour avoir un NetSuiteCredential
     cred = NetSuiteCredential.from_env_file("./auth_netsuite.env")
-    api = RelationShipAPI(credential=cred, search_params=SearchParams(page_size=5, nb_page=2))
+    api = VendorAPI(credential=cred, search_params=SearchParams(page_size=5, nb_page=2))
 
     data_one = api.get_one(54839)
     pprint(data_one)
```

### Comparing `gs-netsuite-api-1.1.3/example/sample_sale_api.py` & `gs-netsuite-api-1.2.0/example/sample_sale_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import dataclasses
 import datetime
+import logging
 from pprint import pprint
 
-import logging
-from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 from gs_netsuite_api.api import SaleAPI
-
+from gs_netsuite_api.ns_utils import NetSuiteCredential, SearchParams
 
 logging.root.setLevel(logging.INFO)
 logging.root.addHandler(logging.StreamHandler())
 
 
 if __name__ == "__main__":
     # Existe d'autre methode pour avoir un NetSuiteCredential
```

### Comparing `gs-netsuite-api-1.1.3/mkdocs.yml` & `gs-netsuite-api-1.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/wsdl/v2022_2_0/netsuite.wsdl` & `gs-netsuite-api-1.2.0/output/wsdl/v2022_2_0/netsuite.wsdl`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/activities/v2022_2_0/scheduling.xsd` & `gs-netsuite-api-1.2.0/output/xsd/activities/v2022_2_0/scheduling.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/activities/v2022_2_0/schedulingTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/activities/v2022_2_0/schedulingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/documents/v2022_2_0/fileCabinet.xsd` & `gs-netsuite-api-1.2.0/output/xsd/documents/v2022_2_0/fileCabinet.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/general/v2022_2_0/communication.xsd` & `gs-netsuite-api-1.2.0/output/xsd/general/v2022_2_0/communication.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/general/v2022_2_0/communicationTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/general/v2022_2_0/communicationTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/accounting.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/accounting.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/accountingTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/accountingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/employeeTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/employeeTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/employees.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/employees.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/marketing.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/marketing.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/marketingTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/marketingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/relationshipTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/relationshipTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/relationships.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/relationships.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/supplyChain.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/supplyChain.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/support.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/support.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/supportTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/supportTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/lists/v2022_2_0/website.xsd` & `gs-netsuite-api-1.2.0/output/xsd/lists/v2022_2_0/website.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/common.xsd` & `gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/common.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/commonTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/commonTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/core.xsd` & `gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/core.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/coreTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/coreTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/faultTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/faultTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/faults.xsd` & `gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/faults.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/platform/v2022_2_0/messages.xsd` & `gs-netsuite-api-1.2.0/output/xsd/platform/v2022_2_0/messages.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/setup/v2022_2_0/customization.xsd` & `gs-netsuite-api-1.2.0/output/xsd/setup/v2022_2_0/customization.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/setup/v2022_2_0/customizationTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/setup/v2022_2_0/customizationTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/bank.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/bank.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/customerTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/customerTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/customers.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/customers.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/demandPlanning.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/demandPlanning.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/employeeTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/employeeTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/employees.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/employees.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/financial.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/financial.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/financialTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/financialTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/general.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/general.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/inventory.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/inventory.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/purchases.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/purchases.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/saleTypes.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/saleTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/output/xsd/transactions/v2022_2_0/sales.xsd` & `gs-netsuite-api-1.2.0/output/xsd/transactions/v2022_2_0/sales.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/pyproject.toml` & `gs-netsuite-api-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.3/src/gs_netsuite_api/api.py` & `gs-netsuite-api-1.2.0/src/gs_netsuite_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import abc
 import asyncio
 import datetime
 import logging
-from typing import Any, TypeVar, Generic, Callable, Coroutine, List
-
+from typing import Any, Callable, Coroutine, Generic, List, TypeVar
 
 from netsuite import NetSuiteSoapApi
-from .ns_utils import search_with_pref, assertSuccess, SearchParams, extract_custom_field, NetSuiteCredential
-from .data_types import RecordRef
-from .data_types import ProductData, ProductAvailability
-from .data_types import PurchaseOrderData, PurchaseOrderLineData
-from .data_types import SaleOrderData, SaleOrderLineData
-from .data_types import ItemPicking, ItemMove
-from .data_types import InventoryAdjustment, InventoryAdjustmentLine
-from .data_types import RelationShip
+
+from .data_types import (InventoryAdjustment, InventoryAdjustmentLine,
+                         ItemMove, ItemPicking, ProductAvailability,
+                         ProductData, PurchaseOrderData, PurchaseOrderLineData,
+                         RecordRef, RelationShip, SaleOrderData,
+                         SaleOrderLineData)
+from .ns_utils import (NetSuiteCredential, SearchParams, assertSuccess,
+                       search_with_pref)
 
 _logger = logging.getLogger(__name__)
 RT = TypeVar("RT", bound=RecordRef)
 R = TypeVar("R", bound=Any)
 
 
 class GsNetSuiteApi(abc.ABC, Generic[RT]):
@@ -412,29 +411,24 @@
         - download ou check des images
 
         """
         product = ProductData(
             name=record.displayName,
             internalId=int(record.internalId),
             ean13=record.upcCode,
-            hs_code=extract_custom_field(record, "custitemnvg_hs_code"),
             ref=record.itemId,
-            price_ttc=extract_custom_field(record, "custitem_nvg_ttcprice"),
             categories=[
                 RecordRef.from_rec_named(node.hierarchyNode)
                 for node in record.hierarchyVersionsList.inventoryItemHierarchyVersions
                 if node.hierarchyNode
             ],
-            custitemnv_master_reference=extract_custom_field(record, "custitemnv_master_reference"),
-            custitemnv_discontinued_item=extract_custom_field(record, "custitemnv_discontinued_item"),
             qty_available=record.quantityAvailable,
-            next_arrival_date=extract_custom_field(record, "custitemnv_item_next_arrival_date"),
             create_date=record.createdDate,
             last_write_date=record.lastModifiedDate,
-            custitemnvg_image_url_text=extract_custom_field(record, "custitemnvg_image_url_text"),
+            custom_fields=record.customFieldList.customField,
         )
         return product
 
     def _get_criteria_created_since(self, created_since: datetime.datetime) -> Any:
         assert created_since
         return self.netsuite_api.Accounting.ItemSearch(
             basic=self.netsuite_api.Common.ItemSearchBasic(
@@ -506,54 +500,55 @@
             supplier=RecordRef.from_rec_named(record.entity),
             employee=record.employee and RecordRef.from_rec_named(record.employee) or None,
             total_tax_excluded=record.subTotal,
             total_tax=record.taxTotal,
             total_tax_included=record.total,
             order_date=record.tranDate,
             state=record.status,
+            custom_fields=record.customFieldList.customField,
         )
         for sub_el in record.itemList.item:
             pol = PurchaseOrderLineData(
                 name=str(sub_el.line),
                 internalId=0,
                 product=RecordRef.from_rec_named(sub_el.item),
                 expected_receipt_date=sub_el.expectedReceiptDate,
-                make_item_available=extract_custom_field(sub_el, "custcolpo_make_item_available"),
                 amount_tax_excluded=sub_el.amount,
                 amount_tax=sub_el.tax1Amt,
                 amount_tax_included=sub_el.grossAmt,
                 order_qty=sub_el.quantity,
                 recieved_qty=sub_el.quantityOnShipments,
                 billed_qty=sub_el.quantityBilled,
                 closed=sub_el.isClosed,
+                custom_fields=sub_el.customFieldList.customField,
             )
             purchase.lines.append(pol)
         return purchase
 
 
 class SaleAPI(_TransactionAPI[SaleOrderData]):
     _netsuite_ressource_name = "salesOrder"
 
     def _convert_to_data(self, record):
         sale = SaleOrderData(
             name=record.tranId,
             internalId=int(record.internalId),
+            customer=RecordRef.from_rec_named(record.entity),
             currency=RecordRef.from_rec_named(record.currency),
             supplier=RecordRef.from_rec_named(record.entity),
             total_tax_excluded=record.subTotal,
             total_tax=record.taxTotal or record.tax2Total or 0,
             total_tax_included=record.total,
             order_date=record.tranDate,
             state=record.status,
             # discountRate contient en fait des montants de réduction.
             discount_amount=record.discountRate,
             shipping_cost=record.shippingCost,
-            is_quote=extract_custom_field(record, "custbodynv_is_quote"),
             shipping_country=record.shippingAddress.country,
-            custbodynv_sales_origin=extract_custom_field(record, "custbodynv_sales_origin"),
+            custom_fields=record.customFieldList.customField,
         )
 
         for sub_el in record.itemList.item:
             sale.lines.append(
                 SaleOrderLineData(
                     name=str(sub_el.line),
                     internalId=0,
@@ -564,14 +559,15 @@
                     amount_tax_included=sub_el.grossAmt,
                     order_qty=sub_el.quantity,
                     billed_qty=sub_el.quantityBilled,
                     backordered_qty=sub_el.quantityBackOrdered,
                     committed_qty=sub_el.quantityCommitted,
                     on_hand_qty=sub_el.quantityOnHand,
                     closed=sub_el.isClosed,
+                    custom_fields=sub_el.customFieldList.customField,
                 )
             )
         return sale
 
 
 class _BaseItemStockAPI(_TransactionAPI[ItemPicking]):
     def _convert_to_data(self, record) -> ItemPicking:
@@ -629,15 +625,15 @@
                 new_quantity=sub_el.newQuantity,
                 inventory_detail=sub_el.inventoryDetail,
             )
             data.lines.append(line)
         return data
 
 
-class RelationShipAPI(BaseGsNetSuiteApi[RelationShip]):
+class VendorAPI(BaseGsNetSuiteApi[RelationShip]):
     _netsuite_ressource_name = "vendor"
 
     def _get_criteria_created_since(self, created_since: datetime.datetime) -> Any:
         raise NotImplementedError()
 
     def search_record_type(self, **construc_kwargs) -> Any:
         raise NotImplementedError()
@@ -650,9 +646,34 @@
 
     def _convert_to_data(self, record) -> RT:
         return RelationShip(
             internalId=record.internalId,
             name=record.entityId,
             company_name=record.companyName,
             email=record.email or record.altEmail,
-            custentitynv_vendor_lead_time=extract_custom_field(record, "custentitynv_vendor_lead_time"),
+            custom_fields=record.customFieldList.customField,
+        )
+
+
+class CustomerAPI(BaseGsNetSuiteApi[RelationShip]):
+    _netsuite_ressource_name = "customer"
+
+    def _get_criteria_created_since(self, created_since: datetime.datetime) -> Any:
+        raise NotImplementedError()
+
+    def search_record_type(self, **construc_kwargs) -> Any:
+        raise NotImplementedError()
+
+    def _column_search_selector(self) -> Any:
+        raise NotImplementedError()
+
+    def _default_criteria(self) -> Any:
+        raise NotImplementedError()
+
+    def _convert_to_data(self, record) -> RT:
+        return RelationShip(
+            internalId=record.internalId,
+            name=record.entityId,
+            company_name=record.companyName,
+            email=record.email or record.altEmail,
+            custom_fields=record.customFieldList.customField,
         )
```

### Comparing `gs-netsuite-api-1.1.3/src/gs_netsuite_api/data_types.py` & `gs-netsuite-api-1.2.0/src/gs_netsuite_api/data_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import dataclasses
 import datetime
-from typing import List
-
+from typing import Any, List
 
 __all__ = [
     "RecordRef",
     "ProductData",
     "ProductAvailability",
     "PurchaseOrderData",
     "PurchaseOrderLineData",
@@ -16,45 +15,49 @@
 ]
 
 
 @dataclasses.dataclass
 class RecordRef:
     internalId: int
     name: str
+    custom_fields: dict
 
     @staticmethod
     def from_rec_named(record) -> "RecordRef":
-        return RecordRef(internalId=record.internalId, name=record.name)
+        return RecordRef(internalId=record.internalId, name=record.name, custom_fields={})
+
+    def extract_custom_field(record, field_name: str) -> Any:
+        """
+        Extrait la valeur du champ `field_name` depuis l'attribut `customFieldList.customField` de `record`.
+        """
+        custom_fields = record.custom_fields or []
+        for field_dict in custom_fields:
+            if "scriptId" in field_dict and "value" in field_dict and field_dict["scriptId"] == field_name:
+                return field_dict["value"]
+        return None
 
 
 @dataclasses.dataclass
 class RelationShip(RecordRef):
     company_name: str
     email: str
-    custentitynv_vendor_lead_time: int
 
 
 @dataclasses.dataclass
 class ProductData(RecordRef):
     """
     Classe contenant les champs "Catalogue" du fichier excel
     """
 
     ean13: str
-    hs_code: str
-    price_ttc: float
     categories: List[RecordRef]
     ref: str
-    custitemnv_master_reference: str
-    custitemnv_discontinued_item: bool
     qty_available: float
-    next_arrival_date: datetime.datetime
     create_date: datetime.datetime
     last_write_date: datetime.datetime
-    custitemnvg_image_url_text: str
     availabilities: List["ProductAvailability"] = dataclasses.field(default_factory=list, repr=True)
 
 
 @dataclasses.dataclass
 class ProductAvailability:
     product: RecordRef
     location: RecordRef
@@ -71,15 +74,14 @@
     """
     FROM : transactions/purchases.xsd
     COMPLEXE_TYPE:
     """
 
     product: RecordRef
     expected_receipt_date: datetime.datetime
-    make_item_available: bool
     amount_tax_excluded: float
     amount_tax: float
     amount_tax_included: float
     order_qty: float
     recieved_qty: float
     billed_qty: float
     closed: bool
@@ -119,26 +121,25 @@
 
 @dataclasses.dataclass
 class SaleOrderData(RecordRef):
     """
     Classe contenant les champs de vente
     """
 
+    customer: RecordRef
     currency: RecordRef
     supplier: RecordRef
     total_tax_excluded: float
     total_tax: float
     total_tax_included: float
     order_date: datetime.datetime
     state: str
     discount_amount: float
     shipping_cost: float
-    is_quote: bool
     shipping_country: str
-    custbodynv_sales_origin: str
     lines: List[SaleOrderLineData] = dataclasses.field(default_factory=list, repr=True)
 
 
 @dataclasses.dataclass
 class ItemMove(RecordRef):
     """
     Class convertit depuis
```

### Comparing `gs-netsuite-api-1.1.3/src/gs_netsuite_api/ns_utils.py` & `gs-netsuite-api-1.2.0/src/gs_netsuite_api/ns_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import dataclasses
 import logging
 import os
-from typing import TypeVar, Callable, Any, Mapping
+from typing import Any, Mapping, TypeVar
 
 import zeep
-from netsuite import NetSuite, Config, TokenAuth, NetSuiteSoapApi
+from netsuite import Config, NetSuite, NetSuiteSoapApi, TokenAuth
 
 _logger = logging.getLogger(__name__)
 
 __all__ = [
-    "extract_custom_field",
     "request_with_headers",
     "search_with_pref",
     "SearchParams",
     "NetSuiteCredential",
     "assertSuccess",
 ]
 
@@ -127,17 +126,7 @@
     Assert que la reponse est en succes, sinon raise
     Et retourne la valeur de la clef de resultat
     Raises: ValueError si la reponse n'est pas en succes
     """
     if not response.status.isSuccess:
         raise ValueError(response.status)
     return getattr(response, result_key)
-
-
-def extract_custom_field(record, field_name: str, converter: Callable[[Any], Any] = None) -> Any:
-    """
-    Extrait la valeur du champ `field_name` depuis l'attribut `customFieldList.customField` de `record`.
-    """
-    for field in record.customFieldList.customField:
-        if field.scriptId == field_name:
-            return converter and converter(field.value) or field.value
-    return None
```

### Comparing `gs-netsuite-api-1.1.3/src/gs_netsuite_api.egg-info/SOURCES.txt` & `gs-netsuite-api-1.2.0/src/gs_netsuite_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 docs/modules/ROOT/nav.adoc
 docs/modules/ROOT/examples/src
 docs/modules/ROOT/examples/xsd
 docs/modules/ROOT/pages/api.adoc
 docs/modules/ROOT/pages/convertion.adoc
 docs/modules/ROOT/pages/index.adoc
 docs/modules/ROOT/pages/types.adoc
+example/sample_customer_api.py
 example/sample_item_fulfillment_api.py
 example/sample_item_receipt_api.py
 example/sample_product_api.py
 example/sample_purchase_api.py
-example/sample_relationship_api.py
 example/sample_sale_api.py
+example/sample_vendor_api.py
 output/wsdl/v2022_2_0/netsuite.wsdl
 output/xsd/activities/v2022_2_0/scheduling.xsd
 output/xsd/activities/v2022_2_0/schedulingTypes.xsd
 output/xsd/documents/v2022_2_0/fileCabinet.xsd
 output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd
 output/xsd/general/v2022_2_0/communication.xsd
 output/xsd/general/v2022_2_0/communicationTypes.xsd
```

### Comparing `gs-netsuite-api-1.1.3/wsdldownloader.py` & `gs-netsuite-api-1.2.0/wsdldownloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #! /usr/bin/env python
-from __future__ import print_function, annotations
+from __future__ import annotations, print_function
 
 import dataclasses
 import os
-from functools import cached_property
-from pathlib import Path
 import shutil
 import urllib.parse as urlparse
 import urllib.request as urlrequest
+from functools import cached_property
+from pathlib import Path
 from typing import Optional
 from xml.dom import minidom
+
 import src.gs_netsuite_api.ns_utils as ns_utils
 
 INDENT_LEVEL = 2
 
 
 @dataclasses.dataclass
 class ArgsDT:
```

