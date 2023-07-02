# Comparing `tmp/meth-1.0.1.tar.gz` & `tmp/meth-1.1.0.tar.gz`

## Comparing `meth-1.0.1.tar` & `meth-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 meth-1.0.1/test.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 meth-1.0.1/examples/calculator.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 meth-1.0.1/meth/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 meth-1.0.1/meth/builtins.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 meth-1.0.1/meth/error.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 meth-1.0.1/meth/interpreter.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 meth-1.0.1/meth/lexer.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 meth-1.0.1/meth/nodes.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 meth-1.0.1/meth/parser.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 meth-1.0.1/meth/token.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 meth-1.0.1/meth/utils.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 meth-1.0.1/meth/functions/__init__.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 meth-1.0.1/meth/functions/simplify.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 meth-1.0.1/meth/functions/stringify.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 meth-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 meth-1.0.1/tests/test_evaluate.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 meth-1.0.1/tests/test_simplify.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 meth-1.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 meth-1.0.1/LICENSE
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 meth-1.0.1/README.md
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 meth-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 meth-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 meth-1.1.0/test.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 meth-1.1.0/examples/calculator.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 meth-1.1.0/meth/__init__.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 meth-1.1.0/meth/builtins.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 meth-1.1.0/meth/error.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 meth-1.1.0/meth/interpreter.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 meth-1.1.0/meth/lexer.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 meth-1.1.0/meth/nodes.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 meth-1.1.0/meth/parser.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 meth-1.1.0/meth/token.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 meth-1.1.0/meth/utils.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 meth-1.1.0/meth/functions/__init__.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 meth-1.1.0/meth/functions/simplify.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 meth-1.1.0/meth/functions/stringify.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 meth-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 meth-1.1.0/tests/test_evaluate.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 meth-1.1.0/tests/test_simplify.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 meth-1.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 meth-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 meth-1.1.0/README.md
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 meth-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 meth-1.1.0/PKG-INFO
```

### Comparing `meth-1.0.1/meth/builtins.py` & `meth-1.1.0/meth/builtins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Any
 import math
 
 
 def meth_ln(x: float | int):
     return math.log(x)
 
 
@@ -66,19 +67,35 @@
     "floor": math.floor,
     "ceil": math.ceil,
     "round": round,
     "min": meth_min,
     "max": meth_max
 }
 
-def is_builtin(name: str):
-    """Checks to see if name is a builtin."""
+def is_builtin(name: str) -> bool:
+    """
+    Checks to see if name is a builtin.
+
+    Args:
+        name: str
+            Name to check.
+
+    Returns: bool
+    """
     return name in BUILTINS or name in CONSTANTS or name in SPECIAL_CONST_SYM
 
-def get_builtin(name: str):
-    """Get builtin from name."""
+def get_builtin(name: str) -> Any:
+    """
+    Get builtin from name.
+    
+    Args:
+        name: str
+            Name of builtin.
+
+    Returns: Any | None if not found
+    """
     if name in BUILTINS:
         return BUILTINS[name]
     elif name in CONSTANTS:
         return CONSTANTS[name]
     elif name in SPECIAL_CONST_SYM:
-        return SPECIAL_CONST_SYM[name]
+        return SPECIAL_CONST_SYM[name]
```

### Comparing `meth-1.0.1/meth/interpreter.py` & `meth-1.1.0/meth/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .nodes import *
 from .token import *
 from . import error
 
 
 class Function:
     def __init__(self, func_node: FunctionNode, func: BaseNode) -> None:
