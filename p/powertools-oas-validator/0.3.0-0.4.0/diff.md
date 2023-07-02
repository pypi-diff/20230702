# Comparing `tmp/powertools_oas_validator-0.3.0.tar.gz` & `tmp/powertools_oas_validator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powertools_oas_validator-0.3.0.tar", max compression
+gzip compressed data, was "powertools_oas_validator-0.4.0.tar", max compression
```

## Comparing `powertools_oas_validator-0.3.0.tar` & `powertools_oas_validator-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/LICENSE
--rw-r--r--   0        0        0     2696 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/README.md
--rw-r--r--   0        0        0       13 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/__init__.py
--rw-r--r--   0        0        0      145 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/exceptions.py
--rw-r--r--   0        0        0     1580 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/middleware.py
--rw-r--r--   0        0        0       13 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/services/__init__.py
--rw-r--r--   0        0        0     3693 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/services/request_validator.py
--rw-r--r--   0        0        0     1198 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/services/spec_loader.py
--rw-r--r--   0        0        0     3635 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/services/spec_validator.py
--rw-r--r--   0        0        0      681 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/powertools_oas_validator/types.py
--rw-r--r--   0        0        0      801 2023-07-01 17:16:03.073293 powertools_oas_validator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3590 1970-01-01 00:00:00.000000 powertools_oas_validator-0.3.0/setup.py
--rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 powertools_oas_validator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2766 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/README.md
+-rw-r--r--   0        0        0       13 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/exceptions.py
+-rw-r--r--   0        0        0      928 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/middleware.py
+-rw-r--r--   0        0        0      135 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/overrides/__init__.py
+-rw-r--r--   0        0        0     1144 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/overrides/unmarshallers.py
+-rw-r--r--   0        0        0      944 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/overrides/validators.py
+-rw-r--r--   0        0        0       13 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/services/__init__.py
+-rw-r--r--   0        0        0     3196 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/services/event_parser.py
+-rw-r--r--   0        0        0     1120 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/services/spec_loader.py
+-rw-r--r--   0        0        0      427 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/services/spec_parser.py
+-rw-r--r--   0        0        0     3321 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/services/spec_validator.py
+-rw-r--r--   0        0        0     1805 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/powertools_oas_validator/types.py
+-rw-r--r--   0        0        0      756 2023-07-02 19:03:35.473708 powertools_oas_validator-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.0/setup.py
+-rw-r--r--   0        0        0     3381 1970-01-01 00:00:00.000000 powertools_oas_validator-0.4.0/PKG-INFO
```

### Comparing `powertools_oas_validator-0.3.0/LICENSE` & `powertools_oas_validator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `powertools_oas_validator-0.3.0/README.md` & `powertools_oas_validator-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # powertools-oas-validator
-<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://pypi.org/project/powertools-oas-validator/) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Publish/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)
+<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://pypi.org/project/powertools-oas-validator/) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)
 
 ## Introduction
 
 [Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.
 
 The *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.
 
@@ -49,20 +49,22 @@
 @app.post("/example")
 def example() -> Response:
   ...
 
 @validate_request(
   oas_path="openapi.yaml",
   validate_spec=True,  # default True, disable to not validate OpenAPI Schema
-  validate_body=True,  # default True, disable to not validate event["body"] 
+  validate_body=True,  # default True, disable to not validate event["body"]
   validate_headers=True,  # default True, disable to not validate event["headers"]
   validate_query=True,  # default True, disable to not validate event["rawQueryString"]
   validate_path=True,  # default True, disable to not validate path parameters
   validate_cookies=True, # default True, disable to not validate cookies
 
 )
 def lambda_handler(event: Dict, context: LambdaContext) -> Dict:
     response = app.resolve(event, context)
 
     return response
 ```
 
+## Contributions
+Please make a pull request and I will review it ASAP.
```

### Comparing `powertools_oas_validator-0.3.0/pyproject.toml` & `powertools_oas_validator-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "powertools-oas-validator"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Rasmus Hansen <R.FangelHansen@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "powertools_oas_validator"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aws-lambda-powertools = "^2.18.0"
 jmespath = "^1.0.1"
-openapi-spec-validator = "^0.5.7"
-chocs-middleware-openapi = "^1.2.2"
 fastjsonschema = "^2.17.1"
+openapi-core = "^0.17.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 mypy = "^1.4.1"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
```

### Comparing `powertools_oas_validator-0.3.0/setup.py` & `powertools_oas_validator-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['powertools_oas_validator', 'powertools_oas_validator.services']
+['powertools_oas_validator',
+ 'powertools_oas_validator.overrides',
+ 'powertools_oas_validator.services']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aws-lambda-powertools>=2.18.0,<3.0.0',
- 'chocs-middleware-openapi>=1.2.2,<2.0.0',
  'fastjsonschema>=2.17.1,<3.0.0',
  'jmespath>=1.0.1,<2.0.0',
