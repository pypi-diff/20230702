# Comparing `tmp/pip_audit-2.5.6.tar.gz` & `tmp/pip_audit-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_audit-2.5.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pip_audit-2.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pip_audit-2.5.6.tar` & `pip_audit-2.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    10174 2023-05-23 00:26:07.678217 pip_audit-2.5.6/LICENSE
--rw-r--r--   0        0        0    20850 2023-05-23 00:26:07.682217 pip_audit-2.5.6/README.md
--rw-r--r--   0        0        0       53 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/__init__.py
--rw-r--r--   0        0        0      144 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/__main__.py
--rw-r--r--   0        0        0     3158 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_audit.py
--rw-r--r--   0        0        0     6214 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_cache.py
--rw-r--r--   0        0        0    19415 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_cli.py
--rw-r--r--   0        0        0      490 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/__init__.py
--rw-r--r--   0        0        0     1552 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/interface.py
--rw-r--r--   0        0        0     6853 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/pip.py
--rw-r--r--   0        0        0     5416 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/pyproject.py
--rw-r--r--   0        0        0    10810 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_dependency_source/requirement.py
--rw-r--r--   0        0        0     3683 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_fix.py
--rw-r--r--   0        0        0      380 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/__init__.py
--rw-r--r--   0        0        0     5318 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/columns.py
--rw-r--r--   0        0        0     2957 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/cyclonedx.py
--rw-r--r--   0        0        0     1119 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/interface.py
--rw-r--r--   0        0        0     3160 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/json.py
--rw-r--r--   0        0        0     4844 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_format/markdown.py
--rw-r--r--   0        0        0      536 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_service/__init__.py
--rw-r--r--   0        0        0     5265 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_service/interface.py
--rw-r--r--   0        0        0     5898 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_service/osv.py
--rw-r--r--   0        0        0     5047 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_service/pypi.py
--rw-r--r--   0        0        0     8716 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_state.py
--rw-r--r--   0        0        0     2332 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_subprocess.py
--rw-r--r--   0        0        0      662 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_util.py
--rw-r--r--   0        0        0     6326 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pip_audit/_virtual_env.py
--rw-r--r--   0        0        0     3400 2023-05-23 00:26:07.682217 pip_audit-2.5.6/pyproject.toml
--rw-r--r--   0        0        0    23048 1970-01-01 00:00:00.000000 pip_audit-2.5.6/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-07-02 13:32:31.064548 pip_audit-2.6.0/LICENSE
+-rw-r--r--   0        0        0    21113 2023-07-02 13:32:31.064548 pip_audit-2.6.0/README.md
+-rw-r--r--   0        0        0       53 2023-07-02 13:32:31.064548 pip_audit-2.6.0/pip_audit/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-02 13:32:31.064548 pip_audit-2.6.0/pip_audit/__main__.py
+-rw-r--r--   0        0        0     3158 2023-07-02 13:32:31.064548 pip_audit-2.6.0/pip_audit/_audit.py
+-rw-r--r--   0        0        0     6223 2023-07-02 13:32:31.064548 pip_audit-2.6.0/pip_audit/_cache.py
+-rw-r--r--   0        0        0    19978 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_cli.py
+-rw-r--r--   0        0        0      579 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/__init__.py
+-rw-r--r--   0        0        0     1738 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/interface.py
+-rw-r--r--   0        0        0     6853 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/pip.py
+-rw-r--r--   0        0        0     5416 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/pyproject.py
+-rw-r--r--   0        0        0    15336 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_dependency_source/requirement.py
+-rw-r--r--   0        0        0     3683 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_fix.py
+-rw-r--r--   0        0        0      380 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/__init__.py
+-rw-r--r--   0        0        0     5318 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/columns.py
+-rw-r--r--   0        0        0     2800 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/cyclonedx.py
+-rw-r--r--   0        0        0     1119 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/interface.py
+-rw-r--r--   0        0        0     3160 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/json.py
+-rw-r--r--   0        0        0     4844 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_format/markdown.py
+-rw-r--r--   0        0        0      536 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_service/__init__.py
+-rw-r--r--   0        0        0     5265 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_service/interface.py
+-rw-r--r--   0        0        0     5898 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_service/osv.py
+-rw-r--r--   0        0        0     5047 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_service/pypi.py
+-rw-r--r--   0        0        0     8716 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_state.py
+-rw-r--r--   0        0        0     2332 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_subprocess.py
+-rw-r--r--   0        0        0      662 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_util.py
+-rw-r--r--   0        0        0     6326 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pip_audit/_virtual_env.py
+-rw-r--r--   0        0        0     3166 2023-07-02 13:32:31.068548 pip_audit-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    23270 1970-01-01 00:00:00.000000 pip_audit-2.6.0/PKG-INFO
```

### Comparing `pip_audit-2.5.6/LICENSE` & `pip_audit-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/README.md` & `pip_audit-2.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 `pip-audit` has [`pre-commit`](https://pre-commit.com/) support.
 
 For example, using `pip-audit` via `pre-commit` to audit a requirements file:
 
 ```yaml
   - repo: https://github.com/pypa/pip-audit
-    rev: v2.5.6
+    rev: v2.6.0
     hooks:
       -   id: pip-audit
           args: ["-r", "requirements.txt"]
 
 ci:
   # Leave pip-audit to only run locally and not in CI
   # pre-commit.ci does not allow network calls
@@ -132,14 +132,15 @@
 ```
 usage: pip-audit [-h] [-V] [-l] [-r REQUIREMENT] [-f FORMAT] [-s SERVICE] [-d]
                  [-S] [--desc [{on,off,auto}]] [--cache-dir CACHE_DIR]
                  [--progress-spinner {on,off}] [--timeout TIMEOUT]
                  [--path PATH] [-v] [--fix] [--require-hashes]
                  [--index-url INDEX_URL] [--extra-index-url URL]
                  [--skip-editable] [--no-deps] [-o FILE] [--ignore-vuln ID]
+                 [--disable-pip]
                  [project_path]
 
 audit the Python environment for dependencies with known vulnerabilities
 
 positional arguments:
   project_path          audit a local Python project at the given path
                         (default: None)
@@ -202,14 +203,17 @@
                         requirements are pinned to an exact version (default:
                         False)
   -o FILE, --output FILE
                         output results to the given file (default: stdout)
   --ignore-vuln ID      ignore a specific vulnerability by its vulnerability
                         ID; this option can be used multiple times (default:
                         [])
+  --disable-pip         don't use `pip` for dependency resolution; this can
+                        only be used with hashed requirements files or if the
+                        `--no-deps` flag has been provided (default: False)
 ```
 <!-- @end-pip-audit-help@ -->
 
 ### Exit codes
 
 On completion, `pip-audit` will exit with a code indicating its status.
```

### Comparing `pip_audit-2.5.6/pip_audit/_audit.py` & `pip_audit-2.6.0/pip_audit/_audit.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_cache.py` & `pip_audit-2.6.0/pip_audit/_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     A rough mirror of `pip`'s `SafeFileCache` that *should* be runtime-compatible
     with `pip` (i.e., does not interfere with `pip` when it shares the same
     caching directory as a running `pip` process).
     """
 
     def __init__(self, directory: Path):
         self._logged_warning = False
-        super().__init__(directory)
+        super().__init__(str(directory))
 
     def get(self, key: str) -> Any | None:
         try:
             return super().get(key)
         except Exception as e:  # pragma: no cover
             if not self._logged_warning:
                 logger.warning(
@@ -138,15 +138,15 @@
             if not self._logged_warning:
                 logger.warning(
                     f"Failed to delete file from cache directory, performance may be degraded: {e}"
                 )
                 self._logged_warning = True
 
 
-def caching_session(cache_dir: Path | None, *, use_pip: bool = False) -> CacheControl:
+def caching_session(cache_dir: Path | None, *, use_pip: bool = False) -> requests.Session:
     """
     Return a `requests` style session, with suitable caching middleware.
 
     Uses the given `cache_dir` for the HTTP cache.
 
     `use_pip` determines how the fallback cache directory is determined, if `cache_dir` is None.
     When `use_pip` is `False`, `caching_session` will use a `pip-audit` internal cache directory.
```

### Comparing `pip_audit-2.5.6/pip_audit/_cli.py` & `pip_audit-2.6.0/pip_audit/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,21 @@
         dest="ignore_vulns",
         default=[],
         help=(
             "ignore a specific vulnerability by its vulnerability ID; "
             "this option can be used multiple times"
         ),
     )
