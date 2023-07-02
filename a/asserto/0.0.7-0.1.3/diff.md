# Comparing `tmp/asserto-0.0.7.tar.gz` & `tmp/asserto-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asserto-0.0.7.tar", max compression
+gzip compressed data, was "asserto-0.1.3.tar", max compression
```

## Comparing `asserto-0.0.7.tar` & `asserto-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1064 2022-06-25 09:18:32.927103 asserto-0.0.7/LICENSE
--rw-r--r--   0        0        0     3842 2022-06-25 09:18:32.927103 asserto-0.0.7/README.md
--rw-r--r--   0        0        0      281 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/__init__.py
--rw-r--r--   0        0        0     2609 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_api.py
--rw-r--r--   0        0        0    18094 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_asserto.py
--rw-r--r--   0        0        0     1281 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_constants.py
--rw-r--r--   0        0        0      562 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_decorators.py
--rw-r--r--   0        0        0     3182 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_error_handling.py
--rw-r--r--   0        0        0     1935 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_exc_handling.py
--rw-r--r--   0        0        0      912 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_exceptions.py
--rw-r--r--   0        0        0        0 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_protocols.py
--rw-r--r--   0        0        0     1187 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_softly.py
--rw-r--r--   0        0        0     1281 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_templates.py
--rw-r--r--   0        0        0      340 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_types.py
--rw-r--r--   0        0        0      800 2022-06-25 09:18:32.927103 asserto-0.0.7/asserto/_util.py
--rw-r--r--   0        0        0      130 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/_warnings.py
--rw-r--r--   0        0        0      142 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/descriptors/__init__.py
--rw-r--r--   0        0        0      561 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/descriptors/_abc.py
--rw-r--r--   0        0        0      704 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/descriptors/_validators.py
--rw-r--r--   0        0        0      254 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/handlers/__init__.py
--rw-r--r--   0        0        0     2520 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/handlers/_base.py
--rw-r--r--   0        0        0      130 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/handlers/_date.py
--rw-r--r--   0        0        0      114 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/handlers/_files.py
--rw-r--r--   0        0        0     1099 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/handlers/_handler.py
--rw-r--r--   0        0        0     2055 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/handlers/_numeric.py
--rw-r--r--   0        0        0     1784 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/handlers/_regex.py
--rw-r--r--   0        0        0     1094 2022-06-25 09:18:32.931103 asserto-0.0.7/asserto/handlers/_strings.py
--rw-r--r--   0        0        0     1660 2022-06-25 09:18:32.931103 asserto-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4648 2022-06-25 09:19:17.435635 asserto-0.0.7/setup.py
--rw-r--r--   0        0        0     4298 2022-06-25 09:19:17.436128 asserto-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-02 11:38:03.004915 asserto-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3841 2023-07-02 11:38:03.004915 asserto-0.1.3/README.md
+-rw-r--r--   0        0        0      303 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/__init__.py
+-rw-r--r--   0        0        0     2609 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_api.py
+-rw-r--r--   0        0        0    19516 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_asserto.py
+-rw-r--r--   0        0        0     1369 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_constants.py
+-rw-r--r--   0        0        0      562 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_decorators.py
+-rw-r--r--   0        0        0     3182 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_error_handling.py
+-rw-r--r--   0        0        0     2714 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_exc_handling.py
+-rw-r--r--   0        0        0      923 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_protocols.py
+-rw-r--r--   0        0        0     1187 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_softly.py
+-rw-r--r--   0        0        0     1281 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_templates.py
+-rw-r--r--   0        0        0      295 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_types.py
+-rw-r--r--   0        0        0      928 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_util.py
+-rw-r--r--   0        0        0      130 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/_warnings.py
+-rw-r--r--   0        0        0      142 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/descriptors/__init__.py
+-rw-r--r--   0        0        0      561 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/descriptors/_abc.py
+-rw-r--r--   0        0        0      704 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/descriptors/_validators.py
+-rw-r--r--   0        0        0      254 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/__init__.py
+-rw-r--r--   0        0        0     2520 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_base.py
+-rw-r--r--   0        0        0        0 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_date.py
+-rw-r--r--   0        0        0        0 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_files.py
+-rw-r--r--   0        0        0     1199 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_handler.py
+-rw-r--r--   0        0        0     3544 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_numeric.py
+-rw-r--r--   0        0        0     1784 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_regex.py
+-rw-r--r--   0        0        0     1094 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/handlers/_strings.py
+-rw-r--r--   0        0        0        0 2023-07-02 11:38:03.004915 asserto-0.1.3/asserto/py.typed
+-rw-r--r--   0        0        0     1709 2023-07-02 11:38:03.008915 asserto-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 asserto-0.1.3/PKG-INFO
```

### Comparing `asserto-0.0.7/LICENSE` & `asserto-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/README.md` & `asserto-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 >through a fixture.  Asserto will work on any runner or even without one.  Note: It is common practice for a
 >test runner to apply assertion rewriting to change the behaviour of the `assert` keyword under the hood.
 
 The main features of asserto are (and will be):
 
 + Chainable and Fluent API.
 + Ability for both `Hard` and `Soft` assertions.