- 'openapi-spec-validator>=0.5.7,<0.6.0']
+ 'openapi-core>=0.17.2,<0.18.0']
 
 setup_kwargs = {
     'name': 'powertools-oas-validator',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': '',
-    'long_description': '# powertools-oas-validator\n<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://pypi.org/project/powertools-oas-validator/) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Publish/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request (and schema) will be validated on a request.\n\nSchema validation is enabled per default but can be disabled if you already validate your schema (perhaps as part of a pipeline)\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom aws_lambda_powertools.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n\n### Extended Example\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom aws_lambda_powertools.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(\n  oas_path="openapi.yaml",\n  validate_spec=True,  # default True, disable to not validate OpenAPI Schema\n  validate_body=True,  # default True, disable to not validate event["body"] \n  validate_headers=True,  # default True, disable to not validate event["headers"]\n  validate_query=True,  # default True, disable to not validate event["rawQueryString"]\n  validate_path=True,  # default True, disable to not validate path parameters\n  validate_cookies=True, # default True, disable to not validate cookies\n\n)\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n',
+    'long_description': '# powertools-oas-validator\n<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://pypi.org/project/powertools-oas-validator/) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)\n\n## Introduction\n\n[Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.\n\nThe *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.\n\n\n## Usage\nDecorate your functions with `@validate_request(oas_path="openapi.yaml")` and your request (and schema) will be validated on a request.\n\nSchema validation is enabled per default but can be disabled if you already validate your schema (perhaps as part of a pipeline)\n\n### Minimal Example\n\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom aws_lambda_powertools.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(oas_path="openapi.yaml")\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n\n### Extended Example\n```python\nfrom typing import Dict\nfrom aws_lambda_powertools.event_handler import APIGatewayRestResolve, Rresponse\nfrom aws_lambda_powertools.utilities.typing import LambdaContext\nfrom aws_lambda_powertools.middleware import validate_request\n\n\napp = APIGatewayRestResolver()\n\n@app.post("/example")\ndef example() -> Response:\n  ...\n\n@validate_request(\n  oas_path="openapi.yaml",\n  validate_spec=True,  # default True, disable to not validate OpenAPI Schema\n  validate_body=True,  # default True, disable to not validate event["body"]\n  validate_headers=True,  # default True, disable to not validate event["headers"]\n  validate_query=True,  # default True, disable to not validate event["rawQueryString"]\n  validate_path=True,  # default True, disable to not validate path parameters\n  validate_cookies=True, # default True, disable to not validate cookies\n\n)\ndef lambda_handler(event: Dict, context: LambdaContext) -> Dict:\n    response = app.resolve(event, context)\n\n    return response\n```\n\n## Contributions\nPlease make a pull request and I will review it ASAP.\n',
     'author': 'Rasmus Hansen',
     'author_email': 'R.FangelHansen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `powertools_oas_validator-0.3.0/PKG-INFO` & `powertools_oas_validator-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: powertools-oas-validator
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 License: MIT
 Author: Rasmus Hansen
 Author-email: R.FangelHansen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aws-lambda-powertools (>=2.18.0,<3.0.0)
-Requires-Dist: chocs-middleware-openapi (>=1.2.2,<2.0.0)
 Requires-Dist: fastjsonschema (>=2.17.1,<3.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
-Requires-Dist: openapi-spec-validator (>=0.5.7,<0.6.0)
+Requires-Dist: openapi-core (>=0.17.2,<0.18.0)
 Description-Content-Type: text/markdown
 
 # powertools-oas-validator
-<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://pypi.org/project/powertools-oas-validator/) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Publish/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)
+<br>[![PyPI version](https://badge.fury.io/py/powertools-oas-validator.svg)](https://pypi.org/project/powertools-oas-validator/) ![Release](https://github.com/RasmusFangel/powertools-oas-validator/workflows/Release/badge.svg) ![CI](https://github.com/RasmusFangel/powertools-oas-validator/workflows/CI/badge.svg)
 
 ## Introduction
 
 [Powertools for AWS Lambda (Python)](https://github.com/aws-powertools/powertools-lambda-python) is an awesome set of tools for supercharging your lambdas. Powertools supports validating incoming requests (or event in PT lingo) against [JSONSchema](https://json-schema.org/) which is not ideal if you are using OpenAPI schemas to define your API contracts.
 
 The *Powertools OAS Validator* adds a decorator that you can use with your lambda handlers and have the events validated against an OpenAPI schema instead.
 
@@ -68,21 +67,23 @@
 @app.post("/example")
 def example() -> Response:
   ...
 
 @validate_request(
   oas_path="openapi.yaml",
   validate_spec=True,  # default True, disable to not validate OpenAPI Schema
-  validate_body=True,  # default True, disable to not validate event["body"] 
+  validate_body=True,  # default True, disable to not validate event["body"]
   validate_headers=True,  # default True, disable to not validate event["headers"]
   validate_query=True,  # default True, disable to not validate event["rawQueryString"]
   validate_path=True,  # default True, disable to not validate path parameters
   validate_cookies=True, # default True, disable to not validate cookies
 
 )
 def lambda_handler(event: Dict, context: LambdaContext) -> Dict:
     response = app.resolve(event, context)
 
     return response
 ```
 
+## Contributions
+Please make a pull request and I will review it ASAP.
```

