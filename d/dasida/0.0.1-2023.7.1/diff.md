# Comparing `tmp/dasida-0.0.1.tar.gz` & `tmp/dasida-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dasida-0.0.1.tar", last modified: Sun May 28 09:39:26 2023, max compression
+gzip compressed data, was "dasida-2023.7.1.tar", last modified: Sun Jul  2 01:56:01 2023, max compression
```

## Comparing `dasida-0.0.1.tar` & `dasida-2023.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 09:39:26.800706 dasida-0.0.1/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1063 2023-05-28 07:15:02.000000 dasida-0.0.1/LICENSE
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      157 2023-05-28 09:39:26.800706 dasida-0.0.1/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       34 2023-05-28 07:15:02.000000 dasida-0.0.1/README.md
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 09:39:26.800706 dasida-0.0.1/dasida/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       59 2023-05-28 07:45:19.000000 dasida-0.0.1/dasida/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 09:39:26.800706 dasida-0.0.1/dasida/aws/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      101 2023-05-28 07:45:06.000000 dasida-0.0.1/dasida/aws/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1680 2023-05-28 07:15:02.000000 dasida-0.0.1/dasida/aws/common.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     8466 2023-05-28 07:15:02.000000 dasida-0.0.1/dasida/aws/s3.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4580 2023-05-28 07:42:47.000000 dasida-0.0.1/dasida/aws/secrets_manager.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    12353 2023-05-28 07:15:02.000000 dasida-0.0.1/dasida/aws/sqs.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4008 2023-05-28 07:15:02.000000 dasida-0.0.1/dasida/aws/ssm.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 09:39:26.800706 dasida-0.0.1/dasida/docker/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       33 2023-05-28 07:15:02.000000 dasida-0.0.1/dasida/docker/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1240 2023-05-28 07:42:30.000000 dasida-0.0.1/dasida/docker/docker.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     7099 2023-05-28 07:48:25.000000 dasida-0.0.1/dasida/scripts.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-05-28 09:39:26.800706 dasida-0.0.1/dasida.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      157 2023-05-28 09:39:26.000000 dasida-0.0.1/dasida.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      438 2023-05-28 09:39:26.000000 dasida-0.0.1/dasida.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-05-28 09:39:26.000000 dasida-0.0.1/dasida.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       49 2023-05-28 09:39:26.000000 dasida-0.0.1/dasida.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       68 2023-05-28 09:39:26.000000 dasida-0.0.1/dasida.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        7 2023-05-28 09:39:26.000000 dasida-0.0.1/dasida.egg-info/top_level.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      262 2023-05-28 07:15:02.000000 dasida-0.0.1/pyproject.toml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      425 2023-05-28 09:39:26.800706 dasida-0.0.1/setup.cfg
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-02 01:56:01.092437 dasida-2023.7.1/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1063 2023-07-02 01:00:04.000000 dasida-2023.7.1/LICENSE
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-02 01:56:01.092437 dasida-2023.7.1/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       34 2023-07-02 01:00:04.000000 dasida-2023.7.1/README.md
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-02 01:56:01.092437 dasida-2023.7.1/dasida/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       58 2023-07-02 01:54:32.000000 dasida-2023.7.1/dasida/__init__.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-02 01:56:01.092437 dasida-2023.7.1/dasida/aws/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       99 2023-07-02 01:54:15.000000 dasida-2023.7.1/dasida/aws/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1680 2023-07-02 01:00:04.000000 dasida-2023.7.1/dasida/aws/common.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     8466 2023-07-02 01:00:04.000000 dasida-2023.7.1/dasida/aws/s3.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     9428 2023-07-02 01:52:41.000000 dasida-2023.7.1/dasida/aws/secretsmanager.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)    12353 2023-07-02 01:00:04.000000 dasida-2023.7.1/dasida/aws/sqs.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     4008 2023-07-02 01:00:04.000000 dasida-2023.7.1/dasida/aws/ssm.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-02 01:56:01.092437 dasida-2023.7.1/dasida/docker/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       33 2023-07-02 01:00:04.000000 dasida-2023.7.1/dasida/docker/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1240 2023-07-02 01:00:04.000000 dasida-2023.7.1/dasida/docker/docker.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     7096 2023-07-02 01:03:06.000000 dasida-2023.7.1/dasida/scripts.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-02 01:56:01.092437 dasida-2023.7.1/dasida.egg-info/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-02 01:56:01.000000 dasida-2023.7.1/dasida.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      437 2023-07-02 01:56:01.000000 dasida-2023.7.1/dasida.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        1 2023-07-02 01:56:01.000000 dasida-2023.7.1/dasida.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       49 2023-07-02 01:56:01.000000 dasida-2023.7.1/dasida.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       68 2023-07-02 01:56:01.000000 dasida-2023.7.1/dasida.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        7 2023-07-02 01:56:01.000000 dasida-2023.7.1/dasida.egg-info/top_level.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      262 2023-07-02 01:00:04.000000 dasida-2023.7.1/pyproject.toml
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      425 2023-07-02 01:56:01.092437 dasida-2023.7.1/setup.cfg
```

### Comparing `dasida-0.0.1/LICENSE` & `dasida-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dasida-0.0.1/dasida/aws/common.py` & `dasida-2023.7.1/dasida/aws/common.py`

 * *Files identical despite different names*

### Comparing `dasida-0.0.1/dasida/aws/s3.py` & `dasida-2023.7.1/dasida/aws/s3.py`

 * *Files identical despite different names*

### Comparing `dasida-0.0.1/dasida/aws/secrets_manager.py` & `dasida-2023.7.1/dasida/aws/ssm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,148 +1,137 @@
-import ast
-import base64
 import fnmatch
 import json
 import logging
 from typing import Union
 
 import boto3
