# Comparing `tmp/Blockthon-4.6.9.tar.gz` & `tmp/Blockthon-4.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Blockthon-4.6.9.tar", last modified: Sun Jul  2 01:38:11 2023, max compression
+gzip compressed data, was "Blockthon-4.9.6.tar", last modified: Sun Jul  2 02:31:47 2023, max compression
```

## Comparing `Blockthon-4.6.9.tar` & `Blockthon-4.9.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 01:38:11.945119 Blockthon-4.6.9/
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 01:38:11.944138 Blockthon-4.6.9/Blockthon/
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1716 2023-07-01 10:53:50.000000 Blockthon-4.6.9/Blockthon/Bitcoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:26:12.000000 Blockthon-4.6.9/Blockthon/BitcoinGold.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3810 2023-06-30 08:06:48.000000 Blockthon-4.6.9/Blockthon/Check.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:26:50.000000 Blockthon-4.6.9/Blockthon/Dash.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:29:40.000000 Blockthon-4.6.9/Blockthon/Digibyte.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:27:46.000000 Blockthon-4.6.9/Blockthon/Dogecoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:24:32.000000 Blockthon-4.6.9/Blockthon/Ethereum.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1356 2023-07-01 10:52:46.000000 Blockthon-4.6.9/Blockthon/Litecoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:30:34.000000 Blockthon-4.6.9/Blockthon/Qtum.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:30:06.000000 Blockthon-4.6.9/Blockthon/Ravencoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      455 2023-07-01 10:24:32.000000 Blockthon-4.6.9/Blockthon/Tron.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3339 2023-06-30 09:21:44.000000 Blockthon-4.6.9/Blockthon/Utils.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    13912 2023-07-01 22:48:40.000000 Blockthon-4.6.9/Blockthon/Wallet.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      581 2023-07-01 10:38:46.000000 Blockthon-4.6.9/Blockthon/__init__.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    20274 2023-07-01 06:20:10.000000 Blockthon-4.6.9/Blockthon/lib.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:31:18.000000 Blockthon-4.6.9/Blockthon/zCash.py
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 01:38:11.944797 Blockthon-4.6.9/Blockthon.egg-info/
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/PKG-INFO
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      509 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/SOURCES.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/dependency_links.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      166 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/requires.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/top_level.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 01:38:11.944992 Blockthon-4.6.9/PKG-INFO
--rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     6378 2023-07-02 01:04:09.000000 Blockthon-4.6.9/README.md
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-02 01:38:11.945163 Blockthon-4.6.9/setup.cfg
--rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     1498 2023-07-02 01:17:15.000000 Blockthon-4.6.9/setup.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 02:31:47.699440 Blockthon-4.9.6/
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 02:31:47.698354 Blockthon-4.9.6/Blockthon/
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1716 2023-07-01 10:53:50.000000 Blockthon-4.9.6/Blockthon/Bitcoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:26:12.000000 Blockthon-4.9.6/Blockthon/BitcoinGold.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3810 2023-06-30 08:06:48.000000 Blockthon-4.9.6/Blockthon/Check.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:26:50.000000 Blockthon-4.9.6/Blockthon/Dash.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:29:40.000000 Blockthon-4.9.6/Blockthon/Digibyte.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:27:46.000000 Blockthon-4.9.6/Blockthon/Dogecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:24:32.000000 Blockthon-4.9.6/Blockthon/Ethereum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1356 2023-07-01 10:52:46.000000 Blockthon-4.9.6/Blockthon/Litecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:30:34.000000 Blockthon-4.9.6/Blockthon/Qtum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:30:06.000000 Blockthon-4.9.6/Blockthon/Ravencoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      455 2023-07-01 10:24:32.000000 Blockthon-4.9.6/Blockthon/Tron.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3339 2023-06-30 09:21:44.000000 Blockthon-4.9.6/Blockthon/Utils.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    13912 2023-07-01 22:48:40.000000 Blockthon-4.9.6/Blockthon/Wallet.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      581 2023-07-01 10:38:46.000000 Blockthon-4.9.6/Blockthon/__init__.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    18089 2023-07-02 02:20:10.000000 Blockthon-4.9.6/Blockthon/lib.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:31:18.000000 Blockthon-4.9.6/Blockthon/zCash.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 02:31:47.699116 Blockthon-4.9.6/Blockthon.egg-info/
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/PKG-INFO
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      509 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      166 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/requires.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/top_level.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 02:31:47.699322 Blockthon-4.9.6/PKG-INFO
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     6378 2023-07-02 01:04:09.000000 Blockthon-4.9.6/README.md
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-02 02:31:47.699481 Blockthon-4.9.6/setup.cfg
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     1498 2023-07-02 02:31:18.000000 Blockthon-4.9.6/setup.py
```

### Comparing `Blockthon-4.6.9/Blockthon/Bitcoin.py` & `Blockthon-4.9.6/Blockthon/Bitcoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.6.9/Blockthon/Check.py` & `Blockthon-4.9.6/Blockthon/Check.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.6.9/Blockthon/Litecoin.py` & `Blockthon-4.9.6/Blockthon/Litecoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.6.9/Blockthon/Utils.py` & `Blockthon-4.9.6/Blockthon/Utils.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.6.9/Blockthon/Wallet.py` & `Blockthon-4.9.6/Blockthon/Wallet.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.6.9/Blockthon/__init__.py` & `Blockthon-4.9.6/Blockthon/__init__.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.6.9/Blockthon/lib.py` & `Blockthon-4.9.6/Blockthon/lib.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,106 +11,38 @@
     b'\xfe\xba\xae\xdc\xe6\xafH\xa0;\xbf\xd2^\x8c\xd06AA'
 )
 GROUP_ORDER_INT = 0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFEBAAEDCE6AF48A03BBFD25E8CD0364141
 KEY_SIZE = 32
 ZERO = b'\x00'
 
 