+        """Initializes a meth function."""
         self.name = func_node.value.value
         self.args = func_node.left
         self.func = func
 
     def __call__(self, *args) -> None:
         if len(args) != len(self.args):
             raise error.ArgumentError(
@@ -20,23 +21,37 @@
 
         return Interpreter(
             {self.args[i].value: args[i] for i in range(len(self.args))}
         ).interpret(self.func)
 
 
 class Interpreter:
-    def __init__(self, vars: dict = {}) -> None:
-        """Initialize the interpreter."""
+    def __init__(self, vars: dict[str, int | float] = {}) -> None:
+        """
+        Initializes the interpreter.
+
+        Args:
+            vars: dict[str, int | float] = {}
+                Dictionary of variables.
+        """
         self.vars = vars
 
-    def interpret(self, ast: BaseNode) -> int | float:
-        """Interpret an AST."""
+    def interpret(self, ast: BaseNode) -> int | float | None:
+        """
+        Interpret an AST.
+
+        Args:
+            ast: Node
+                Tree to interpret.
+
+        Returns: int | float | None
+        """
         return self._visit(ast)
 
-    def _visit(self, node: BaseNode) -> int | float:
+    def _visit(self, node: BaseNode):
         return getattr(self, "_visit_" + type(node).__name__)(node)
 
     def _visit_Token(self, token: Token):
         if token.type == TT_IDENTIFIER:
             is_var = token.value in self.vars
             if not is_var and (builtin := get_builtin(token.value)) is None:
                 raise error.VarNotDefinedError(f"{token.value} is not defined.")
```

### Comparing `meth-1.0.1/meth/lexer.py` & `meth-1.1.0/meth/lexer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,95 +1,85 @@
 import string
 
 from .builtins import *
 from .token import *
 from . import error
 
 
-TOKENS = {
-    "(": TT_LBRACKET,
-    ")": TT_RBRACKET,
-    "=": TT_EQUAL,
-    ",": TT_COMMA,
-    "+": TT_PLUS,
-    "-": TT_MINUS,
-    "*": TT_MUL,
-    "/": TT_DIV,
-    "%": TT_MOD,
-    "^": TT_POW,
-}
-
-
 class Lexer:
-    def __init__(self, expr: str) -> None:
+    def __init__(self) -> None:
         """Initialize the lexer / tokenizer."""
-        self.expr = expr
-        self.i = -1
-        self.next()
+        pass
 
-    def next(self):
+    def _next(self):
         """Advances to the next character."""
         self.i += 1
         self.curr = self.expr[self.i] if self.i < len(self.expr) else None
 
-    def tokenize(self):
-        """Tokenizes the expression."""
+    def tokenize(self, expr: str) -> list[Token]:
+        """
+        Tokenizes the expression.
+
+        Args:
+            expr: str
+                Expression to tokenize.
+
+        Returns: list[Token]
+        """
+        self.expr = expr
+        self.i = -1
+        self._next()
+
         tokens = []
 
         while self.curr:
             if self.curr == " ":
-                pass
+                self._next()
             elif self.curr in string.digits:
-                tokens.append(self.number())
-            elif self.curr in TOKENS:
-                tokens.append(Token(TOKENS[self.curr]))
+                tokens.append(self._number())
             elif self.curr in string.ascii_letters:
-                tokens += self.identifier()
+                tokens += self._identifier()
+            elif self.curr in OPERATORS:
+                tokens.append(Token(OPERATORS[self.curr]))
+                self._next()
             elif self.curr in SPECIAL_CONST_SYM:
                 tokens.append(Token(TT_IDENTIFIER, self.curr))
+                self._next()
             else:
                 raise error.SyntaxError(f"Invalid character '{self.curr}'")
 
-            self.next()
-
         return tokens
 
-    def number(self) -> Token:
+    def _number(self) -> Token:
         """Tokenizes a number."""
         number = ""
         is_float = False
 
         while self.curr and self.curr in string.digits + ".":
             if self.curr == ".":
                 if is_float:
                     raise error.SyntaxError("Unexpected '.'")
 
                 is_float = True
 
             number += self.curr
-            self.next()
-
-        self.i -= 1
-        self.curr = self.expr[self.i]
+            self._next()
 
         return Token(
             TT_FLOAT if is_float else TT_INT, (float if is_float else int)(number)
         )
 
-    def identifier(self) -> list[Token]:
+    def _identifier(self) -> list[Token]:
         """Tokenizes an identifier."""
         identifier = ""
 
         while self.curr and (
             self.curr in string.ascii_letters or self.curr in string.digits
         ):
             identifier += self.curr
-            self.next()
-
-        self.i -= 1
-        self.curr = self.expr[self.i]
+            self._next()
 
         return (
             [Token(TT_IDENTIFIER, identifier)]
             if is_builtin(identifier)
             else [Token(TT_IDENTIFIER, idf) for idf in identifier]
         )
```

### Comparing `meth-1.0.1/meth/nodes.py` & `meth-1.1.0/meth/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .token import *
 
 
 class BaseNode:
     def __init__(self, value, left=None, right=None, is_paren=False) -> None:
-        """Base class for all nodes."""
+        """Base class for all node tyoes."""
         self.value = value
         self.left = left
         self.right = right
         self.is_paren = is_paren
 
         self.name = type(self).__name__
```

### Comparing `meth-1.0.1/meth/parser.py` & `meth-1.1.0/meth/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,66 @@
 from . import utils, error
 from .token import *
 from .nodes import *
 
 
 class Parser:
-    def __init__(self, tokens: list[Token]) -> None:
+    def __init__(self) -> None:
         """Initialize the parser."""
-        self.tokens = tokens
-        self.node = None
-        self.i = -1
-        self.next()
+        pass
 
-    def next(self, check_EOF: bool = False, change_curr=True):
+    def _next(self, check_EOF: bool = False, change_curr: bool = True):
         """Advances to the next token."""
-        if not change_curr:
-            n = self.tokens[self.i + 1] if self.i + 1 < len(self.tokens) else None
-            if check_EOF and n is None:
-                raise error.SyntaxError("Unexpected end of expression.")
-
-            return n
-
         self.i += 1
-        self.curr = self.tokens[self.i] if self.i < len(self.tokens) else None
+        token = self.tokens[self.i] if self.i < len(self.tokens) else None
 
-        if check_EOF and self.curr is None:
+        if check_EOF and token is None:
             raise error.SyntaxError("Unexpected end of expression.")
 
-        return self.curr
+        if change_curr:
+            self.curr = token
+        else:
+            self.i -= 1
+
+        return token
+
+    def parse(
+        self,
+        tokens: list[Token],
+        disallow_assign: bool = False,
+        in_args: bool = False,
+        is_paren: bool = False,
+    ) -> BaseNode:
+        """
+        Parse the inputted tokens.
+
+        Args:
+            tokens: list[Token]
+                List of tokens to parse.
+
+        Internal Args:
+            disallow_assign: bool = False
+                Raises an error if an assignment is found.
+            in_args: bool = False
+                Parses tokens as arguments.
+            is_paren: bool = False
+                Sets the is_paren value of the node.
+
+        Returns: Node
+        """
+        self.tokens = tokens
+        self.i = -1
+        self._next()
 
-    def parse(self, disallow_assign=False, args=False, is_paren=False):
-        """Parse the inputted tokens."""
         if self.curr is None:
             return None
 
         self.node = self.curr
-        if args:
-            res = []
+        if in_args:
+            args = []
 
         if self.curr not in [
             TT_PLUS,
             TT_MINUS,
             TT_LBRACKET,
             TT_IDENTIFIER,
             TT_INT,
@@ -48,114 +69,116 @@
             raise error.SyntaxError(f"Unexpected character {self.curr.type}.")
 
         while self.curr:
             last_tok = self.tokens[self.i - 1] if self.i > 0 else None
 
             if self.curr in [TT_PLUS, TT_MINUS]:
                 op_type = self.curr.type
-                right = self.factor()
+                right = self._factor()
 
                 self.node = (
                     UnaryOpNode(op_type, right)
                     if self.node in [TT_PLUS, TT_MINUS]
                     else BinaryOpNode(op_type, self.node, right)
                 )
             elif self.curr in [TT_MUL, TT_DIV, TT_MOD]:
-                self.binary_op(self.curr.type, stop_at=[TT_POW])
+                self._binary_op(self.curr.type, stop_at=[TT_POW])
             elif self.curr == TT_POW:
-                self.binary_op(TT_POW)
+                self._binary_op(TT_POW)
             elif self.curr == TT_LBRACKET:
-                node = utils.get_final_node(self.node)
+                node = utils.get_leaf_node_right(self.node, True)
 
-                # check if its like 2(x + 1)
+                # check for 2(x + 1) or (1 + 2)(2 * 2)
                 is_mul = last_tok in [TT_INT, TT_FLOAT] or getattr(
                     node, "is_paren", False
                 )
                 is_func = last_tok == TT_IDENTIFIER
 
-                right = self.factor(is_func)
+                right = self._factor(is_func)
                 fr = right if is_func else [right]
 
                 if type(node) != Token and not node.is_paren:
                     node.right = (
                         FunctionNode(node.right, fr) if is_func or is_mul else right
                     )
                 else:
                     self.node = FunctionNode(node, fr) if is_func or is_mul else right
             elif self.curr == TT_IDENTIFIER:
                 if last_tok in [
                     TT_INT,
                     TT_FLOAT,
                     TT_IDENTIFIER,
                 ]:
-                    self.binary_op(TT_MUL, self.curr, is_paren=True)
+                    self._binary_op(TT_MUL, self.curr, is_paren=True)
             elif not disallow_assign and self.curr == TT_EQUAL:
                 self.node = AssignNode(
-                    self.node, Parser(self.tokens[self.i + 1 :]).parse(True)
+                    self.node, Parser().parse(self.tokens[self.i + 1 :], True)
                 )
                 self.i = len(self.tokens)
-            elif args and self.curr == TT_COMMA:
+            elif in_args and self.curr == TT_COMMA:
                 self.node.is_paren = is_paren
-                res.append(self.node)
-                self.node = self.next(True, False)
+                args.append(self.node)
+                self.node = self._next(check_EOF=True, change_curr=False)
             else:
                 if (last_tok in [TT_INT, TT_FLOAT, TT_IDENTIFIER, TT_RBRACKET]) or (
-                    self.next(change_curr=False)
+                    self._next(change_curr=False)
                     in [
                         TT_INT,
                         TT_FLOAT,
                         TT_RBRACKET,
                     ]
                 ):
                     raise error.SyntaxError(f"Unexpected character {self.curr}")
 
-            self.next()
+            self._next()
 
-        if args:
-            res.append(self.node)
+        if in_args:
+            args.append(self.node)
         else:
             self.node.is_paren = is_paren
 
-        return self.node if not args else res
+        return args if in_args else self.node
 
-    def factor(self, func=False):
+    def _factor(self, in_args: bool = False):
         """Parse a factor."""
-        self.next(True)
+        self._next(True)
 
         if TT_LBRACKET in [self.curr, self.tokens[self.i - 1]]:
             if self.curr == TT_LBRACKET:
-                self.next(True)
+                self._next(True)
 
             tokens = []
             opened = 1
 
             # get all tokens in bracket
             while opened:
                 tokens.append(self.curr)
-                self.next(True)
+                self._next(True)
 
                 if self.curr == TT_RBRACKET:
                     opened -= 1
                 elif self.curr == TT_LBRACKET:
                     opened += 1
 
-            return Parser(tokens).parse(True, func, True)
+            return Parser().parse(tokens, True, in_args, True)
         elif self.curr in [TT_INT, TT_FLOAT, TT_IDENTIFIER]:
             return self.curr
         elif self.curr in [TT_PLUS, TT_MINUS]:
             # cases like -1, +1
-            return UnaryOpNode(self.curr.type, self.factor())
+            return UnaryOpNode(self.curr.type, self._factor())
         else:
             raise error.SyntaxError(f"Invalid character {self.curr.type}")
 
-    def binary_op(self, op_type, right=None, stop_at=[], is_paren=False):
+    def _binary_op(
+        self, op_type, right=None, stop_at: list = [], is_paren: bool = False
+    ):
         """Parse a binary operation."""
-        node = utils.get_final_node(self.node, stop_at=stop_at)
+        node = utils.get_leaf_node_right(self.node, True, stop_at=stop_at)
         if right is None:
-            right = self.factor()
+            right = self._factor()
 
         # if is_paren is True then i shouldn't change it
         if type(node) not in [Token, UnaryOpNode] and not getattr(
             node.right, "is_paren", False
         ):
             node.right = BinaryOpNode(op_type, node.right, right, is_paren)
         else:
```

### Comparing `meth-1.0.1/meth/functions/simplify.py` & `meth-1.1.0/meth/functions/simplify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,29 @@
+from ..utils import create_number_token
 from ..parser import Parser
 from ..lexer import Lexer
 from ..token import *
 from ..nodes import *
 
 
 def simplify(expr: BaseNode | str):
     "Simplify an expression. WARNING: This is unfinished and may contain bugs."
     if type(expr) == str:
-        expr = Parser(Lexer(expr).tokenize()).parse()
+        expr = Parser().parse(Lexer().tokenize(expr))
     return simplify_node(expr)
 
 
 def is_number(token: Token):
     return token in [TT_INT, TT_FLOAT]
 
 
 def is_var_mul(node: BinaryOpNode):
     return node.value == TT_MUL and is_number(node.left) and node.right == TT_IDENTIFIER
 
 
-def create_number_token(number: int | float) -> Token:
-    is_int = type(number) == int
-    return Token(TT_INT if is_int else TT_FLOAT, number)
-
-
 def simplify_node(node: BaseNode | Token):
     node_t = type(node)
 
     if node is None or type(node) == Token:
         return node
     elif node_t == BinaryOpNode:
         return simplify_binaryop(node)
```

### Comparing `meth-1.0.1/meth/functions/stringify.py` & `meth-1.1.0/meth/functions/stringify.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,14 +12,23 @@
     TT_DIV: "/",
     TT_MOD: "%",
     TT_POW: "^",
 }
 
 
 def stringify(node: BaseNode | Token) -> str:
+    """
+    Stringifies a tree into an equation string.
+
+    Args:
+        node: Node | Token
+            The tree to turn into an equation string.
+
+    Returns: str
+    """
     node_t = type(node)
 
     if node_t == Token:
         return str(node.value) if node.value else TT_CONV[node.type]
     elif node_t == BinaryOpNode:
         # check for 3x
         if (
```

### Comparing `meth-1.0.1/tests/test_evaluate.py` & `meth-1.1.0/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `meth-1.0.1/tests/test_simplify.py` & `meth-1.1.0/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `meth-1.0.1/LICENSE` & `meth-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meth-1.0.1/README.md` & `meth-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,25 @@
 # Examples
 
 > _More examples in the [examples/](https://github.com/sertdfyguhi/meth/tree/master/examples) directory._
 
 ```py
 import meth
 
+# tokenizing equations
+meth.tokenize("5 + 2") # INT(5), PLUS, INT(2)
+
+# parsing equations
+meth.parse("2 * 10") # BinaryOpNode(INT(2), MUL, INT(10))
+
+# evaluating equations
 meth.evaluate("2 + 2") # 4
 meth.evaluate("sqrt(9)") # 3
 
-# using variables
+# evaluation with variables
 evaluator = meth.Evaluator()
 evaluator.evaluate("x = 5")
 evaluator.evaluate("x") # 5
 ```
 
 # Todo
 
@@ -44,12 +51,13 @@
   - [x] Functions
 - [x] Interpreter
   - [x] Binary Operations
   - [x] Unary Operations
   - [x] Variables
   - [x] Functions
 - [x] Add mathematical functions
+- [ ] Accurate float calculations
 - [ ] Simplify an expression
 - [ ] Expand an expression
 - [x] AST to Equation String
 - [ ] Documentation
-- [ ] Publish to PyPI
+- [x] Publish to PyPI
```

### Comparing `meth-1.0.1/pyproject.toml` & `meth-1.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "meth"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="sertdfyguhi" },
 ]
 description = "A mathematical expression parser and evaluator."
 readme = "README.md"
 requires-python = ">=3.2"
 classifiers = [
@@ -27,9 +27,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sertdfyguhi/meth"
 "Bug Tracker" = "https://github.com/sertdfyguhi/meth/issues"
 
 [tool.hatch.build.targets.wheel]
-packages = ["meth"]
-exclude = ["examples"]
+packages = ["meth"]
```

### Comparing `meth-1.0.1/PKG-INFO` & `meth-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meth
-Version: 1.0.1
+Version: 1.1.0
 Summary: A mathematical expression parser and evaluator.
 Project-URL: Homepage, https://github.com/sertdfyguhi/meth
 Project-URL: Bug Tracker, https://github.com/sertdfyguhi/meth/issues
 Author: sertdfyguhi
 License-File: LICENSE
 Keywords: evaluator,math,math evaluator,math parser,mathematical,parser,parsing
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -35,18 +35,25 @@
 # Examples
 
 > _More examples in the [examples/](https://github.com/sertdfyguhi/meth/tree/master/examples) directory._
 
 ```py
 import meth
 
+# tokenizing equations
+meth.tokenize("5 + 2") # INT(5), PLUS, INT(2)
+
+# parsing equations
+meth.parse("2 * 10") # BinaryOpNode(INT(2), MUL, INT(10))
+
+# evaluating equations
 meth.evaluate("2 + 2") # 4
 meth.evaluate("sqrt(9)") # 3
 
-# using variables
+# evaluation with variables
 evaluator = meth.Evaluator()
 evaluator.evaluate("x = 5")
 evaluator.evaluate("x") # 5
 ```
 
 # Todo
 
@@ -59,12 +66,13 @@
   - [x] Functions
 - [x] Interpreter
   - [x] Binary Operations
   - [x] Unary Operations
   - [x] Variables
   - [x] Functions
 - [x] Add mathematical functions
+- [ ] Accurate float calculations
 - [ ] Simplify an expression
 - [ ] Expand an expression
 - [x] AST to Equation String
 - [ ] Documentation
-- [ ] Publish to PyPI
+- [x] Publish to PyPI
```

