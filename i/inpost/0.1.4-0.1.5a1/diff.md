# Comparing `tmp/inpost-0.1.4.tar.gz` & `tmp/inpost-0.1.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpost-0.1.4.tar", max compression
+gzip compressed data, was "inpost-0.1.5a1.tar", max compression
```

## Comparing `inpost-0.1.4.tar` & `inpost-0.1.5a1.tar`

### file list

```diff
@@ -1,29 +1,14 @@
--rw-r--r--   0        0        0      646 2023-04-25 09:56:56.661671 inpost-0.1.4/README.md
--rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.4/inpost/__init__.py
--rw-r--r--   0        0        0    55209 2023-06-24 11:24:08.133079 inpost-0.1.4/inpost/api.py
--rw-r--r--   0        0        0     3320 2023-06-24 11:18:00.607432 inpost-0.1.4/inpost/static/__init__.py
--rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.1.4/inpost/static/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3534 2023-06-24 11:12:59.058908 inpost-0.1.4/inpost/static/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.1.4/inpost/static/__pycache__/endpoints.cpython-310.pyc
--rw-r--r--   0        0        0     3638 2023-06-18 11:17:01.501585 inpost-0.1.4/inpost/static/__pycache__/endpoints.cpython-311.pyc
--rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.1.4/inpost/static/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     5477 2023-06-18 11:17:01.504918 inpost-0.1.4/inpost/static/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.1.4/inpost/static/__pycache__/friends.cpython-310.pyc
--rw-r--r--   0        0        0     3066 2023-06-18 14:14:33.201671 inpost-0.1.4/inpost/static/__pycache__/friends.cpython-311.pyc
--rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.1.4/inpost/static/__pycache__/headers.cpython-310.pyc
--rw-r--r--   0        0        0      223 2023-05-16 17:58:27.076532 inpost-0.1.4/inpost/static/__pycache__/headers.cpython-311.pyc
--rw-r--r--   0        0        0     1658 2023-06-18 11:17:01.534918 inpost-0.1.4/inpost/static/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.1.4/inpost/static/__pycache__/parcels.cpython-310.pyc
--rw-r--r--   0        0        0    65008 2023-06-24 11:12:59.105575 inpost-0.1.4/inpost/static/__pycache__/parcels.cpython-311.pyc
--rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.1.4/inpost/static/__pycache__/statuses.cpython-310.pyc
--rw-r--r--   0        0        0    11956 2023-06-24 11:12:59.148909 inpost-0.1.4/inpost/static/__pycache__/statuses.cpython-311.pyc
--rw-r--r--   0        0        0     2987 2023-06-17 20:11:38.099610 inpost-0.1.4/inpost/static/endpoints.py
--rw-r--r--   0        0        0     2617 2023-06-18 09:47:44.436586 inpost-0.1.4/inpost/static/exceptions.py
--rw-r--r--   0        0        0     1717 2023-06-18 13:52:29.830316 inpost-0.1.4/inpost/static/friends.py
--rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.4/inpost/static/headers.py
--rw-r--r--   0        0        0      839 2023-06-18 10:28:12.228334 inpost-0.1.4/inpost/static/notifications.py
--rw-r--r--   0        0        0    44755 2023-06-24 11:18:02.150775 inpost-0.1.4/inpost/static/parcels.py
--rw-r--r--   0        0        0     8052 2023-06-24 11:18:01.110768 inpost-0.1.4/inpost/static/statuses.py
--rw-r--r--   0        0        0     1425 2023-06-24 11:43:19.908612 inpost-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1525 1970-01-01 00:00:00.000000 inpost-0.1.4/setup.py
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 inpost-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1307 2023-06-24 19:18:25.396890 inpost-0.1.5a1/README.md
+-rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.1.5a1/inpost/__init__.py
+-rw-r--r--   0        0        0    59055 2023-06-24 21:34:19.057880 inpost-0.1.5a1/inpost/api.py
+-rw-r--r--   0        0        0     3541 2023-06-24 17:20:24.712098 inpost-0.1.5a1/inpost/static/__init__.py
+-rw-r--r--   0        0        0     2951 2023-06-24 16:59:22.179852 inpost-0.1.5a1/inpost/static/endpoints.py
+-rw-r--r--   0        0        0     2715 2023-06-24 17:48:43.048073 inpost-0.1.5a1/inpost/static/exceptions.py
+-rw-r--r--   0        0        0     2677 2023-06-24 21:04:10.186415 inpost-0.1.5a1/inpost/static/friends.py
+-rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.1.5a1/inpost/static/headers.py
+-rw-r--r--   0        0        0     1559 2023-06-24 20:38:42.495391 inpost-0.1.5a1/inpost/static/notifications.py
+-rw-r--r--   0        0        0    46977 2023-07-02 08:49:07.499846 inpost-0.1.5a1/inpost/static/parcels.py
+-rw-r--r--   0        0        0     8116 2023-06-24 19:22:24.781835 inpost-0.1.5a1/inpost/static/statuses.py
+-rw-r--r--   0        0        0     1517 2023-07-02 08:49:07.499846 inpost-0.1.5a1/pyproject.toml
+-rw-r--r--   0        0        0     2225 1970-01-01 00:00:00.000000 inpost-0.1.5a1/setup.py
+-rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 inpost-0.1.5a1/PKG-INFO
```

### Comparing `inpost-0.1.4/inpost/api.py` & `inpost-0.1.5a1/inpost/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,76 +29,75 @@
     Sender,
     SentParcel,
     SingleParamError,
     SmsCodeError,
     UnauthorizedError,
     UnidentifiedAPIError,
     appjson,
-    blik_status,
-    collect,
-    compartment_open,
-    compartment_status,
-    confirm_sms_code,
-    create,
-    create_blik,
-    friends,
-    friendship,
-    logout,
-    multi,
-    open_sent,
-    parcel,
-    parcel_points,
-    parcel_prices,
-    parcels,
-    refresh_token,
-    returns,
-    send_sms_code,
-    sent,
-    shared,
-    status_sent,
-    terminate_collect_session,
-    validate_friendship,
-    validate_sent,
+    blik_status_url,
+    collect_url,
+    compartment_open_url,
+    compartment_status_url,
+    confirm_sms_code_url,
+    create_blik_url,
+    create_url,
+    friendship_url,
+    logout_url,
+    multi_url,
+    open_sent_url,
+    parcel_points_url,
+    parcel_prices_url,
+    refresh_token_url,
+    returns_url,
+    send_sms_code_url,
+    sent_url,
+    shared_url,
+    status_sent_url,
+    terminate_collect_session_url,
+    tracked_url,
+    validate_friendship_url,
+    validate_sent_url,
 )
 
 
 class Inpost:
     """Python representation of an Inpost app. Essentially implements methods to manage all incoming parcels"""
 
     def __init__(self, phone_number):
         """Constructor method
 
         :param phone_number: phone number
         :type phone_number: str
-        :raises PhoneNumberError: Wrong phone number format or is not digit"""
+        :raises PhoneNumberError: Wrong phone number format or is not digit
+        """
+
         if isinstance(phone_number, int):
             phone_number = str(phone_number)
 
         if not (len(phone_number) == 9 and phone_number.isdigit()):
             raise PhoneNumberError(f"Wrong phone number format: {phone_number} (should be 9 digits)")
 
         self.phone_number: str = phone_number
         self.sms_code: str | None = None
         self.auth_token: str | None = None
         self.refr_token: str | None = None
         self.sess: ClientSession = ClientSession()
-        # self.parcel: Parcel | SentParcel | ReturnParcel | None = None
         self._log = logging.getLogger(f"{self.__class__.__name__}.{phone_number}")
 
         self._log.setLevel(level=logging.DEBUG)
         self._log.info(f"initialized inpost object with phone number {phone_number}")
 
     def __repr__(self):
         return f"{self.__class__.__name__}(phone_number={self.phone_number})"
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        return self.logout()
+        return self.disconnect()
 
     async def request(
         self,
         method: str,
         action: str,
         url: StrOrURL,
         auth: bool = True,
@@ -128,15 +127,16 @@
         :type autorefresh: bool
         :param kwargs: additional keyword arguments
         :return: response of http request
         :rtype: ClientResponse
         :raises UnauthorizedError: User not authenticated in inpost service
         :raises NotFoundError: URL not found
         :raises UnidentifiedAPIError: Unexpected things happened
-        :raises ValueError: Doubled authorization header in request"""
+        :raises ValueError: Doubled authorization header in request
+        """
 
         if auth and headers:
             if "Authorization" in headers:
                 raise ValueError("Both auth==True and Authorization in additional headers")
 
         headers_ = {} if headers is None else headers
 
@@ -169,15 +169,17 @@
     def from_dict(cls, data: dict) -> "Inpost":
         """`Classmethod` to initialize :class:`Inpost` object with dict.
         Should be used when retrieving configuration from database.
 
         :param data: User's Inpost data (e.g. phone_number, sms_code, auth_token, refr_token)
         :type data: dict
         :return: Inpost object from provided dict
-        :rtype: Inpost"""
+        :rtype: Inpost
+        """
+
         inp = cls(phone_number=data["phone_number"])
         inp.sms_code = data["sms_code"]
         inp.auth_token = data["auth_token"]
         inp.refr_token = data["refr_token"]
 
         inp._log.info("initialized by from_dict")
         return inp
@@ -185,23 +187,24 @@
     async def send_sms_code(self) -> bool:
         """Sends sms code to `Inpost.phone_number`
 
         :return: True if sms code is sent else False
         :rtype: bool
         :raises PhoneNumberError: Missing phone number
         """
+
         if not self.phone_number:  # can't log it cuz if there's no phone number no logger initialized @shrug
             raise PhoneNumberError("Phone number missing")
 
         self._log.info("sending sms code")
 
         resp = await self.request(
             method="post",
             action="send sms code",
-            url=send_sms_code,
+            url=send_sms_code_url,
             auth=False,
             headers=None,
             data={"phoneNumber": f"{self.phone_number}"},
             autorefresh=False,
         )
 
         return resp.status == 200
@@ -227,15 +230,15 @@
             raise SmsCodeError(reason=f"Wrong sms code format: {sms_code} (should be 6 digits)")
 
         self._log.info("confirming sms code")
 
         resp = await self.request(
             method="post",
             action="confirm sms code",
-            url=confirm_sms_code,
+            url=confirm_sms_code_url,
             auth=False,
             headers=appjson,
             data={"phoneNumber": self.phone_number, "smsCode": sms_code, "phoneOS": "Android"},
             autorefresh=False,
         )
 
         if resp.status == 200:
@@ -255,24 +258,25 @@
         :rtype: bool
         :raises RefreshTokenError: Missing refresh token
         :raises ReAuthenticationError: Re-authentication needed
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
         :raises UnidentifiedAPIError: Unexpected thing happened
         """
+
         self._log.info("refreshing token")
 
         if not self.refr_token:
             self._log.error("refresh token missing")
             raise RefreshTokenError(reason="Refresh token missing")
 
         resp = await self.request(
             method="post",
             action="refresh token",
-            url=refresh_token,
+            url=refresh_token_url,
             auth=False,
             headers=appjson,
             data={"refreshToken": self.refr_token, "phoneOS": "Android"},
             autorefresh=False,
         )
 
         if resp.status == 200:
@@ -291,23 +295,25 @@
         """Logouts user from inpost api service
 
         :return: True if the user is logged out
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
-        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info("logging out")
 
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
-            method="post", action="logout", url=logout, auth=True, headers=None, data=None, autorefresh=True
+            method="post", action="logout", url=logout_url, auth=True, headers=None, data=None, autorefresh=True
         )
 
         if resp.status == 200:
             self.phone_number = ""
             self.refr_token = None
             self.auth_token = None
             self.sms_code = None
