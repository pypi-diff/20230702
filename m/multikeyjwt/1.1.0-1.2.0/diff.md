# Comparing `tmp/multikeyjwt-1.1.0.tar.gz` & `tmp/multikeyjwt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multikeyjwt-1.1.0.tar", max compression
+gzip compressed data, was "multikeyjwt-1.2.0.tar", max compression
```

## Comparing `multikeyjwt-1.1.0.tar` & `multikeyjwt-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-05-29 13:16:14.231452 multikeyjwt-1.1.0/LICENSE
--rw-r--r--   0        0        0     3072 2023-05-29 20:28:56.570713 multikeyjwt-1.1.0/README.rst
--rw-r--r--   0        0        0     1966 2023-05-30 17:05:33.004719 multikeyjwt-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      273 2023-05-30 17:05:33.005035 multikeyjwt-1.1.0/src/multikeyjwt/__init__.py
--rw-r--r--   0        0        0     2482 2023-05-29 21:00:03.225700 multikeyjwt-1.1.0/src/multikeyjwt/config.py
--rw-r--r--   0        0        0     3750 2023-05-30 17:05:33.005340 multikeyjwt-1.1.0/src/multikeyjwt/console.py
--rw-r--r--   0        0        0       25 2023-05-29 17:53:07.186037 multikeyjwt-1.1.0/src/multikeyjwt/jwt/__init__.py
--rw-r--r--   0        0        0      852 2023-05-29 20:27:36.579042 multikeyjwt-1.1.0/src/multikeyjwt/jwt/common.py
--rw-r--r--   0        0        0     2522 2023-05-30 06:11:54.955482 multikeyjwt-1.1.0/src/multikeyjwt/jwt/issuer.py
--rw-r--r--   0        0        0     2659 2023-05-29 20:28:56.589049 multikeyjwt-1.1.0/src/multikeyjwt/jwt/verifier.py
--rw-r--r--   0        0        0      114 2023-05-30 05:14:23.983577 multikeyjwt-1.1.0/src/multikeyjwt/middleware/__init__.py
--rw-r--r--   0        0        0     1809 2023-05-30 04:10:07.248745 multikeyjwt-1.1.0/src/multikeyjwt/middleware/jwtbearer.py
--rw-r--r--   0        0        0        0 2023-05-29 13:13:11.057378 multikeyjwt-1.1.0/src/multikeyjwt/py.typed
--rw-r--r--   0        0        0     4311 1970-01-01 00:00:00.000000 multikeyjwt-1.1.0/setup.py
--rw-r--r--   0        0        0     4042 1970-01-01 00:00:00.000000 multikeyjwt-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-29 13:16:14.231452 multikeyjwt-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3047 2023-07-02 12:05:20.984411 multikeyjwt-1.2.0/README.rst
+-rw-r--r--   0        0        0     1989 2023-07-02 12:05:20.985789 multikeyjwt-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      273 2023-07-02 12:05:20.986086 multikeyjwt-1.2.0/src/multikeyjwt/__init__.py
+-rw-r--r--   0        0        0     2482 2023-05-29 21:00:03.225700 multikeyjwt-1.2.0/src/multikeyjwt/config.py
+-rw-r--r--   0        0        0     4269 2023-07-02 12:05:20.986696 multikeyjwt-1.2.0/src/multikeyjwt/console.py
+-rw-r--r--   0        0        0       25 2023-05-29 17:53:07.186037 multikeyjwt-1.2.0/src/multikeyjwt/jwt/__init__.py
+-rw-r--r--   0        0        0      852 2023-05-29 20:27:36.579042 multikeyjwt-1.2.0/src/multikeyjwt/jwt/common.py
+-rw-r--r--   0        0        0     2487 2023-07-02 12:05:20.987031 multikeyjwt-1.2.0/src/multikeyjwt/jwt/issuer.py
+-rw-r--r--   0        0        0     2635 2023-07-02 12:05:20.987324 multikeyjwt-1.2.0/src/multikeyjwt/jwt/verifier.py
+-rw-r--r--   0        0        0     1680 2023-07-02 12:05:20.987757 multikeyjwt-1.2.0/src/multikeyjwt/keygen.py
+-rw-r--r--   0        0        0      114 2023-05-30 05:14:23.983577 multikeyjwt-1.2.0/src/multikeyjwt/middleware/__init__.py
+-rw-r--r--   0        0        0     1809 2023-05-30 04:10:07.248745 multikeyjwt-1.2.0/src/multikeyjwt/middleware/jwtbearer.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:13:11.057378 multikeyjwt-1.2.0/src/multikeyjwt/py.typed
+-rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 multikeyjwt-1.2.0/PKG-INFO
```

### Comparing `multikeyjwt-1.1.0/LICENSE` & `multikeyjwt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.1.0/README.rst` & `multikeyjwt-1.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 Verify JWTs with multiple public keys, FastAPI middleware for auth
 
 Creating signing keys
 ---------------------
 
 .. code-block:: bash
 