-from botocore.exceptions import ClientError
 from rich import print
 
 from .common import session_maker
 
-logger = logging.getLogger(__file__)
+logger = logging.getLogger()
+
+PS_PREFIX = "clutter"
 
 
 ################################################################
 # HELPERS
 ################################################################
-# _get_secrets
-def _get_secrets(client, secret_name):
-    # get secrets
-    try:
-        get_secret_value_response = client.get_secret_value(SecretId=secret_name)
-    except ClientError as e:
-        code = e.response["Error"]["Code"]
-        description = ERROR_DESCRIPTIONS.get(code, "unknown").replace("\n", " ")
-        if code == "ResourceNotFoundException":
-            logger.info(f"{code}: secret '{secret_name}' not found! return None.")
-            return None
-        logger.error(f"{code}: {description}")
-        raise e
-    else:
-        if "SecretString" in get_secret_value_response:
-            secrets = get_secret_value_response["SecretString"]
-            try:
-                secrets = json.loads(secrets)
-            except json.JSONDecodeError:
-                secrets = ast.literal_eval(secrets)
-            except Exception as ex:
-                logger.error(f"[CLUTTER] Cannot Decode JSON, {secrets}")
-        else:
-            secrets = base64.b64decode(get_secret_value_response["SecretBinary"])
-
-    return secrets
+# exception
+class ClutterAWSException(Exception):
+    pass
 
 
 ################################################################
 # FUNCTIONS
 ################################################################
-# list secrets
-def list_secrets(
-    patterns: Union[str, list] = "*",
-    profile_name: str = None,
-    aws_access_key_id: str = None,
-    aws_secret_access_key: str = None,
-    region_name: str = "ap-northeast-2",
-    load_docker_secret: bool = True,
+# list parameters
+def list_parameters(
+    patterns: Union[str, list] = None,
     session: boto3.Session = None,
-):
-    """
-    (TODO)
-      - filter tags
+) -> list:
+    """List Parameters in AWS Parameter Store.
+
+    Args:
+        session (boto3.Session, optional): create new session if None. Defaults to None.
+
+    Returns:
+        list: list of parameters
     """
     # correct args
+    patterns = patterns or "*"
     if patterns:
         patterns = patterns if isinstance(patterns, (tuple, list)) else [patterns]
 
     # get client
-    session = session or session_maker(
-        profile_name=profile_name,
-        aws_access_key_id=aws_access_key_id,
-        aws_secret_access_key=aws_secret_access_key,
-        region_name=region_name,
-        load_docker_secret=load_docker_secret,
-    )
-    client = session.client("secretsmanager")
+    session = session or session_maker()
+    client = session.client("ssm")
 
-    # get secrets
-    opts = {"MaxResults": 100}
-    secrets = []
-    while True:
-        response = client.list_secrets(**opts)
-        secrets += response.get("SecretList", [])
-        next_token = response.get("NextToken")
-        if next_token is None:
-            break
-        opts.update({"NextToken": next_token})
-
-    for secret in secrets:
-        secret_name = secret["Name"]
-        if not any([fnmatch.fnmatch(secret_name, f"*{pat.strip('*')}*") for pat in patterns]):
+    parameter_filters = [{"Key": "Name", "Option": "BeginsWith", "Values": [f"/{PS_PREFIX}"]}]
+    resp = client.describe_parameters(ParameterFilters=parameter_filters)
+
+    for param in resp["Parameters"]:
+        _, name = param["Name"].strip("/").split("/")
+        if not any([fnmatch.fnmatch(name, f"*{pat.strip('*')}*") for pat in patterns]):
             continue
-        body = _get_secrets(client, secret_name)
-        print(f"[[bold]{secret['Name']}[/bold]]")
-        if secret.get("Description"):
-            print(f" DESCRIPTION: {secret['Description']}")
+        print(f"[[bold]{name}[/bold]]")
+        if param.get("Description"):
+            print(f" DESCRIPTION: {param['Description']}")
+        print(f""" SSM NAME: '{param["Name"]}'""")
         print(" VALUES:")
-        if isinstance(body, dict):
-            for k, v in body.items():
+        values = get_parameters(name)
+        if isinstance(values, dict):
+            for k, v in values.items():
                 print(f"  - {k}: {v}")
         else:
-            print(f"  - {body}")
+            print(f"  - {values}")
 
 
-# get secrets
-def get_secrets(
-    secret_name: str,
-    profile_name: str = None,
-    aws_access_key_id: str = None,
-    aws_secret_access_key: str = None,
-    region_name: str = "ap-northeast-2",
-    load_docker_secret: bool = True,
+# set parameters
+def set_parameters(
+    name: str,
+    parameters: dict,
+    description: str = None,
+    tags: dict = None,
+    overwrite: bool = False,
     session: boto3.Session = None,
-):
-    """Get secrets from AWS SecretsManager.
+) -> None:
+    """Set New Parameters.
 
-    Example
-    -------
-    >>> conf = get_secrets("some/secrets")
-    """
+    Args:
+        name (str): Name.
+        parameters (dict): i.e. {"host": "example.com", "port": 80, "user": "eugene"}
+        description (str, optional): i.e. "This is Description.". Defaults to None.
+        tags (dict, optional): i.e. {"creator": "eugene"}. Defaults to None.
+        overwrite (bool, optional): overwrite exist parameters if True. Defaults to False.
+        session (boto3.Session, optional): create new session if None. Defaults to None.
 