@@ -316,15 +322,17 @@
 
         return False
 
     async def disconnect(self) -> bool:
         """Simplified method to logout and close user's session
 
         :return: True if user is logged out and session is closed else False
-        :raises NotAuthenticatedError: User not authenticated in inpost service"""
+        :raises NotAuthenticatedError: User not authenticated in inpost service
+        """
+
         self._log.info("disconnecting")
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         if await self.logout():
             await self.sess.close()
@@ -332,15 +340,15 @@
             return True
 
         self._log.error("could not disconnect")
         return False
 
     async def get_parcel(
         self, shipment_number: int | str, parcel_type: ParcelType = ParcelType.TRACKED, parse=False
-    ) -> dict | Parcel | SentParcel | ReturnParcel:  # TODO: make selector of which parcel we are looking for
+    ) -> dict | Parcel | SentParcel | ReturnParcel:
         """Fetches single parcel from provided shipment number
 
         :param shipment_number: Parcel's shipment number
         :type shipment_number: int | str
         :param parcel_type: Parcel type (e.g. received, sent, returned)
         :type parcel_type: ParcelType
         :param parse: if set to True method will return :class:`Parcel` else :class:`dict`
@@ -349,33 +357,34 @@
         :rtype: dict | Parcel
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
         :raises UnidentifiedAPIError: Unexpected thing happened
         :raises ParcelTypeError: Unknown parcel type selected
         """
+
         self._log.info(f"getting parcel with shipment number: {shipment_number}")
 
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         match parcel_type:
             case ParcelType.TRACKED:
                 self._log.debug(f"getting parcel type {parcel_type}")
-                url = parcels
+                url = tracked_url
             case ParcelType.SENT:
                 self._log.debug(f"getting parcel type {parcel_type}")
-                url = sent
+                url = sent_url
             case ParcelType.RETURNS:
                 self._log.debug(f"getting parcel type {parcel_type}")
-                url = returns
+                url = returns_url
             case _:
-                self._log.error(f"wrong parcel type {parcel_type}")
-                raise ParcelTypeError(reason=f"Unknown parcel type: {parcel_type}")
+                self._log.error(f"unexpected parcel type {parcel_type}")
+                raise ParcelTypeError(reason=f"Unexpected parcel type: {parcel_type}")
 
         resp = await self.request(
             method="get",
             action=f"parcel with shipment number {shipment_number}",
             url=f"{url}{shipment_number}",
             auth=True,
             headers=None,
@@ -420,31 +429,33 @@
         :type parse: bool
         :return: fetched parcels data
         :rtype: list[dict] | list[Parcel]
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises ParcelTypeError: Unknown parcel type selected
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
-        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info("getting parcels")
 
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         match parcel_type:
             case ParcelType.TRACKED:
                 self._log.debug(f"getting parcel type {parcel_type}")
-                url = parcels
+                url = tracked_url
             case ParcelType.SENT:
                 self._log.debug(f"getting parcel type {parcel_type}")
-                url = sent
+                url = sent_url
             case ParcelType.RETURNS:
                 self._log.debug(f"getting parcel type {parcel_type}")
-                url = returns
+                url = returns_url
             case _:
                 self._log.error(f"wrong parcel type {parcel_type}")
                 raise ParcelTypeError(reason=f"Unknown parcel type: {parcel_type}")
 
         async with await self.request(
             method="get", action="get parcels", url=url, auth=True, headers=None, data=None, autorefresh=True
         ) as resp:
@@ -475,25 +486,35 @@
                     _parcel
                     for _parcel in _parcels
                     if ParcelShipmentType[_parcel["shipmentType"]] in list(shipment_type)
                 )
 
             return list(_parcels) if not parse else [Parcel(parcel_data=data, logger=self._log) for data in _parcels]
 
-    async def get_multi_compartment(
-        self, multi_uuid: str | int, parse: bool = False
-    ) -> dict | List[Parcel]:  # TODO: do docs
+    async def get_multi_compartment(self, multi_uuid: str | int, parse: bool = False) -> dict | List[Parcel]:
+        """Fetches all available parcels for set `Inpost.phone_number` and optionally filters them
+
+        :param multi_uuid: multicompartment uuid
+        :type multi_uuid: str | int
+        :param parse: switch for parsing response
+        :type parse: bool
+        :return: multicompartment parcels
+        :rtype: dict | List[Parcel]
+        :raises NotAuthenticatedError: User not authenticated in inpost service
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="get",
             action=f"parcel with multi-compartment uuid {multi_uuid}",
-            url=f"{multi}{multi_uuid}",
+            url=f"{multi_url}{multi_uuid}",
             auth=True,
             headers=None,
             data=None,
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -523,15 +544,16 @@
         :raises SingleParamError: Fields shipment_number and parcel_obj filled in but only one of them is required
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises NoParcelError: Could not get parcel object from provided data
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
         :raises UnidentifiedAPIError: Unexpected thing happened
 
-        .. warning:: you must fill in only one parameter - shipment_number or parcel_obj!"""
+        .. warning:: you must fill in only one parameter - shipment_number or parcel_obj!
+        """
 
         parcel_obj_: Parcel | None = None
         if shipment_number is None is parcel_obj:
             self._log.error("none of shipment_number and parcel_obj filled in")
             raise MissingParamsError(reason="None of params are filled (one required)")
         elif shipment_number is not None is not parcel_obj:
             self._log.error("shipment_number and parcel_obj filled in")
@@ -546,15 +568,15 @@
             raise NoParcelError(reason="Could not obtain desired parcel!")
 
         self._log.info(f"collecting compartment properties for {parcel_obj_.shipment_number}")
 
         resp = await self.request(
             method="post",
             action="collect compartment properties",
-            url=collect,
+            url=collect_url,
             auth=True,
             headers=None,
             data={
                 "parcel": parcel_obj_.compartment_open_data,
                 "geoPoint": location if location is not None else parcel_obj_.mocked_location,
             },
             autorefresh=True,
@@ -573,25 +595,27 @@
         :param parcel_obj: Parcel object
         :type parcel_obj: Parcel
         :return: True if compartment gets opened
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
-        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info(f"opening compartment for {parcel_obj.shipment_number}")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action=f"open compartment for {parcel_obj.shipment_number}",
-            url=compartment_open,
+            url=compartment_open_url,
             auth=True,
             headers=None,
             data={"sessionUuid": parcel_obj.compartment_properties.session_uuid},
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -610,25 +634,27 @@
         :param expected_status: Compartment expected status
         :type expected_status: CompartmentExpectedStatus
         :return: True if actual status equals expected status else False
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
-        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info(f"checking compartment status for {parcel_obj.shipment_number}")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action="check compartment status",
-            url=compartment_status,
+            url=compartment_status_url,
             auth=True,
             headers=None,
             data={
                 "sessionUuid": parcel_obj.compartment_properties.session_uuid,
                 "expectedStatus": expected_status.name,
             },
             autorefresh=True,
@@ -647,39 +673,41 @@
         :param parcel_obj: Parcel object
         :type parcel_obj: Parcel
         :return: True if the user session is terminated
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
-        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info(f"terminating collect session for {parcel_obj.shipment_number}")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action="terminate collect session",
-            url=terminate_collect_session,
+            url=terminate_collect_session_url,
             auth=True,
             headers=None,
             data={"sessionUuid": parcel_obj.compartment_properties.session_uuid},
             autorefresh=True,
         )
         if resp.status == 200:
             self._log.debug(f"terminated collect session for {parcel_obj.shipment_number}")
             return True
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def collect(
         self, shipment_number: str | None = None, parcel_obj: Parcel | None = None, location: dict | None = None
-    ) -> bool:
+    ) -> Parcel | None:
         """Simplified method to open compartment
 
         :param shipment_number: Parcel's shipment number
         :type shipment_number: int | str | None
         :param parcel_obj: :class:`Parcel` object to obtain data from
         :type parcel_obj: Parcel | None
         :param location: Fetched parcels have to be picked from this pickup point (e.g. `GXO05M`)
@@ -689,15 +717,16 @@
         :raises SingleParamError: Fields shipment_number and parcel_obj filled in but only one of them is required
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises NoParcelError: Could not get parcel object from provided data
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
         :raises UnidentifiedAPIError: Unexpected thing happened
 
-        .. warning:: you must fill in only one parameter - shipment_number or parcel_obj!"""
+        .. warning:: you must fill in only one parameter - shipment_number or parcel_obj!
+        """
 
         if shipment_number and parcel_obj:
             self._log.error("shipment_number and parcel_obj filled in")
             raise SingleParamError(reason="Fields shipment_number and parcel_obj filled! Choose one!")
 
         if not self.auth_token:
             self._log.error("authorization token missing")
@@ -707,29 +736,31 @@
             parcel_obj = await self.get_parcel(shipment_number=shipment_number, parse=True)
 
         if parcel_obj is None:
             raise NoParcelError(reason="Could not obtain desired parcel!")
 
         self._log.info(f"collecting parcel with shipment number {parcel_obj.shipment_number}")
 
-        if await self.collect_compartment_properties(parcel_obj=parcel_obj, location=location):
-            if await self.open_compartment(parcel_obj=parcel_obj):
-                if await self.check_compartment_status(parcel_obj=parcel_obj):
-                    return True
+        if parcel_obj_ := await self.collect_compartment_properties(parcel_obj=parcel_obj, location=location):
+            if await self.open_compartment(parcel_obj=parcel_obj_):
+                if await self.check_compartment_status(parcel_obj=parcel_obj_):
+                    return parcel_obj_
 
-        return False
+        return None
 
     async def close_compartment(self, parcel_obj: Parcel) -> bool:
         """Checks whether actual compartment status and expected one matches then notifies inpost api that
-        compartment is closed
+        compartment is closed. Should be invoked after collecting parcel
 
         :param parcel_obj: Parcel object
         :type parcel_obj: Parcel
         :return: True if compartment status is closed and successfully terminates user's session else False
-        :rtype: bool"""
+        :rtype: bool
+        """
+
         self._log.info(f"closing compartment for {parcel_obj.shipment_number}")
 
         if await self.check_compartment_status(expected_status=CompartmentExpectedStatus.CLOSED, parcel_obj=parcel_obj):
             if await self.terminate_collect_session(parcel_obj=parcel_obj):
                 return True
 
         return False