-+ Rich diffs to highlight problems, reduce churn and improve effeciency and debuggability.
-+ Dynamic assertions; check any obj attribute or invoke any of it's function types.
++ Rich diffs to highlight problems, reduce churn and improve efficiency and debug-ability.
++ Dynamic assertions; check any obj attribute or invoke any of its function types.
 + Robust set of methods out of the box for common types.
 + Extensibility.  Bolt on your own assertions at runtime.
 + Human error detection, elaborate warnings when something is amiss.
 + Much more to come.
 
 
 ## Feature Set:
```

### Comparing `asserto-0.0.7/asserto/_api.py` & `asserto-0.1.3/asserto/_api.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/asserto/_asserto.py` & `asserto-0.1.3/asserto/_asserto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
-import numbers
 import types
 import typing
 import warnings
 
 from ._constants import Methods
 from ._error_handling import ErrorHandler
 from ._error_handling import RaisesErrors
 from ._exc_handling import ExceptionChecker
 from ._exceptions import DynamicCallableWithArgsError
-from ._exceptions import HandlerTypeError
+from ._exceptions import UnsupportedHandlerTypeError
 from ._types import EXC_TYPES_ALIAS
 from ._types import RE_FLAGS_ALIAS
 from ._types import RE_PATTERN_ALIAS
 from ._util import is_namedtuple_like
 from ._warnings import NoAssertAttemptedWarning
 from .handlers import BaseHandler
 from .handlers import Handler
 from .handlers import NumberHandler
 from .handlers import RegexHandler
 from .handlers import StringHandler
 
 # Todo: base: `tidy up docstrings`
 # Todo: base `remove duplication here`
 # Todo: Api feels cumbersome with decorators; can we improve DRY-ness?
+# Todo: Consider short hand methods; are they worth it vs a single API?
 
 
 class Asserto:
     """
     The entrypoint into asserting objects.
 
     :param actual: ...
@@ -45,42 +45,36 @@
         self._triggered = False
         self.warn_unused = warn_unused
         self._in_context = False
         self._error_handler = error_handler()
         self.category: typing.Optional[str] = None
         self.description: typing.Optional[str] = None
 
+    def reassign(self, actual: typing.Any) -> Asserto:
+        """Binds the actual value to the given asserto instances actual value.  This is purposefully not
+        added as a property or promoted via simply attr assignment as it should be seldom used as is an
+        experimental API for now.
+
+        :param actual: The new actual value for underlying assertions.
+
+        ** EXPERIMENTAL: Subject to change **
+        """
+        self.actual = actual
+        return self
+
     def error(self, cause: typing.Union[AssertionError, str]) -> Asserto:
         """
         The single point of assertion failing.  All functions delegate here to raise the underlying
         assertion errors.
         :param cause: A reason for the failure. if description was set; it takes precedence.
         :return: The `Asserto` instance for fluency
         """
         self._error_handler.check_should_raise(self._in_context, cause, self.category, self.description)
         return self
 
-    @property
-    def triggered(self) -> bool:
-        """
-        Check if the instance has invoked any methods that could have raised an `AssertionError`.
-        :return: boolean indicating if a method has been invoked.
-        """
-        return self._triggered
-
-    @triggered.setter
-    def triggered(self, _) -> None:
-        """
-        Consider the asserto instance as `triggered`.  Instances which are instantiated but do not
-        invoke any assertion methods will omit a warning as this usually indicates user error and
-        helps to reduce mistakes in test code leading to misguided confidence in the test suite.
-        :return: The `Asserto` instance for fluency.
-        """
-        self._triggered = True
-
     def set_category(self, category: str) -> Asserto:
         """
         Set the category for the assertion.  Categories are prefixed to the assertion
         messages, for example:
 
             Example:
                 Usage::
