# Comparing `tmp/powertools_oas_validator-0.4.1.tar.gz` & `tmp/powertools_oas_validator-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.4.1.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.4.2.tar", max compression
```

## Comparing `powertools_oas_validator-0.4.1.tar` & `powertools_oas_validator-0.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/LICENSE
--rw-r--r--   0        0        0     1622 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/README.md
--rw-r--r--   0        0        0       13 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      199 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0      928 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0      135 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/overrides/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/overrides/unmarshallers.py
--rw-r--r--   0        0        0      944 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/overrides/validators.py
--rw-r--r--   0        0        0       13 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     3196 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/services/event_parser.py
--rw-r--r--   0        0        0     1120 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0      427 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/services/spec_parser.py
--rw-r--r--   0        0        0     3321 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0     1805 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      756 2023-07-02 19:07:03.729616 powertools_oas_validator-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.1/setup.py
--rw-r--r--   0        0        0     2237 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-02 19:15:53.318829 powertools_oas_validator-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2216 2023-07-02 19:15:53.318829 powertools_oas_validator-0.4.2/README.md
+-rw-r--r--   0        0        0       13 2023-07-02 19:15:53.318829 powertools_oas_validator-0.4.2/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0      944 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     3196 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     3321 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1805 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      756 2023-07-02 19:15:53.322829 powertools_oas_validator-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.2/setup.py
+-rw-r--r--   0        0        0     2831 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.2/PKG-INFO
```

### Comparing `powertools_oas_validator-0.4.1/LICENSE` & `powertools_oas_validator-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.1/README.md` & `powertools_oas_validator-0.4.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.
 
 The *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.
 
 
 ## Usage
-Decorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request (and schema) will be validated on a request.
+Decorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.
 
 
 ### Minimal Example
 
 ```python
 from typing import Dict
 from aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse
@@ -30,9 +30,20 @@
 @validate_request(oas_path="openapi.yaml")
 def lambda_handler(event: Dict, context: LambdaContext) -> Dict:
     response = app.resolve(event, context)
 
     return response
 ```
 
+## Error Handling
+If the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.
+
+
+## Know Issues
+While all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`
+(same as the Powertools validator would), with as much of the optional attributes as possible.
+
+In summary, it is possible that not all `SchemaValidationErrors`'s will have a nice validation message, in case you rely on piping it straight back to the client.
+
+
 ## Contributions
 Please make a pull request and I will review it ASAP.
```

### Comparing `powertools_oas_validator-0.4.1/powertools_oas_validator/middleware.py` & `powertools_oas_validator-0.4.2/powertools_oas_validator/middleware.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.1/powertools_oas_validator/overrides/unmarshallers.py` & `powertools_oas_validator-0.4.2/powertools_oas_validator/overrides/unmarshallers.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.1/powertools_oas_validator/overrides/validators.py` & `powertools_oas_validator-0.4.2/powertools_oas_validator/overrides/validators.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.1/powertools_oas_validator/services/event_parser.py` & `powertools_oas_validator-0.4.2/powertools_oas_validator/services/event_parser.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.1/powertools_oas_validator/services/spec_loader.py` & `powertools_oas_validator-0.4.2/powertools_oas_validator/services/spec_loader.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.1/powertools_oas_validator/services/spec_validator.py` & `powertools_oas_validator-0.4.2/powertools_oas_validator/services/spec_validator.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.1/powertools_oas_validator/types.py` & `powertools_oas_validator-0.4.2/powertools_oas_validator/types.py`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.4.1/pyproject.toml` & `powertools_oas_validator-0.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "powertools_oas_validator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `powertools_oas_validator-0.4.1/setup.py` & `powertools_oas_validator-0.4.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 ['aws-lambda-powertools>=2.18.0,<3.0.0',
  'fastjsonschema>=2.17.1,<3.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'openapi-core>=0.17.2,<0.18.0']
 
 setup_kwargs = {
     'name': 'powertools-oas-validator',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': '',
-    'long_description': '# powertools-oas-validator\n<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://pypi.org/project/powertools-oas-validator/) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom aws_lambda_powertools.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
+    'long_description': '# powertools-oas-validator\n<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://pypi.org/project/powertools-oas-validator/) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.\n\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom aws_lambda_powertools.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Error Handling\nIf the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.\n\n\n## Know Issues\nWhile all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`\n(same as the Powertools validator would), with as much of the optional attributes as possible.\n\nIn summary, it is possible that not all `SchemaValidationErrors`\'s will have a nice validation message, in case you rely on piping it straight back to the client.\n\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
     'author': 'Rasmus Hansen',
     'author_email': 'R.FangelHansen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `powertools_oas_validator-0.4.1/PKG-INFO` & `powertools_oas_validator-0.4.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powertools-oas-validator
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 License: MIT
 Author: Rasmus Hansen
 Author-email: R.FangelHansen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 
 [Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.
 
 The *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.
 
 
 ## Usage
-Decorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request (and schema) will be validated on a request.
+Decorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request/event (and schema) will be validated on a request.
 
 
 ### Minimal Example
 
 ```python
 from typing import Dict
 from aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse
@@ -48,10 +48,21 @@
 @validate_request(oas_path="openapi.yaml")
 def lambda_handler(event: Dict, context: LambdaContext) -> Dict:
     response = app.resolve(event, context)
 
     return response
 ```
 
+## Error Handling
+If the validation fails, the decorator throws a `SchemaValidatonError` with relevant information about the failed validation.
+
+
+## Know Issues
+While all validation errors are caught, there is only limited information about the various errors. The decorator will try its best to throw a `SchemaValidatonError`
+(same as the Powertools validator would), with as much of the optional attributes as possible.
+
+In summary, it is possible that not all `SchemaValidationErrors`'s will have a nice validation message, in case you rely on piping it straight back to the client.
+
+
 ## Contributions
 Please make a pull request and I will review it ASAP.
```