@@ -740,25 +771,27 @@
         :param parcel_obj: Parcel object
         :type parcel_obj: Parcel
         :return: True if compartment gets reopened
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
-        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info(f"reopening compartment for {parcel_obj.shipment_number}")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action=f"reopen compartment for {parcel_obj.shipment_number}",
-            url=compartment_open,
+            url=compartment_open_url,
             auth=True,
             headers=None,
             data={"sessionUuid": parcel_obj.compartment_properties.session_uuid},
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -772,15 +805,15 @@
         query: str | None = None,
         latitude: float | None = None,
         longitude: float | None = None,
         per_page: int = 1000,
         operation: ParcelPointOperations = ParcelPointOperations.CREATE,
         parse: bool = True,
     ) -> dict | List[Point]:
-        """Fetches prices for inpost services
+        """Fetches parcel points for inpost services
 
         :param query: parcel point search query (e.g. GXO05M)
         :type query: str | None
         :param latitude: latitude of place we are looking for nearby parcel points
         :type latitude: float | None
         :param longitude: longitude of place we are looking for nearby parcel points
         :type longitude: float | None
@@ -793,14 +826,15 @@
         :return: :class:`dict` of prices for inpost services
         :rtype: dict
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises SingleParamError: query and location params filled, but only one is required
         :raises MissingParamsError: none of required query and location params are filled
         :raises UnidentifiedAPIError: Unexpected thing happened
         """
+
         self._log.info("getting parcel prices")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         if query is not None and (latitude is not None and longitude is not None):
@@ -815,15 +849,15 @@
             _params.update({"relative_point": f"{latitude},{longitude}"})
         else:
             raise MissingParamsError(reason="None of params are filled (one required)")
 
         resp = await self.request(
             method="get",
             action="get parcel points",
-            url=parcel_points,
+            url=parcel_points_url,
             auth=True,
             headers=None,
             params=_params,
             data=None,
             autorefresh=True,
         )
         if resp.status == 200:
@@ -832,23 +866,36 @@
                 await resp.json()
                 if not parse
                 else [Point(point_data=point, logger=self._log) for point in (await resp.json())["points"]]
             )
 
         raise UnidentifiedAPIError(reason=resp)
 
-    async def blik_status(self) -> bool:  # TODO: do docs
+    async def blik_status(self) -> bool:
+        """Checks if user has active blik session
+
+
+        :return: True if user has no active blik sessions else False
+        :rtype: bool
+        :raises NotAuthenticatedError: User not authenticated in inpost service
+        """
+
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         self._log.info("checking if user has opened blik session")
 
         resp = await self.request(
-            method="get", action="check user blik session", url=blik_status, auth=True, headers=None, autorefresh=True
+            method="get",
+            action="check user blik session",
+            url=blik_status_url,
+            auth=True,
+            headers=None,
+            autorefresh=True,
         )
 
         if resp.status == 200 and not (await resp.json())["active"]:
             self._log.debug("user has no active blik sessions")
             return True
 
         return False
@@ -857,25 +904,45 @@
         self,
         delivery_type: DeliveryType,
         parcel_size: ParcelLockerSize | ParcelCarrierSize,
         price: float | str,
         sender: Sender,
         receiver: Receiver,
         delivery_point: Point,
-    ) -> None | dict:  # TODO: do docs
+    ) -> dict | None:
+        """Fetches parcel points for inpost services
+
+        :param delivery_type: a way parcel will be delivered
+        :type delivery_type: DeliveryType
+        :param parcel_size: size of parcel
+        :type parcel_size: ParcelLockerSize | ParcelCarrierSize
+        :param price: price for chosen parcel size
+        :type price: float | str
+        :param sender: parcel sender
+        :type sender: Sender
+        :param receiver: parcel receiver
+        :type receiver: Receiver
+        :param delivery_point: parcel delivery point
+        :type delivery_point: Point
+        :return: :class:`dict` with response
+        :rtype: dict | None
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        :raises NotAuthenticatedError: User not authenticated in inpost service
+        """
+
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         self._log.info("creating new parcel")
 
         resp = await self.request(
             method="post",
             action="create parcel",
-            url=create,
+            url=create_url,
             auth=True,
             headers=None,
             data={
                 "deliveryType": delivery_type.value,
                 "parcelSize": parcel_size.name,
                 "price": price,
                 "sender": {"name": sender.sender_name, "email": sender.sender_email},
@@ -888,25 +955,39 @@
         if resp.status == 200:
             return await resp.json()
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def create_blik_session(
         self, amount: float | str, shipment_number: str, currency: str = "PLN"
-    ) -> None | dict:  # TODO: do docs
+    ) -> None | dict:
+        """Creates blik session for sending parcel
+
+        :param amount: amount of money that has to be paid
+        :type amount: float | str
+        :param shipment_number: shipment number of parcel that is being sent
+        :type shipment_number: str
+        :param currency: currency of `amount`
+        :type currency: str
+        :return: True if user has no active blik sessions else False
+        :rtype: bool
+        :raises NotAuthenticatedError: User not authenticated in inpost service
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         self._log.info(f"creating blik session for {shipment_number}")
 
         resp = await self.request(
             method="post",
             action="create blik session",
-            url=create_blik,
+            url=create_blik_url,
             auth=True,
             headers=None,
             data={
                 "shipmentNumber": shipment_number,
                 "amount": amount,
                 "currency": currency,
                 "process": "C2X",
@@ -919,19 +1000,39 @@
             self._log.debug(f"created blik session for {shipment_number}")
             return await resp.json()
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def validate_send(
         self,
+        drop_off_point: str,
         shipment_number: str | None = None,
         parcel_obj: SentParcel | None = None,
         location: dict | None = None,
-        drop_off_point: str | None = None,
-    ) -> SentParcel:  # TODO: do docs
+    ) -> SentParcel:
+        """Validates sending parcel
+
+        :param drop_off_point: parcel machine codename where you want to drop-opp parcel
+        :type drop_off_point: str
+        :param shipment_number: sent parcel shipment number
+        :type shipment_number: str | None
+        :param parcel_obj: sent parcel object
+        :type parcel_obj: SentParcel | None
+        :param location: ...
+        :type location: dict | None
+        :return: Sent parcel with filled compartment properties
+        :rtype: SentParcel
+        :raises SingleParamError: Fields shipment_number and parcel_obj filled in but only one of them is required
+        :raises NotAuthenticatedError: User not authenticated in inpost service
+        :raises NoParcelError: Could not get parcel object from provided data
+        :raises MissingParamsError: None of required shipment number and parcel object params are filled
+        :raises ValueError: Missing drop-off point
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         if not self.auth_token:
             self._log.error("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         parcel_obj_: SentParcel | None = None
         if shipment_number is None is parcel_obj:
             self._log.error("none of shipment_number and parcel_obj filled in")
@@ -949,59 +1050,60 @@
 
         if parcel_obj_ is None:
             raise NoParcelError(reason="Could not obtain parcel!")
 
         if parcel_obj_.drop_off_point is None:
             raise ValueError("Missing drop-off point!")
 
-        self._log.info(f"collecting compartment properties for {parcel_obj_.shipment_number}")
+        self._log.info(f"validating send for {parcel_obj_.shipment_number}")
 
         resp = await self.request(
             method="post",
             action="validate send parcel data",
-            url=validate_sent,
+            url=validate_sent_url,
             auth=True,
             headers=None,
             data={
                 "parcel": {
                     "shipmentNumber": parcel_obj_.shipment_number,
                     "quickSendCode": parcel_obj_.quick_send_code,
                 },
                 "geoPoint": location,
-                "boxMachineName": drop_off_point if drop_off_point is not None else parcel_obj_.drop_off_point.name,
+                "boxMachineName": drop_off_point,
             },
             autorefresh=True,
         )
 
         if resp.status == 200:
-            self._log.debug(f"collected compartment properties for {parcel_obj_.shipment_number}")
+            self._log.debug(f"validated send for for {parcel_obj_.shipment_number}")
             parcel_obj_.compartment_properties = await resp.json()
             return parcel_obj_
 
         raise UnidentifiedAPIError(reason=resp)
 
     async def open_send_compartment(self, parcel_obj: Parcel) -> bool:
         """Opens compartment on parcel that is being sent
 
         :param parcel_obj: Parcel object
         :type parcel_obj: Parcel
         :return: True if successfully opened compartment else False
         :rtype: bool
         :raises NotAuthenticatedError: User not logged in (missing auth_token)
         """
+
         self._log.info(f"opening compartment for {parcel_obj.shipment_number}")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action=f"open send compartment for {parcel_obj.shipment_number}",
-            url=open_sent,
+            url=open_sent_url,
             auth=True,
             headers=None,
             data={"sessionUuid": parcel_obj.compartment_properties.session_uuid},
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -1015,24 +1117,25 @@
 
         :param parcel_obj: Parcel object
         :type parcel_obj: SentParcel
         :return: True if successfully reopened compartment else False
         :rtype: bool
         :raises NotAuthenticatedError: User not logged in (missing auth_token)
         """
+
         self._log.info(f"reopening send compartment for {parcel_obj.shipment_number}")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action=f"reopen compartment for {parcel_obj.shipment_number}",
-            url=compartment_open,
+            url=compartment_open_url,
             auth=True,
             headers=None,
             data={"sessionUuid": parcel_obj.compartment_properties.session_uuid},
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -1051,25 +1154,27 @@
         :param expected_status: Compartment expected status
         :type expected_status: CompartmentExpectedStatus
         :return: True if actual status equals expected status else False
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
-        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info(f"checking compartment status for {parcel_obj.shipment_number}")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action="check send compartment status",
-            url=status_sent,
+            url=status_sent_url,
             auth=True,
             headers=None,
             data={
                 "sessionUuid": parcel_obj.compartment_properties.session_uuid,
                 "expectedStatus": expected_status.name,
             },
             autorefresh=True,
@@ -1086,23 +1191,31 @@
         """Fetches prices for inpost services
 
         :return: :class:`dict` of prices for inpost services
         :rtype: dict
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
-        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info("getting parcel prices")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
-            method="get", action="get prices", url=parcel_prices, auth=True, headers=None, data=None, autorefresh=True
+            method="get",
+            action="get prices",
+            url=parcel_prices_url,
+            auth=True,
+            headers=None,
+            data=None,
+            autorefresh=True,
         )
         if resp.status == 200:
             self._log.debug("got parcel prices")
             return await resp.json()
 
         raise UnidentifiedAPIError(reason=resp)
 
@@ -1112,46 +1225,60 @@
         :param parse: switch for parsing response
         :type parse: bool
         :return: :class:`dict` of user friends for inpost services
         :rtype: dict
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Phone number not found
-        :raises UnidentifiedAPIError: Unexpected thing happened"""
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info("getting friends")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
-            method="get", action="get friends", url=friendship, auth=True, headers=None, data=None, autorefresh=True
+            method="get", action="get friends", url=friendship_url, auth=True, headers=None, data=None, autorefresh=True
         )
         if resp.status == 200:
             self._log.debug("got user friends")
             _friends = await resp.json()
             return (
                 _friends
                 if not parse
                 else [Friend(friend_data=friend, logger=self._log) for friend in _friends["friends"]]
             )
 
         raise UnidentifiedAPIError(reason=resp)
 