@@ -136,14 +130,46 @@
     def is_digit(self) -> Asserto:
         """
         Asserts that the actual value contains only unicode letters and that the string has
         at least a single character.
         """
         return self._dispatch(StringHandler, Methods.IS_DIGIT)
 
+    def is_between(self, low: float, high: float, inclusive: bool = False):
+        """
+        Asserts that the actual value is between a low and high bounds.  If inclusive is true
+        the actual value is considered between if it is equal to either of those bounds.
+        """
+        return self._dispatch(NumberHandler, Methods.IS_BETWEEN, low, high, inclusive)
+
+    def is_between_inclusive(self, low: float, high: float) -> Asserto:
+        """
+        Asserts that the actual value is equal to or between the log and high bounds.
+        """
+        return self.is_between(low, high, inclusive=True)
+
+    is_between_incl = is_between_inclusive
+
+    def is_not_between(self, low: float, high: float, inclusive: bool = False):
+        """
+        Asserts that the actual value is between a **NOT** between a low and high bounds.  If inclusive is true
+        the actual value is only considered not between if it is strictly less than the low bounds and higher than
+        the high bounds, if it equals either it is considered to be between.
+        """
+        return self._dispatch(NumberHandler, Methods.IS_NOT_BETWEEN, low, high, inclusive)
+
+    def is_not_between_inclusive(self, low: float, high: float):
+        """
+        Asserts that the actual value is not between the low and high bounds.  if the actual value
+        is equal to the low or high bounds it is considered to be between them
+        """
+        return self.is_not_between(low, high, inclusive=True)
+
+    is_not_between_incl = is_not_between_inclusive
+
     def is_alpha(self) -> Asserto:
         """
         Asserts that the actual value contains only unicode letters and that the string has
         at least a single character.
         """
         return self._dispatch(StringHandler, Methods.IS_ALPHA)
 
@@ -221,14 +247,16 @@
         Compares the value against `other` for equality.
 
         :param other: The other object to compare against.
         :return: The instance of `Asserto` to chain asserts.
         """
         return self._dispatch(BaseHandler, Methods.IS_EQUAL_TO, other)
 
+    equals = is_equal_to
+
     def is_not_equal_to(self, other: typing.Any) -> Asserto:
         """
         Compares the value against `other` for non equality.
 
         :param other: The other object to compare against.
         :return: The instance of `Asserto` to chain asserts.
         """
@@ -297,30 +325,34 @@
     def is_not_zero(self) -> Asserto:
         """
         Checks the actual value is not zero.
         :return: The `Asserto` instance for fluency.
         """
         return self._dispatch(NumberHandler, Methods.IS_NOT_ZERO)
 
-    def is_greater_than(self, other: numbers.Number) -> Asserto:
+    def is_greater_than(self, other: float) -> Asserto:
         """Asserts that the value is numeric, and it is greater than other
 
         :param other: A number.Number to compare the value against.
         :return: This Asserto instance.
         """
         return self._dispatch(NumberHandler, Methods.IS_GREATER_THAN, other)
 
-    def is_lesser_than(self, other: numbers.Number) -> Asserto:
+    is_more_than = is_greater_than
+
+    def is_lesser_than(self, other: float) -> Asserto:
         """Asserts that the value is numeric, and it is lesser than other
 
         :param other: A number.Number to compare the value against.
         :return: This Asserto instance.
         """
         return self._dispatch(NumberHandler, Methods.IS_LESSER_THAN, other)
 
+    is_less_than = is_lesser_than
+
     def is_positive(self) -> Asserto:
         """Asserts that the value is numeric, and is greater than 0
 
         :return: This Asserto instance.
         """
         return self._dispatch(NumberHandler, Methods.IS_POSITIVE)
 
@@ -339,25 +371,25 @@
 
         Arbitrary args & kwargs to pass through to the handler method.
 
         Note: Debugging this with an IDE can yield unrealistic as debugging tends to insert
         arbitrary code into the stack and this relies on frame inspection.
         """
         __tracebackhide__ = True  # pytest magic.