+    parser.add_argument(
+        "--disable-pip",
+        action="store_true",
+        help="don't use `pip` for dependency resolution; "
+        "this can only be used with hashed requirements files or if the `--no-deps` flag has been "
+        "provided",
+    )
     return parser
 
 
 def _parse_args(parser: argparse.ArgumentParser) -> argparse.Namespace:  # pragma: no cover
     args = parser.parse_args()
 
     # Configure logging upfront, so that we don't miss anything.
@@ -376,19 +383,24 @@
             parser.error("The --require-hashes flag can only be used with --requirement (-r)")
         elif args.index_url:
             parser.error("The --index-url flag can only be used with --requirement (-r)")
         elif args.extra_index_urls:
             parser.error("The --extra-index-url flag can only be used with --requirement (-r)")
         elif args.no_deps:
             parser.error("The --no-deps flag can only be used with --requirement (-r)")
+        elif args.disable_pip:
+            parser.error("The --disable-pip flag can only be used with --requirement (-r)")
 
     # Nudge users to consider alternate workflows.
     if args.require_hashes and args.no_deps:
         logger.warning("The --no-deps flag is redundant when used with --require-hashes")
 
+    if args.no_deps and args.disable_pip:
+        logger.warning("The --no-deps flag is redundant when used with --disable-pip")
+
     if args.require_hashes and isinstance(service, OsvService):
         logger.warning(
             "The --require-hashes flag with --service osv only enforces hash presence NOT hash "
             "validity. Use --service pypi to enforce hash validity."
         )
 
     if args.no_deps:
@@ -410,14 +422,15 @@
         source: DependencySource
         if args.requirements is not None:
             req_files: list[Path] = [Path(req.name) for req in args.requirements]
             source = RequirementSource(
                 req_files,
                 require_hashes=args.require_hashes,
                 no_deps=args.no_deps,
+                disable_pip=args.disable_pip,
                 skip_editable=args.skip_editable,
                 index_url=args.index_url,
                 extra_index_urls=args.extra_index_urls,
                 state=state,
             )
         elif args.project_path is not None:
             # NOTE: We'll probably want to support --skip-editable here,
```

### Comparing `pip_audit-2.5.6/pip_audit/_dependency_source/interface.py` & `pip_audit-2.6.0/pip_audit/_dependency_source/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,7 +53,16 @@
     fails to upgrade a package to a different version.
 
     Concrete implementations are expected to subclass this exception to provide
     more context.
     """
 
     pass
+
+
+class InvalidRequirementSpecifier(DependencySourceError):
+    """
+    A `DependencySourceError` specialized for the case of a non-PEP 440 requirements
+    specifier.
+    """
+
+    pass
```

### Comparing `pip_audit-2.5.6/pip_audit/_dependency_source/pip.py` & `pip_audit-2.6.0/pip_audit/_dependency_source/pip.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_dependency_source/pyproject.py` & `pip_audit-2.6.0/pip_audit/_dependency_source/pyproject.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_fix.py` & `pip_audit-2.6.0/pip_audit/_fix.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_format/columns.py` & `pip_audit-2.6.0/pip_audit/_format/columns.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_format/cyclonedx.py` & `pip_audit-2.6.0/pip_audit/_format/cyclonedx.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,46 +7,45 @@
 import logging
 from typing import cast
 
 from cyclonedx import output
 from cyclonedx.model.bom import Bom
 from cyclonedx.model.component import Component
 from cyclonedx.model.vulnerability import Vulnerability
-from cyclonedx.parser import BaseParser
 
 import pip_audit._fix as fix
 import pip_audit._service as service
 
 from .interface import VulnerabilityFormat
 
 logger = logging.getLogger(__name__)
 
 
-class _PipAuditResultParser(BaseParser):
-    def __init__(self, result: dict[service.Dependency, list[service.VulnerabilityResult]]):
-        super().__init__()
-
-        for dep, vulns in result.items():
-            # TODO(alex): Is there anything interesting we can do with skipped dependencies in
-            # the CycloneDX format?
-            if dep.is_skipped():
-                continue
-            dep = cast(service.ResolvedDependency, dep)
-
-            c = Component(name=dep.name, version=str(dep.version))
-            for vuln in vulns:
-                c.add_vulnerability(
-                    Vulnerability(
-                        id=vuln.id,
-                        description=vuln.description,
-                        recommendation="Upgrade",
-                    )
-                )
+def _pip_audit_result_to_bom(
+    result: dict[service.Dependency, list[service.VulnerabilityResult]]
+) -> Bom:
+    vulnerabilities = []
+    components = []
+
+    for dep, vulns in result.items():
+        # TODO(alex): Is there anything interesting we can do with skipped dependencies in
+        # the CycloneDX format?
+        if dep.is_skipped():
+            continue
+        dep = cast(service.ResolvedDependency, dep)
+
+        c = Component(name=dep.name, version=str(dep.version))
+        for vuln in vulns:
+            vulnerabilities.append(
+                Vulnerability(id=vuln.id, description=vuln.description, recommendation="Upgrade")
+            )
 
-            self._components.append(c)
+        components.append(c)
+
+    return Bom(components=components, vulnerabilities=vulnerabilities)
 
 
 class CycloneDxFormat(VulnerabilityFormat):
     """
     An implementation of `VulnerabilityFormat` that formats vulnerability results using CycloneDX.
     The container format used by CycloneDX can be additionally configured.
     """
@@ -86,17 +85,15 @@
         results.
 
         See `VulnerabilityFormat.format`.
         """
         if fixes:
             logger.warning("--fix output is unsupported by CycloneDX formats")
 