-    async def get_parcel_friends(self, shipment_number: int | str, parse=False) -> dict:  # TODO: do docs
+    async def get_parcel_friends(self, shipment_number: int | str, parse=False) -> dict:
+        """Fetches parcel friends
+
+        :param shipment_number: shipment number of parcel that friends are fetched
+        :type shipment_number: int | str
+        :param parse: switch for parsing response
+        :type parse: bool
+        :return: dict containing friends data
+        :rtype: dict
+        :raises NotAuthenticatedError: User not authenticated in inpost service
+        :raises UnidentifiedAPIError: Unexpected thing happened
+        """
+
         self._log.info("getting parcel friends")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="get",
             action="get parcel friends",
-            url=f"{friendship}{shipment_number}",
+            url=f"{friendship_url}{shipment_number}",
             auth=True,
             headers=None,
             data=None,
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -1185,15 +1312,16 @@
         :type parse: bool
         :return: :class:`dict` with friends details
         :rtype: dict
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: User with specified phone number not found
         :raises UnidentifiedAPIError: Unexpected thing happened
-        :raises ValueError: Name length exceeds 20 characters"""
+        :raises ValueError: Name length exceeds 20 characters
+        """
 
         self._log.info("adding user friend")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
@@ -1203,15 +1331,15 @@
         if code:
             if isinstance(code, int):
                 code = str(code)
 
             resp = await self.request(
                 method="post",
                 action="add friend",
-                url=validate_friendship,
+                url=validate_friendship_url,
                 auth=True,
                 headers=None,
                 data={"invitationCode": code},
                 autorefresh=True,
             )
 
             if resp.status == 200:
@@ -1221,15 +1349,15 @@
         else:
             if isinstance(phone_number, int):
                 phone_number = str(phone_number)
 
             resp = await self.request(
                 method="post",
                 action="add friend",
-                url=friendship,
+                url=friendship_url,
                 auth=True,
                 headers=None,
                 data={"phoneNumber": phone_number, "name": name},
                 autorefresh=True,
             )
 
             if resp.status == 200:
@@ -1262,15 +1390,16 @@
         :return: True if friend is removed
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Friend not found
         :raises UnidentifiedAPIError: Unexpected thing happened
         :raises ValueError: Name length exceeds 20 characters
-        :raises MissingParamsError: none of required uuid, name or phone_number params are filled"""
+        :raises MissingParamsError: none of required uuid, name or phone_number params are filled
+        """
 
         self._log.info("removing user friend")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
@@ -1289,15 +1418,15 @@
                 uuid = next((friend["uuid"] for friend in f["friends"] if friend["phoneNumber"] == phone_number))
             else:
                 uuid = next((friend["uuid"] for friend in f["friends"] if friend["name"] == name))
 
         resp = await self.request(
             method="delete",
             action="remove user friend",
-            url=f"{friendship}{uuid}",
+            url=f"{friendship_url}{uuid}",
             auth=True,
             headers=None,
             data=None,
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -1317,15 +1446,16 @@
         :type phone_number: str | int | None
         :return: True if friend is updated
         :rtype: bool
         :raises NotAuthenticatedError: User not authenticated in inpost service
         :raises UnauthorizedError: Unauthorized access to inpost services,
         :raises NotFoundError: Friend not found
         :raises UnidentifiedAPIError: Unexpected thing happened
-        :raises ValueError: Name length exceeds 20 characters"""
+        :raises ValueError: Name length exceeds 20 characters
+        """
 
         self._log.info("updating user friend")
 
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
@@ -1341,15 +1471,15 @@
                 return False
 
             uuid = next((friend["uuid"] for friend in obtained_friends if friend["phoneNumber"] == phone_number))
 
         resp = await self.request(
             method="patch",
             action="update user friend",
-            url=f"{friends}{uuid}",
+            url=f"{friendship_url}{uuid}",
             auth=True,
             headers=None,
             data=None,
             autorefresh=True,
         )
 
         if resp.status == 200:
@@ -1376,15 +1506,15 @@
         if not self.auth_token:
             self._log.debug("authorization token missing")
             raise NotAuthenticatedError(reason="Not logged in")
 
         resp = await self.request(
             method="post",
             action=f"share parcel: {shipment_number}",
-            url=shared,
+            url=shared_url,
             auth=True,
             headers=None,
             data={
                 "parcels": [{"shipmentNumber": shipment_number, "friendUuids": [uuid]}],
             },
             autorefresh=True,
         )
```

### Comparing `inpost-0.1.4/inpost/static/__init__.py` & `inpost-0.1.5a1/inpost/static/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 from .endpoints import (
-    accept_friendship,
-    blik_status,
-    collect,
-    compartment_open,
-    compartment_status,
-    confirm_sent,
-    confirm_sms_code,
-    create,
-    create_blik,
-    friendship,
-    login,
-    logout,
-    multi,
-    open_sent,
-    parcel,
-    parcel_notifications,
-    parcel_points,
-    parcel_prices,
-    parcels,
-    refresh_token,
-    reopen_sent,
-    returns,
-    send_sms_code,
-    sent,
-    shared,
-    status_sent,
-    terminate_collect_session,
-    tickets,
-    validate_friendship,
-    validate_sent,
+    accept_friendship_url,
+    blik_status_url,
+    collect_url,
+    compartment_open_url,
+    compartment_status_url,
+    confirm_sent_url,
+    confirm_sms_code_url,
+    create_blik_url,
+    create_url,
+    friendship_url,
+    login_url,
+    logout_url,
+    multi_url,
+    open_sent_url,
+    parcel_notifications_url,
+    parcel_points_url,
+    parcel_prices_url,
+    refresh_token_url,
+    reopen_sent_url,
+    returns_url,
+    send_sms_code_url,
+    sent_url,
+    shared_url,
+    status_sent_url,
+    terminate_collect_session_url,
+    tickets_url,
+    tracked_url,
+    validate_friendship_url,
+    validate_sent_url,
 )
 from .exceptions import (
     MissingParamsError,
     NoParcelError,
     NotAuthenticatedError,
     NotFoundError,
     ParcelTypeError,
@@ -83,44 +82,44 @@
     PaymentStatus,
     PaymentType,
     PointType,
     ReturnsStatus,
 )
 
 __all__ = [
-    "accept_friendship",
-    "blik_status",
-    "collect",
-    "compartment_open",
-    "compartment_status",
-    "confirm_sent",
-    "confirm_sms_code",
-    "create",
-    "create_blik",
-    "friendship",
-    "login",
-    "logout",
-    "multi",
-    "open_sent",
-    "parcel",
-    "parcel_notifications",
-    "parcel_points",
-    "parcel_prices",
+    "accept_friendship_url",
+    "blik_status_url",
+    "collect_url",
+    "compartment_open_url",
+    "compartment_status_url",
+    "confirm_sent_url",
+    "confirm_sms_code_url",
+    "create_url",
+    "create_blik_url",
+    "friendship_url",
+    "login_url",
+    "logout_url",
+    "multi_url",
+    "open_sent_url",
+    "tracked_url",
+    "parcel_notifications_url",
+    "parcel_points_url",
+    "parcel_prices_url",
     "parcels",
-    "refresh_token",
-    "reopen_sent",
-    "returns",
-    "send_sms_code",
-    "sent",
-    "shared",
-    "status_sent",
-    "terminate_collect_session",
-    "tickets",
-    "validate_friendship",
-    "validate_sent",
+    "refresh_token_url",
+    "reopen_sent_url",
+    "returns_url",
+    "send_sms_code_url",
+    "sent_url",
+    "shared_url",
+    "status_sent_url",
+    "terminate_collect_session_url",
+    "tickets_url",
+    "validate_friendship_url",
+    "validate_sent_url",
     "MissingParamsError",
     "NoParcelError",
     "NotAuthenticatedError",
     "NotFoundError",
     "ParcelTypeError",
     "PhoneNumberError",
     "ReAuthenticationError",
```

### Comparing `inpost-0.1.4/inpost/static/endpoints.py` & `inpost-0.1.5a1/inpost/static/endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 # AUTH #
-login: str = "https://api-inmobile-pl.easypack24.net/v1/authenticate"
-send_sms_code: str = "https://api-inmobile-pl.easypack24.net/v1/sendSMSCode/"  # get
-confirm_sms_code: str = "https://api-inmobile-pl.easypack24.net/v1/confirmSMSCode"  # post
-logout: str = "https://api-inmobile-pl.easypack24.net/v1/logout"  # post
-refresh_token: str = "https://api-inmobile-pl.easypack24.net/v1/authenticate"  # post
+login_url: str = "https://api-inmobile-pl.easypack24.net/v1/authenticate"
+send_sms_code_url: str = "https://api-inmobile-pl.easypack24.net/v1/sendSMSCode/"  # get
+confirm_sms_code_url: str = "https://api-inmobile-pl.easypack24.net/v1/confirmSMSCode"  # post
+logout_url: str = "https://api-inmobile-pl.easypack24.net/v1/logout"  # post
+refresh_token_url: str = "https://api-inmobile-pl.easypack24.net/v1/authenticate"  # post
 
 # INCOMING PARCELS #
-parcels: str = "https://api-inmobile-pl.easypack24.net/v3/parcels/tracked"  # get
-parcel: str = "https://api-inmobile-pl.easypack24.net/v3/parcels/tracked/"  # get
-multi: str = "https://api-inmobile-pl.easypack24.net/v3/parcels/multi/"  # get
-collect: str = "https://api-inmobile-pl.easypack24.net/v1/collect/validate"  # post
-reopen: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/reopen"  # post
-compartment_open: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/open"  # post
-compartment_status: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/status"  # post
-terminate_collect_session: str = "https://api-inmobile-pl.easypack24.net/v1/collect/terminate"  # post
-shared: str = "https://api-inmobile-pl.easypack24.net/v1/parcels/shared"  # post
+tracked_url: str = "https://api-inmobile-pl.easypack24.net/v3/parcels/tracked/"  # get
+multi_url: str = "https://api-inmobile-pl.easypack24.net/v3/parcels/multi/"  # get
+collect_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/validate"  # post
+reopen_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/reopen"  # post
+compartment_open_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/open"  # post
+compartment_status_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/compartment/status"  # post
+terminate_collect_session_url: str = "https://api-inmobile-pl.easypack24.net/v1/collect/terminate"  # post
+shared_url: str = "https://api-inmobile-pl.easypack24.net/v1/parcels/shared"  # post
 
 # CREATING PARCEL #
-create: str = "https://api-inmobile-pl.easypack24.net/v1/parcels"
-points: str = "https://api-inmobile-pl.easypack24.net/v3/points"
-blik_status: str = "https://api-inmobile-pl.easypack24.net/v1/payments/blik/alias/status"
-create_blik: str = "https://api-inmobile-pl.easypack24.net/v1/payments/transactions/create/blik"
+create_url: str = "https://api-inmobile-pl.easypack24.net/v1/parcels"
+points_url: str = "https://api-inmobile-pl.easypack24.net/v3/points"
+blik_status_url: str = "https://api-inmobile-pl.easypack24.net/v1/payments/blik/alias/status"
+create_blik_url: str = "https://api-inmobile-pl.easypack24.net/v1/payments/transactions/create/blik"
 
 # OUTGOING PARCELS #
-# sent: str = 'https://api-inmobile-pl.easypack24.net/v3/parcels/sent/'  # get
-sent: str = "https://api-inmobile-pl.easypack24.net/v2/parcels/sent/"  # get
-parcel_points: str = "https://api-inmobile-pl.easypack24.net/v3/points/"  # get
-validate_sent: str = "https://api-inmobile-pl.easypack24.net/v1/send/validate/"  # post
-open_sent: str = "https://api-inmobile-pl.easypack24.net/v1/send/compartment/open"  # post
-reopen_sent: str = "https://api-inmobile-pl.easypack24.net/v1/send/compartment/reopen"  # post
-status_sent: str = "https://api-inmobile-pl.easypack24.net/v1/send/compartment/status"  # post
-confirm_sent: str = "https://api-inmobile-pl.easypack24.net/v1/send/confirm"  # post
-parcel_prices: str = "https://api-inmobile-pl.easypack24.net/v1/prices/parcels"  # get
+sent_url: str = "https://api-inmobile-pl.easypack24.net/v2/parcels/sent/"  # get
+parcel_points_url: str = "https://api-inmobile-pl.easypack24.net/v3/points/"  # get
+validate_sent_url: str = "https://api-inmobile-pl.easypack24.net/v1/send/validate/"  # post
+open_sent_url: str = "https://api-inmobile-pl.easypack24.net/v1/send/compartment/open"  # post
+reopen_sent_url: str = "https://api-inmobile-pl.easypack24.net/v1/send/compartment/reopen"  # post
+status_sent_url: str = "https://api-inmobile-pl.easypack24.net/v1/send/compartment/status"  # post
+confirm_sent_url: str = "https://api-inmobile-pl.easypack24.net/v1/send/confirm"  # post
+parcel_prices_url: str = "https://api-inmobile-pl.easypack24.net/v1/prices/parcels"  # get
 
 # RETURNS #
-returns: str = "https://api-inmobile-pl.easypack24.net/v1/returns/parcels/"  # get
-tickets: str = "https://api-inmobile-pl.easypack24.net/v1/returns/tickets"  # get
-parcel_notifications: str = "https://api-inmobile-pl.easypack24.net/v2/notifications?type=PUSH%2CNEWS%2CTILE"  # get
+returns_url: str = "https://api-inmobile-pl.easypack24.net/v1/returns/parcels/"  # get
+tickets_url: str = "https://api-inmobile-pl.easypack24.net/v1/returns/tickets"  # get
+parcel_notifications_url: str = "https://api-inmobile-pl.easypack24.net/v2/notifications?type=PUSH%2CNEWS%2CTILE"  # get
 
 # FRIENDS #
-friendship: str = "https://api-inmobile-pl.easypack24.net/v1/friends/"  # get, post, patch, delete
-validate_friendship: str = "https://api-inmobile-pl.easypack24.net/v1/invitations/validate"  # post
-accept_friendship: str = "https://api-inmobile-pl.easypack24.net/v1/invitations/accept"  # post
+friendship_url: str = "https://api-inmobile-pl.easypack24.net/v1/friends/"  # get, post, patch, delete
+validate_friendship_url: str = "https://api-inmobile-pl.easypack24.net/v1/invitations/validate"  # post
+accept_friendship_url: str = "https://api-inmobile-pl.easypack24.net/v1/invitations/accept"  # post
```

### Comparing `inpost-0.1.4/inpost/static/exceptions.py` & `inpost-0.1.5a1/inpost/static/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 
 class NoParcelError(BaseInpostError):
     """Is raised when no parcel is set in :class:`Parcel`"""
 
     pass
 
 
+class UnknownStatusError(BaseInpostError):
+    """Is raised when no status matches"""
+
+    pass
+
+
 class UnidentifiedParcelError(BaseInpostError):
     """Is raised when no other :class:`Parcel` error match"""
 
     pass
 
 
 # ----------------- API ----------------- #
```

### Comparing `inpost-0.1.4/inpost/static/friends.py` & `inpost-0.1.5a1/inpost/static/friends.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,56 @@
 import logging
 
 from arrow import Arrow, get
 
 
 class Friend:
-    def __init__(self, friend_data, logger: logging.Logger):
+    """Object representation of :class:`inpost.api.Inpost` friend
+
+    :param friend_data: :class:`dict` containing all friend data
+    :type friend_data: dict
+    :param logger: :class:`logging.Logger` parent instance
+    :type logger: logging.Logger
+    """
+
+    def __init__(self, friend_data: dict, logger: logging.Logger):
+        """Constructor method
+
+        :param friend_data: :class:`dict` containing all friend data
+        :type friend_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+
         self.uuid: str = friend_data["uuid"] if "uuid" in friend_data else None
         self.phone_number: str = friend_data["phoneNumber"]
         self.name: str = friend_data["name"]
         self._log: logging.Logger = logger.getChild(f"{self.__class__.__name__}.{self.uuid}")
         self.invitaion_code: str | None = friend_data["invitationCode"] if "invitationCode" in friend_data else None
         self.created_date: Arrow | None = get(friend_data["createdDate"]) if "createdDate" in friend_data else None
         self.expiry_date: Arrow | None = get(friend_data["expiryDate"]) if "expiryDate" in friend_data else None
 
         if self.invitaion_code:
             self._log.debug(f"created friendship with {self.name} using from_invitation")
         else:
             self._log.debug(f"created friendship with {self.name}")
 
     @classmethod
-    def from_invitation(cls, invitation_data, logger: logging.Logger):
+    def from_invitation(cls, invitation_data: dict, logger: logging.Logger):
+        """`Classmethod` to initialize :class:`Friend` from incitation.
+        Should be used when retrieving configuration from database.
+
+        :param invitation_data: :class:`dict` containing all friend data
+        :type invitation_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        :return: Friend object from provided invitation
+        :rtype: Friend
+        """
+
         return cls(
             friend_data={
                 "uuid": invitation_data["friend"]["uuid"],
                 "phoneNumber": invitation_data["friend"]["phoneNumber"],
                 "name": invitation_data["friend"]["name"],
                 "invitationCode": invitation_data["invitationCode"],
                 "createdDate": invitation_data["createdDate"],
```

### Comparing `inpost-0.1.4/inpost/static/parcels.py` & `inpost-0.1.5a1/inpost/static/parcels.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import random
 from io import BytesIO
 from typing import List, Tuple
 
 import qrcode
 from arrow import arrow, get
 
+from inpost.static.exceptions import UnknownStatusError
 from inpost.static.statuses import (
     CompartmentActualStatus,
     ParcelCarrierSize,
     ParcelDeliveryType,
     ParcelLockerSize,
     ParcelOwnership,
     ParcelShipmentType,
@@ -18,14 +19,22 @@
     PaymentType,
     PointType,
     ReturnsStatus,
 )
 
 
 class BaseParcel:
+    """Object representation of :class:`inpost.api.Inpost` parcel base. Gather things shared by all parcel types.
+
+    :param parcel_data: :class:`dict` containing all parcel data
+    :type parcel_data: dict
+    :param logger: :class:`logging.Logger` parent instance
+    :type logger: logging.Logger
+    """
+
     def __init__(self, parcel_data: dict, logger: logging.Logger):
         self.shipment_number = parcel_data.get("shipmentNumber")
         self._log: logging.Logger = logger.getChild(f"{self.__class__.__name__}.{self.shipment_number}")
         self.status: ParcelStatus = ParcelStatus[parcel_data.get("status")]
         self.expiry_date: arrow | None = get(parcel_data["expiryDate"]) if "expiryDate" in parcel_data else None
         self.operations: Operations = Operations(operations_data=parcel_data["operations"], logger=self._log)
         self.event_log: List[EventLog] = [
@@ -35,24 +44,26 @@
 
 class Parcel(BaseParcel):
     """Object representation of :class:`inpost.api.Inpost` incoming parcel
 
     :param parcel_data: :class:`dict` containing all parcel data
     :type parcel_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, parcel_data: dict, logger: logging.Logger):
         """Constructor method
 
         :param parcel_data: dict containing parcel data
         :type parcel_data: dict
         :param logger: logger instance
         :type logger: logging.Logger
         """
+
         super().__init__(parcel_data, logger)
         self._log: logging.Logger = logger.getChild(f"{self.__class__.__name__}.{self.shipment_number}")
         self.shipment_type: ParcelShipmentType = ParcelShipmentType[parcel_data.get("shipmentType")]
         self._open_code: str | None = parcel_data.get("openCode", None)
         self._qr_code: QRCode | None = (
             QRCode(qrcode_data=parcel_data["qrCode"], logger=self._log) if "qrCode" in parcel_data else None
         )
@@ -120,208 +131,271 @@
         )
 
     @property
     def open_code(self) -> str | None:
         """Returns an open code for :class:`Parcel`
 
         :return: Open code for :class:`Parcel`
-        :rtype: str"""
+        :rtype: str
+        """
+
         self._log.debug("getting open code")
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got open code")
             return self._open_code
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @property
     def generate_qr_image(self) -> BytesIO | None:
         """Returns a QR image for :class:`Parcel`
 
         :return: QR image for :class:`Parcel`