-        self.triggered = True
+        self._triggered = True
         # for now allow this to be bypassed as not all methods have a handler defined.
         try:
             handler_instance = handler(self.actual)  # descriptors enforce types here.
         except ValueError:
             # The type of actual is not viable for the given handler.
-            raise HandlerTypeError(handler, method, self.actual) from None
+            raise UnsupportedHandlerTypeError(handler, method, self.actual) from None
         except KeyError:
             raise KeyError(f"{method} does not have a dedicated handler.") from None
         assertion_method: typing.Optional[types.MethodType] = getattr(handler_instance, method)
-        if assertion_method is None or not callable(assertion_method):
+        if not callable(assertion_method):
             raise TypeError(f"assertion method was not a bound method on the handler {handler_instance}")
         try:
             _ = assertion_method(*args, **kwargs)
         except AssertionError as e:
             if description := self.description:
                 e = AssertionError(description)
             self.error(e)
@@ -393,15 +425,15 @@
             if not named_tuple_like and mapping_like:
                 if key_attr not in self.actual:
                     failure = f"{self.actual!r} missing key: {key_attr}"
             else:
                 failure = f"{self.actual!r} missing attribute: {key_attr}"
 
         def _dynamic_callable(*args):
-            self.triggered = True  # Dynamic wrapper has been invoked!
+            self._triggered = True  # Dynamic wrapper has been invoked!
             if failure:
                 self.error(failure)
             if len(args) != 1:
                 raise TypeError(f"Dynamic assertion takes 1 argument but {len(args)} was given. {args}")
             value = self.actual[key_attr] if not named_tuple_like and mapping_like else getattr(self.actual, key_attr)
             if callable(value):
                 try:
@@ -433,11 +465,11 @@
 
     def __exit__(
         self,
         exc_type: typing.Optional[typing.Type[BaseException]] = None,
         exc_val: typing.Optional[BaseException] = None,
         exc_tb: typing.Optional[types.TracebackType] = None,
     ):
-        if self.warn_unused and not self.triggered:
+        if self.warn_unused and not self._triggered:
             self._warn_not_triggered()
         self._error_handler.check_soft_raise()
         self._error_handler.reset()
```

### Comparing `asserto-0.0.7/asserto/_constants.py` & `asserto-0.1.3/asserto/_constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-import dataclasses
+from enum import Enum
 
 
-@dataclasses.dataclass(frozen=True)
-class Methods:
+# StrEnum does not exist in 3.8
+class Methods(str, Enum):
     """
     Encapsulation of method names.  These are used as part of the dynamic dispatch
     to various handlers responsible for individual assertion methods.
     """
 
     # -- Strings
 
     ENDS_WITH: str = "ends_with"
     STARTS_WITH: str = "starts_with"
     IS_DIGIT: str = "is_digit"
     IS_ALPHA: str = "is_alpha"
+    IS_BETWEEN: str = "is_between"
+    IS_NOT_BETWEEN: str = "is_not_between"
 
     # -- Regular Expressions
 
     MATCH: str = "match"
     SEARCH: str = "search"
     FULLMATCH: str = "fullmatch"
     FINDALL: str = "findall"