+    Raises:
+        ClutterAWSException
+    """
     # get client
-    session = session or session_maker(
-        profile_name=profile_name,
-        aws_access_key_id=aws_access_key_id,
-        aws_secret_access_key=aws_secret_access_key,
-        region_name=region_name,
-        load_docker_secret=load_docker_secret,
+    session = session or session_maker()
+    client = session.client("ssm")
+
+    opts = {
+        "Type": "SecureString",
+        "Tier": "Standard",
+    }
+    if description:
+        opts.update({"Description": description})
+    if tags:
+        Tags = []
+        for k, v in tags.items():
+            tags.append({"Key": k, "Value": v})
+        opts.update({"Tags": Tags})
+
+    resp = client.put_parameter(
+        Name=f"/{PS_PREFIX}/{name}",
+        Value=json.dumps(parameters) if isinstance(parameters, dict) else parameters,
+        Overwrite=overwrite,
+        **opts,
     )
-    client = session.client("secretsmanager")
+    if resp["ResponseMetadata"]["HTTPStatusCode"] != 200:
+        raise ClutterAWSException(str(resp))
 
-    return _get_secrets(client, secret_name)
 
+# get parameters
+def get_parameters(name: str, session: boto3.Session = None) -> Union[dict, str]:
+    """Get Parameters from AWS Parameter Store.
 
-# errors
-ERROR_DESCRIPTIONS = {
-    "DecryptionFailureException": """\
-    Secrets Manager can't decrypt the protected secret text using the provided KMS key.""",
-    "InternalServiceErrorException": """\
-    An error occurred on the server side.""",
-    "InvalidParameterException": """\
-    You provided an invalid value for a parameter.""",
-    "InvalidRequestException": """\
-    You provided a parameter value that is not valid for the current state of the resource.""",
-    "ResourceNotFoundException": """\
-    We can't find the resource that you asked for.""",
-}
+    Args:
+        name (str): name of parameters
+        session (boto3.Session, optional): create new session if None. Defaults to None.
+
+    Returns:
+        Union[dict, str]: parameters.
+    """
+    session = session or session_maker()
+    client = session.client("ssm")
+
+    Name = f"/{PS_PREFIX}/{name}"
+    resp = client.get_parameter(Name=Name, WithDecryption=True)
+    values = resp["Parameter"]["Value"]
+    try:
+        return json.loads(values)
+    except json.JSONDecodeError as exc:
+        return values
```

### Comparing `dasida-0.0.1/dasida/aws/sqs.py` & `dasida-2023.7.1/dasida/aws/sqs.py`

 * *Files identical despite different names*

### Comparing `dasida-0.0.1/dasida/docker/docker.py` & `dasida-2023.7.1/dasida/docker/docker.py`

 * *Files identical despite different names*

### Comparing `dasida-0.0.1/dasida/scripts.py` & `dasida-2023.7.1/dasida/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     pass
 
 
 ################################################################
 # AWS SecretsManager
 ################################################################
 @dasida.group()
-def secrets_manager():
+def secretsmanager():
     pass
 
 
-@secrets_manager.command()
+@secretsmanager.command()
 @click.argument("patterns", default="*")
 @click.option("--profile", default=None)
 def list(patterns, profile):
-    aws.secrets_manager.list_secrets(patterns=patterns, profile_name=profile)
+    aws.secretsmanager.list_secrets(patterns=patterns, profile_name=profile)
 
 
 ################################################################
 # AWS S3
 ################################################################
 @dasida.group()
 def s3():
```