-        :rtype: BytesIO"""
+        :rtype: BytesIO
+        """
+
         self._log.debug("generating qr image")
         if self.shipment_type == ParcelShipmentType.parcel and self._qr_code is not None:
             self._log.debug("got qr image")
             return self._qr_code.qr_image
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @property
     def compartment_properties(self):
         """Returns a compartment properties for :class:`Parcel`
 
         :return: Compartment properties for :class:`Parcel`
-        :rtype: CompartmentProperties"""
+        :rtype: CompartmentProperties
+        """
+
         self._log.debug("getting comparment properties")
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got compartment properties")
             return self._compartment_properties
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @compartment_properties.setter
     def compartment_properties(self, compartmentproperties_data: dict):
         """Set compartment properties for :class:`Parcel`
 
         :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`
-        :type compartmentproperties_data: dict"""
+        :type compartmentproperties_data: dict
+        """
+
         self._log.debug(f"setting compartment properties with {compartmentproperties_data}")
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("compartment properties set")
             self._compartment_properties = CompartmentProperties(
                 compartmentproperties_data=compartmentproperties_data, logger=self._log
             )
+            return
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
 
     @property
     def compartment_location(self):
         """Returns a compartment location for :class:`Parcel`
 
         :return: Compartment location for :class:`Parcel`
-        :rtype: CompartmentLocation"""
+        :rtype: CompartmentLocation
+        """
+
         self._log.debug("getting compartment location")
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got compartment location")
             return self._compartment_properties.location if self._compartment_properties else None
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @compartment_location.setter
     def compartment_location(self, location_data: dict):
         """Set compartment location for :class:`Parcel`
 
         :param location_data: :class:`dict` containing `compartment properties` data for :class:`Parcel`
-        :type location_data: dict"""
+        :type location_data: dict
+        """
+
         self._log.debug(f"setting compartment location with {location_data}")
         if self.shipment_type == ParcelShipmentType.parcel and self._compartment_properties is not None:
             self._log.debug("compartment location set")
             self._compartment_properties.location = location_data
+            return
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
 
     @property
     def compartment_status(self) -> CompartmentActualStatus | None:
         """Returns a compartment status for :class:`Parcel`
 
         :return: Compartment status for :class:`Parcel`
-        :rtype: CompartmentActualStatus"""
+        :rtype: CompartmentActualStatus
+        """
+
         self._log.debug("getting compartment status")
 
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got compartment status")
             return self._compartment_properties.status if self._compartment_properties else None
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @compartment_status.setter
     def compartment_status(self, status) -> None:
+        """Set compartment location for :class:`SentParcel`
+
+        :param status: compartment properties status for :class:`SentParcel`
+        :type status: str | CompartmentActualStatus
+        """
+
         self._log.debug(f"setting compartment status with {status}")
         if self._compartment_properties is None:
-            return  # TODO: think out
+            self._log.warning("tried to assign status to empty _compartment_properties")
+            return
 
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("compartment status set")
             self._compartment_properties.status = status
+            return
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
 
     @property
     def compartment_open_data(self) -> dict | None:
         """Returns a compartment open data for :class:`Parcel`
 
         :return: dict containing compartment open data for :class:`Parcel`
-        :rtype: dict"""
+        :rtype: dict
+        """
+
         self._log.debug("getting compartment open data")
         if self.receiver is None:
-            return None  # TODO: think out
+            return None
 
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got compartment open data")
             return {
                 "shipmentNumber": self.shipment_number,
                 "openCode": self._open_code,
                 "receiverPhoneNumber": self.receiver.phone_number,
             }
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @property
     def mocked_location(self) -> dict | None:
         """Returns a mocked location for :class:`Parcel`
 
         :return: dict containing mocked location for :class:`Parcel or None if wrong parcel shipment type`
-        :rtype: dict | None"""
+        :rtype: dict | None
+        """
+
         self._log.debug("getting mocked location")
         if self.pickup_point is None:
-            return None  # TODO: think out
+            return None
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got mocked location")
             return {
                 "latitude": round(self.pickup_point.latitude + random.uniform(-0.00005, 0.00005), 6),
                 "longitude": round(self.pickup_point.longitude + random.uniform(-0.00005, 0.00005), 6),
                 "accuracy": round(random.uniform(1, 4), 1),
             }
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @property
     def is_multicompartment(self) -> bool:
         """Specifies if parcel is in multi compartment
 
         :return: True if parcel is in multicompartment
-        :rtype: bool"""
+        :rtype: bool
+        """
+
         return self.multi_compartment is not None
 
     @property
     def is_main_multicompartment(self) -> bool | None:
         """Specifies if parcel is main parcel in multi compartment
+
         :return: True if parcel is in multicompartment
-        :rtype: bool"""
+        :rtype: bool
+        """
+
         if self.is_multicompartment and self.multi_compartment is not None:
             return self.multi_compartment.shipment_numbers is not None
 
         return None
 
     @property
     def has_airsensor(self) -> bool | None:
         if self.pickup_point is not None:
             return self.pickup_point.air_sensor_data is not None
 
         return None
 
-    # @property
-    # def get_from_multicompartment(self):
-    #     return
 
+class ReturnParcel(BaseParcel):
+    # TODO: Prepare properties required to ease up access
+    """Object representation of :class:`inpost.api.Inpost` returned parcel
+
+    :param parcel_data: :class:`dict` containing all parcel data
+    :type parcel_data: dict
+    :param logger: :class:`logging.Logger` parent instance
+    :type logger: logging.Logger
+    """
 
-class ReturnParcel(BaseParcel):  # TODO: see properties and create
     def __init__(self, parcel_data: dict, logger: logging.Logger):
+        """Constructor method
+
+        :param parcel_data: dict containing parcel data
+        :type parcel_data: dict
+        :param logger: logger instance
+        :type logger: logging.Logger
+        """
+
         super().__init__(parcel_data, logger)
         self.uuid: str = parcel_data["uuid"]
         self.rma: str = parcel_data["rma"]
         self.organization_name: str = parcel_data["organizationName"]
         self.created_date: arrow = get(parcel_data["createdDate"])
         self.accepted_date: arrow = get(parcel_data["acceptedDate"])
         self.expiry_date: arrow = get(parcel_data["expiryDate"])
         self.sent_date: arrow = get(parcel_data["sentDate"])
         self.delivered_date: arrow = get(parcel_data["deliveredDate"])
         self.order_number: str = parcel_data["orderNumber"]
         self.form_type: str = parcel_data["formType"]
 
 
-class SentParcel(BaseParcel):  # TODO: check properties
+class SentParcel(BaseParcel):
+    # TODO: Recheck properties
+    """Object representation of :class:`inpost.api.Inpost` sent parcel
+
+    :param parcel_data: :class:`dict` containing all parcel data
+    :type parcel_data: dict
+    :param logger: :class:`logging.Logger` parent instance
+    :type logger: logging.Logger
+    """
+
     def __init__(self, parcel_data: dict, logger: logging.Logger):
+        """Constructor method
+
+        :param parcel_data: dict containing parcel data
+        :type parcel_data: dict
+        :param logger: logger instance
+        :type logger: logging.Logger
+        """
+
         super().__init__(parcel_data, logger)
         self.origin_system: str = parcel_data.get("originSystem", None)
         self.quick_send_code: int = parcel_data.get("quickSendCode", None)
         self._qr_code: QRCode | None = (
             QRCode(qrcode_data=parcel_data["qrCode"], logger=self._log) if "qrCode" in parcel_data else None
         )
         self.confirmation_date: arrow = get(parcel_data.get("confirmationDate", None))
@@ -352,205 +426,193 @@
         )
         self.payment: Payment | None = (
             Payment(payment_details=parcel_data["payment"], logger=self._log) if "payment" in parcel_data else None
         )
         self.unlabeled: bool = parcel_data.get("unlabeled", None)
         self.is_end_off_week_collection: bool | None = parcel_data.get("endOfWeekCollection", None)
         self.status: ParcelStatus | None = ParcelStatus[parcel_data.get("status")]
-
-    @property
-    def open_code(self) -> int | None:
-        """Returns an open code for :class:`Parcel`
-
-        :return: Open code for :class:`Parcel`
-        :rtype: int"""
-        self._log.debug("getting open code")
-        if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug("got open code")
-            return self.quick_send_code
-
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
-        return None
-
-    @property
-    def generate_qr_image(self) -> BytesIO | None:
-        """Returns a QR image for :class:`Parcel`
-
-        :return: QR image for :class:`Parcel`
-        :rtype: BytesIO"""
-        self._log.debug("generating qr image")
-        if self.shipment_type == ParcelShipmentType.parcel and self._qr_code is not None:
-            self._log.debug("got qr image")
-            return self._qr_code.qr_image
-
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
-        return None
+        self._compartment_properties: CompartmentProperties | None = None
 
     @property
     def compartment_properties(self):
-        """Returns a compartment properties for :class:`Parcel`
+        """Returns a compartment properties for :class:`SentParcel`
 
-        :return: Compartment properties for :class:`Parcel`
-        :rtype: CompartmentProperties"""
-        self._log.debug("getting comparment properties")
+        :return: Compartment properties for :class:`SentParcel`
+        :rtype: CompartmentProperties
+        """
+
+        self._log.debug("getting compartment properties")
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got compartment properties")
             return self._compartment_properties
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @compartment_properties.setter
     def compartment_properties(self, compartmentproperties_data: dict):
-        """Set compartment properties for :class:`Parcel`
+        """Set compartment properties for :class:`SentParcel`
+
+        :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`SentParcel`
+        :type compartmentproperties_data: dict
+        """
 
-        :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`
-        :type compartmentproperties_data: dict"""
         self._log.debug(f"setting compartment properties with {compartmentproperties_data}")
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("compartment properties set")
             self._compartment_properties = CompartmentProperties(
                 compartmentproperties_data=compartmentproperties_data, logger=self._log
             )
+            return
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
 
     @property
     def compartment_location(self):
-        """Returns a compartment location for :class:`Parcel`
+        """Returns a compartment location for :class:`SentParcel`
+
+        :return: Compartment location for :class:`SentParcel`
+        :rtype: CompartmentLocation
+        """
 