```

### Comparing `asserto-0.0.7/asserto/_decorators.py` & `asserto-0.1.3/asserto/_decorators.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/asserto/_error_handling.py` & `asserto-0.1.3/asserto/_error_handling.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/asserto/_exc_handling.py` & `asserto-0.1.3/asserto/_exc_handling.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(
         self,
         exc_types: EXC_TYPES_ALIAS,
         value: typing.Callable[[typing.Any], typing.Any],
         _referent,
         match: typing.Optional[RE_PATTERN_ALIAS] = None,
     ) -> None:
-        self.exc_types: typing.Iterable[BaseException] = to_iterable(exc_types)
+        self.exc_types: typing.Iterable[typing.Type[BaseException]] = to_iterable(exc_types)
         self._proxy_val = value
         self.asserto_ref = _referent
         self.pattern: typing.Optional[re.Pattern[str]] = re.compile(match) if isinstance(match, str) else match
 
     def when_called_with(self, *args, **kwargs) -> None:
         """
         Call the underlying function with the user supplied arguments;  This returns the result
@@ -36,14 +36,26 @@
 
         # Todo: In future support a pattern match.
         # Todo: limitations in this API; what if the called arg has a `reason` attribute?
         """
         try:
             # update 'triggered' status to avoid unnecessary warnings
             self.asserto_ref.triggered = True  # type: ignore[attr-defined]
-            _ = self._proxy_val(*args, **kwargs)
+            self._proxy_val(*args, **kwargs)
+            # No exception was raised at all; raise an assertion error.
             self.asserto_ref.error(f"{self._proxy_val} never raised any of: {self.exc_types}")
-        except self.exc_types as e:  # type: ignore[misc]
-            if self.pattern is not None and self.pattern.match(str(e)) is None:
-                self.asserto_ref.error(
-                    f"Exception occurred but did not match pattern: {self.pattern} instead was: {str(e)}"
-                )
+        except BaseException as e:
+            exc_type, exc_string = type(e), str(e)
+            if isinstance(e, self.exc_types):  # type: ignore [arg-type]
+                if self.pattern:
+                    if self.pattern.match(exc_string) is None:
+                        # Type matched, but the pattern regex did not, raise.
+                        self.asserto_ref.error(
+                            f"{exc_type} occurred but did not match pattern: {self.pattern} instead was: {exc_string}"
+                        )
+                # type matched, no expected pattern, it was a success.
+                return
+            # The exception was not as expected, raise an assertion error against the type.
+            arguments = f"{args, kwargs}" if all((args, kwargs)) else "no arguments"
+            self.asserto_ref.error(
+                f"{self._proxy_val.__name__} did not raise any of {self.exc_types}.  Instead it raised {exc_type} when called with {arguments}."  # noqa
+            )
```

### Comparing `asserto-0.0.7/asserto/_exceptions.py` & `asserto-0.1.3/asserto/_exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,12 +19,12 @@
     """
     Raised when a dynamic lookup via `attr_is` returns a callable that expects arguments.
     Asserto currently only supports 0-arg callables as part of its dynamic lookup and
     invocations.
     """
 
 
-class HandlerTypeError(ValueError):
+class UnsupportedHandlerTypeError(ValueError):
     """Raised when the actual value passed to a handler is not suitable for it to handle."""
 
     def __init__(self, handler: typing.Type[Handler], method: str, value: typing.Any) -> None:
         super().__init__(f"`{handler.__name__}` cannot accept type: {type(value)} when calling: {method}")
```

### Comparing `asserto-0.0.7/asserto/_softly.py` & `asserto-0.1.3/asserto/_softly.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/asserto/_templates.py` & `asserto-0.1.3/asserto/_templates.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/asserto/_util.py` & `asserto-0.1.3/asserto/_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,7 +25,12 @@
     bases = t.__bases__
     if len(bases) != 1 and bases[0] != tuple:
         return False
     fields = getattr(obj, "_fields", None)
     if not isinstance(fields, tuple):
         return False
     return all(type(f) == str for f in fields)