-    echo "My very g00d Passphrase" >/tmp/jwtRS256_passphrase.txt
-    ./make_keypair.sh
+    multikeyjwt genkey ./jwtsign.key
 
+see --help for more info
 
 Docker
 ------
 
 For more controlled deployments and to get rid of "works on my computer" -syndrome, we always
 make sure our software works under docker.
```

### Comparing `multikeyjwt-1.1.0/pyproject.toml` & `multikeyjwt-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multikeyjwt"
-version = "1.1.0"
+version = "1.2.0"
 description = "Verify JWTs with multiple public keys, FastAPI middleware for auth"
 authors = ["Eero af Heurlin <eero.afheurlin@iki.fi>"]
 homepage = "https://github.com/pvarki/python-multikeyjwt/"
 repository = "https://github.com/pvarki/python-multikeyjwt/"
 license = "MIT"
 readme = "README.rst"
 
@@ -61,14 +61,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0"
 pyjwt = {version = "^2.6", extras = ["crypto"]}
 libadvian = "^1.0"
 pendulum = "^2.1"
 fastapi = {version=">0.89,<1.0", optional = true} # caret behaviour on 0.x is to lock to 0.x.*
+cryptography = "^41.0"
 
 [tool.poetry.extras]
 fastapi = ["fastapi"]
 all = ["fastapi"]
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `multikeyjwt-1.1.0/src/multikeyjwt/config.py` & `multikeyjwt-1.2.0/src/multikeyjwt/config.py`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.1.0/src/multikeyjwt/console.py` & `multikeyjwt-1.2.0/src/multikeyjwt/console.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """CLI entrypoints for multikeyjwt"""
+from typing import Any, Sequence
 import logging
 import json
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import Any, Sequence
 
 import click
 from jwt import InvalidSignatureError
 from libadvian.logging import init_logging
 
 from multikeyjwt import __version__, Issuer, Verifier
 from multikeyjwt.config import Secret
+from multikeyjwt.keygen import generate_keypair
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_from_stdin(ctx: click.Context, param: Any, value: Any) -> Any:  # pylint: disable=unused-argument
     """Get value from stdin if value not given"""
@@ -64,15 +65,15 @@
 
 @cli_group.command(name="sign")
 @click.argument("keypath", callback=get_from_stdin, required=False)
 @click.option("-p", "--passphrase", help="Passhphrase to use", default=None)
 @click.option("-c", "--claim", help="Claim to issue JWT with", type=(str, str), multiple=True)
 def sign_cmd(keypath: str, passphrase: str, claim: Sequence[Any]) -> None:
     """
-    Sign the given key
+    Sign the given claims
 
     The key can be piped from stdin: cat mykey.key | multikeyjwt sign -p
       mypassphrase -c key value -c secondkey secondvalue \n
     or provided directly (as a path): multikeyjwt sign path/to/key.key -p
     mypassphrase -c key value -c secondkey secondvalue
     """
 
@@ -101,11 +102,25 @@
             issuer = Issuer(privkeypath=Path(tmpfile.name), keypasswd=Secret(passphrase))
             return click.echo(issuer.issue(dict(claim)))
 
         except Exception as exc:  # pylint: disable=broad-except
             return click.echo(f"{exc}")
 
 
+@cli_group.command(name="genkey")
+@click.argument("keypath", required=True)
+@click.option(
+    "-p", "--passphrase", help="Passhphrase to use", prompt=True, hide_input=True, confirmation_prompt=True, default=""
+)
+def genkey_cmd(keypath: str, passphrase: str) -> None:
+    """
+    Generate a new keypair, give the path you wish the .key -file have
+    """
+    genkey, genpub = generate_keypair(Path(keypath), passphrase)
+    click.echo(genkey)
+    click.echo(genpub)
+
+
 def multikeyjwt_cli() -> None:
     """CLI entrypoint"""
     init_logging(logging.WARNING)
     cli_group()  # pylint: disable=no-value-for-parameter
```

### Comparing `multikeyjwt-1.1.0/src/multikeyjwt/jwt/common.py` & `multikeyjwt-1.2.0/src/multikeyjwt/jwt/common.py`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.1.0/src/multikeyjwt/jwt/issuer.py` & `multikeyjwt-1.2.0/src/multikeyjwt/jwt/issuer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Creator/signer aka issuer for JWTs"""
-from typing import Optional, Any, Dict, cast
+from typing import Optional, Any, Dict, cast, ClassVar
 from dataclasses import dataclass, field
 from pathlib import Path
 import functools
 
 import pendulum
 from libadvian.binpackers import ensure_utf8
 import jwt as pyJWT  # too easy to accidentally override the module
@@ -24,14 +24,15 @@
     privkeypath: Path = field(default_factory=functools.partial(ENVCONFIG, "JWT_PRIVKEY_PATH", cast=Path))
     keypasswd: Optional[Secret] = field(
         default_factory=functools.partial(ENVCONFIG, "JWT_PRIVKEY_PASS", cast=Secret, default=None)
     )
 
     # Private props
     _privkey: PrivateKeyTypes = field(init=False, repr=False)
+    _singleton: ClassVar[Optional["Issuer"]] = None
 
     def __post_init__(self) -> None:
         """Read the keys"""
         if self.privkeypath and self.privkeypath.exists():
             with self.privkeypath.open("rb") as fpntr:
                 passphrase: Optional[bytes] = None
                 if self.keypasswd:
@@ -53,15 +54,11 @@
         if self.config.audience:
             claims["aud"] = self.config.audience
         return pyJWT.encode(payload=claims, key=cast(Any, self._privkey), algorithm=self.config.algorithm)
 
     @classmethod
     def singleton(cls, **kwargs: Any) -> "Issuer":
         """Get a singleton"""
-        global ISSUER_SINGLETON  # pylint: disable=W0603
-        if ISSUER_SINGLETON is None:
-            ISSUER_SINGLETON = Issuer(**kwargs)
-        assert ISSUER_SINGLETON is not None
-        return ISSUER_SINGLETON
-
-
-ISSUER_SINGLETON: Optional[Issuer] = None
+        if Issuer._singleton is None:
+            Issuer._singleton = Issuer(**kwargs)
+        assert Issuer._singleton is not None
+        return Issuer._singleton
```

