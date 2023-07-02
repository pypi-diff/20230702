# Comparing `tmp/trongrid_extractor-0.3.9.tar.gz` & `tmp/trongrid_extractor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trongrid_extractor-0.3.9.tar", max compression
+gzip compressed data, was "trongrid_extractor-0.4.0.tar", max compression
```

## Comparing `trongrid_extractor-0.3.9.tar` & `trongrid_extractor-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1216 2023-07-01 02:48:46.590358 trongrid_extractor-0.3.9/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.3.9/LICENSE
--rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.3.9/README.md
--rw-r--r--   0        0        0      710 2023-07-01 02:48:46.593961 trongrid_extractor-0.3.9/pyproject.toml
--rw-r--r--   0        0        0      459 2023-06-28 08:24:37.997172 trongrid_extractor-0.3.9/trongrid_extractor/__init__.py
--rw-r--r--   0        0        0    10593 2023-07-01 02:48:05.498975 trongrid_extractor-0.3.9/trongrid_extractor/api.py
--rw-r--r--   0        0        0      326 2023-06-29 00:31:04.580384 trongrid_extractor-0.3.9/trongrid_extractor/config.py
--rw-r--r--   0        0        0     1888 2023-07-01 01:36:13.931502 trongrid_extractor-0.3.9/trongrid_extractor/helpers/address_helpers.py
--rw-r--r--   0        0        0     2243 2023-06-28 19:11:14.811112 trongrid_extractor-0.3.9/trongrid_extractor/helpers/argument_parser.py
--rw-r--r--   0        0        0     2194 2023-06-30 02:06:04.627545 trongrid_extractor-0.3.9/trongrid_extractor/helpers/csv_helper.py
--rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.3.9/trongrid_extractor/helpers/dict_helper.py
--rw-r--r--   0        0        0      311 2023-06-30 21:31:49.148646 trongrid_extractor-0.3.9/trongrid_extractor/helpers/string_constants.py
--rw-r--r--   0        0        0     1431 2023-06-27 21:52:41.750623 trongrid_extractor-0.3.9/trongrid_extractor/helpers/time_helpers.py
--rw-r--r--   0        0        0     3097 2023-06-30 21:31:49.149188 trongrid_extractor-0.3.9/trongrid_extractor/progress_tracker.py
--rw-r--r--   0        0        0     4436 2023-07-01 02:39:18.865395 trongrid_extractor-0.3.9/trongrid_extractor/response.py
--rw-r--r--   0        0        0     4336 2023-06-28 19:40:28.066469 trongrid_extractor-0.3.9/trongrid_extractor/trc20_txn.py
--rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 trongrid_extractor-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1742 2023-07-02 01:23:16.068613 trongrid_extractor-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.4.0/README.md
+-rw-r--r--   0        0        0      710 2023-07-02 01:23:16.074603 trongrid_extractor-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      664 2023-07-02 01:06:33.646837 trongrid_extractor-0.4.0/trongrid_extractor/__init__.py
+-rw-r--r--   0        0        0    10728 2023-07-02 00:36:08.783069 trongrid_extractor-0.4.0/trongrid_extractor/api.py
+-rw-r--r--   0        0        0      256 2023-07-02 01:07:20.257342 trongrid_extractor-0.4.0/trongrid_extractor/config.py
+-rw-r--r--   0        0        0     2416 2023-07-02 00:28:20.059440 trongrid_extractor-0.4.0/trongrid_extractor/helpers/address_helpers.py
+-rw-r--r--   0        0        0     3281 2023-07-02 01:08:44.223494 trongrid_extractor-0.4.0/trongrid_extractor/helpers/argument_parser.py
+-rw-r--r--   0        0        0     2177 2023-07-01 03:19:57.513786 trongrid_extractor-0.4.0/trongrid_extractor/helpers/csv_helper.py
+-rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.4.0/trongrid_extractor/helpers/dict_helper.py
+-rw-r--r--   0        0        0      328 2023-07-02 00:33:07.504060 trongrid_extractor-0.4.0/trongrid_extractor/helpers/rich_helpers.py
+-rw-r--r--   0        0        0      408 2023-07-01 19:49:23.669130 trongrid_extractor-0.4.0/trongrid_extractor/helpers/string_constants.py
+-rw-r--r--   0        0        0     1726 2023-07-02 01:02:30.797593 trongrid_extractor-0.4.0/trongrid_extractor/helpers/time_helpers.py
+-rw-r--r--   0        0        0     4339 2023-07-02 00:33:40.029157 trongrid_extractor-0.4.0/trongrid_extractor/progress_tracker.py
+-rw-r--r--   0        0        0     1781 2023-07-01 22:52:26.788565 trongrid_extractor-0.4.0/trongrid_extractor/request_params.py
+-rw-r--r--   0        0        0     5531 2023-07-01 22:28:24.965541 trongrid_extractor-0.4.0/trongrid_extractor/response.py
+-rw-r--r--   0        0        0     4544 2023-07-02 00:25:20.662207 trongrid_extractor-0.4.0/trongrid_extractor/trc20_txn.py
+-rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 trongrid_extractor-0.4.0/PKG-INFO
```

### Comparing `trongrid_extractor-0.3.9/CHANGELOG.md` & `trongrid_extractor-0.4.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 # NEXT RELEASE
 
