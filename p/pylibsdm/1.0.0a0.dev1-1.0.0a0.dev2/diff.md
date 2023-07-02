# Comparing `tmp/pylibsdm-1.0.0a0.dev1.tar.gz` & `tmp/pylibsdm-1.0.0a0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibsdm-1.0.0a0.dev1.tar", max compression
+gzip compressed data, was "pylibsdm-1.0.0a0.dev2.tar", max compression
```

## Comparing `pylibsdm-1.0.0a0.dev1.tar` & `pylibsdm-1.0.0a0.dev2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0        0        0        0 2023-06-23 09:22:02.460136 pylibsdm-1.0.0a0.dev1/LICENSES/
--rw-r--r--   0        0        0    24842 2023-06-23 09:22:02.460136 pylibsdm-1.0.0a0.dev1/LICENSES/LGPL-2.0-or-later.txt
--rw-r--r--   0        0        0     3627 2023-06-27 19:42:08.823943 pylibsdm-1.0.0a0.dev1/README.md
--rw-r--r--   0        0        0      116 2023-06-27 15:04:34.683120 pylibsdm-1.0.0a0.dev1/pylibsdm/__init__.py
--rw-r--r--   0        0        0      116 2023-06-27 15:04:34.703120 pylibsdm-1.0.0a0.dev1/pylibsdm/backend/__init__.py
--rw-r--r--   0        0        0     8846 2023-07-02 18:13:13.345489 pylibsdm-1.0.0a0.dev1/pylibsdm/backend/validate.py
--rw-r--r--   0        0        0     1299 2023-06-27 20:26:53.087181 pylibsdm-1.0.0a0.dev1/pylibsdm/cli/__init__.py
--rw-r--r--   0        0        0     4450 2023-07-02 18:13:37.981485 pylibsdm-1.0.0a0.dev1/pylibsdm/cli/provision.py
--rw-r--r--   0        0        0     2122 2023-06-27 20:30:02.430861 pylibsdm-1.0.0a0.dev1/pylibsdm/cli/tap.py
--rw-r--r--   0        0        0      116 2023-06-27 17:30:02.589313 pylibsdm-1.0.0a0.dev1/pylibsdm/tag/__init__.py
--rw-r--r--   0        0        0      465 2023-06-27 20:20:27.310522 pylibsdm-1.0.0a0.dev1/pylibsdm/tag/ntag424dna/__init__.py
--rw-r--r--   0        0        0      973 2023-06-27 15:04:34.739120 pylibsdm-1.0.0a0.dev1/pylibsdm/tag/ntag424dna/const.py
--rw-r--r--   0        0        0    16245 2023-07-02 18:13:07.441490 pylibsdm-1.0.0a0.dev1/pylibsdm/tag/ntag424dna/structs.py
--rw-r--r--   0        0        0    12307 2023-06-27 19:42:34.123921 pylibsdm-1.0.0a0.dev1/pylibsdm/tag/ntag424dna/tag.py
--rw-r--r--   0        0        0     1414 2023-06-27 20:20:27.346524 pylibsdm-1.0.0a0.dev1/pylibsdm/tag/tag.py
--rw-r--r--   0        0        0      221 2023-06-27 15:04:34.731120 pylibsdm-1.0.0a0.dev1/pylibsdm/util.py
--rw-r--r--   0        0        0     1613 2023-07-02 18:16:42.641446 pylibsdm-1.0.0a0.dev1/pyproject.toml
--rw-r--r--   0        0        0     4883 1970-01-01 00:00:00.000000 pylibsdm-1.0.0a0.dev1/setup.py
--rw-r--r--   0        0        0     4889 1970-01-01 00:00:00.000000 pylibsdm-1.0.0a0.dev1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-06-23 09:22:02.460136 pylibsdm-1.0.0a0.dev2/LICENSES/
+-rw-r--r--   0        0        0    24842 2023-06-23 09:22:02.460136 pylibsdm-1.0.0a0.dev2/LICENSES/LGPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     3627 2023-06-27 19:42:08.823943 pylibsdm-1.0.0a0.dev2/README.md
+-rw-r--r--   0        0        0      116 2023-06-27 15:04:34.683120 pylibsdm-1.0.0a0.dev2/pylibsdm/__init__.py
+-rw-r--r--   0        0        0      116 2023-06-27 15:04:34.703120 pylibsdm-1.0.0a0.dev2/pylibsdm/backend/__init__.py
+-rw-r--r--   0        0        0     8846 2023-07-02 19:13:51.098124 pylibsdm-1.0.0a0.dev2/pylibsdm/backend/validate.py
+-rw-r--r--   0        0        0     1299 2023-06-27 20:26:53.087181 pylibsdm-1.0.0a0.dev2/pylibsdm/cli/__init__.py
+-rw-r--r--   0        0        0     4440 2023-07-02 19:11:16.781959 pylibsdm-1.0.0a0.dev2/pylibsdm/cli/provision.py
+-rw-r--r--   0        0        0     2122 2023-06-27 20:30:02.430861 pylibsdm-1.0.0a0.dev2/pylibsdm/cli/tap.py
+-rw-r--r--   0        0        0      116 2023-06-27 17:30:02.589313 pylibsdm-1.0.0a0.dev2/pylibsdm/tag/__init__.py
+-rw-r--r--   0        0        0      465 2023-06-27 20:20:27.310522 pylibsdm-1.0.0a0.dev2/pylibsdm/tag/ntag424dna/__init__.py
+-rw-r--r--   0        0        0      973 2023-06-27 15:04:34.739120 pylibsdm-1.0.0a0.dev2/pylibsdm/tag/ntag424dna/const.py
+-rw-r--r--   0        0        0    16428 2023-07-02 19:12:47.858065 pylibsdm-1.0.0a0.dev2/pylibsdm/tag/ntag424dna/structs.py
+-rw-r--r--   0        0        0    12307 2023-06-27 19:42:34.123921 pylibsdm-1.0.0a0.dev2/pylibsdm/tag/ntag424dna/tag.py
+-rw-r--r--   0        0        0     1414 2023-06-27 20:20:27.346524 pylibsdm-1.0.0a0.dev2/pylibsdm/tag/tag.py
+-rw-r--r--   0        0        0      221 2023-06-27 15:04:34.731120 pylibsdm-1.0.0a0.dev2/pylibsdm/util.py
+-rw-r--r--   0        0        0     1619 2023-07-02 19:15:01.146177 pylibsdm-1.0.0a0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     4883 1970-01-01 00:00:00.000000 pylibsdm-1.0.0a0.dev2/setup.py
+-rw-r--r--   0        0        0     4889 1970-01-01 00:00:00.000000 pylibsdm-1.0.0a0.dev2/PKG-INFO
```

### Comparing `pylibsdm-1.0.0a0.dev1/LICENSES/LGPL-2.0-or-later.txt` & `pylibsdm-1.0.0a0.dev2/LICENSES/LGPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pylibsdm-1.0.0a0.dev1/README.md` & `pylibsdm-1.0.0a0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pylibsdm-1.0.0a0.dev1/pylibsdm/backend/validate.py` & `pylibsdm-1.0.0a0.dev2/pylibsdm/backend/validate.py`

 * *Files identical despite different names*

### Comparing `pylibsdm-1.0.0a0.dev1/pylibsdm/cli/__init__.py` & `pylibsdm-1.0.0a0.dev2/pylibsdm/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pylibsdm-1.0.0a0.dev1/pylibsdm/cli/provision.py` & `pylibsdm-1.0.0a0.dev2/pylibsdm/cli/provision.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     ctx: typer.Context,
     file_nr: int = typer.Argument(help="File number to retrieve settings for"),
     yes: bool = typer.Option(help="Confirm changing file settings", prompt=True),
 ):
     """Change settings for a file on tag"""
     if ctx.obj["json"]:
         with open(ctx.obj["json"], "rt") as json_file:
-            file_settings = ctx.obj["tag_module"].FileSettings.model_validate_json(
+            file_settings = ctx.obj["tag_module"].FileSettings.parse_raw(
                 json_file.read()
             )
     else:
         logger.critical(
             "Changing file settings is currently only possible with --json input"
         )
         raise typer.Exit(code=2)
```

### Comparing `pylibsdm-1.0.0a0.dev1/pylibsdm/cli/tap.py` & `pylibsdm-1.0.0a0.dev2/pylibsdm/cli/tap.py`

 * *Files identical despite different names*

### Comparing `pylibsdm-1.0.0a0.dev1/pylibsdm/tag/ntag424dna/const.py` & `pylibsdm-1.0.0a0.dev2/pylibsdm/tag/ntag424dna/const.py`

 * *Files identical despite different names*

### Comparing `pylibsdm-1.0.0a0.dev1/pylibsdm/tag/ntag424dna/structs.py` & `pylibsdm-1.0.0a0.dev2/pylibsdm/tag/ntag424dna/structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # SPDX-License-Identifier: LGPL-2.0-or-later
 
 """Structures for communication with NTAG424DNA"""
 
 from enum import IntEnum
 from logging import getLogger
 from struct import pack, unpack
-from typing import Optional, Self
+from types import SimpleNamespace
+from typing import Any, Optional, Self
 
-from pydantic import BaseModel, model_validator
+from pydantic import BaseModel, root_validator
 from pydantic.types import NonNegativeInt, PositiveInt
 
 logger = getLogger(__name__)
 
 
 class CommMode(IntEnum):
     """Communication mode for commands sent to PICC.
@@ -237,19 +238,22 @@
     #: Limit for read counter
     read_ctr_limit: Optional[PositiveInt] = None
 
     file_type: FileType = FileType.STANDARD_DATA
     #: Available size for file data
     file_size: Optional[PositiveInt] = None
 
-    @model_validator(mode="after")
-    def _check_combinations(cls, self: Self) -> Self:
+    @root_validator(pre=False, skip_on_failure=True)
+    def _check_combinations(cls, data: dict[str, Any]) -> dict[str, Any]:
         # ref: page 71, table 69
         logger.debug("Validating combinations of SDM options/offsets/lengths")
 
+        # FIXME Workaround to ease migration to Pydantic 2.0 style
+        self = SimpleNamespace(**data)
+
         if self.file_option.sdm_enabled:
             assert (
                 self.sdm_options is not None
             ), "SDM options must be given if SDM is enabled"
             assert (
                 self.sdm_access_rights is not None
             ), "SDM access rights must be given SDM is enabled"
@@ -313,15 +317,15 @@
                 ), "MAC offset must be greater than or equal to Enc offset + Enc length"
 
         if self.sdm_options and self.sdm_options.read_ctr_limit:
             assert (
                 self.read_ctr_limit is not None
             ), "Read counter limit must be given if enabled"
 
-        return self
+        return data
 
     def to_bytes(self) -> bytes:
         """Serialize for wire (e.g. in ChangeFileSettings).
 
         `file_type` and `file_size` are not encoded; cf. page 70, table 69.
         """
         data = b""
```

### Comparing `pylibsdm-1.0.0a0.dev1/pylibsdm/tag/ntag424dna/tag.py` & `pylibsdm-1.0.0a0.dev2/pylibsdm/tag/ntag424dna/tag.py`

 * *Files identical despite different names*

### Comparing `pylibsdm-1.0.0a0.dev1/pylibsdm/tag/tag.py` & `pylibsdm-1.0.0a0.dev2/pylibsdm/tag/tag.py`

 * *Files identical despite different names*

### Comparing `pylibsdm-1.0.0a0.dev1/pyproject.toml` & `pylibsdm-1.0.0a0.dev2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylibsdm"
-version = "1.0.0a0.dev1"
+version = "1.0.0a0.dev2"
 description = "Python library for handling Secure Dynamic Messaging (SDM) of NFC cards like the NTAG 424 DNA"
 authors = ["Dominik George <nik@naturalnet.de>"]
 repository = "https://codeberg.org/Bergblau/pylibsdm"
 license = "Apache-2.0"
 keywords = ["nfc", "ntag424"]
 readme = "README.md"
 classifiers = [
@@ -19,15 +19,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pycryptodome = "^3.18.0"
 nfcpy = "^1.0.4"
 typer = { version = "^0.9.0", optional = true, extras = ["all"] }
-pydantic = "^2.0"
+pydantic = ">=1.9,<3.0"
 
 [tool.poetry.extras]
 cli = ["typer"]
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `pylibsdm-1.0.0a0.dev1/setup.py` & `pylibsdm-1.0.0a0.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,26 @@
  'pylibsdm.tag',
  'pylibsdm.tag.ntag424dna']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['nfcpy>=1.0.4,<2.0.0', 'pycryptodome>=3.18.0,<4.0.0', 'pydantic>=2.0,<3.0']
+['nfcpy>=1.0.4,<2.0.0', 'pycryptodome>=3.18.0,<4.0.0', 'pydantic>=1.9,<3.0']
 
 extras_require = \
 {'cli': ['typer[all]>=0.9.0,<0.10.0']}
 
 entry_points = \
 {'console_scripts': ['sdmutil = pylibsdm.cli:app'],
  'pylibsdm.tags': ['ntag424dna = pylibsdm.tag.ntag424dna:Tag']}
 
 setup_kwargs = {
     'name': 'pylibsdm',
-    'version': '1.0.0a0.dev1',
+    'version': '1.0.0a0.dev2',
     'description': 'Python library for handling Secure Dynamic Messaging (SDM) of NFC cards like the NTAG 424 DNA',
     'long_description': '<!--\nSPDX-FileCopyrightText: © 2023 Dominik George <nik@velocitux.com>\n\nSPDX-License-Identifier: LGPL-2.0-or-later\n-->\n\n# pylibsdm - NFC Secure Dynamic Messaging with Python\n\npylibsdm is a Python library (SDK) for handling Secure Dynamic Messaging (SDM)\nof NFC cards with Python.\n\nSecure Dynamic Messaging is a technology that adds security features to\nNFC tags using standard mechanisms. While standard NFC data (so-called\nNDEF messages, e.g. texts, URLs, etc.) can be written to any compatible\ntag, SUN-capable tags can cryptographically sign and optionally also\nencrypt parts of the data, which can then still be read by any standard\nNFC reader.\n\n## Features\n\n* Card management / configuration\n  * Configuration of NDEF file settings (mirrors, offsets, used keys,…)\n  * Configuration of NDEF file data (URL)\n  * Provisioning of keys\n* Backend implementation for SUN (Secure Unique NFC)\n  * Decryption and validation of SDM data (mirrors)\n  * Validation of information from URI parameters\n\n## Supported tags\n\n* [NTAG 424 DNA](https://www.nxp.com/products/rfid-nfc/nfc-hf/ntag-for-tags-and-labels/ntag-424-dna-424-dna-tagtamper-advanced-security-and-privacy-for-trusted-iot-applications:NTAG424DNA)\n  ([specification](https://www.nxp.com/docs/en/application-note/AN12196.pdf))\n\n## Installation and usage\n\n`pylibsdm` is shipped as a standard Python library and cann be installed\nfrom PyPI:\n\n```sh\npip install "pylibsdm[cli]"\n```\n\nThe `cli` extra installs the `sdmutil` command-line utility, which can\nbe used as a stand-alone tool to handle tags.\n\n### Usage as a library in own code\n\nThe following examples show how to use `pylibsdm` within custom\napplications. It can, as such, be seen as an SDK for writing SUN-capable\napplications.\n\n#### Configuring a tag in code\n\nWe will configure a tag for the following behaviour:\n\n * Change app keys 1 and 2 to our own keys\n * Configure write access to NDEF data to need authentication with app key 1\n * Configure SDM to encrypt and sign data with key 2\n * Mirror encrypted PICC data (UID and read counter)\n * Mirror a CMAC for validation\n\n```python\nfrom pylibsdm.tag.ntag424dna import Tag\n\n# We need a working tag object from nfcpy\nnfc_tag = ...\n\n# Configure the SDM tag object for communication\nsdm_tag = Tag(nfc_tag)\n\n# Set current master app key nr 0 for authentication\nsdm_tag.set_key(0, b"\\x00\\x11\\x22\\x33\\x44\\x55\\x66\\x77\\x88\\x99\\xaa\\xbb\\xcc\\xdd\\xee\\xff")\n\n# Change app keys 1 and 2 for later use\nsdm_tag.change_key(1, 16 * b"\\xaa")\nsdm_tag.change_key(2, 16 * b"\\xaa")\n\n# Configure attributes for mirroring\nfile_option = FileOption(sdm_enabled=True, comm_mode=CommMode.PLAIN)\nsdm_options = SDMOptions(\n    uid=True,\n    read_ctr=True,\n    read_ctr_limit=False,\n    enc_file_data=False,\n    tt_status=False,\n    ascii_encoding=True,\n)\n\n# We configure free reading access of NDEF, writing data is limited to app key 1,\n#  and changing file settings to the master app key 0\naccess_rights = AccessRights(\n    read=AccessCondition.FREE_ACCESS,\n    write=AccessCondition.1,\n    read_write=AccessCondition.KEY_1,\n    change=AccessCondition.KEY_0,\n)\n# When reading the NDEF message, app key 2 is used for\nsdm_acceess_rights = SDMAccessRights(\n    file_read=AccessCondition.KEY_2,\n    meta_read=AccessCondition.KEY_2,\n    ctr_ret=AccessCondition.KEY_2,\n)\n\n# Aggregate options and offsets in NDEF data\nfile_settings = FileSettings(\n    file_option=file_option,\n    access_rights=access_rights,\n    sdm_options=sdm_options,\n    sdm_access_rights=sdm_acceess_rights,\n    picc_data_offset=32,\n    mac_offset=67,\n    mac_input_offset=67,\n)\nsdm_tag.change_file_settings(2, file_settings)\n```\n',
     'author': 'Dominik George',
     'author_email': 'nik@naturalnet.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/Bergblau/pylibsdm',
```

### Comparing `pylibsdm-1.0.0a0.dev1/PKG-INFO` & `pylibsdm-1.0.0a0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibsdm
-Version: 1.0.0a0.dev1
+Version: 1.0.0a0.dev2
 Summary: Python library for handling Secure Dynamic Messaging (SDM) of NFC cards like the NTAG 424 DNA
 Home-page: https://codeberg.org/Bergblau/pylibsdm
 License: Apache-2.0
 Keywords: nfc,ntag424
 Author: Dominik George
 Author-email: nik@naturalnet.de
 Requires-Python: >=3.9,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Provides-Extra: cli
 Requires-Dist: nfcpy (>=1.0.4,<2.0.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
-Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic (>=1.9,<3.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0) ; extra == "cli"
 Project-URL: Repository, https://codeberg.org/Bergblau/pylibsdm
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: © 2023 Dominik George <nik@velocitux.com>
```