### Comparing `multikeyjwt-1.1.0/src/multikeyjwt/jwt/verifier.py` & `multikeyjwt-1.2.0/src/multikeyjwt/jwt/verifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Verifier for JWTs, using multiple public keys"""
-from typing import Optional, Any, Dict, MutableSequence
+from typing import Optional, Any, Dict, MutableSequence, ClassVar
 from dataclasses import dataclass, field
 from pathlib import Path
 import functools
 import logging
 
 import jwt as pyJWT  # too easy to accidentally override the module
 from cryptography.hazmat.primitives import serialization
@@ -24,14 +24,17 @@
     config: JWTVerifierConfig = field(default_factory=JWTVerifierConfig)
 
     pubkeypath: Path = field(default_factory=functools.partial(ENVCONFIG, "JWT_PUBKEY_PATH", cast=Path))
 
     # Non-init public props
     pubkeys: MutableSequence[PublicKeyTypes] = field(init=False)
 
+    # private
+    _singleton: ClassVar[Optional["Verifier"]] = None
+
     def __post_init__(self) -> None:
         """Read the keys"""
         if not self.pubkeypath.exists():
             raise ValueError(f"{self.pubkeypath} does not exist")
         if self.pubkeypath.is_dir():
             self.pubkeys = []
             for fpth in self.pubkeypath.iterdir():
@@ -57,15 +60,11 @@
                 last_exception = exc
                 continue
         raise last_exception
 
     @classmethod
     def singleton(cls, **kwargs: Any) -> "Verifier":
         """Get a singleton"""
-        global VERIFIER_SINGLETON  # pylint: disable=W0603
-        if VERIFIER_SINGLETON is None:
-            VERIFIER_SINGLETON = Verifier(**kwargs)
-        assert VERIFIER_SINGLETON is not None
-        return VERIFIER_SINGLETON
-
-
-VERIFIER_SINGLETON: Optional[Verifier] = None
+        if Verifier._singleton is None:
+            Verifier._singleton = Verifier(**kwargs)
+        assert Verifier._singleton is not None
+        return Verifier._singleton
```

### Comparing `multikeyjwt-1.1.0/src/multikeyjwt/middleware/jwtbearer.py` & `multikeyjwt-1.2.0/src/multikeyjwt/middleware/jwtbearer.py`

 * *Files identical despite different names*

### Comparing `multikeyjwt-1.1.0/PKG-INFO` & `multikeyjwt-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multikeyjwt
-Version: 1.1.0
+Version: 1.2.0
 Summary: Verify JWTs with multiple public keys, FastAPI middleware for auth
 Home-page: https://github.com/pvarki/python-multikeyjwt/
 License: MIT
 Author: Eero af Heurlin
 Author-email: eero.afheurlin@iki.fi
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: fastapi
 Requires-Dist: click (>=8.0,<9.0)
+Requires-Dist: cryptography (>=41.0,<42.0)
 Requires-Dist: fastapi (>0.89,<1.0) ; extra == "fastapi" or extra == "all"
 Requires-Dist: libadvian (>=1.0,<2.0)
 Requires-Dist: pendulum (>=2.1,<3.0)
 Requires-Dist: pyjwt[crypto] (>=2.6,<3.0)
 Project-URL: Repository, https://github.com/pvarki/python-multikeyjwt/
 Description-Content-Type: text/x-rst
 
@@ -30,17 +31,17 @@
 Verify JWTs with multiple public keys, FastAPI middleware for auth
 
 Creating signing keys
 ---------------------
 
 .. code-block:: bash
 
-    echo "My very g00d Passphrase" >/tmp/jwtRS256_passphrase.txt
-    ./make_keypair.sh
+    multikeyjwt genkey ./jwtsign.key
 
+see --help for more info
 
 Docker
 ------
 
 For more controlled deployments and to get rid of "works on my computer" -syndrome, we always
 make sure our software works under docker.
```