-        :return: Compartment location for :class:`Parcel`
-        :rtype: CompartmentLocation"""
         self._log.debug("getting compartment location")
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got compartment location")
             return self._compartment_properties.location if self._compartment_properties else None
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @compartment_location.setter
     def compartment_location(self, location_data: dict):
-        """Set compartment location for :class:`Parcel`
+        """Set compartment location for :class:`SentParcel`
         :param location_data: :class:`dict` containing `compartment properties` data for :class:`Parcel`
-        :type location_data: dict"""
+        :type location_data: dict
+        """
+
         self._log.debug(f"setting compartment location with {location_data}")
+        if self._compartment_properties is None:
+            self._log.warning("tried to assign location to empty _compartment_properties")
+            return
+
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("compartment location set")
             self._compartment_properties.location = location_data
+            return
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
 
     @property
     def compartment_status(self) -> CompartmentActualStatus | None:
-        """Returns a compartment status for :class:`Parcel`
+        """Returns a compartment status for :class:`SentParcel`
+
+        :return: Compartment status for :class:`SentParcel`
+        :rtype: CompartmentActualStatus
+        """
 
-        :return: Compartment status for :class:`Parcel`
-        :rtype: CompartmentActualStatus"""
         self._log.debug("getting compartment status")
+        if self._compartment_properties is None:
+            self._log.warning("tried to access empty _compartment_properties")
+            return None
 
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got compartment status")
             return self._compartment_properties.status if self._compartment_properties else None
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
     @compartment_status.setter
-    def compartment_status(self, status):
+    def compartment_status(self, status: str | CompartmentActualStatus):
+        """Set compartment location for :class:`SentParcel`
+
+        :param status: compartment properties status for :class:`SentParcel`
+        :type status: str | CompartmentActualStatus
+        """
+        if self._compartment_properties is None:
+            self._log.warning("tried to assign status to empty _compartment_properties")
+            return
+
         self._log.debug(f"setting compartment status with {status}")
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("compartment status set")
             self._compartment_properties.status = status
+            return
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
-
-    @property
-    def compartment_open_data(self):
-        """Returns a compartment open data for :class:`Parcel`
-
-        :return: dict containing compartment open data for :class:`Parcel`
-        :rtype: dict"""
-        self._log.debug("getting compartment open data")
-        if self.shipment_type == ParcelShipmentType.parcel:
-            self._log.debug("got compartment open data")
-            return {
-                "shipmentNumber": self.shipment_number,
-                "openCode": self._open_code,
-                "receiverPhoneNumber": self.receiver.phone_number,
-            }
-
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
-        return None
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
 
     @property
     def mocked_location(self):
-        """Returns a mocked location for :class:`Parcel`
+        """Returns a mocked location for :class:`SentParcel`
+
+        :return: dict containing mocked location for :class:`SentParcel`
+        :rtype: dict
+        """
 