-def sh256k1(data_str: str) -> bytes:
-    return sha256(data_str).digest()
-
-
-def sh256k2(data_str: str) -> bytes:
-    return sha256(sha256(data_str).digest()).digest()
-
-
 def Base58Decode(v):
     if not isinstance(v, str):
         v = v.decode('ascii')
     dec = 0
     for char in v:
         dec = dec * 58 + BASE58_ALPHABET.index(char)
     return dec.to_bytes((dec.bit_length() + 7) // 8, 'big')
 
 
-def Base58Encode(v):
-    p, a = 1, 0
-    for c in reversed(v):
-        a += p * c
-        p = p << 8
-    string = ""
-    while a:
-        a, idx = divmod(a, 58)
-        string = BASE58_ALPHABET[idx] + string
-    for c in v:
-        if c == 0:
-            string = BASE58_ALPHABET[0] + string
-        else:
-            break
-    return string
-
-
-def Base58Encode_Check(ver, payer):
-    data = ver + payer
-    check = sh256k2(data)[:4]
-    return Base58Encode(data + check)
-
-
-def Base58Decode_Check(v):
-    bytes_data = Base58Decode(v)
-    Checksum_Actual = sh256k2(bytes_data[:-4])
-    Checksum_Expect = bytes_data[-4:]
-    if Checksum_Actual[:4] != Checksum_Expect:
-        raise ValueError("Invalid Checksum")
-    else:
-        return bytes_data[:-4]
-
-
 # Bytes To Hex
 def Hexlify(data_str: bytes) -> str:
-    """
-    convert `bytes` to `hex`
-    \n``[ bytes -> hex ]``
-
-    :param data_str:
-    :type: bytes.
-    :return: string_Hex.
-    :type: str.
-    """
     return binascii.hexlify(data_str).decode()
 
 
 # Converting Hex To Bytes
 def unHexlify(data_str: str) -> bytes:
-    """
-    received hex string and convert hex string to bytes
-    \n[ hex ---> bytes ]
-
-    :param data_str:
-    :type: str.
-    :return: bytes_data.
-    :type: str.
-    """
     return binascii.unhexlify(data_str)
 
 
 def SH256(bytes_data: bytes) -> any:
     return hashlib.sha256(bytes_data)
 
 
 def encrypt(data: str) -> str:
-    """
-    received hex string and encodec with sha256 to hex again (recompile).
-    \nhex -> hex
-
-    :param data:
-    :type: str.
-    :return: hexString.
-    :type: str.
-    """
     return SH256(unHexlify(data)).hexdigest()
 
 
 def B58enUnHex(hex_string: str) -> str:
     return base58.b58encode(unHexlify(hex_string)).decode('utf-8')
 
 
@@ -121,70 +53,39 @@
         adder = random.choice(char)
         if adder not in string:
             string += adder
     return string
 
 
 def from_int(integer: int) -> str:
-    """
-    convert number or decimal to hex
-
-    :param integer:
-    :type: int.
-    :return: hexString.
-    :type: str.
-    """
     return '{:02x}'.format(integer)
 
 
 def PVK() -> str:
-    """
-    generated random private key `hex` without repeat.
-    received string data from hexadecimal character word `abcdef1234567890`\n
-    on in string without repeat. loop process to complete 64 character\n
-    and return string hex
-
-    :return: hexString.
-    """
     key = ''
     for _ in range(6):
         norepeat = getSec()
         if norepeat not in key:
             key += norepeat
     if len(key) < 64:
         equal = (64 - len(key)) * '0'
         return equal + key
     else:
         return key[0:64]
 
 
 def DecToHex(dec: int) -> str:
-    """
-    convert number to hex string
-    :param dec:
-    :type: int.
-    :return: stringHex.
-    :type: str.
-    """
     decKey = from_int(dec)
     if len(decKey) < 64:
         return decKey.zfill(64)
     else:
         return decKey
 
 
 def b58_encodec(data: str) -> str:
-    """
-    convertor hex string to string b58 decode decompile
-
-    :param data:
-    :type: str.
-    :return: string_b58.
-    :type: str.
-    """
     return base58.b58encode(unHexlify(data)).decode('utf-8')
 
 
 def HexToBin(hexed: str) -> str:
     return bin(int(hexed, 16))[2:].zfill(256)
 
 
@@ -201,14 +102,15 @@
 
 
 def BytsToRIPEMD160(byte: bytes) -> bytes:
     RIPEMD160 = hashlib.new('ripemd160')
     RIPEMD160.update(byte)
     return RIPEMD160.digest()
 
+
 def BytesToMne(bytes_string: bytes) -> str:
     return Mnemonic('english').to_mnemonic(bytes_string)
 
 
 def BytesToMnemonic(bytes_string: bytes, size: int) -> str:
     mne = BytesToMne(bytes_string)
     if size == 12:
@@ -223,30 +125,26 @@
         return ' '.join(str(mne).split(' ')[0:12])
 
 
 def BytesToHex(bytes_string: bytes) -> str:
     return Hexlify(bytes_string)
 
 
-def BytesToWif(bytes_key: bytes, compress=False) -> str:
-    vb = b'\x80'
-    cv = b'\x01'
-    uv = b''
-    if compress:
-        bytes_key += cv
-    else:
-        bytes_key += uv
-
-    return Base58Encode_Check(vb, bytes_key)
-
-
 def BytesToDec(bytestr: bytes) -> int:
     return int.from_bytes(bytestr, 'big')
 
 
+def BytesToWif(byte, compress=False):
+    from bit.format import bytes_to_wif
+    if compress:
+        return bytes_to_wif(byte, compressed=True)
+    else:
+        return bytes_to_wif(byte, compressed=False)
+
+
 def BytesToAddr(bytes_data: bytes, compress=False) -> str:
     from bit import Key
     from bit.format import bytes_to_wif as btw
     if compress:
         wif = btw(bytes_data, compressed=True)
         bits = Key(wif)
         return bits.address
@@ -274,19 +172,20 @@
 def WifAddr(wif: str) -> str:
     from bit import Key
     bits = Key(wif)
     return bits.address
 
 
 def WifToBytes(wif: str) -> bytes:
-    wif_Bytes = Base58Decode_Check(wif)
-    return wif_Bytes[1:]
+    wifbyte = base58.b58decode_check(wif)
+    # wif_Bytes = Base58Decode_Check(wif)
+    return wifbyte[1:]
 
 
-def getMnemonic(size: int) -> str | None:
+def getMnemonic(size: int) -> str:
     ml = ''
     words = "AbandonAbilityAbleAboutAboveAbsentAbsorbAbstractAbsurdAbuseAccessAccidentAccountAccuseAchieveAcidAcousticAcquireAcrossActActionActorActressActualAdaptAddAddictAddressAdjustAdmitAdultAdvanceAdviceAerobicAffairAffordAfraidAgainAgeAgentAgreeAheadAimAirAirportAisleAlarmAlbumAlcoholAlertAlienAllAlleyAllowAlmostAloneAlphaAlreadyAlsoAlterAlwaysAmateurAmazingAmongAmountAmusedAnalystAnchorAncientAngerAngleAngryAnimalAnkleAnnounceAnnualAnotherAnswerAntennaAntiqueAnxietyAnyApartApologyAppearAppleApproveAprilArchArcticAreaArenaArgueArmArmedArmorArmyAroundArrangeArrestArriveArrowArtArtefactArtistArtworkAskAspectAssaultAssetAssistAssumeAsthmaAthleteAtomAttackAttendAttitudeAttractAuctionAuditAugustAuntAuthorAutoAutumnAverageAvocadoAvoidAwakeAwareAwayAwesomeAwfulAwkwardAxisBabyBachelorBaconBadgeBagBalanceBalconyBallBambooBananaBannerBarBarelyBargainBarrelBaseBasicBasketBattleBeachBeanBeautyBecauseBecomeBeefBeforeBeginBehaveBehindBelieveBelowBeltBenchBenefitBestBetrayBetterBetweenBeyondBicycleBidBikeBindBiologyBirdBirthBitterBlackBladeBlameBlanketBlastBleakBlessBlindBloodBlossomBlouseBlueBlurBlushBoardBoatBodyBoilBombBoneBonusBookBoostBorderBoringBorrowBossBottomBounceBoxBoyBracketBrainBrandBrassBraveBreadBreezeBrickBridgeBriefBrightBringBriskBroccoliBrokenBronzeBroomBrotherBrownBrushBubbleBuddyBudgetBuffaloBuildBulbBulkBulletBundleBunkerBurdenBurgerBurstBusBusinessBusyButterBuyerBuzzCabbageCabinCableCactusCageCakeCallCalmCameraCampCanCanalCancelCandyCannonCanoeCanvasCanyonCapableCapitalCaptainCarCarbonCardCargoCarpetCarryCartCaseCashCasinoCastleCasualCatCatalogCatchCategoryCattleCaughtCauseCautionCaveCeilingCeleryCementCensusCenturyCerealCertainChairChalkChampionChangeChaosChapterChargeChaseChatCheapCheckCheeseChefCherryChestChickenChiefChildChimneyChoiceChooseChronicChuckleChunkChurnCigarCinnamonCircleCitizenCityCivilClaimClapClarifyClawClayCleanClerkCleverClickClientCliffClimbClinicClipClockClogCloseClothCloudClownClubClumpClusterClutchCoachCoastCoconutCodeCoffeeCoilCoinCollectColorColumnCombineComeComfortComicCommonCompanyConcertConductConfirmCongressConnectConsiderControlConvinceCookCoolCopperCopyCoralCoreCornCorrectCostCottonCouchCountryCoupleCourseCousinCoverCoyoteCrackCradleCraftCramCraneCrashCraterCrawlCrazyCreamCreditCreekCrewCricketCrimeCrispCriticCropCrossCrouchCrowdCrucialCruelCruiseCrumbleCrunchCrushCryCrystalCubeCultureCupCupboardCuriousCurrentCurtainCurveCushionCustomCuteCycleDadDamageDampDanceDangerDaringDashDaughterDawnDayDealDebateDebrisDecadeDecemberDecideDeclineDecorateDecreaseDeerDefenseDefineDefyDegreeDelayDeliverDemandDemiseDenialDentistDenyDepartDependDepositDepthDeputyDeriveDescribeDesertDesignDeskDespairDestroyDetailDetectDevelopDeviceDevoteDiagramDialDiamondDiaryDiceDieselDietDifferDigitalDignityDilemmaDinnerDinosaurDirectDirtDisagreeDiscoverDiseaseDishDismissDisorderDisplayDistanceDivertDivideDivorceDizzyDoctorDocumentDogDollDolphinDomainDonateDonkeyDonorDoorDoseDoubleDoveDraftDragonDramaDrasticDrawDreamDressDriftDrillDrinkDripDriveDropDrumDryDuckDumbDuneDuringDustDutchDutyDwarfDynamicEagerEagleEarlyEarnEarthEasilyEastEasyEchoEcologyEconomyEdgeEditEducateEffortEggEightEitherElbowElderElectricElegantElementElephantElevatorEliteElseEmbarkEmbodyEmbraceEmergeEmotionEmployEmpowerEmptyEnableEnactEndEndlessEndorseEnemyEnergyEnforceEngageEngineEnhanceEnjoyEnlistEnoughEnrichEnrollEnsureEnterEntireEntryEnvelopeEpisodeEqualEquipEraEraseErodeErosionErrorEruptEscapeEssayEssenceEstateEternalEthicsEvidenceEvilEvokeEvolveExactExampleExcessExchangeExciteExcludeExcuseExecuteExerciseExhaustExhibitExileExistExitExoticExpandExpectExpireExplainExposeExpressExtendExtraEyeEyebrowFabricFaceFacultyFadeFaintFaithFallFalseFameFamilyFamousFanFancyFantasyFarmFashionFatFatalFatherFatigueFaultFavoriteFeatureFebruaryFederalFeeFeedFeelFemaleFenceFestivalFetchFeverFewFiberFictionFieldFigureFileFilmFilterFinalFindFineFingerFinishFireFirmFirstFiscalFishFitFitnessFixFlagFlameFlashFlatFlavorFleeFlightFlipFloatFlockFloorFlowerFluidFlushFlyFoamFocusFogFoilFoldFollowFoodFootForceForestForgetForkFortuneForumForwardFossilFosterFoundFoxFragileFrameFrequentFreshFriendFringeFrogFrontFrostFrownFrozenFruitFuelFunFunnyFurnaceFuryFutureGadgetGainGalaxyGalleryGameGapGarageGarbageGardenGarlicGarmentGasGaspGateGatherGaugeGazeGeneralGeniusGenreGentleGenuineGestureGhostGiantGiftGiggleGingerGiraffeGirlGiveGladGlanceGlareGlassGlideGlimpseGlobeGloomGloryGloveGlowGlueGoatGoddessGoldGoodGooseGorillaGospelGossipGovernGownGrabGraceGrainGrantGrapeGrassGravityGreatGreenGridGriefGritGroceryGroupGrowGruntGuardGuessGuideGuiltGuitarGunGymHabitHairHalfHammerHamsterHandHappyHarborHardHarshHarvestHatHaveHawkHazardHeadHealthHeartHeavyHedgehogHeightHelloHelmetHelpHenHeroHiddenHighHillHintHipHireHistoryHobbyHockeyHoldHoleHolidayHollowHomeHoneyHoodHopeHornHorrorHorseHospitalHostHotelHourHoverHubHugeHumanHumbleHumorHundredHungryHuntHurdleHurryHurtHusbandHybridIceIconIdeaIdentifyIdleIgnoreIllIllegalIllnessImageImitateImmenseImmuneImpactImposeImproveImpulseInchIncludeIncomeIncreaseIndexIndicateIndoorIndustryInfantInflictInformInhaleInheritInitialInjectInjuryInmateInnerInnocentInputInquiryInsaneInsectInsideInspireInstallIntactInterestIntoInvestInviteInvolveIronIslandIsolateIssueItemIvoryJacketJaguarJarJazzJealousJeansJellyJewelJobJoinJokeJourneyJoyJudgeJuiceJumpJungleJuniorJunkJustKangarooKeenKeepKetchupKeyKickKidKidneyKindKingdomKissKitKitchenKiteKittenKiwiKneeKnifeKnockKnowLabLabelLaborLadderLadyLakeLampLanguageLaptopLargeLaterLatinLaughLaundryLavaLawLawnLawsuitLayerLazyLeaderLeafLearnLeaveLectureLeftLegLegalLegendLeisureLemonLendLengthLensLeopardLessonLetterLevelLiarLibertyLibraryLicenseLifeLiftLightLikeLimbLimitLinkLionLiquidListLittleLiveLizardLoadLoanLobsterLocalLockLogicLonelyLongLoopLotteryLoudLoungeLoveLoyalLuckyLuggageLumberLunarLunchLuxuryLyricsMachineMadMagicMagnetMaidMailMainMajorMakeMammalManManageMandateMangoMansionManualMapleMarbleMarchMarginMarineMarketMarriageMaskMassMasterMatchMaterialMathMatrixMatterMaximumMazeMeadowMeanMeasureMeatMechanicMedalMediaMelodyMeltMemberMemoryMentionMenuMercyMergeMeritMerryMeshMessageMetalMethodMiddleMidnightMilkMillionMimicMindMinimumMinorMinuteMiracleMirrorMiseryMissMistakeMixMixedMixtureMobileModelModifyMomMomentMonitorMonkeyMonsterMonthMoonMoralMoreMorningMosquitoMotherMotionMotorMountainMouseMoveMovieMuchMuffinMuleMultiplyMuscleMuseumMushroomMusicMustMutualMyselfMysteryMythNaiveNameNapkinNarrowNastyNationNatureNearNeckNeedNegativeNeglectNeitherNephewNerveNestNetNetworkNeutralNeverNewsNextNiceNightNobleNoiseNomineeNoodleNormalNorthNoseNotableNoteNothingNoticeNovelNowNuclearNumberNurseNutOakObeyObjectObligeObscureObserveObtainObviousOccurOceanOctoberOdorOffOfferOfficeOftenOilOkayOldOliveOlympicOmitOnceOneOnionOnlineOnlyOpenOperaOpinionOpposeOptionOrangeOrbitOrchardOrderOrdinaryOrganOrientOriginalOrphanOstrichOtherOutdoorOuterOutputOutsideOvalOvenOverOwnOwnerOxygenOysterOzonePactPaddlePagePairPalacePalmPandaPanelPanicPantherPaperParadeParentParkParrotPartyPassPatchPathPatientPatrolPatternPausePavePaymentPeacePeanutPearPeasantPelicanPenPenaltyPencilPeoplePepperPerfectPermitPersonPetPhonePhotoPhrasePhysicalPianoPicnicPicturePiecePigPigeonPillPilotPinkPioneerPipePistolPitchPizzaPlacePlanetPlasticPlatePlayPleasePledgePluckPlugPlungePoemPoetPointPolarPolePolicePondPonyPoolPopularPortionPositionPossiblePostPotatoPotteryPovertyPowderPowerPracticePraisePredictPreferPreparePresentPrettyPreventPricePridePrimaryPrintPriorityPrisonPrivatePrizeProblemProcessProduceProfitProgramProjectPromoteProofPropertyProsperProtectProudProvidePublicPuddingPullPulpPulsePumpkinPunchPupilPuppyPurchasePurityPurposePursePushPutPuzzlePyramidQualityQuantumQuarterQuestionQuickQuitQuizQuoteRabbitRaccoonRaceRackRadarRadioRailRainRaiseRallyRampRanchRandomRangeRapidRareRateRatherRavenRawRazorReadyRealReasonRebelRebuildRecallReceiveRecipeRecordRecycleReduceReflectReformRefuseRegionRegretRegularRejectRelaxReleaseReliefRelyRemainRememberRemindRemoveRenderRenewRentReopenRepairRepeatReplaceReportRequireRescueResembleResistResourceResponseResultRetireRetreatReturnReunionRevealReviewRewardRhythmRibRibbonRiceRichRideRidgeRifleRightRigidRingRiotRippleRiskRitualRivalRiverRoadRoastRobotRobustRocketRomanceRoofRookieRoomRoseRotateRoughRoundRouteRoyalRubberRudeRugRuleRunRunwayRuralSadSaddleSadnessSafeSailSaladSalmonSalonSaltSaluteSameSampleSandSatisfySatoshiSauceSausageSaveSayScaleScanScareScatterSceneSchemeSchoolScienceScissorsScorpionScoutScrapScreenScriptScrubSeaSearchSeasonSeatSecondSecretSectionSecuritySeedSeekSegmentSelectSellSeminarSeniorSenseSentenceSeriesServiceSessionSettleSetupSevenShadowShaftShallowShareShedShellSheriffShieldShiftShineShipShiverShockShoeShootShopShortShoulderShoveShrimpShrugShuffleShySiblingSickSideSiegeSightSignSilentSilkSillySilverSimilarSimpleSinceSingSirenSisterSituateSixSizeSkateSketchSkiSkillSkinSkirtSkullSlabSlamSleepSlenderSliceSlideSlightSlimSloganSlotSlowSlushSmallSmartSmileSmokeSmoothSnackSnakeSnapSniffSnowSoapSoccerSocialSockSodaSoftSolarSoldierSolidSolutionSolveSomeoneSongSoonSorrySortSoulSoundSoupSourceSouthSpaceSpareSpatialSpawnSpeakSpecialSpeedSpellSpendSphereSpiceSpiderSpikeSpinSpiritSplitSpoilSponsorSpoonSportSpotSpraySpreadSpringSpySquareSqueezeSquirrelStableStadiumStaffStageStairsStampStandStartStateStaySteakSteelStemStepStereoStickStillStingStockStomachStoneStoolStoryStoveStrategyStreetStrikeStrongStruggleStudentStuffStumbleStyleSubjectSubmitSubwaySuccessSuchSuddenSufferSugarSuggestSuitSummerSunSunnySunsetSuperSupplySupremeSureSurfaceSurgeSurpriseSurroundSurveySuspectSustainSwallowSwampSwapSwarmSwearSweetSwiftSwimSwingSwitchSwordSymbolSymptomSyrupSystemTableTackleTagTailTalentTalkTankTapeTargetTaskTasteTattooTaxiTeachTeamTellTenTenantTennisTentTermTestTextThankThatThemeThenTheoryThereTheyThingThisThoughtThreeThriveThrowThumbThunderTicketTideTigerTiltTimberTimeTinyTipTiredTissueTitleToastTobaccoTodayToddlerToeTogetherToiletTokenTomatoTomorrowToneTongueTonightToolToothTopTopicToppleTorchTornadoTortoiseTossTotalTouristTowardTowerTownToyTrackTradeTrafficTragicTrainTransferTrapTrashTravelTrayTreatTreeTrendTrialTribeTrickTriggerTrimTripTrophyTroubleTruckTrueTrulyTrumpetTrustTruthTryTubeTuitionTumbleTunaTunnelTurkeyTurnTurtleTwelveTwentyTwiceTwinTwistTwoTypeTypicalUglyUmbrellaUnableUnawareUncleUncoverUnderUndoUnfairUnfoldUnhappyUniformUniqueUnitUniverseUnknownUnlockUntilUnusualUnveilUpdateUpgradeUpholdUponUpperUpsetUrbanUrgeUsageUseUsedUsefulUselessUsualUtilityVacantVacuumVagueValidValleyValveVanVanishVaporVariousVastVaultVehicleVelvetVendorVentureVenueVerbVerifyVersionVeryVesselVeteranViableVibrantViciousVictoryVideoViewVillageVintageViolinVirtualVirusVisaVisitVisualVitalVividVocalVoiceVoidVolcanoVolumeVoteVoyageWageWagonWaitWalkWallWalnutWantWarfareWarmWarriorWashWaspWasteWaterWaveWayWealthWeaponWearWeaselWeatherWebWeddingWeekendWeirdWelcomeWestWetWhaleWhatWheatWheelWhenWhereWhipWhisperWideWidthWifeWildWillWinWindowWineWingWinkWinnerWinterWireWisdomWiseWishWitnessWolfWomanWonderWoodWoolWordWorkWorldWorryWorthWrapWreckWrestleWristWriteWrongYardYearYellowYouYoungYouthZebraZeroZoneZoo"
     mnemonics = re.findall('[A-Z][a-z]+', words)
     if size == 12:
         for r in range(size):
             lx = random.choice(mnemonics)
             ml += f" {lx}"
```

### Comparing `Blockthon-4.6.9/Blockthon.egg-info/PKG-INFO` & `Blockthon-4.9.6/Blockthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 4.6.9
+Version: 4.9.6
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 Project-URL: Documentation, https://blockthon.github.io/Blockthon/
 Project-URL: Personal Website, https://mmdrza.com
 Keywords: blockthon,bitcoin,ethereum,tron,dogecoin,dash,qtum,litecoin,bitcoingold,wallet,private key,mnemonic,seed,binary,hex,hunter,compress,un compress,compress address,un compress address
```

### Comparing `Blockthon-4.6.9/PKG-INFO` & `Blockthon-4.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 4.6.9
+Version: 4.9.6
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 Project-URL: Documentation, https://blockthon.github.io/Blockthon/
 Project-URL: Personal Website, https://mmdrza.com
 Keywords: blockthon,bitcoin,ethereum,tron,dogecoin,dash,qtum,litecoin,bitcoingold,wallet,private key,mnemonic,seed,binary,hex,hunter,compress,un compress,compress address,un compress address
```

### Comparing `Blockthon-4.6.9/README.md` & `Blockthon-4.9.6/README.md`

 * *Files identical despite different names*

### Comparing `Blockthon-4.6.9/setup.py` & `Blockthon-4.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Blockthon",
-    version="4.6.9",
+    version="4.9.6",
     author="Pymmdrza",
     author_email="Pymmdrza@gmail.com",
     description="Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, "
                 "and Decimal.",
     keywords=['blockthon','bitcoin', 'ethereum', 'tron', 'dogecoin', 'dash', 'qtum', 'litecoin', 'bitcoingold', 'wallet', 'private key', 'mnemonic', 'seed', 'binary', 'hex', 'hunter', 'compress', 'un compress', 'compress address', 'un compress address'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