+# 0.4.0
+* `--resume` option automatically determines the token address from the CSV
+* `--debug` option for `extract_tron_transactions` CLI
+* `--list-symbols` option for `extract_tron_transactions` CLI
+* Accept command line args without timezone (assume UTC)
+* Log count of rows extracted.
+* Fix crash when throwing error about unable to resume from CSV
+
+### 0.3.12
+* `RequestParams` class, better logging
+
+### 0.3.11
+* Only use Rich formatted logging when running with the CLI
+
+### 0.3.10
+* Reduce verbosity of logged writes
+
 ### 0.3.9
 * Don't consider small timespan queries failures in need of rescuing if they return 0 rows.
 
 ### 0.3.8
 * Fix buggy handling of false completes
 
 ### 0.3.7
```

### Comparing `trongrid_extractor-0.3.9/README.md` & `trongrid_extractor-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.3.9/pyproject.toml` & `trongrid_extractor-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trongrid-extractor"
-version = "0.3.9"
+version = "0.4.0"
 description = "Extract transactions from the Trongrid API."
 authors = ["Chain Argos"]
 readme = "README.md"
 packages = [{include = "trongrid_extractor"}]
 homepage = "https://chainargos.com"
 
 include = [
```

### Comparing `trongrid_extractor-0.3.9/trongrid_extractor/api.py` & `trongrid_extractor-0.4.0/trongrid_extractor/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import pendulum
 from pendulum import DateTime
 
 from trongrid_extractor.config import log
+from trongrid_extractor.helpers.address_helpers import is_contract_address
 from trongrid_extractor.helpers.csv_helper import *
 from trongrid_extractor.helpers.string_constants import *
 from trongrid_extractor.helpers.time_helpers import *
 from trongrid_extractor.progress_tracker import ProgressTracker
+from trongrid_extractor.request_params import MAX_TRADES_PER_CALL, RequestParams
 from trongrid_extractor.response import Response
 from trongrid_extractor.trc20_txn import Trc20Txn
 
-MAX_TRADES_PER_CALL = 200
-
 RESCUE_DURATION_WALKBACK_SECONDS = [
     20,
     200,
     1000,
 ]
 
 ONE_SECOND_MS = 1000.0
@@ -37,91 +37,105 @@
     def __init__(self, network: str = MAINNET, api_key: str = '') -> None:
         network = '' if network == MAINNET else f".{network}"
         self.base_uri = f"https://api{network}.trongrid.io/v1/"
         self.api_key = api_key
 
     def events_for_token(
             self,
-            contract_addr: str,
+            contract_addr: Optional[str] = None,
             since: Optional[DateTime] = None,
             until: Optional[DateTime] = None,
             output_dir: Optional[Path] = Path(''),
             filename_suffix: Optional[str] = None,
             resume_csv: Optional[Path] = None,
-            event_name: Optional[str] = 'Transfer'
+            event_name: str = 'Transfer'
         ) -> Path:
         """
         Get events by contract address and write to CSV. This is the endpoint that actually works
         to get all transactions (unlike the '[CONTRACT_ADDRESS]/transactions' endpoint).
 
+          - contract_addr:   On-chain address of the token
+          - since:           Start time to retrieve
+          - until:           Start time to retrieve
+          - output_dir:      Directory to write the CSV to
+          - filename_suffix: Optional string to append to the filename
+          - resume_csv:      Path to a CSV you want to resume writing
+          - event_name:      Type of event to retrieve
+
         Test harness: https://developers.tron.network/v4.0/reference/events-by-contract-address
         """
-        contract_url = f"{self.base_uri}contracts/{contract_addr}/events"
-        log.info(f"Retrieving '{event_name}' events since {since} until {until} from '{contract_url}'")
-        params = Api.build_params(since, until, extra={'event_name': event_name})
-        log.info(f"Initial params: {params}")
-
         # Resume from CSV if requested
+        if resume_csv is None and not is_contract_address(contract_addr):
+            raise ValueError(f"Must provide a valid contract address or a CSV to resume.")
+
+        resume_from_csv = resume_csv is not None
         output_csv = resume_csv or output_csv_path(contract_addr, output_dir, filename_suffix)
-        progress_tracker = ProgressTracker(output_csv, resume_from_csv=resume_csv is not None)
-        params[MAX_TIMESTAMP] = progress_tracker.earliest_timestamp_seen_ms or params[MAX_TIMESTAMP]
+        progress_tracker = ProgressTracker(output_csv, resume_from_csv, contract_addr)
+        contract_addr = contract_addr or progress_tracker.token_address
+        log.info(f"Output CSV: '{output_csv}'")
+
+        # Setup params
+        contract_url = f"{self.base_uri}contracts/{contract_addr}/events"
+        params = RequestParams(contract_url, since, until, event_name=event_name)
+        params.max_timestamp = progress_tracker.earliest_timestamp_seen() or params.max_timestamp
 
         # Start retrieving
-        response = Response.get_response(contract_url, params)
+
+        response = Response.get_response(contract_url, params.request_params())
         retrieved_txns = progress_tracker.process_response(response.response)
         write_rows(output_csv, retrieved_txns)
         force_continue_from_rescue = False
 
         # This uses the "next_url" approach which fails after 5 pages
         while response.is_continuable_response() or force_continue_from_rescue:
             # Pull the next record
             if response.next_url() is not None:
                 response = Response.get_response(response.next_url())
             elif force_continue_from_rescue:
                 log.info(f"Forcibly continuing so making a request for {params}")
-                response = Response.get_response(contract_url, params)
+                response = Response.get_response(contract_url, params.request_params())
             else:
                 response.pretty_print()
                 raise ValueError("Unparseable response!")
 
             force_continue_from_rescue = False
 
             # Trongrid doesn't like it when you page more than 5 pages of 200 results. When the
             # "next URL" paging fails we go back to filtering by timestamp but move the
             # max_timestamp parameter back.
             if not response.was_successful():
                 log.info(f"Failed to retrieve provided next URL. Moving end timestamp and restarting...")
-                params[MAX_TIMESTAMP] = progress_tracker.earliest_timestamp_seen_ms
-                response = Response.get_response(contract_url, params)
+                params.max_timestamp = progress_tracker.earliest_timestamp_seen()
+                response = Response.get_response(contract_url, params.request_params())
             elif response.is_paging_complete():
                 log.info(f"Paging complete for {params} so will end loop...")
-                response.print_abbreviated()
 
             retrieved_txns = progress_tracker.process_response(response.response)
 
             # See comment on _rescue_extraction() but tl;dr TronGrid is broken.
-            # TODO: is this actually necessary?
+            # TODO: is this actually necessary? 2023-06-30 still seems to help sometimes.
             if len(retrieved_txns) == 0 and not response.is_continuable_response():
                 for walkback_seconds in RESCUE_DURATION_WALKBACK_SECONDS:
-                    log.warning(f"0 txns found. We seem to be stuck at {ms_to_datetime(params[MAX_TIMESTAMP])}.")
-                    log.warning(f"  (Maybe) Last request params: {params}")
+                    log.warning(f"0 txns found. We seem to be stuck at {params.max_timestamp}.")
+                    log.warning(f"  Current request params: {params}")
                     response.print_abbreviated()
 
                     # Get txns
                     retrieved_txns = self._rescue_extraction(contract_url, params, walkback_seconds)
                     retrieved_txns = progress_tracker.remove_already_processed_txns(retrieved_txns)
 
                     if len(retrieved_txns) > 0:
                         log.info(f"Rescued {len(retrieved_txns)}, forcibly continuing...")
                         force_continue_from_rescue = True
                         break
 
             write_rows(output_csv, retrieved_txns)
 
-        log.info("Extraction loop is complete; here is the last response from the api for params: {params}")
+        log.info(f"Extraction complete. Wrote {progress_tracker.number_of_rows_written()} new rows to '{output_csv}'.")
+        log.info(f"Here is the last response from the api for params: {params}")
         response.print_abbreviated()
         return output_csv
 
     def trc20_xfers_for_wallet(self, contract_addr: str, wallet_addr: str, token_type: str = TRC20) -> List[Trc20Txn]:
         """Use the TRC20 endpoint to get transfers for a particular wallet/token combo."""
         raise ValueError("Needs revision to use ProgressTracker and more.")
         wallet_url = f"{self.base_uri}accounts/{wallet_addr}/transactions/{token_type}"
@@ -152,15 +166,15 @@
         raise ValueError("This endpoint doesn't really work.")
         contract_url = f"{self.base_uri}contracts/{contract_addr}/transactions"
         params = Api.build_params(extra={'contract_address': contract_addr})
         response = Response.get_response(contract_url, params)
         return response
 
     # TODO: this might be defunct.
-    def _rescue_extraction(self, url: str, params: Dict[str, Union[str, float]], walkback: int) -> List[Trc20Txn]:
+    def _rescue_extraction(self, params: RequestParams, walkback: int) -> List[Trc20Txn]:
         """
         Try a smaller time range; maybe the "next URL" thing will work. The idea here is that the
         'next' URL paging doesn't work very well if you request a large timespan - it only lets
         you retrieve a few pages before barfing. So here we temporarily switch to a much smaller
         time range.
 
         IMPORTANT: The 'params' dict is modified by this method!
@@ -168,60 +182,43 @@
 
         Example problematic call:
              extract_tron_transactions TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t -u 2023-06-26T13:16:24+00:00
         """
         log.warning(f"Attempting rescue by requesting from max_timestamp minus {walkback} seconds...")
         log.debug(f"Params before new min_timestamp: {params}")
 
-        if params[MIN_TIMESTAMP] == params[MAX_TIMESTAMP]:
-            log.warning(f"Min and max timestamp are already the same ({ms_to_datetime(params[MIN_TIMESTAMP])})")
+        if params.min_timestamp == params.max_timestamp:
+            log.warning(f"Min and max timestamp are already the same ({params.min_timestamp})")
             return []
 
-        old_min_timestamp = params[MIN_TIMESTAMP]
-        new_min_timestamp = params[MAX_TIMESTAMP] - (walkback * 1000.0)
-        params[MIN_TIMESTAMP] = max(old_min_timestamp, new_min_timestamp)
-        response: Response = Response.get_response(url, params)
+        old_min_timestamp = params.min_timestamp
+        new_min_timestamp = params.max_timestamp.subtract(seconds=walkback)
+        params.min_timestamp = max(old_min_timestamp, new_min_timestamp)
+        response: Response = Response.get_response(params.contract_url, params.request_params())
         txns = Trc20Txn.extract_from_events(response.response)
         has_retrieved_all_pages = True
 
         while response.is_continuable_response():
             next_url = response.next_url()
             log.debug(f"Retrieving next URL '{next_url}'...")
             response = Response.get_response(next_url)
 
             if not response.was_successful():
                 log.error(f"Failed to retrieve next_url: '{next_url}'\n\nFinal response:")
                 response.pretty_print()
-                # If we fail to page all the way we need to be cautious about moving the window
+                # If we fail to page all the way we still need to get the records for the last second
                 has_retrieved_all_pages = False
                 break
 
             last_txns = Trc20Txn.extract_from_events(response.response)
             log.info(f"Rescued {len(last_txns)} more records")
             txns.extend(last_txns)
 
         if has_retrieved_all_pages:
             log.info(f"Retrieved all pages in the rescue attempt!")
-            params[MAX_TIMESTAMP] = params[MIN_TIMESTAMP] - ONE_SECOND_MS
+            params.max_timestamp = params.min_timestamp.subtract(seconds=1)
         else:
-            params[MAX_TIMESTAMP] = min([t.ms_from_epoch for t in txns])
+            params.max_timestamp = min([t.event_time() for t in txns])
 
-        params[MIN_TIMESTAMP] = old_min_timestamp
-        log.info(f"  Returning {len(txns)} transactions from _rescue_extraction(), modified params in place.")
-        log.debug(f"Modified params: {params}")
+        params.min_timestamp = old_min_timestamp
+        log.info(f"  _rescue_extraction() returning {len(txns)} txns.\nNewly modified params: {params}")
         return txns
-
-    @staticmethod
-    def build_params(
-            min_timestamp: Optional[DateTime] = None,
-            max_timestamp: Optional[DateTime] = None,
-            extra: Optional[Dict[str, Any]] = None
-        ) -> Dict[str, Union[str, float, int]]:
-        """Build params for requests. Anything besides min and max timestamp should go in 'extra'."""
-        params = {
-            'only_confirmed': 'true',
-            'limit': MAX_TRADES_PER_CALL,
-            MIN_TIMESTAMP: datetime_to_ms(min_timestamp or TRON_LAUNCH_TIME),
-            MAX_TIMESTAMP: datetime_to_ms(max_timestamp or pendulum.now('UTC').add(seconds=1))
-        }
-
-        return {**params, **(extra or {})}
```

### Comparing `trongrid_extractor-0.3.9/trongrid_extractor/helpers/address_helpers.py` & `trongrid_extractor-0.4.0/trongrid_extractor/helpers/address_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """
 https://stackoverflow.com/questions/57200685/how-to-convert-tron-address-to-different-format
 """
 import logging
 from typing import Optional
 
 import base58
+from rich.console import Console
+from rich.text import Text
 
 from trongrid_extractor.helpers.dict_helper import get_dict_key_by_value
+from trongrid_extractor.helpers.rich_helpers import console
 
 TOKEN_ADDRESSES = {
-    'TN3W4H6rK2ce4vX9YnFQHwKENnHjoxb3m9': 'BTCT',  # BTC on Tron (?!)
+    'TFczxzPhnThNSqr5by8tvxsdCFRRz6cPNq': 'APENFT',
+    'TN3W4H6rK2ce4vX9YnFQHwKENnHjoxb3m9': 'BTCT',   # BTC on Tron (?!)
     'TAFjULxiVgT4qWk6UZwjqwZXTSaGaqnVp4': 'BTT',
     'TMz2SWatiAtZVVcH2ebpsbVtYwUPT9EdjH': 'BUSD',
-    'TDyvndWuvX5xTBwHPYJi7J3Yq8pq8yh62h': 'HT',    # Huobi Token
+    'THbVQp8kMjStKNnf2iCY6NEzThKMK5aBHg': 'DOGET',  # DOGEcoin on Tron (?!)
+    'TDyvndWuvX5xTBwHPYJi7J3Yq8pq8yh62h': 'HT',     # Huobi Token
     'TCFLL5dx5ZJdKnWuesXxi1VPwjLVmWZZy9': 'JST',
     'TSSMHYeV2uE9qYH95DqyoCuNCzEL1NvU3S': 'SUN',
     'TUpMhErZL2fhh4sVNULAbNKLokS4GjC1F4': 'TUSD',
     'TEkxiTehnzSmSe2XqrBj4w32RUN966rdz8': 'USDC',
     'TPYmHEhy5n8TCEfYGqW2rPxsghSfzghPDn': 'USDD',
     'TMwFHYXLJaRUPeW6421aqXL4ZEzPRFGkGT': 'USDJ',
     'TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t': 'USDT',
@@ -43,15 +48,24 @@
 def tron_to_hex(address: str) -> str:
     """Convert a Tron base58 address to a hexadecimal string."""
     return base58.b58decode_check(address).hex()
 
 
 def is_contract_address(address: str) -> bool:
     """Returns true if it looks like a Tron contract address."""
+    if not isinstance(address, str):
+        return False
+
     return address[0] == 'T' and len(address) == 34
 
 
 def address_of_symbol(symbol: str) -> Optional[str]:
     try:
         return get_dict_key_by_value(TOKEN_ADDRESSES, symbol)
     except ValueError:
         logging.warning(f"No address found for '{symbol}'!")
+
+
+def print_symbol_addresses() -> None:
+    for symbol, address in TOKEN_ADDRESSES.items():
+        txt = Text('').append(symbol, style='cyan').append('    ').append(address, style='magenta')
+        console.print(txt)
```

### Comparing `trongrid_extractor-0.3.9/trongrid_extractor/helpers/csv_helper.py` & `trongrid_extractor-0.4.0/trongrid_extractor/helpers/csv_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def write_rows(file_path: Union[str, Path], rows: List[Trc20Txn]) -> None:
     if len(rows) == 0:
         log.warning(f"No rows to write!")
         return
 
-    log.info(f"Writing {len(rows)} rows to '{file_path}'...")
+    log.info(f"Writing {len(rows)} rows...")
     _fields = [fld.name for fld in fields(type(rows[0]))]
 
     if Path(file_path).exists():
         file_mode = 'a'
     else:
         file_mode = 'w'
```

### Comparing `trongrid_extractor-0.3.9/trongrid_extractor/helpers/time_helpers.py` & `trongrid_extractor-0.4.0/trongrid_extractor/helpers/time_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,22 @@
 
     is_valid_timestamp(timestamp)
     return timestamp.timestamp() * 1000
 
 
 def str_to_timestamp(iso_timestamp_string: str) -> DateTime:
     timestamp = DateTime.fromisoformat(iso_timestamp_string)
-    is_valid_timestamp(timestamp)
+
+    try:
+        is_valid_timestamp(timestamp)
+    except TypeError as e:
+        if "can't compare offset-naive and offset-aware datetimes" in str(e):
+            log.warning(f"No timezone provided in '{iso_timestamp_string}'. Appending +00:00 for UTC...")
+            return str_to_timestamp(iso_timestamp_string + '+00:00')
+
     return timestamp
 
 
 def is_valid_timestamp(timestamp: DateTime) -> bool:
     if timestamp < TRON_LAUNCH_TIME:
         raise ValueError(f"{timestamp} is before {TRON_LAUNCH_TIME}!")
     elif timestamp > MAX_TIME:
```

### Comparing `trongrid_extractor-0.3.9/trongrid_extractor/response.py` & `trongrid_extractor-0.4.0/trongrid_extractor/response.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import requests
 from requests_toolbelt.utils import dump
 from rich.pretty import pprint
 from tenacity import after_log, retry, stop_after_attempt, wait_exponential
 
 from trongrid_extractor.config import log
+from trongrid_extractor.request_params import RequestParams
 from trongrid_extractor.helpers.csv_helper import *
 from trongrid_extractor.helpers.string_constants import *
 from trongrid_extractor.helpers.time_helpers import *
 
 # If the distance between min and max_timestamp is less than this don't consider a 0 row
 # result a failure.
 OK_DURATION_FOR_ZERO_TXNS_MS = 10000
@@ -35,77 +36,90 @@
     @retry(wait=wait_exponential(multiplier=1, min=15, max=300), stop=stop_after_attempt(5), after=after_log(log, logging.DEBUG))
     def get_response(cls, url: str, params: Optional[Dict[str, Union[str, int, float]]] = None) -> 'Response':
         """Alternate constructor that calls the API with retries."""
         params = params or {}
 
         # If an API call yields too many rows to fit in one response a 'next URL' is given and
         # our requests use that URL without params.
-        is_new_query = MIN_TIMESTAMP in params and MAX_TIMESTAMP in params
+        is_new_query = (MIN_TIMESTAMP in params) and (MAX_TIMESTAMP in params)
 
         # Min/Max timestamps are INCLUSIVE.
         if is_new_query:
-            msg = f"Requesting records from {ms_to_datetime(params[MIN_TIMESTAMP])} to {ms_to_datetime(params[MAX_TIMESTAMP])}."
+            msg = f"New query requesting data from {ms_to_datetime(params[MIN_TIMESTAMP])} to {ms_to_datetime(params[MAX_TIMESTAMP])}."
             log.info(msg)
 
         log.debug(f"Request URL: {url}\nParams: {params}")
         raw_response = requests.get(url, headers=JSON_HEADERS, params=params)
         response = cls(raw_response, deepcopy(params))
 
+        # Sometimes TronGrid will return 0 rows for no apparent reason. Retrying usually fixes it
+        # so we throw an exception to get a tenacity retry.
+        # It also seems that if the number of responses to a query is a multiple of 200 (the page sizez)
+        # Trongrid may page through to an empty response. That case is not well handled here.
         if response.is_false_complete_response():
+            log.info("Empty response that perhaps should not be empty...")
+
             if is_new_query:
                 duration_queried_ms = params[MAX_TIMESTAMP] - params[MIN_TIMESTAMP]
+                log.info(f"{duration_queried_ms}ms duration from min to max_timestamp in query")
 
                 if duration_queried_ms <= OK_DURATION_FOR_ZERO_TXNS_MS:
-                    log.warning(f"Looks like a bad 'paging complete' response but only {duration_queried_ms}ms in range.")
+                    log.warning(f"Looks like a bad false empty response but only {duration_queried_ms}ms in range so OK.")
                     return response
 
-            msg = f"False positive reponse! {response.response}"
+            msg = f"Seems like an actual error: response shouldn't be empty. Response:\n{response.response}\n\nRetrying.."
             log.error(msg)
             response.pretty_print()
-            log.warning(dump.dump_all(response.raw_response).decode('utf-8'))
             raise ValueError(msg)
 
         return response
 
     def is_continuable_response(self) -> bool:
+        """Return True if the response contains a link to the next page via a url."""
         return self.next_url() is not None
 
     def is_paging_complete(self) -> bool:
+        """Return True if it appears that we successfully paged to the end of the query."""
         page_size = self.page_size() or 0
         return self.was_successful() and page_size > 0 and self.next_url() is None
 
     def is_false_complete_response(self) -> bool:
         """Sometimes for no reason TronGrid just returns 0 rows to a query that would otherwise return rows."""
-        return self.was_successful() and self.page_size() == 0 and DATA and self.next_url() is None
+        return self.was_successful() and self.page_size() == 0 and self.next_url() is None
 
     def was_successful(self) -> bool:
         if SUCCESS not in self.response:
             log.warning(f"No '{SUCCESS}' key found in response!\n{self.response}")
             return False
 
         success = self.response[SUCCESS]
 
         if not isinstance(success, bool):
             raise ValueError(f"{success} is of type {type(success)} instead of bool!")
 
         return success
 
     def next_url(self) -> Optional[str]:
+        """If the number of results is more than the page size Trongrid return a URL for the next page."""
         if META in self.response and LINKS in self.response[META] and NEXT in self.response[META][LINKS]:
             return self.response[META][LINKS][NEXT]
 
     def page_size(self) -> Optional[int]:
+        """Extract the number of results returned in this page of results."""
         if META in self.response and PAGE_SIZE in self.response[META]:
             return self.response[META][PAGE_SIZE]
 
     def without_data(self) -> Dict[str, Any]:
         """Return the response JSON just without the 'data' field."""
         abbreviated_response = deepcopy(self.response)
         abbreviated_response['data'] = f"[Skipping {len(self.response['data'])} elements of 'data' array]"
         return abbreviated_response
 
     def pretty_print(self) -> None:
+        log.info(f"RAW RESPONSE:")
+        log.info(dump.dump_all(self.raw_response).decode('utf-8') + "\n")
+        log.info(f"Response formatted with Rich:")
         pprint(self, expand_all=True)
         pprint(self.response, expand_all=True)
 
     def print_abbreviated(self) -> None:
         pprint(self.without_data(), expand_all=True)
```

### Comparing `trongrid_extractor-0.3.9/trongrid_extractor/trc20_txn.py` & `trongrid_extractor-0.4.0/trongrid_extractor/trc20_txn.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 """
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Tuple
 
 import pendulum
 
-from rich.console import Console
 from trongrid_extractor.config import log
 from trongrid_extractor.helpers.address_helpers import hex_to_tron
+from trongrid_extractor.helpers.rich_helpers import console
 from trongrid_extractor.helpers.string_constants import DATA, RESULT
+from trongrid_extractor.helpers.time_helpers import ms_to_datetime
 
 # Some tokens use src/dst/wad instead of from/to/value
 SRC_DST_WAD = ('src', 'dst', 'wad')
 FROM_TO_VALUE = ('from', 'to', 'value')
 
 
 @dataclass(kw_only=True)
@@ -77,15 +78,16 @@
                         block_number=int(row['block_number']),
                         transaction_id=row['transaction_id'],
                         event_index=row['event_index']
                     )
                 for row in events['data']
             ]
         except Exception:
-            Console().print_exception(show_locals=True)
+            console.print_exception(show_locals=True)
+            raise
 
         log.debug(f"Extracted {len(txns)} txns from the response...")
         return txns
 
     @classmethod
     def extract_from_wallet_transactions(cls, response: dict[str, Any]) -> List['Trc20Txn']:
         """Extract a list of txns from the Trongrid response object."""
@@ -108,12 +110,15 @@
     @staticmethod
     def identify_txn_keys(result_type: Dict[str, str]) -> Tuple[str, str, str]:
         if sorted(result_type.keys()) == sorted(SRC_DST_WAD):
             return SRC_DST_WAD
         else:
             return FROM_TO_VALUE
 
+    def event_time(self) -> pendulum.DateTime:
+        return ms_to_datetime(self.ms_from_epoch)
+
     def __str__(self) -> str:
         msg = f"Token: {self.token_address[0:10]}..., From: {self.from_address[0:10]}..."
         msg += f", To: {self.to_address[0:10]}..., ID: {self.transaction_id[0:10]}.../{self.event_index}"
         msg += f", Amount: {self.amount} (at {self.datetime})"
         return msg
```

### Comparing `trongrid_extractor-0.3.9/PKG-INFO` & `trongrid_extractor-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trongrid-extractor
-Version: 0.3.9
+Version: 0.4.0
 Summary: Extract transactions from the Trongrid API.
 Home-page: https://chainargos.com
 Author: Chain Argos
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