-        :return: dict containing mocked location for :class:`Parcel`
-        :rtype: dict"""
         self._log.debug("getting mocked location")
         if self.shipment_type == ParcelShipmentType.parcel:
             self._log.debug("got mocked location")
             return {
                 "latitude": round(self.pickup_point.latitude + random.uniform(-0.00005, 0.00005), 6),
                 "longitude": round(self.pickup_point.longitude + random.uniform(-0.00005, 0.00005), 6),
                 "accuracy": round(random.uniform(1, 4), 1),
             }
 
-        self._log.debug(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
+        self._log.warning(f"wrong ParcelShipmentType: {repr(self.shipment_type)}")
         return None
 
-    @property
-    def has_airsensor(self) -> bool | None:
-        return self.pickup_point.air_sensor_data is not None if self.pickup_point else None
-
 
 class Receiver:
-    """Object representation of :class:`Parcel` receiver
+    """Object representation of :class:`BaseParcel` receiver
 
-    :param receiver_data: :class:`dict` containing sender data for :class:`Parcel`
+    :param receiver_data: :class:`dict` containing sender data for :class:`BaseParcel` and it's subclasses
     :type receiver_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, receiver_data: dict, logger: logging.Logger):
         """Constructor method
 
         :param receiver_data: dict containing receiver data
         :type receiver_data: dict
         :param logger: logger instance
-        :type logger: logging.Logger"""
+        :type logger: logging.Logger
+        """
+
         self.email: str = receiver_data["email"]
         self.phone_number: str = receiver_data["phoneNumber"]
         self.name: str = receiver_data["name"]
         self._log: logging.Logger = logger.getChild(self.__class__.__name__)
 
         self._log.debug("created")
 
     def __repr__(self):
         fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
         return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class Sender:
-    """Object representation of :class:`Parcel` sender
+    """Object representation of :class:`BaseParcel` sender and it's subclasses
 
-    :param sender_data: :class:`dict` containing sender data for :class:`Parcel`
+    :param sender_data: :class:`dict` containing sender data for :class:`BaseParcel` and it's subclasses
     :type sender_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, sender_data: dict, logger: logging.Logger):
         """Constructor method
 
         :param sender_data: dict containing sender data
         :type sender_data: dict
         :param logger: logger instance
-        :type logger: logging.Logger"""
+        :type logger: logging.Logger
+        """
+
         self.sender_name: str = sender_data.get("name", None)
         self.sender_email: str = sender_data.get("email", None)
         self._log: logging.Logger = logger.getChild(self.__class__.__name__)
 
         self._log.debug("created")
 
     def __repr__(self):
@@ -558,29 +620,31 @@
         return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
     def __str__(self) -> str:
         return self.sender_name
 
 
 class Point:
-    """Object representation of :class:`Parcel` point
+    """Object representation of :class:`BaseParcel` point and it's subclasses
 
-    :param point_data: :class:`dict` containing point data for :class:`Parcel`
+    :param point_data: :class:`dict` containing point data for :class:`BaseParcel` and it's subclasses
     :type point_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, point_data: dict, logger: logging.Logger):
         """Constructor method
 
-        :param point_data: :class:`dict` containing point data for :class:`Parcel`
+        :param point_data: :class:`dict` containing point data for :class:`BaseParcel` and it's subclasses
         :type point_data: dict
         :param logger: :class:`logging.Logger` parent instance
         :type logger: logging.Logger
         """
+
         self._log: logging.Logger = logger.getChild(self.__class__.__name__)
         self.name: str = point_data["name"]
         self.latitude: float = point_data["location"]["latitude"]
         self.longitude: float = point_data["location"]["longitude"]
         self.description: str = point_data["locationDescription"]
         self.opening_hours: str = point_data["openingHours"]
         self.post_code: str = point_data["addressDetails"]["postCode"]
@@ -605,66 +669,95 @@
             AirSensorData(point_data["airSensorData"], self._log) if "airSensorData" in point_data else None
         )
         self.remote_send: bool = point_data.get("remoteSend", None)
         self.remote_return: bool = point_data.get("remoteReturn", None)
 
         self._log.debug("created")
         if ParcelDeliveryType.UNKNOWN in self.type:
-            self._log.debug(f'unknown delivery type: {point_data["type"]}')
+            self._log.warning(f'unknown delivery type: {point_data["type"]}')
 
     def __repr__(self):
         fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
         return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
     def __str__(self) -> str:
         return self.name
 
     @property
     def location(self) -> Tuple[float, float]:
-        """Returns a mocked location for :class:`PickupPoint`
+        """Returns a mocked location for :class:`Point`
+
+        :return: tuple containing location for :class:`Point`
+        :rtype: tuple
+        """
 
-        :return: tuple containing location for :class:`PickupPoint`
-        :rtype: tuple"""
         self._log.debug("getting location")
         return self.latitude, self.longitude
 
 
 class PickupPoint(Point):
-    """Object representation of :class:`Parcel` pick up point
+    """Object representation of :class:`BaseParcel` and it's subclasses pick up point
 
-    :param point_data: :class:`dict` containing pickup point data for :class:`Parcel`
+    :param point_data: :class:`dict` containing pickup point data for :class:`BaseParcel` and it's subclasses
     :type point_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, point_data: dict, logger: logging.Logger):
+        """Constructor method
+
+        :param point_data: :class:`dict` containing pickup point data for :class:`BaseParcel` and it's subclasses
+        :type point_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
         super().__init__(point_data, logger)
 
 
 class DropOffPoint(Point):
-    """Object representation of :class:`Parcel` drop off point
+    """Object representation of :class:`BaseParcel` and it's subclasses drop off point
 
-    :param point_data: :class:`dict` containing pickup point data for :class:`Parcel`
+    :param point_data: :class:`dict` containing pickup point data for :class:`BaseParcel` and it's subclasses
     :type point_data: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, point_data: dict, logger: logging.Logger):
+        """Constructor method
+
+        :param point_data: :class:`dict` containing pickup point data for :class:`BaseParcel` and it's subclasses
+        :type point_data: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+
         super().__init__(point_data, logger)
 
 
 class DeliveryPoint:
-    """Object representation of :class: DeliveryPoint
+    """Object representation of :class:`BaseParcel` and it's subclasses delivery point
 
-    :param delivery_point: :class:`dict` containing delivery point data for :class:`DeliveryPoint`
+    :param delivery_point: :class:`dict` containing delivery point data for :class:`BaseParcel` and it's subclasses delivery point
     :type delivery_point: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, delivery_point: dict, logger: logging.Logger):
+        """Constructor method
+
+        :param delivery_point: :class:`dict` containing delivery point data for :class:`BaseParcel`
+        and it's subclasses delivery point
+        :type delivery_point: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
+
         self.name = delivery_point.get("name")
         self.company_name = delivery_point.get("companyName")
         self.post_code = delivery_point["address"]["postCode"] if "address" in delivery_point else None
         self.city = delivery_point["address"]["city"] if "address" in delivery_point else None
         self.street = delivery_point["address"]["street"] if "address" in delivery_point else None
         self.building_number = delivery_point["address"]["buildingNumber"] if "address" in delivery_point else None
         self.flat_numer = delivery_point["address"]["flatNumber"] if "address" in delivery_point else None
@@ -674,27 +767,30 @@
 
     def __repr__(self):
         fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
         return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class Payment:
-    """Object representation of :class: Payment
-    :param payment_details: :class:`dict` containing payment data for :class:`Payment`
+    """Object representation of :class:`BaseParcel` and it's subclasses payment
+
+    :param payment_details: :class:`dict` containing payment data for :class:`BaseParcel` and it's subclasses payment
     :type payment_details: dict
     :param logger: :class:`logging.Logger` parent instance
-    :type logger: logging.Logger"""
+    :type logger: logging.Logger
+    """
 
     def __init__(self, payment_details: dict, logger: logging.Logger):
-        # self.paid: bool = payment_details.get("paid")
-        # self.total_price: float = payment_details.get("totalPrice")
-        # self.insurance_price: float = payment_details.get("insurancePrice")
-        # self.end_of_week_collection_price: float = payment_details.get("endOfWeekCollectionPrice")
-        # self.shipment_discounted: bool = payment_details.get("shipmentDiscounted")
-        # self.transaction_status: str = payment_details.get("transactionStatus")
+        """Constructor method
+
+        :param payment_details: :class:`dict` containing payment data for :class:`BaseParcel` and it's subclasses payment
+        :type payment_details: dict
+        :param logger: :class:`logging.Logger` parent instance
+        :type logger: logging.Logger
+        """
 
         self.paid = payment_details.get("paid")
         self.total_price = payment_details.get("totalPrice")
         self.insurance_price = payment_details.get("insurancePrice")
         self.end_of_week_collection_price = payment_details.get("endOfWeekCollectionPrice")
         self.shipment_discounted = payment_details.get("shipmentDiscounted")
         self.transaction_status = payment_details.get("transactionStatus")
@@ -719,14 +815,15 @@
     def __init__(self, multicompartment_data: dict, logger: logging.Logger):
         """Constructor method:param multicompartment_data: :class:`dict` containing multicompartment data for :class:`Parcel`
 
         :type multicompartment_data: dict
         :param logger: :class:`logging.Logger` parent instance
         :type logger: logging.Logger
         """
+
         self.uuid = multicompartment_data["uuid"]
         self.shipment_numbers: List[str] | None = (
             multicompartment_data["shipmentNumbers"] if "shipmentNumbers" in multicompartment_data else None
         )
         self.presentation: bool = multicompartment_data["presentation"]
         self.collected: bool = multicompartment_data["collected"]
 
@@ -751,14 +848,15 @@
         """Constructor method
 
         :param operations_data: :class:`dict` containing operations data for :class:`Parcel`
         :type operations_data: dict
         :param logger: :class:`logging.Logger` parent instance
         :type logger: logging.Logger
         """
+
         self.manual_archive: bool = operations_data["manualArchive"]
         self.auto_archivable_since: arrow | None = (
             get(operations_data["autoArchivableSince"]) if "autoArchivableSince" in operations_data else None
         )
         self.delete: bool = operations_data.get("delete", None)
         self.pay_to_send: bool = operations_data.get("payToSend", None)
         self.collect: bool = operations_data.get("collect", None)
@@ -792,32 +890,36 @@
     def __init__(self, eventlog_data: dict, logger: logging.Logger):
         """Constructor method
 
         :param eventlog_data: :class:`dict` containing single eventlog data for :class:`Parcel`
         :type eventlog_data: dict
         :param logger: :class:`logging.Logger` parent instance
         :type logger: logging.Logger
+        :raises UnknownStatusError: Unknown status in EventLog
         """
+
         self.type: str = eventlog_data["type"]
+        self.date: arrow = get(eventlog_data["date"])
+        self.details: dict | None = eventlog_data.get("details")
+        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
+
         if self.type == "PARCEL_STATUS":
             self.name = ParcelStatus[eventlog_data.get("name")]
         elif self.type == "RETURN_STATUS":
             self.name = ReturnsStatus[eventlog_data.get("name")]
         elif self.type == "PAYMENT":
             self.name = PaymentStatus[eventlog_data.get("name")]
         else:
-            ...
-        self.date: arrow = get(eventlog_data["date"])
-        self.details: dict | None = eventlog_data.get("details")
+            self._log.warning(f'Unknown status type {eventlog_data.get("name")}!')
+            raise UnknownStatusError(reason=eventlog_data.get("name"))
 
-        self._log: logging.Logger = logger.getChild(self.__class__.__name__)
         self._log.debug("created")
 
         if self.name == ParcelStatus.UNKNOWN or self.name == ReturnsStatus.UNKNOWN:
-            self._log.debug(f'unknown {self.type}: {eventlog_data["name"]}')
+            self._log.warning(f'unknown {self.type}: {eventlog_data["name"]}')
 
     def __repr__(self):
         fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
         return self.__class__.__name__ + str(tuple(sorted(fields))).replace("'", "")
 
 
 class SharedTo:
@@ -833,14 +935,15 @@
         """Constructor method
 
         :param sharedto_data: :class:`dict` containing shared to data for :class:`Parcel`
         :type sharedto_data: dict
         :param logger: :class:`logging.Logger` parent instance
         :type logger: logging.Logger
         """
+
         self.uuid: str = sharedto_data["uuid"]
         self.name: str = sharedto_data["name"]
         self.phone_number = sharedto_data["phoneNumber"]
 
         self._log: logging.Logger = logger.getChild(self.__class__.__name__)
         self._log.debug("created")
 
@@ -862,14 +965,15 @@
         """Constructor method
 
         :param qrcode_data: :class:`str` containing qrcode data for :class:`Parcel`
         :type qrcode_data: str
         :param logger: :class:`logging.Logger` parent instance
         :type logger: logging.Logger
         """
+
         self._qr_code = qrcode_data
 
         self._log: logging.Logger = logger.getChild(self.__class__.__name__)
         self._log.debug("created")
 
     def __repr__(self):
         fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != "_log")
@@ -877,14 +981,15 @@
 
     @property
     def qr_image(self) -> BytesIO:
         """Returns a generated QR image for :class:`QRCode`
 
         :return: QR Code image
         :rtype: BytesIO"""
+
         self._log.debug("generating qr image")
         qr = qrcode.QRCode(
             version=3, error_correction=qrcode.constants.ERROR_CORRECT_H, box_size=20, border=4, mask_pattern=5
         )
 
         qr.add_data(self._qr_code)
         qr.make(fit=False)
@@ -910,14 +1015,15 @@
         """Constructor method
 
         :param compartmentlocation_data: :class:`dict` containing compartment location data for :class:`Parcel`
         :type compartmentlocation_data: dict
         :param logger: :class:`logging.Logger` parent instance
         :type logger: logging.Logger
         """
+
         self.name: str = compartmentlocation_data["compartment"]["name"]
         self.side: str = compartmentlocation_data["compartment"]["location"]["side"]
         self.column: str = compartmentlocation_data["compartment"]["location"]["column"]
         self.row: str = compartmentlocation_data["compartment"]["location"]["row"]
         self.open_compartment_waiting_time: int = compartmentlocation_data["openCompartmentWaitingTime"]
         self.action_time: int = compartmentlocation_data["actionTime"]
         self.confirm_action_time: int = compartmentlocation_data["confirmActionTime"]
@@ -942,14 +1048,15 @@
         """Constructor method
 
         :param compartmentproperties_data: :class:`dict` containing compartment properties data for :class:`Parcel`
         :type compartmentproperties_data: dict
         :param logger: :class:`logging.Logger` parent instance
         :type logger: logging.Logger
         """
+
         self._session_uuid: str = compartmentproperties_data["sessionUuid"]
         self._session_expiration_time: int = compartmentproperties_data["sessionExpirationTime"]
         self._location: CompartmentLocation | None = None
         self._status: CompartmentActualStatus | None = None
 
         self._log: logging.Logger = logger.getChild(self.__class__.__name__)
         self._log.debug("created")
@@ -960,41 +1067,48 @@
 
     @property
     def session_uuid(self):
         """Returns a session unique identified for :class:`CompartmentProperties`
 
         :return: string containing session unique identified for :class:`CompartmentProperties`
         :rtype: str"""
+
         self._log.debug("getting session uuid")
         return self._session_uuid
 
     @property
     def location(self):
         """Returns a compartment location for :class:`CompartmentProperties`
 
         :return: compartment location for :class:`CompartmentProperties`
-        :rtype: str"""
+        :rtype: str
+        """
+
         self._log.debug("getting location")
         return self._location
 
     @location.setter
     def location(self, location_data: dict):
         """Set a compartment location for :class:`CompartmentProperties`
 
         :param location_data: dict containing compartment location data for :class:`CompartmentProperties`
-        :type location_data: dict"""
+        :type location_data: dict
+        """
+
         self._log.debug("setting location")
         self._location = CompartmentLocation(location_data, self._log)
 
     @property
     def status(self):
         """Returns a compartment status for :class:`CompartmentProperties`
 
         :return: compartment location for :class:`CompartmentProperties`
-        :rtype: CompartmentActualStatus"""
+        :rtype: CompartmentActualStatus
+        """
+
         self._log.debug("getting status")
         return self._status
 
     @status.setter
     def status(self, status_data: str | CompartmentActualStatus):
         self._log.debug("setting status")
         self._status = (
@@ -1018,14 +1132,15 @@
         """Constructor method
 
         :param airsensor_data: :class:`dict` containing air sensor data for :class:`Parcel`
         :type airsensor_data: dict
         :param logger: :class:`logging.Logger` parent instance
         :type logger: logging.Logger
         """
+
         self.updated_until: arrow = airsensor_data["updatedUntil"]
         self.air_quality: str = airsensor_data["airQuality"]
         self.temperature: float = airsensor_data["temperature"]
         self.humidity: float = airsensor_data["humidity"]
         self.pressure: float = airsensor_data["pressure"]
         self.pm25_value: float = airsensor_data["pollutants"]["pm25"]["value"]
         self.pm25_percent: float = airsensor_data["pollutants"]["pm25"]["percent"]
```

### Comparing `inpost-0.1.4/inpost/static/statuses.py` & `inpost-0.1.5a1/inpost/static/statuses.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,24 +116,26 @@
     SENT = "Wysłane"
     RETURNS = "Zwroty"
 
 
 class PointType(ParcelBase):
     """:class: `Enum` that holds point types"""
 
+    # TODO: get known what does superpop stand for
     UNKNOWN = "UNNKOWN DATA"
     PL = "Paczkomat"
-    parcel_locker_superpop = "some paczkomat or pok stuff"  # TODO: get known what does superpop stand for
+    parcel_locker_superpop = "some paczkomat or pok stuff"
     POK = "Mobilny punkt obsługi klienta"
     POP = "Punkt odbioru paczki"
 
 
 class ParcelPointOperations(ParcelBase):
     """:class: `Enum` that holds parcel operation types"""
 
+    # TODO: Probably missing something, recheck needed
     UNKNOWN = "UNNKOWN DATA"
     CREATE = "c2x-target"
     SEND = "remote-send"
 
 
 class ParcelStatus(ParcelBase):
     """:class:`Enum` that holds parcel statuses"""
@@ -181,20 +183,22 @@
     PICKUP_REMINDER_SENT_ADDRESS = "Wysłano przypomnienie o odbiorze"  # TODO: translate from app
     UNDELIVERED_WRONG_ADDRESS = "Nie dostarczono z powodu złego adresu"  # TODO: translate from app
     UNDELIVERED_COD_CASH_RECEIVER = "Nie dostarczono z powodu nieopłacenia"  # TODO: translate from app
     REDIRECT_TO_BOX = "Przekierowana do paczkomatu"  # TODO: translate from app
     CANCELED_REDIRECT_TO_BOX = "Anulowano przekierowanie do paczkomatu"  # TODO: translate from app
 
 
-class DeliveryType(ParcelBase):  # TODO: look for more types
+class DeliveryType(ParcelBase):
+    # TODO: look for more types
     UNKNOWN = "UNKNOWN DATA"
     BOX_MACHINE = "Paczkomat"
 
 
-class ReturnsStatus(ParcelBase):  # TODO: translate from app and fill missing ones
+class ReturnsStatus(ParcelBase):
+    # TODO: translate from app and fill missing ones
     ACCEPTED = "Zaakceptowano"
     USED = "Nadano"
     DELIVERED = "Dostarczono"
     UNKNOWN = "UNKNOWN DATA"
 
 
 class ParcelOwnership(ParcelBase):
```

### Comparing `inpost-0.1.4/pyproject.toml` & `inpost-0.1.5a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inpost"
-version = "0.1.4"
+version = "0.1.5a1"
 description = "Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app"
 authors = ["loboda4450 <loboda4450@gmail.com>", "MrKazik99 <mrkazik99@gmail.com>"]
 maintainers = ["loboda4450 <loboda4450@gmail.com>"]
 documentation = 'https://inpost-python.readthedocs.io/en/latest/index.html'
 repository = "https://github.com/IFOSSA/inpost-python"
 readme = "README.md"
 packages = [
@@ -17,20 +17,25 @@
         "Framework :: aiohttp",
         "Intended Audience :: Developers",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
         "Development Status :: 3 - Alpha"
     ]
 
+[tool.poetry.dev-dependencies]
+pre-commit = "^3.3.3"
+pytest = "^7.4.0"
+
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.1"
 arrow = "^1.2.3"
 qrcode = "^7.3.1"
 Pillow = "^9.4.0"
+pytest = "^7.4.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `inpost-0.1.4/PKG-INFO` & `inpost-0.1.5a1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inpost
-Version: 0.1.4
+Version: 0.1.5a1
 Summary: Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app
 Home-page: https://github.com/IFOSSA/inpost-python
 Author: loboda4450
 Author-email: loboda4450@gmail.com
 Maintainer: loboda4450
 Maintainer-email: loboda4450@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -17,52 +17,65 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.4.0,<10.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: qrcode (>=7.3.1,<8.0.0)
 Project-URL: Documentation, https://inpost-python.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/IFOSSA/inpost-python
 Description-Content-Type: text/markdown
 
+[![CodeFactor](https://www.codefactor.io/repository/github/ifossa/inpost-python/badge)](https://www.codefactor.io/repository/github/ifossa/inpost-python)
+![Code Quality](https://github.com/ifossa/inpost-python/actions/workflows/lint.yml/badge.svg?barnch=main)
+![Todos](https://github.com/ifossa/inpost-python/actions/workflows/todos.yml/badge.svg?barnch=main)
 
 # Inpost Python
 
 Fully async Inpost library using Python 3.10.
 
 
-
-
 ## Documentation
 
 [Readthedocs.io](https://inpost-python.readthedocs.io/en/latest/)
 
 
 ## Usage/Examples
 
 
 ```python
 from inpost.api import Inpost
 
-inp = await Inpost.from_phone_number('555333444')
+inp = Inpost('555333444')
 await inp.send_sms_code():
 ...
 if await inp.confirm_sms_code(123321):
    print('Congratulations, you initialized successfully!')
 ```
 
+## Before you contribute
+
+![Contributors](https://contrib.rocks/image?repo=ifossa/inpost-python)
+
+Install linters and checkers, unlinted pull requests will not be approved
+```commandline
+poetry run pre-commit install
+```
 
 ## Authors
 
 - [@loboda4450](https://www.github.com/loboda4450)
 - [@mrkazik99](https://www.github.com/mrkazik99)
 
 
 ## Used By
 
 This project is used by the following repos:
 
 [Inpost Telegram Bot](https://github.com/loboda4450/inpost-telegram-bot)
 
 
+
+## 😂 Here is a random joke that'll make you laugh!
+![Jokes Card](https://readme-jokes.vercel.app/api)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