-        parser = _PipAuditResultParser(result)
-        bom = Bom.from_parser(parser)
-
+        bom = _pip_audit_result_to_bom(result)
         formatter = output.get_instance(
             bom=bom,
             output_format=self._inner_format.value,
             schema_version=output.SchemaVersion.V1_4,
         )
 
         return formatter.output_as_string()
```

### Comparing `pip_audit-2.5.6/pip_audit/_format/interface.py` & `pip_audit-2.6.0/pip_audit/_format/interface.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_format/json.py` & `pip_audit-2.6.0/pip_audit/_format/json.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_format/markdown.py` & `pip_audit-2.6.0/pip_audit/_format/markdown.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_service/__init__.py` & `pip_audit-2.6.0/pip_audit/_service/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_service/interface.py` & `pip_audit-2.6.0/pip_audit/_service/interface.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_service/osv.py` & `pip_audit-2.6.0/pip_audit/_service/osv.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_service/pypi.py` & `pip_audit-2.6.0/pip_audit/_service/pypi.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_state.py` & `pip_audit-2.6.0/pip_audit/_state.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_subprocess.py` & `pip_audit-2.6.0/pip_audit/_subprocess.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_util.py` & `pip_audit-2.6.0/pip_audit/_util.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pip_audit/_virtual_env.py` & `pip_audit-2.6.0/pip_audit/_virtual_env.py`

 * *Files identical despite different names*

### Comparing `pip_audit-2.5.6/pyproject.toml` & `pip_audit-2.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,39 +23,35 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Security",
 ]
 dependencies = [
-    "CacheControl[filecache] >= 0.12.0",
+    "CacheControl[filecache] >= 0.13.0",
     # NOTE(ww): Release 2.5.0 is broken, subsequent 2.5.x releases fix it.
     # See: https://github.com/CycloneDX/cyclonedx-python-lib/issues/245
-    "cyclonedx-python-lib ~= 2.0, != 2.5.0",
+    "cyclonedx-python-lib ~= 4.0",
     "html5lib>=1.1",
-    "packaging>=23.0.0",                     # https://github.com/pypa/pip-audit/issues/464
+    "packaging>=23.0.0",               # https://github.com/pypa/pip-audit/issues/464
     "pip-api>=0.0.28",
     "pip-requirements-parser>=32.0.0",
     "requests >= 2.31.0",
-    # NOTE(ww): We constrain this subdepency because of CacheControl's incompatibility
-    # with urllib3 ~= 2.0 by way of requests.
-    # See: https://github.com/ionrock/cachecontrol/issues/292
-    "urllib3 ~= 1.26",
     "rich>=12.4",
     "toml>=0.10",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 test = ["coverage[toml]", "pretend", "pytest", "pytest-cov"]
 lint = [
     "black>=22.3.0",
     # NOTE(ww): ruff is under active development, so we pin conservatively here
     # and let Dependabot periodically perform this update.
-    "ruff < 0.0.270",
+    "ruff < 0.0.276",
     "interrogate",
     "isort",
     "mypy",
     "types-html5lib",
     "types-requests",
     "types-toml",
 ]
```

### Comparing `pip_audit-2.5.6/PKG-INFO` & `pip_audit-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_audit
-Version: 2.5.6
+Version: 2.6.0
 Summary: A tool for scanning Python environments for known vulnerabilities
 Author-email: Alex Cameron <alex.cameron@trailofbits.com>, Dustin Ingram <di@python.org>, William Woodruff <william@trailofbits.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,30 +12,29 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
-Requires-Dist: CacheControl[filecache] >= 0.12.0
-Requires-Dist: cyclonedx-python-lib ~= 2.0, != 2.5.0
+Requires-Dist: CacheControl[filecache] >= 0.13.0
+Requires-Dist: cyclonedx-python-lib ~= 4.0
 Requires-Dist: html5lib>=1.1
 Requires-Dist: packaging>=23.0.0
 Requires-Dist: pip-api>=0.0.28
 Requires-Dist: pip-requirements-parser>=32.0.0
 Requires-Dist: requests >= 2.31.0
-Requires-Dist: urllib3 ~= 1.26
 Requires-Dist: rich>=12.4
 Requires-Dist: toml>=0.10
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: bump>=1.3.2 ; extra == "dev"
 Requires-Dist: pip-audit[doc,test,lint] ; extra == "dev"
 Requires-Dist: pdoc ; extra == "doc"
 Requires-Dist: black>=22.3.0 ; extra == "lint"
-Requires-Dist: ruff < 0.0.270 ; extra == "lint"
+Requires-Dist: ruff < 0.0.276 ; extra == "lint"
 Requires-Dist: interrogate ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: types-html5lib ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
 Requires-Dist: types-toml ; extra == "lint"
 Requires-Dist: coverage[toml] ; extra == "test"
@@ -154,15 +153,15 @@
 
 `pip-audit` has [`pre-commit`](https://pre-commit.com/) support.
 
 For example, using `pip-audit` via `pre-commit` to audit a requirements file:
 
 ```yaml
   - repo: https://github.com/pypa/pip-audit
-    rev: v2.5.6
+    rev: v2.6.0
     hooks:
       -   id: pip-audit
           args: ["-r", "requirements.txt"]
 
 ci:
   # Leave pip-audit to only run locally and not in CI
   # pre-commit.ci does not allow network calls
@@ -184,14 +183,15 @@
 ```
 usage: pip-audit [-h] [-V] [-l] [-r REQUIREMENT] [-f FORMAT] [-s SERVICE] [-d]
                  [-S] [--desc [{on,off,auto}]] [--cache-dir CACHE_DIR]
                  [--progress-spinner {on,off}] [--timeout TIMEOUT]
                  [--path PATH] [-v] [--fix] [--require-hashes]
                  [--index-url INDEX_URL] [--extra-index-url URL]
                  [--skip-editable] [--no-deps] [-o FILE] [--ignore-vuln ID]
+                 [--disable-pip]
                  [project_path]
 
 audit the Python environment for dependencies with known vulnerabilities
 
 positional arguments:
   project_path          audit a local Python project at the given path
                         (default: None)
@@ -254,14 +254,17 @@
                         requirements are pinned to an exact version (default:
                         False)
   -o FILE, --output FILE
                         output results to the given file (default: stdout)
   --ignore-vuln ID      ignore a specific vulnerability by its vulnerability
                         ID; this option can be used multiple times (default:
                         [])
+  --disable-pip         don't use `pip` for dependency resolution; this can
+                        only be used with hashed requirements files or if the
+                        `--no-deps` flag has been provided (default: False)
 ```
 <!-- @end-pip-audit-help@ -->
 
 ### Exit codes
 
 On completion, `pip-audit` will exit with a code indicating its status.
```