+
+
+def object_to_name(obj: typing.Any) -> str:
+    """Returns the class name of any object."""
+    return obj.__class__.__name__
```

### Comparing `asserto-0.0.7/asserto/descriptors/_abc.py` & `asserto-0.1.3/asserto/descriptors/_abc.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/asserto/descriptors/_validators.py` & `asserto-0.1.3/asserto/descriptors/_validators.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/asserto/handlers/_base.py` & `asserto-0.1.3/asserto/handlers/_base.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/asserto/handlers/_handler.py` & `asserto-0.1.3/asserto/handlers/_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,7 +22,10 @@
 
     def raise_if_length_equals(self, length: int = 0) -> typing.Literal[True]:
         """Checks the length of a Sized implementation and raises a ValueError if it is zero.
         Returns `True` if it succeeds to allow chaining of checks in handler subclasses."""
         if len(self.actual) == length:
             raise ValueError(f"{self.actual} is empty.")
         return True
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(actual={self.actual!r})"
```

### Comparing `asserto-0.0.7/asserto/handlers/_regex.py` & `asserto-0.1.3/asserto/handlers/_regex.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/asserto/handlers/_strings.py` & `asserto-0.1.3/asserto/handlers/_strings.py`

 * *Files identical despite different names*

### Comparing `asserto-0.0.7/pyproject.toml` & `asserto-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.towncrier]
 directory = "changes"
 filename = "CHANGELOG.rst"
-version = "0.0.7"
+version = "21.9.0"
 name = "asserto"
 underlines = "=-~"
 all_bullets = true
 
 [tool.poetry]
 name = "asserto"
-version = "0.0.7"
+version = "0.1.3"
 description = "A fluent DSL for python assertions."
 authors = ["symonk <jackofspaces@gmail.com>"]
 readme = "README.md"
+include = ["asserto/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-rich = "^12.4.4"
+rich = "^13.3.4"
 
 [tool.poetry.dev-dependencies]
 codecov = "^2.1.12"
-pre-commit = "^2.19.0"
-mkdocs = "^1.3.0"
-mkdocs-material = "^8.3.8"
+pre-commit = "^2.20.0"
+mkdocs = "^1.4.0"
+mkdocs-material = "^9"
 mkdocstrings= {extras = ["python"], version = "^0.19.0"}
-pytest = "^7.1.2"
-tox = "^3.25.0"
-pip = "^22.0.4"
-coverage = "^6.4.1"
-towncrier = "^21.9.0"
-poetryup = "^0.8.1"
+pytest = "^7"
+tox = "^4"
+pip = "^22"
+coverage = "^7"
+towncrier = "^22"
+
+[tool.poetry.group.dev.dependencies]
+pytest-xdist = "^3.3.1"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore:RequestsDependencyWarning:"
 ]
 
 [tool.isort]
```

### Comparing `asserto-0.0.7/setup.py` & `asserto-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,159 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: asserto
+Version: 0.1.3
+Summary: A fluent DSL for python assertions.
+Author: symonk
+Author-email: jackofspaces@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['asserto', 'asserto.descriptors', 'asserto.handlers']
+![Asserto](.github/images/logo.png)
 
-package_data = \
-{'': ['*']}
+![version](https://img.shields.io/pypi/v/asserto?color=%2342f54b&label=asserto&style=flat-square)
+[![codecov](https://codecov.io/gh/symonk/asserto/branch/main/graph/badge.svg)](https://codecov.io/gh/symonk/asserto)
+[![docs](https://img.shields.io/badge/documentation-online-brightgreen.svg)](https://symonk.github.io/asserto/)
 
-install_requires = \
-['rich>=12.4.4,<13.0.0']
-
-setup_kwargs = {
-    'name': 'asserto',
-    'version': '0.0.7',
-    'description': 'A fluent DSL for python assertions.',
-    'long_description': '![Asserto](.github/images/logo.png)\n\n![version](https://img.shields.io/pypi/v/asserto?color=%2342f54b&label=asserto&style=flat-square)\n[![codecov](https://codecov.io/gh/symonk/asserto/branch/main/graph/badge.svg)](https://codecov.io/gh/symonk/asserto)\n[![docs](https://img.shields.io/badge/documentation-online-brightgreen.svg)](https://symonk.github.io/asserto/)\n\n## Asserto:\n\nAsserto is a clean, fluent and powerful assertion library for python.  We recommend using `pytest` as a test\nrunner but asserto will work well with any test runner.\n\n>Asserto was developed using pytest as it\'s test runner and has a `pytest-asserto` plugin that exposes asserto\n>through a fixture.  Asserto will work on any runner or even without one.  Note: It is common practice for a\n>test runner to apply assertion rewriting to change the behaviour of the `assert` keyword under the hood.\n\nThe main features of asserto are (and will be):\n\n+ Chainable and Fluent API.\n+ Ability for both `Hard` and `Soft` assertions.\n+ Rich diffs to highlight problems, reduce churn and improve effeciency and debuggability.\n+ Dynamic assertions; check any obj attribute or invoke any of it\'s function types.\n+ Robust set of methods out of the box for common types.\n+ Extensibility.  Bolt on your own assertions at runtime.\n+ Human error detection, elaborate warnings when something is amiss.\n+ Much more to come.\n\n\n## Feature Set:\n\n#### Fluent API:\n\n`Asserto` exposes a fully fluent API for chaining assertions against a value.\n\n```python\nfrom asserto import asserto\n\n\ndef test_multiple_assert_fluency() -> None:\n    asserto("Hello").has_length(5).match(r"\\w{5}$").ends_with("lo").starts_with("Hel")\n```\n\n----\n\n#### Soft Assertions:\n\n\n`Asserto` Has `soft` capabilities; allowing multiple assertions to be performed before failing with a\nsummary of the failures.\n\n```python\nfrom asserto import asserto\n\ndef test_baz() -> None:\n    with asserto("Baz") as context:\n        # asserto when used in a python context is run in \'soft\' mode;\n        # upon exiting the context; congregated errors are subsequently raised (if any)\n        context.starts_with("B").ends_with("z").is_equal_to("Baz").has_length(2)  # Ends in a failure.\n```\n\nWill result in the following:\n\n```shell\n    def test_foo(asserto) -> None:\n>       with asserto("Bar") as context:\nE       AssertionError: 1 Soft Assertion Failures\nE       [AssertionError("Length of: \'Bar\' was not equal to: 2")]\n```\n\n-----\n\n#### Exception Handling:\n\n`Asserto` has the ability to assert exceptions are raised on `callables` using a simple API.\n\n```python\nfrom asserto import asserto\nimport typing\n\n\ndef simple_callable(x: int) -> typing.NoReturn:\n    raise ValueError(x)\n\n\ndef test_exc_handling():\n    asserto(simple_callable).should_raise(ValueError).when_called_with(25)\n```\n\n-----\n\n#### Dynamic Lookups:\n\n`Asserto` has the ability to dynamically lookup attributes on any object type.  This is\nhandled using the `attr_is(expected)` syntax.\n\n```python\nfrom asserto import asserto\n\n\nclass Foo:\n\n    def __init__(self, x) -> None:\n        self.x = x\n\n    def double_x(self) -> int:\n        return self.x * 2\n\n\ndef test_foo_dynamically() -> None:\n     # dynamically looking up `x` (attr) or `double_x` bound method & invoking it!\n    asserto(Foo(10)).x_is(10).double_x_is(20)\n```\n\n-----\n\n#### Dynamic assert registration\n\n`Asserto` allows users to easily bolt on their assertion functions.\n\n```python\nfrom asserto import asserto\nfrom asserto import register_assert\n\n\n@register_assert  # Option 1.\ndef custom_assert(self):\n    if self.actual != 5:\n        self.check_should_raise(f"{self.actual} did not equal five!")\n\n\nregister_assert(custom_assert)  # Option 2\n\n\ndef test_user_defined_callables() -> None:\n    asserto(6).custom_assert()\n```\n\nyields the following:\n\n```console\nE       AssertionError: 6 did not equal five!\n```\n\n-----\n',
-    'author': 'symonk',
-    'author_email': 'jackofspaces@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+## Asserto:
 
+Asserto is a clean, fluent and powerful assertion library for python.  We recommend using `pytest` as a test
+runner but asserto will work well with any test runner.
+
+>Asserto was developed using pytest as it's test runner and has a `pytest-asserto` plugin that exposes asserto
+>through a fixture.  Asserto will work on any runner or even without one.  Note: It is common practice for a
+>test runner to apply assertion rewriting to change the behaviour of the `assert` keyword under the hood.
+
+The main features of asserto are (and will be):
+
++ Chainable and Fluent API.
++ Ability for both `Hard` and `Soft` assertions.
++ Rich diffs to highlight problems, reduce churn and improve efficiency and debug-ability.
++ Dynamic assertions; check any obj attribute or invoke any of its function types.
++ Robust set of methods out of the box for common types.
++ Extensibility.  Bolt on your own assertions at runtime.
++ Human error detection, elaborate warnings when something is amiss.
++ Much more to come.
+
+
+## Feature Set:
+
+#### Fluent API:
+
+`Asserto` exposes a fully fluent API for chaining assertions against a value.
+
+```python
+from asserto import asserto
+
+
+def test_multiple_assert_fluency() -> None:
+    asserto("Hello").has_length(5).match(r"\w{5}$").ends_with("lo").starts_with("Hel")
+```
+
+----
+
+#### Soft Assertions:
+
+
+`Asserto` Has `soft` capabilities; allowing multiple assertions to be performed before failing with a
+summary of the failures.
+
+```python
+from asserto import asserto
+
+def test_baz() -> None:
+    with asserto("Baz") as context:
+        # asserto when used in a python context is run in 'soft' mode;
+        # upon exiting the context; congregated errors are subsequently raised (if any)
+        context.starts_with("B").ends_with("z").is_equal_to("Baz").has_length(2)  # Ends in a failure.
+```
+
+Will result in the following:
+
+```shell
+    def test_foo(asserto) -> None:
+>       with asserto("Bar") as context:
+E       AssertionError: 1 Soft Assertion Failures
+E       [AssertionError("Length of: 'Bar' was not equal to: 2")]
+```
+
+-----
+
+#### Exception Handling:
+
+`Asserto` has the ability to assert exceptions are raised on `callables` using a simple API.
+
+```python
+from asserto import asserto
+import typing
+
+
+def simple_callable(x: int) -> typing.NoReturn:
+    raise ValueError(x)
+
+
+def test_exc_handling():
+    asserto(simple_callable).should_raise(ValueError).when_called_with(25)
+```
+
+-----
+
+#### Dynamic Lookups:
+
+`Asserto` has the ability to dynamically lookup attributes on any object type.  This is
+handled using the `attr_is(expected)` syntax.
+
+```python
+from asserto import asserto
+
+
+class Foo:
+
+    def __init__(self, x) -> None:
+        self.x = x
+
+    def double_x(self) -> int:
+        return self.x * 2
+
+
+def test_foo_dynamically() -> None:
+     # dynamically looking up `x` (attr) or `double_x` bound method & invoking it!
+    asserto(Foo(10)).x_is(10).double_x_is(20)
+```
+
+-----
+
+#### Dynamic assert registration
+
+`Asserto` allows users to easily bolt on their assertion functions.
+
+```python
+from asserto import asserto
+from asserto import register_assert
+
+
+@register_assert  # Option 1.
+def custom_assert(self):
+    if self.actual != 5:
+        self.check_should_raise(f"{self.actual} did not equal five!")
+
+
+register_assert(custom_assert)  # Option 2
+
+
+def test_user_defined_callables() -> None:
+    asserto(6).custom_assert()
+```
+
+yields the following:
+
+```console
+E       AssertionError: 6 did not equal five!
+```
+
+-----
 
-setup(**setup_kwargs)
```

