# Comparing `tmp/mathpad-1.2.0.tar.gz` & `tmp/mathpad-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathpad-1.2.0.tar", max compression
+gzip compressed data, was "mathpad-2.0.0.tar", max compression
```

## Comparing `mathpad-1.2.0.tar` & `mathpad-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,38 @@
--rw-r--r--   0        0        0     1095 2022-10-26 00:57:03.396863 mathpad-1.2.0/LICENSE
--rw-r--r--   0        0        0     4433 2022-10-26 00:57:03.396863 mathpad-1.2.0/README.md
--rw-r--r--   0        0        0     1291 2022-10-26 00:57:05.436860 mathpad-1.2.0/mathpad/__init__.py
--rw-r--r--   0        0        0     2304 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/_generate_units.py
--rw-r--r--   0        0        0     2753 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/_quality_of_life.py
--rw-r--r--   0        0        0     3970 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/algebra.py
--rw-r--r--   0        0        0     3068 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/calculus.py
--rw-r--r--   0        0        0     1436 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/codegen.py
--rw-r--r--   0        0        0      945 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/constants.py
--rw-r--r--   0        0        0     6347 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/dimensions.py
--rw-r--r--   0        0        0     1798 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/elec.py
--rw-r--r--   0        0        0     4135 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/equation.py
--rw-r--r--   0        0        0      965 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/functions.py
--rw-r--r--   0        0        0      435 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/global_options.py
--rw-r--r--   0        0        0     9095 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/matrix.py
--rw-r--r--   0        0        0     1867 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/mech.py
--rw-r--r--   0        0        0     9767 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/simulate_dynamic_system.py
--rw-r--r--   0        0        0     3372 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/solve.py
--rw-r--r--   0        0        0     1068 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/trigonometry.py
--rw-r--r--   0        0        0    11557 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/units.py
--rw-r--r--   0        0        0    17837 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/val.py
--rw-r--r--   0        0        0    11969 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/vector.py
--rw-r--r--   0        0        0     9131 2022-10-26 00:57:04.088862 mathpad-1.2.0/mathpad/vector_space.py
--rw-r--r--   0        0        0     1700 2022-10-26 00:57:05.452860 mathpad-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5346 1970-01-01 00:00:00.000000 mathpad-1.2.0/setup.py
--rw-r--r--   0        0        0     5778 1970-01-01 00:00:00.000000 mathpad-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-07-02 06:04:04.822873 mathpad-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6921 2023-07-02 06:04:04.822873 mathpad-2.0.0/README.md
+-rw-r--r--   0        0        0      825 2023-07-02 06:04:06.246876 mathpad-2.0.0/mathpad/__init__.py
+-rw-r--r--   0        0        0      435 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/_global_options.py
+-rw-r--r--   0        0        0     2045 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/codegen.py
+-rw-r--r--   0        0        0      449 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/__init__.py
+-rw-r--r--   0        0        0     2424 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/_generate_units_py.py
+-rw-r--r--   0        0        0      786 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/common_vals.py
+-rw-r--r--   0        0        0     6352 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/dimensions.py
+-rw-r--r--   0        0        0     5489 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/equation.py
+-rw-r--r--   0        0        0     8318 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/frame.py
+-rw-r--r--   0        0        0    12173 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/matrix.py
+-rw-r--r--   0        0        0    11562 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/units.py
+-rw-r--r--   0        0        0    18813 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/val.py
+-rw-r--r--   0        0        0    13290 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/vector.py
+-rw-r--r--   0        0        0     7775 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/core/vector_space.py
+-rw-r--r--   0        0        0      950 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/library/constants.py
+-rw-r--r--   0        0        0     1913 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/library/electrical.py
+-rw-r--r--   0        0        0     2282 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/library/mathpad_constructor.py
+-rw-r--r--   0        0        0     1878 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/library/mechanic.py
+-rw-r--r--   0        0        0      730 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/library/trigonometry.py
+-rw-r--r--   0        0        0      266 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/math/__init__.py
+-rw-r--r--   0        0        0     3930 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/math/algebra.py
+-rw-r--r--   0        0        0     3411 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/math/calculus.py
+-rw-r--r--   0        0        0     1229 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/math/functions.py
+-rw-r--r--   0        0        0     3409 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/math/solve.py
+-rw-r--r--   0        0        0      414 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/math/trigonometry.py
+-rw-r--r--   0        0        0     9641 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/simulate_dynamic_system.py
+-rw-r--r--   0        0        0    12032 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/sympy_extensions/SymbolicMatrixFunction.py
+-rw-r--r--   0        0        0      284 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/sympy_extensions/__init__.py
+-rw-r--r--   0        0        0      267 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/sympy_extensions/monkeypatch.py
+-rw-r--r--   0        0        0     1756 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/sympy_extensions/monkeypatch_ArrayDerivative___len__and__iter__.py
+-rw-r--r--   0        0        0      924 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/sympy_extensions/monkeypatch_MatrixOperations_subs.py
+-rw-r--r--   0        0        0     1522 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/sympy_extensions/monkeypatch_VectorLatexPrinter_print_Derivative.py
+-rw-r--r--   0        0        0        0 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/viz/viz2d.py
+-rw-r--r--   0        0        0     4901 2023-07-02 06:04:04.902874 mathpad-2.0.0/mathpad/viz/viz3d.py
+-rw-r--r--   0        0        0     1617 2023-07-02 06:04:06.266876 mathpad-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8274 1970-01-01 00:00:00.000000 mathpad-2.0.0/PKG-INFO
```

### Comparing `mathpad-1.2.0/LICENSE` & `mathpad-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathpad-1.2.0/mathpad/__init__.py` & `mathpad-2.0.0/mathpad/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,35 +5,25 @@
     micropip.install(['sympy', 'typing_extensions', 'plotly', 'scipy', 'tqdm'])
 except ImportError:
     # if micropip isn't available, we're not running in pyodide.
     pass
 
 import sympy
 
-from mathpad.val import *
-from mathpad.dimensions import *
-from mathpad.units import *
-
-from mathpad.solve import solve, Solution
-from mathpad.equation import Equation
-from mathpad._quality_of_life import t, pi, i, e, dimensionless, mathpad_constructor
-from mathpad.algebra import subs, simplify, factor, expand
-
-from mathpad.functions import piecewise, sqrt
-from mathpad.calculus import diff, integral
-from mathpad.trigonometry import cos, sin, tan
-from mathpad.vector_space import VectorSpace, R2, R3
-from mathpad.vector import Vector
-from mathpad.matrix import Matrix
+from mathpad.core import *
+from mathpad.math import *
+
+from mathpad.library.mathpad_constructor import mathpad_constructor
 from mathpad.simulate_dynamic_system import simulate_dynamic_system
-from mathpad.codegen import as_numpy_func
+
+import mathpad.codegen
 
 try:
     from IPython.display import display
 except ImportError:
     pass
 
 
 sympy.init_printing()  # type: ignore
 sympy.printing.printer.Printer.set_global_settings(min=-3, max=4)  # type: ignore
 
-__version__ = "1.2.0"
+__version__ = "2.0.0"
```

### Comparing `mathpad-1.2.0/mathpad/_generate_units.py` & `mathpad-2.0.0/mathpad/core/_generate_units_py.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+
+"Only run this script if you want to regenerate the 'units.py' and 'constants.py' files."
+
 import os
 
 import sympy.physics.units.definitions as u
 from sympy.physics.units.quantities import Quantity
 from sympy.physics.units.systems.si import dimsys_SI
 
-from mathpad.val import Val
-import mathpad.dimensions as dims
+from mathpad.core.val import Val
+import mathpad.core.dimensions as dims
 
 HERE = os.path.dirname(__file__)
 
 AUTOGEN_WARNING = '"WARNING: this file was automatically generated by commented code within mathpad.py, and then modified slightly"\n'
 
 print("writing to " + f"{HERE}/units.py\nand {HERE}/constants.py")
 
@@ -52,15 +55,15 @@
                     )
                     break
 
                 elif (
                     isinstance(quantity_cls, type)
                     and issubclass(quantity_cls, Val)
                     and quantity_cls is not Val
-                    and dimsys_SI.equivalent_dims(qty.dimension, quantity_cls.dimension)
+                    and dimsys_SI.equivalent_dims(qty.dimension, quantity_cls.dimension) # type: ignore
                 ):
                     units_f.write(
                         f"""
 {name} = {quantity_cls_name}(u.{name})"""
                     )
                     break
             else:
```

### Comparing `mathpad-1.2.0/mathpad/algebra.py` & `mathpad-2.0.0/mathpad/math/algebra.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 from typing import ItemsView, KeysView, TypeVar, Union, ValuesView, overload
 from typing_extensions import Protocol
 
 import sympy
 
-from mathpad.val import Q, ValT, Val
-from mathpad.vector import Vector, VecT
-from mathpad.equation import Equation
+from mathpad.core import Q, ValT, Val, Vector, VecT, Equation, EquationT
 
 
 @overload
 def simplify(obj: ValT) -> ValT:
     ...
 
 @overload
-def simplify(obj: Equation) -> Equation:
+def simplify(obj: EquationT) -> EquationT:
     ...
 
 @overload
 def simplify(obj: VecT) -> VecT:
     ...
 
-def simplify(obj: Union[ValT, Equation, VecT]) -> Union[ValT, Equation, VecT]:
+def simplify(obj: Union[ValT, EquationT, VecT]) -> Union[ValT, EquationT, VecT]:
     if isinstance(obj, Equation):
         # TODO: simplification that actually makes use of equality
 
         return Equation(
             simplify(obj.lhs),
             simplify(obj.rhs)
         )
     
     elif isinstance(obj, Vector):
         return obj.__class__(
-            obj.space,
+            obj.frame,
             sympy.simplify(obj.expr) # type: ignore
         )
 
     else:
         return obj.__class__(
             obj.units,
             sympy.simplify(obj.expr)
@@ -66,15 +64,15 @@
             factor(obj.lhs),
             factor(obj.rhs)
         )
     
     elif isinstance(obj, Vector):
             
         return obj.__class__(
-            obj.space,
+            obj.frame,
             sympy.factor(obj.expr)
         )
 
     else:
         return obj.__class__(
             obj.units,
             sympy.factor(obj.expr) # type: ignore
@@ -101,15 +99,15 @@
 ) -> Union[ValT, Equation, VecT]:
     if isinstance(obj, Equation):
         # TODO: simplification that actually makes use of equality
         return Equation(expand(obj.lhs), expand(obj.rhs))
 
     elif isinstance(obj, Vector):
         return obj.__class__(
-            obj.space,
+            obj.frame,
             sympy.expand(obj.expr)
         )
 
     else:
         return obj.__class__(
             obj.units,
             sympy.expand(obj.expr)
@@ -157,10 +155,10 @@
         for from_, to in substitutions.items():
             if not isinstance(to, (Val, Vector)):
                 to = from_.__class__(from_.units, to)
 
             sympy_subsmap[from_.expr] = to.in_units(from_ if isinstance(from_, Val) else from_.space).expr
 
         return obj.__class__(
-            obj.units if isinstance(obj, Val) else obj.space,
+            obj.units if isinstance(obj, Val) else obj.frame,
             obj.expr.subs(sympy_subsmap) # type: ignore
         )
```

### Comparing `mathpad-1.2.0/mathpad/constants.py` & `mathpad-2.0.0/mathpad/library/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 "WARNING: this file was automatically generated by commented code within mathpad.py, and then modified slightly"
 import sympy.physics.units.definitions.unit_definitions as u
-from mathpad.val import Val
+from mathpad.core.val import Val
 
 atomic_mass_constant = Val(u.atomic_mass_constant, 1)
 avogadro_constant = Val(u.avogadro_constant, 1)
 boltzmann_constant = Val(u.boltzmann_constant, 1)
 coulomb_constant = Val(u.coulomb_constant, 1)
 coulombs_constant = Val(u.coulombs_constant, 1)
 electric_constant = Val(u.electric_constant, 1)
```

### Comparing `mathpad-1.2.0/mathpad/dimensions.py` & `mathpad-2.0.0/mathpad/core/dimensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sympy.physics.units.definitions as u
 import sympy.physics.units.definitions.dimension_definitions as d
 
-from mathpad.val import Unit, Dimensionless
+from mathpad.core.val import Unit, Dimensionless
 
 # TODO: rearrange in alphabetical order
 
 __all__ = [
     "Dimensionless",
     "Length",
     "Time",
```

### Comparing `mathpad-1.2.0/mathpad/elec.py` & `mathpad-2.0.0/mathpad/library/electrical.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 from typing import List
-from mathpad import *
+from mathpad.core import *
+from .mathpad_constructor import mathpad_constructor
 
 @mathpad_constructor
 def resistance_resistivity(
     *,
-    R: X[Impedance],  # resistance
-    rho: X[Resistivity],  # resisitivity
-    l: X[Length],  # length of strip
-    A: X[Area]  # cross-sectional area of strip (usually very flat, but wide(ish))
-) -> Equation:
-    "Relate resistance and resistivity"
+    R: Q[Impedance],  # resistance
+    rho: Q[Resistivity],  # resisitivity
+    l: Q[Length],  # length of strip
+    A: Q[Area]  # cross-sectional area of strip (usually very flat, but wide(ish))
+) -> Equation[Resistivity]:
+    "Resistance and resistivity of a strip of material"
     return R == rho * l * A
 
 
 @mathpad_constructor
 def ohms_law(
     *,
-    R: X[Impedance],  # resistance
-    V: X[Voltage],  # voltage
-    I: X[Current]  # current
-) -> Equation:
+    R: Q[Impedance],  # resistance
+    V: Q[Voltage],  # voltage
+    I: Q[Current]  # current
+) -> Equation[Voltage]:
     """
     Ohm's law:
     
     V == I * R
     """
     return V == I * R
 
-# TODO: support List[X[Voltage]] in @mathpad_constructor
+# TODO: support List[Q[Voltage]] in @mathpad_constructor
 # @mathpad_constructor
 def kerchoffs_voltage_law(
     *,
-    producers: List[X[Voltage]],  # voltage sources
-    consumers: List[X[Voltage]],  # voltage drops
-) -> Equation:
+    producers: List[Q[Voltage]],  # voltage sources
+    consumers: List[Q[Voltage]],  # voltage drops
+) -> Equation[Voltage]:
     """
     Kirchoff's voltage law. 
 
     The sum of voltage sources is equal to the sum of voltage drops.
     
     sum(producers) == sum(consumers)
 
     """
 
     assert producers or consumers, "At least one voltage must be specified"
 
     return sum(producers) == sum(consumers) # type: ignore - assert should prevent both being 0 length lists
 
 
-# TODO: support List[X[Voltage]] in @mathpad_constructor
+# TODO: support List[Q[Voltage]] in @mathpad_constructor
 # @mathpad_constructor
 def kerchoffs_current_law(
     *,
-    into: List[X[Current]],  # current into node
-    out: List[X[Current]],  # current
-) -> Equation:
+    into: List[Q[Current]],  # current into node
+    out: List[Q[Current]],  # current
+) -> Equation[Current]:
     """
     Kirchoff's current law. 
 
     The sum of currents into a node is equal to the sum of currents out of the node.
     
     sum(into) == sum(out)
```

### Comparing `mathpad-1.2.0/mathpad/equation.py` & `mathpad-2.0.0/mathpad/core/equation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,104 @@
-from typing import TYPE_CHECKING, Type, Union, overload
+from typing import Type, Union, overload, Generic, TypeVar, Tuple, Any
 
 import sympy
+import sympy.physics.units as su
 from sympy import MatrixSymbol, MatrixExpr
 from sympy.physics.vector.printing import vlatex
 
-if TYPE_CHECKING:
-    from mathpad.val import ValT, Q
-    from mathpad.vector import VecT
+from mathpad.core.val import Val, Q
+from mathpad.core.vector import Vector
+from mathpad.core.vector_space import VectorSpace
+from mathpad.core.matrix import Matrix
+from mathpad.core.frame import Frame
 
 
-class Equation:
+
+T = TypeVar("T", bound=Union[Val, VectorSpace, Matrix])
+
+
+class Equation(Generic[T]):
 
     @overload
     def __init__(
         self,
-        lhs: "Q[ValT]",
-        rhs: "Q[ValT]",
+        lhs: "Q[T]",
+        rhs: "Q[T]",
     ):
         ...
     
     @overload
     def __init__(
         self,
-        lhs: "VecT",
-        rhs: "VecT",
+        lhs: "Vector[T]",
+        rhs: "Vector[T]",
+    ):
+        ...
+        
+    @overload
+    def __init__(
+        self,
+        lhs: "T",
+        rhs: "T",
     ):
         ...
 
     def __init__(
         self,
-        lhs: Union["Q[ValT]", "VecT"],
-        rhs: Union["Q[ValT]", "VecT"]
+        lhs: Union["Q[T]", "Vector[T]", "T"],
+        rhs: Union["Q[T]", "Vector[T]", "T"]
     ):
-        from mathpad import Val, Vector
+        from mathpad.core import Val, Vector
         
         lhs_is_val = isinstance(lhs, Val)
         rhs_is_val = isinstance(rhs, Val)
 
+        self.units: Union[su.Quantity, Frame[T], Tuple[Frame[Any], Frame[Any]]] = None
+
         if lhs_is_val or rhs_is_val:
             # one of them is a Val. The other is either a Val or a Num
             
             if lhs_is_val and rhs_is_val:
                 # both are Val. handle unit conversion and rescaling if necessary.
 
                 # convert rhs into units of lhs, scaling rhs' val if necessary
                 rhs = rhs.in_units(lhs)
 
             val_cls: Type[Val] = (lhs if lhs_is_val else rhs).__class__ # type: ignore
             self.units = lhs.units if lhs_is_val else rhs.units # type: ignore
             self.lhs = lhs if lhs_is_val else val_cls(self.units, lhs) # type: ignore
             self.rhs = rhs if rhs_is_val else val_cls(self.units, rhs) # type: ignore
 
-        else:
+        elif isinstance(lhs, Vector) or isinstance(rhs, Vector):
             # both are Vector. handle unit conversion and rescaling if necessary.
             assert isinstance(lhs, Vector) and isinstance(rhs, Vector)
+
+            assert lhs.frame == rhs.frame, f"Vectors must be in the same frame to be equated. {lhs.frame} != {rhs.frame}"
             
             # convert rhs into units of lhs, scaling rhs' val if necessary
-            self.units = lhs.space
+            self.units = lhs.frame
             self.lhs = lhs
-            self.rhs: Union[VecT, ValT] = rhs.in_units(lhs.space)
+            self.rhs = rhs.in_units(lhs.frame.space.base_units) # type: ignore
+        
+        else: # matrix equation
+            # don't do automatic rescaling for matrixes.
+            # shouldn't be necessary most of the time and the user can do it easily if they want.
+            assert isinstance(lhs, Matrix) and isinstance(rhs, Matrix)
+            assert lhs.left_frame == rhs.left_frame
+            assert lhs.right_frame == rhs.right_frame
+            self.lhs = lhs
+            self.rhs = rhs
+            self.units = (lhs.left_frame, lhs.right_frame)
     
     def __getitem__(self, idx: int):
         """
         Get an equation for a single component of a vector equation.
         If the equation is not a vector equation, this will raise an error.
         """
-        from mathpad import VectorSpace
+        from mathpad.core import VectorSpace
 
         assert isinstance(self.units, VectorSpace), "Can only get a component of a vector equation"
         
         return Equation(self.lhs[idx], self.rhs[idx]) # type: ignore
 
     def __repr__(self):
         return f"{self.lhs._repr(False)} = {self.rhs._repr(False)} {self.units}"
@@ -78,21 +107,25 @@
         return sympy.Equality(self.lhs.expr, self.rhs.expr)  # type: ignore
 
     # def as_units_eq_without_unknowns(self, unknowns: Collection[Val]):
     #     return sympy.Equality(self.lhs.units, self.rhs.units)
 
     # Rich displays; Ipython etc
     def _repr_latex_(self):
-        from mathpad import VectorSpace
+        from mathpad.core.frame import Frame
 
         # use vlatex because it applies dot notation where possible
-        lhs_ltx = (vlatex(self.lhs.expr)).replace("- 1.0 ", "-")
-        rhs_ltx = (vlatex(self.rhs.expr)).replace("- 1.0 ", "-")
+        lhs_ltx = vlatex(self.lhs.expr) \
+            .replace("- 1.0 ", "-") \
+            .replace("\\text{\\textbackslashvec", "\\vec")
+        rhs_ltx = vlatex(self.rhs.expr) \
+            .replace("- 1.0 ", "-") \
+            .replace("\\textbackslashvec", "\\vec")
 
-        units_ltx = self.units._repr_latex_(wrapped=False) if isinstance(self.units, VectorSpace) \
+        units_ltx = self.units._repr_latex_(wrapped=False) if isinstance(self.units, Frame) \
             else "dimensionless" if self.units == 1 \
             else vlatex(self.units)
 
         spacer_ltx = "\\hspace{1.25em}"
 
         return f"$$ {lhs_ltx} = {rhs_ltx} {spacer_ltx} {units_ltx} $$"
 
@@ -106,8 +139,10 @@
         # this appears to be because there is no link between a as a matrix symbol and a[0] as a matrix element
         lhs = self.lhs.expr.as_explicit() if isinstance(self.lhs.expr, (MatrixSymbol, MatrixExpr)) else self.lhs.expr
         rhs = self.rhs.expr.as_explicit() if isinstance(self.rhs.expr, (MatrixSymbol, MatrixExpr)) else self.rhs.expr
     
         # TODO: check if this will affect solve() in any way
         # TODO: what happens if the equation cannot be evaluated?
         res = lhs.doit() == rhs.doit()
-        return res
+        return res
+
+EquationT = TypeVar("EquationT", bound=Equation)
```

### Comparing `mathpad-1.2.0/mathpad/functions.py` & `mathpad-2.0.0/mathpad/math/functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List, Optional, Tuple, overload
-from sympy import Piecewise
+import sympy
 
-from mathpad.val import Dimensionless, Num, Val, ValT, Q
+from mathpad.core.val import Dimensionless, Num, Val, ValT, Q
+from mathpad.core.common_vals import e
 
 # TODO: improve API once ">", "<", ">=" etc operators are implemented for Val
 def piecewise(x: Val, region_vals: List[Tuple[float, Q[ValT]]]) -> ValT:
     "a piecewise series of <"
     assert any(region_vals)
     assert region_vals[-1][0] == float("inf")
     inp = []
@@ -15,21 +16,27 @@
         inp.append((rescaled.expr, x.expr < lt))
         prev_val = val
     
     assert prev_val
 
     return prev_val.__class__(
         prev_val.units,
-        Piecewise(*inp)
+        sympy.Piecewise(*inp)
     )
 
 @overload
 def sqrt(x: Num) -> Num:
     ...
 
 @overload
 def sqrt(x: Val) -> Val:
     ...
 
 def sqrt(x: Q[Val]) -> Q[Val]:
     from sympy import sqrt as _sqrt
-    return Val(x.units**0.5, _sqrt(x.expr))
+    return Val(x.units**0.5, _sqrt(x.expr if isinstance(x, Val) else x))
+
+def log(x: Q[Val], base: Q[Val] = e) -> Q[Val]:
+    return Dimensionless(1, sympy.log(
+        x.expr if isinstance(x, Val) else x,
+        base.expr if isinstance(base, Val) else base
+    ))
```

### Comparing `mathpad-1.2.0/mathpad/mech.py` & `mathpad-2.0.0/mathpad/library/mechanic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-from typing import Type, cast
 from mathpad import *
+from .mathpad_constructor import mathpad_constructor
         
 
 @mathpad_constructor
-def kinetic_energy(*, m: X[Mass], v: X[Velocity]) -> Energy:
+def kinetic_energy(*, m: Q[Mass], v: Q[Velocity]) -> Energy:
     """
     Calculate the kinetic energy of a particle.
 
     Args:
         m: Mass of the particle
         v: Velocity of the particle
     
     Returns:
         Kinetic energy of the particle in joules
 
     Example:
-        >>> kinetic_energy(m=1 * kg, v=2 * m/s)
-        2 joules
         >>> kinetic_energy(m="m" * kg, v="v" * m/s)
         0.5*mv**2 joules
+        >>> kinetic_energy(m=1 * kg, v=2 * m/s)
+        2 joules
 
     """
     return (m * v ** 2 / 2).in_units(joules)  # type: ignore
 
 
 @mathpad_constructor
-def elastic_energy(*, k: X[Elasticity], dx: X[Length]) -> Energy:
+def elastic_energy(*, k: Q[Elasticity], dx: Q[Length]) -> Energy:
     return k * dx ** 2 / 2  # type: ignore
 
 
 @mathpad_constructor
-def gravitational_energy(*, m: X[Mass], h: X[Length], g: X[Acceleration]) -> Energy:
+def gravitational_energy(*, m: Q[Mass], h: Q[Length], g: Q[Acceleration]) -> Energy:
     return m * g * h  # type: ignore
 
 
 @mathpad_constructor
 def euler_lagrange(
     *,
-    KE: X[Energy],
-    PE: X[Energy],
-    NCF: X[Force],
+    KE: Q[Energy],
+    PE: Q[Energy],
+    NCF: Q[Force],
     var: Val,
-) -> Equation:
+) -> Equation[Force]:
     """
     Euler-Lagrange equation for a system of particles.
 
     Arguments:
-        sum_KE: sum of kinetic energies of particles
-        sum_PE: sum of potential energies of particles
-        sum_NCF: sum of net contact forces on particles
+        KE: sum of kinetic energies of particles
+        PE: sum of potential energies of particles
+        NCF: sum of net contact forces on particles
         var: variable you are interested in finding the dynamics for
-    
     """
     L = KE - PE
     return diff(diff(L, wrt=diff(var)), wrt=t) - diff(L, wrt=var) == NCF # type: ignore
 
 
 @mathpad_constructor
 def impulse_momentum(
     *,
-    m: X[Mass],  # mass
-    v1: X[Velocity],  # initial velocity
-    F: X[Force],  # impulse force required
-    t: X[Time],  # impulse duration in seconds
-    v2: X[Velocity],  # final velocity
-) -> Equation:
+    m: Q[Mass],  # mass
+    v1: Q[Velocity],  # initial velocity
+    F: Q[Force],  # impulse force required
+    t: Q[Time],  # impulse duration
+    v2: Q[Velocity],  # final velocity
+) -> Equation[Momentum]:
     "The force required during an instant to change an object's velocity"
     return m * v1 + integral(F, wrt=t) == m * v2
```

### Comparing `mathpad-1.2.0/mathpad/simulate_dynamic_system.py` & `mathpad-2.0.0/mathpad/simulate_dynamic_system.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,19 @@
 from sympy import Derivative
 import plotly.graph_objects as go
 from sympy.utilities.lambdify import lambdify
 from scipy.integrate import RK45
 from IPython.display import display
 import plotly.io as pio
 
-from mathpad.val import Val
-from mathpad.equation import Equation
-from mathpad.algebra import subs, SubstitutionMap, simplify
-from mathpad._quality_of_life import t
-try:
-    from tqdm.notebook import tqdm
-except ImportError:
-    from tqdm import tqdm
+from mathpad.core.val import Val
+from mathpad.core.equation import Equation
+from mathpad.math.algebra import subs, SubstitutionMap, simplify
+from mathpad.core.common_vals import t
+from tqdm import tqdm
 
 
 def simulate_dynamic_system(
     dynamics_equations: Collection[Equation],
     *,
     x_final: float,
     initial_conditions: SubstitutionMap,
@@ -31,36 +28,36 @@
     substitute: SubstitutionMap = {},
     x_axis: Val = t,
     all_solutions: bool = False,
     # output display options
     verbose: bool = True,
     display_plots: bool = True,
     display_progress_bar: bool = True,
-    display_explanation: bool = False,
+    explain: bool = False,
     # plot formatting (display_plots=True)
     plot_static: bool = False,
     plot_static_figsize: Tuple[int, int] = (960, 400),
     plot_title: str = "Solution #{solutionNo}",
     _NEW_SOLVE: bool = False # TODO: fix this properly
 ) -> List[Tuple[float, List[float]]]:
     "simulates a differential system specified by dynamics_equations from initial conditions at x_axis=0 (typically t=0) to x_final"
 
-    verbose = verbose or display_explanation
+    verbose = verbose or explain
 
     if plot_static:
         # make static renderings a certain size, the default one is too square for my liking
         svg_renderer = pio.renderers["svg"]
         width, height = plot_static_figsize
         svg_renderer.width = width
         svg_renderer.height = height
 
     # TODO: support plotting on separate axes, and subplots
     # TODO: ensure we aren't subbing out something that is required for a 'record' output
 
-    if display_explanation:
+    if explain:
         print("Using Input Equations:")
         for eqn in dynamics_equations:
             display(eqn)
         
         if substitute:
             print("Subbing in Values:")
             for replace, _with in substitute.items():
@@ -107,17 +104,17 @@
         if not lvl == lowest_derivatives[fn]
     ]
 
     solve_for_recorded_data = [val.expr for val in record]
 
     solve_for = solve_for_highest_derivatives + solve_for_recorded_data
 
-    _print_if(verbose, f"Solving subbed Equations{':' if display_explanation else '...'}")
+    _print_if(verbose, f"Solving subbed Equations{':' if explain else '...'}")
 
-    if display_explanation:
+    if explain:
         for eqn in problem_eqns:
             display(eqn)
 
         print("For values:")
         display(solve_for)
 
     solutions = sympy.solve(
@@ -138,15 +135,15 @@
         for val in solve_for:
             if val not in solution:
                 solution[val] = val
 
         # convert it to a vector for lambdify below
         solution_vec = [solution[val] for val in solve_for]
 
-        if display_explanation:
+        if explain:
             print(
                 "Found Solution" + (f"#{solution_idx + 1}:" if all_solutions else ":")
             )
             for solve_val, result in zip(solve_for, solution_vec):
                 eqn = sympy.Eq(solve_val, result)
                 if eqn != True:  # this happens with passthrough variables
                     display(eqn)
@@ -186,15 +183,15 @@
             deriv
             for derivatives in zip_longest(*input_unzipped)
             for deriv in derivatives
             if deriv is not None
         ]
 
         # outputs are highest of input derviatives plus recorded data
-        # ie [dddx, record[0], record[1]]
+        # ie [ddx, ddy, record[0], record[1]]
         lambdified = lambdify([x_axis.expr, inputs], solution_vec, 'numpy')
 
         data = []
 
         # define this integration function to record data and let outputs = diff(inputs)
         def step(x: float, state: np.ndarray):
 
@@ -233,18 +230,18 @@
             y0.append(val)
 
         integrator = RK45(step, t0=0, y0=y0, t_bound=x_final, max_step=max_step)
 
         _print_if(
             verbose,
             f"Simulating from t=0 to t={x_final} with a max_step of {max_step}"
-            + (" with initial conditions:" if display_explanation else "."),
+            + (" with initial conditions:" if explain else "."),
         )
 
-        if display_explanation:
+        if explain:
             for replace, _with in initial_conditions.items():
                 display(replace == _with)
 
         t_prev = 0
 
         pbar = tqdm(total=x_final, leave=False) if display_progress_bar else None
 
@@ -281,15 +278,15 @@
                         "text": plot_title.format(solutionNo=solution_idx + 1),
                         "y": 0.9,
                         "x": 0.5,
                         "xanchor": "center",
                         "yanchor": "top",
                     },
                 },
-            ).show("svg" if plot_static else None)
+            ).show("svg" if plot_static else None) # type: ignore
 
         all_data.extend(data)
 
         if not all_solutions:
             break
 
     return all_data
```

### Comparing `mathpad-1.2.0/mathpad/solve.py` & `mathpad-2.0.0/mathpad/math/solve.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import TYPE_CHECKING, Collection, Dict, List, Union, overload
 import sympy
 
-from mathpad.val import Val, ValT
-from mathpad.equation import Equation
+from mathpad.core.val import Val, ValT
+from mathpad.core.equation import Equation
 if TYPE_CHECKING:
-    from mathpad.vector import Vector, VecT
+    from mathpad.core.vector import Vector, VecT
 
 
 class Solution:
     def __init__(self, result_dict: Dict[Union[Val, 'Vector'], Union[Val, 'Vector']]):
         self.result_dict = result_dict
 
     @overload
@@ -17,20 +17,20 @@
     
     @overload
     def __getitem__(self, key: 'VecT') -> 'VecT':
         ...
 
     
     def __getitem__(self, k: Union[ValT, 'VecT']) -> Union[ValT, 'VecT']: # type: ignore
-        from mathpad import Vector
+        from mathpad.core import Vector
         result = self.result_dict[k]
         if isinstance(result, Val):
             assert result.units == k.units
         elif isinstance(result, Vector):
-            assert result.space == k.space # type: ignore
+            assert result.frame.space == k.frame.space # type: ignore
         return result # type: ignore
 
     def __repr__(self):
         return self._repr("", " ")
 
     def _repr(self, newline: str, indent: str):
         # TODO: print latex
@@ -46,15 +46,15 @@
         return self.result_dict.items()
 
 def solve(
     equations: Collection[Equation],
     solve_for: Collection[Union[Val, 'Vector']]
     # domain: Literal["complex", "real", "integers", "naturals", "naturals0"] = "real",
 ) -> List[Solution]:
-    from mathpad import Vector
+    from mathpad.core import Vector
     
     solve_for_vectors_split: List[Val] = []
     for x in solve_for:
         if isinstance(x, Vector):
             solve_for_vectors_split += list(x)
         else:
             solve_for_vectors_split.append(x)
```

### Comparing `mathpad-1.2.0/mathpad/trigonometry.py` & `mathpad-2.0.0/mathpad/library/trigonometry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,22 @@
-from re import L
-import sympy
-from mathpad import *
-
-
-def sin(x: Q[Angle]) -> Dimensionless:
-    return Dimensionless(1, sympy.sin(x.expr))  # type: ignore
-
-
-def cos(x: Q[Angle]) -> Dimensionless:
-    return Dimensionless(1, sympy.cos(x.expr))  # type: ignore
-
-
-def tan(x: Q[Angle]) -> Dimensionless:
-    return Dimensionless(1, sympy.tan(x.expr))  # type: ignore
-
-# TODO: add more trig functions
-
-
-def sine_rule(
-    a: Q[Length],  # length of side a
-    b: Q[Length],  # length of side b
-    alpha: Q[Angle],  # internal angle opposite to side a
-    beta: Q[Angle],  # internal angle opposite to side b
-) -> Equation:
-    "Relates lengths of two sides of any triangle the internal angle opposite"
-    return a == b * sin(alpha) / sin(beta) # type: ignore
-
-
-def cosine_rule(
-    a: Q[Length],  # length of side a
-    b: Q[Length],  # length of side b
-    c: Q[Length],  # length of side c
-    C: Q[Angle],  # internal angle opposite to side c
-) -> Equation:
-    return c ** 2 == a ** 2 + b ** 2 - 2 * a * b * cos(C) # type: ignore
+
+from mathpad.core import *
+from .mathpad_constructor import mathpad_constructor
+
+
+def sine_rule(
+    a: Q[Length],  # length of side a
+    b: Q[Length],  # length of side b
+    alpha: Q[Angle],  # internal angle opposite to side a
+    beta: Q[Angle],  # internal angle opposite to side b
+) -> Equation[Length]:
+    "Relates lengths of two sides of any triangle the internal angle opposite"
+    return a == b * sin(alpha) / sin(beta) # type: ignore
+
+
+def cosine_rule(
+    a: Q[Length],  # length of side a
+    b: Q[Length],  # length of side b
+    c: Q[Length],  # length of side c
+    C: Q[Angle],  # internal angle opposite to side c
+) -> Equation[Area]:
+    return c ** 2 == a ** 2 + b ** 2 - 2 * a * b * cos(C) # type: ignore
```

### Comparing `mathpad-1.2.0/mathpad/units.py` & `mathpad-2.0.0/mathpad/core/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 "WARNING: this file was automatically generated by commented code within mathpad.py, and then modified slightly"
 import sympy.physics.units.definitions.unit_definitions as u
-from mathpad.dimensions import *
+from mathpad.core.dimensions import *
 
 __all__ = [
     "A", "Bq", "C", "D", "F", "G", "Gy", "H", "Hz", "J", "K", "N", "Pa", "R", "S", "T", "V", "W", "Wb", "Z0",
     "acceleration_due_to_gravity", "ampere", "amperes", "amu", "amus", "rad", "angular_mil", "angular_mils",
     "anomalistic_year", "anomalistic_years", "astronomical_unit", "astronomical_units", "atm", "atmosphere",
     "atmospheres", "atomic_mass_unit", "au", "avogadro_number", "bar", "bars", "becquerel", "bit", "bits", "byte",
     "c", "candela", "candelas", "cd", "centiliter", "centiliters", "centimeter", "centimeters", "cl", "cm",
```

### Comparing `mathpad-1.2.0/mathpad/val.py` & `mathpad-2.0.0/mathpad/core/val.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from types import FrameType
-from typing import TYPE_CHECKING, Any, Optional, Tuple, Union, TypeVar, overload, Callable
+from typing import TYPE_CHECKING, Any, Collection, Iterator, Optional, Tuple, Type, Union, TypeVar, overload, Callable
 import re
-from abc import ABC
 from typing_extensions import Self, Literal
 import inspect
 
 import sympy
 import sympy.physics.units as su
 from sympy.physics.units.dimensions import Dimension
 from sympy.physics.units.systems.si import dimsys_SI
 from sympy.physics.units.unitsystem import UnitSystem
 from sympy.physics.vector.printing import vlatex
 from sympy.physics.units.util import (
     quantity_simplify,
     convert_to,
 )
 
-from mathpad.equation import Equation
+if TYPE_CHECKING:
+    from mathpad.core.equation import Equation
+
 
 # TODO: support numpy arrays
 Num = Union[int, float, complex]
 
 # this should be a classmethod, but it isn't
 _units2dimensional_expr = UnitSystem.get_default_unit_system().get_dimensional_expr
 
@@ -28,15 +29,15 @@
 class Val:
     "An value with a set of units. For example 10 ohms or 20 meters / second**2"
 
 
     def __init__(
         self,
         units: Union[su.Quantity, sympy.Expr],  # may also be a sympy expression of su.Quantities, ie su.meter**2
-        val: Union[sympy.Expr, Num] = 1,
+        val: Union[sympy.Expr, sympy.Basic, Num] = 1,
     ):
     
         # clean up the case where you get units**1.0
         if isinstance(units, sympy.Pow) and units.exp == 1:
             units = units.base
 
         self.expr: sympy.Expr = sympy.sympify(val)
@@ -60,27 +61,29 @@
             # otherwise assign it to the dimensionality of the units provided
             self.dimension = units_dimension
 
     def __hash__(self):
         return hash(self.expr)
 
     @overload
-    def __eq__(self, other: "Val") -> "Equation":
+    def __eq__(self, other: "Val") -> "Equation[Self]":
         ...
 
     @overload
-    def __eq__(self, other: "Q[Self]") -> "Equation":
+    def __eq__(self, other: "Q[Self]") -> "Equation[Self]":
         ...
 
-    def __eq__(self, other: "Q[Val]") -> "Equation":
+    def __eq__(self, other: "Q[Val]") -> "Equation[Self]":
+        from mathpad.core.equation import Equation
         if isinstance(other, Val):
             SumDimensionsMismatchError.check(self, "==", other)
         return Equation(self, other)
 
-    def __req__(self, other: Num) -> "Equation":
+    def __req__(self, other: Num) -> "Equation[Self]":
+        from mathpad.core.equation import Equation
         return Equation(other, self)
 
     def __repr__(self) -> str:
         return self._repr(True)
 
     # Rich displays; Ipython etc
     def _repr_latex_(self, wrapped: bool = True):
@@ -102,15 +105,15 @@
                 # remove trailing zeros for whole numbers
                 whole, decimals = expr_str.split(".")
                 decimals = decimals.rstrip('0')
                 if not any(decimals):
                     expr_ltx = whole
                 else:
                     # TODO: global / context managed sigfig settings
-                    expr_ltx = f"{whole}.{decimals[:4]}{'..' if len(decimals) > 4 else ''}"
+                    expr_ltx = f"{whole}.{decimals[:4]}"
             else:
                 expr_ltx = expr_str
         else:
             expr_ltx = vlatex(self.expr)
         
         # remove '1.0's
         clean_expr_ltx = expr_ltx.replace("- 1.0 ", "-")
@@ -179,15 +182,15 @@
         units_factor, new_units = _split_coeff_and_units(
             convert_to(self.units, new_units)  # type: ignore
         )
         new_val = units_factor * self.expr
 
         return self.__class__(new_units, new_val)
 
-    def re(self, units: "Val") -> "Val":
+    def re(self, units: 'ValT') -> 'ValT':
         """
         Return a new value with the same value but replaced units.
 
         Useful for defining functions of other values with numeric literals in place of dimensionally-accurate Vals.
 
         For example,
         >>> acceleration = (6 * t).re(m/s**2)
@@ -211,46 +214,69 @@
         return self._sum_op(other, lambda a, b: b - a, "-", True)
 
     def __neg__(self):
         return self.__class__(self.units, -self.expr) # type: ignore
 
     def __mul__(self, other: "Q[Val]") -> "Val":
         return self._prod_op(other, lambda a, b: a * b, is_pow=False)
-
+    
+    def __call__(self, other: "Q[Val]") -> "Val":
+        return self * other
+    
+        
+    @overload
     def __rmul__(self, other: Union[Num, str]) -> Self:
+        ...
+    
+    @overload
+    def __rmul__(self, other: Tuple[str, ...]) -> Tuple[Self, ...]:
+        ...
 
-        if isinstance(other, str):
+    def __rmul__(self, other: Union[Num, str, Tuple[str, ...]]) -> Union[Self, Tuple[Self, ...]]:
+
+        if isinstance(other, tuple):
+            return tuple(
+                symbolName * self
+                for symbolName in other
+            )
+            
+
+        elif isinstance(other, str):
             assert self.expr == 1, "Attempted to create variable with a non-unit Val"
 
             # TODO: support variables which are functions of a symbol other than t. should this be a fn() fn?
             if "(" in other:
 
                 caller_frame = inspect.currentframe().f_back # type: ignore
                 assert caller_frame
-                sym = _sym_func(other, caller_frame)
+                
+                func_name, _depstr = other.split("(") # TODO: refactor similar implementation with VectorSpace.__rmatmul__
+                deps = _extract_deps_from_fn_str(other, caller_frame, allow_only=(sympy.Function, sympy.Symbol))
+
+                expr = sympy.Function(func_name)(*(d.expr for d in deps)) # type: ignore
 
             else:
-                sym = sympy.Symbol(other)
+                expr = sympy.Symbol(other)
 
-            return self.__class__(self.units, sym)
+            return self.__class__(self.units, expr) # type: ignore
 
         else:
             return self._prod_op(other, lambda a, b: b * a, is_pow=False)
 
 
     def __truediv__(self, other: "Q[Val]") -> "Val":
         return self._prod_op(other, lambda a, b: a / b, is_pow=False)
 
     def __rtruediv__(self, other: Num) -> "Val":
         return self._prod_op(other, lambda a, b: b / a, is_pow=False)
 
     def __pow__(self, other: "Q[Val]") -> "Val":
-        from mathpad.vector_space import VectorSpace
-        from mathpad.vector import Vector
-        from mathpad.matrix import Matrix
+        from mathpad.core.vector_space import VectorSpace
+        from mathpad.core.vector import Vector
+        from mathpad.core.matrix import Matrix
 
         # exponents should always be dimensionless
         if isinstance(other, Val) and not _is_dimensionless(other.dimension):
             raise DimensionalExponentError(
                 f"Exponents must always be dimensionless. Instead got {other.dimension}: {other}"
             )
         
@@ -287,15 +313,15 @@
     def _sum_op(
         self,
         other: "Q[Self]",
         op: Callable[[Any, Any], Any],
         op_str: str,
         reverse: bool,
     ) -> Self:
-        from mathpad.vector import Vector
+        from mathpad.core.vector import Vector
 
         assert not isinstance(other, Vector)
 
         other_units, other_val = (
             (other.units, other.expr) if isinstance(other, Val) else (self.units, other)
         )
 
@@ -327,19 +353,20 @@
 
     def _prod_op(
         self,
         other: "Q[Val]",
         op: Callable[[Any, Any], Any],
         is_pow: bool,
     ) -> "Val":
-        from mathpad.vector_space import VectorSpace
-        from mathpad.vector import Vector
-        from mathpad.matrix import Vector, Matrix
+        from mathpad.core.vector_space import VectorSpace
+        from mathpad.core.vector import Vector
+        from mathpad.core.matrix import Vector, Matrix
+        from mathpad.core.frame import Frame
 
-        if isinstance(other, (Vector, VectorSpace, Matrix)):
+        if isinstance(other, (Vector, VectorSpace, Frame, Matrix)):
             # let the Vector/VectorSpace obj handle the multiplication by returning NotImplemented
             return NotImplemented
 
         other_units, other_val = (
             (other.units, other.expr)
             if isinstance(other, Val)
             else (other if is_pow else 1, other)
@@ -374,16 +401,16 @@
 
         return res
 
 
 ValT = TypeVar("ValT", bound=Val)
 Q = Union[ValT, Num, Val]
 "Any Val, specific or not - or a number"
-X = Union[ValT, Val]
-"Any Val, specific or not - but not a number"
+# X = Union[ValT, Val]
+# "Any Val, specific or not - but not a number"
 
 
 class DimensionError(TypeError):
     
     @classmethod
     def check(cls, a: Val, b: Val):
         
@@ -457,23 +484,25 @@
 class Dimensionless(Unit):
 
     dimension = su.Dimension(1)  # type: ignore
     base_units = sympy.sympify(1)
 
     def __init__(
         self,
-        units: Union[su.Quantity, sympy.Expr, Literal[1]],  # may also be a sympy expression of su.Quantities, ie su.meter**2
+        units: Union[su.Quantity, sympy.Expr, Literal[1]] = 1,  # may also be a sympy expression of su.Quantities, ie su.meter**2
         val: Union[sympy.Expr, Num] = 1,  # gets set in __init__
     ):
         # measures of angle are technically dimensionless
         assert _is_dimensionless(_units2dimensional_expr(units))
         super().__init__(units, val) # type: ignore
+    
+
 
 def _is_dimensionless(dimension):
-    from mathpad.dimensions import Angle, AngularMil, SteRadian
+    from mathpad.core.dimensions import Angle, AngularMil, SteRadian
 
     # accepts output of units2dimensional_expr (an expression, not a dimension object); so normalize here
     if isinstance(dimension, Dimension):
         dimension = dimension.args[0]
 
     return (
         dimension in [
@@ -483,31 +512,28 @@
             Dimensionless.dimension.args[0],
             SteRadian.dimension.args[0],
             AngularMil.dimension.args[0],
         ]
         or dimsys_SI.get_dimensional_dependencies(dimension) == {}
     )
 
-def _sym_func(text: str, caller_frame: FrameType) -> sympy.Expr:
+def _extract_deps_from_fn_str(name: str, caller_frame: FrameType, allow_only: Collection[Type[sympy.Expr]]) -> Iterator[Val]:
     assert (
-        text.count("(") == 1 and text.count(")") == 1 and text[-1] == ")"
-    ), f"Malformed variable name. Variables which are functions of symbols must take the form 'f(x[, y, ...])'. Insted got {other}"
+        name.count("(") == 1 and name.count(")") == 1 and name[-1] == ")"
+    ), f"Malformed variable name. Variables which are functions of symbols must take the form 'f(x[, y, ...])'. Insted got {name}"
 
-    function_name, depstr = text.split("(")
+    _function_name, depstr = name.split("(")
     deps = [x.strip() for x in depstr[:-1].split(",")]
 
     caller_vars = {**caller_frame.f_locals, **caller_frame.f_globals}
-    dep_syms = []
+    
     for dep in deps:
 
         val: Optional[Val] = caller_vars.get(dep, None)
-        assert val, f"Symbolic Function {text} depends on unknown symbol {dep}. " \
+        assert val, f"Symbolic Function {name} depends on unknown symbol {dep}. " \
             "Please ensure a variable with this name is defined in the caller's scope."
         
-        assert isinstance(val.expr, (sympy.Symbol, sympy.Function)), \
-            f"Variable {text} depends on non-symbolic Val '{val}'. \n" \
-            f"Expected {dep}.expr to be a sympy.Symbol, but got {val.expr} ({type(val.expr)})."
-        
-        dep_syms.append(val.expr)
+        assert isinstance(val.expr, tuple(allow_only)), \
+            f"Variable {name} depends on non-symbolic Val '{val}'. \n" \
+            f"Expected {dep}.expr to be one of {allow_only}, but got {val.expr} ({type(val.expr)})."
         
-    sym = sympy.Function(function_name)(*dep_syms) # type: ignore
-    return sym
+        yield val
```

### Comparing `mathpad-1.2.0/mathpad/vector.py` & `mathpad-2.0.0/mathpad/core/vector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,119 +1,143 @@
 
-from typing import Generic, Sequence, Union, Any, TypeVar
-from typing_extensions import Self
+from typing import TYPE_CHECKING, Generic, Iterator, Optional, Sequence, TypeVar, Union, Any
+from typing_extensions import Self, Literal
 
 from sympy.physics.vector import vlatex
-from sympy.vector import Dot, Vector
-from sympy import MatrixSymbol, Matrix, MatrixExpr, Expr, Derivative, Function
+from sympy.vector import Dot, Vector as SympyVector
+from sympy.physics.units.util import convert_to
+from sympy.physics.units.unitsystem import UnitSystem
+from sympy.tensor.array.array_derivatives import ArrayDerivative
+from sympy import Basic, MatrixSymbol, Matrix, MatrixExpr, Expr, Derivative, Function, Symbol
+
+from mathpad.core.val import DimensionError, SumDimensionsMismatchError, Val, Q, _split_coeff_and_units
+from mathpad.core.vector_space import VectorSpace, VectorSpaceT, Homogeneous
+from mathpad.core.frame import Frame
+from mathpad.sympy_extensions import SymbolicMatrixFunction
 
-from mathpad.val import DimensionError, SumDimensionsMismatchError, Val, Q
-from mathpad.vector_space import VectorSpaceT
-from mathpad.equation import Equation
+if TYPE_CHECKING:
+    from mathpad.core.equation import Equation
 
+__all__ = ["Vector"]
 
 class Vector(Generic[VectorSpaceT]):
     """
     A Vector is an instance of a VectorSpace
     """
     
     def __init__(
         self,
-        vector_space: VectorSpaceT,
-        expr: Union[
-            str,
-            Sequence[Q[Val]],
-            MatrixExpr
-        ],
+        frame: Frame[VectorSpaceT],
+        expr: Union[Sequence[Q[Val]], MatrixExpr, ArrayDerivative, SymbolicMatrixFunction],
+        check: bool = False
     ):
-        self.space = vector_space
+        self.frame = frame
 
-        if isinstance(expr, Expr):
-            # expr is the result of a matrix operation. It should be good to use as-is
-            self.expr = expr # type: ignore
+        if isinstance(expr, (MatrixExpr, ArrayDerivative, SymbolicMatrixFunction, self.Cross)):
+            # expr is good to use as-is
+            self.expr = expr
         
-        elif isinstance(expr, str):
-            # construct a symbolic vector
+        else: # must be a sequence of Q[Val] - construct a Matrix from it
+            assert len(expr) == len(frame.space.base_units), \
+                f"Vector must have the same number of elements as the space \"{frame.space.name}\":\n\tExpected {frame.space.base_units}, got {expr}"
+
+            if check:
+                # TODO: make this error message more obviously related to the vector-spaces
+                for val, unit in zip(expr, frame.space.base_units):
+                    if isinstance(val, Val):
+                        DimensionError.check(val, unit) # type: ignore
 
-            sym = "\\vec{" + expr + "}"
-
-            self.expr: MatrixSymbol = MatrixSymbol(sym, len(vector_space.base_units), 1) # type: ignore
-            print()
-        
-        else: # must be a sequence of Q[Val]
-
-            # TODO: make this error message more obviously related to the vector-spaces
-            for val, unit in zip(expr, vector_space.base_units):
-                if isinstance(val, Val):
-                    DimensionError.check(val, unit) # type: ignore
-
-            self.expr: Matrix = Matrix([val.expr if isinstance(val, Val) else val for val in expr]) # type: ignore
-    
-    def in_units(self, space: VectorSpaceT) -> 'Vector[VectorSpaceT]':
-        """
-        Convert the units of this vector to a different VectorSpace while retaining its true physical value
-        """
-
-        return Vector(space, [
-            Val(base_units.units, expr).in_units(new_units)
-            for expr, base_units, new_units in zip(
-                self.expr, # type: ignore
-                self.space.base_units,
-                space.base_units
-            )
-        ])
-    
-    def re(self, space: VectorSpaceT) -> 'Vector[VectorSpaceT]':
-        return self.in_units(space)
+            self.expr \
+                = Matrix([val.expr if isinstance(val, Val) else val for val in expr])
     
-    def __eq__(self, other: 'Vector') -> "Equation":
+    def __eq__(self, other: 'Vector') -> "Equation[VectorSpaceT]":
+        from mathpad.core.equation import Equation
         
-        for a, b in zip(self.space.base_units, other.space.base_units):
+        for a, b in zip(self.frame.space.base_units, other.frame.space.base_units):
             SumDimensionsMismatchError.check(a, "==", b) # type: ignore
 
         return Equation(self, other)
     
     def __hash__(self):
-        return hash((self.expr, self.space))
+        return hash((str(self.expr), self.frame.space))
     
-    def __add__(self, other: Self) -> Self:
+    def __add__(self, other: 'Vector[VectorSpaceT]') -> 'Vector[VectorSpaceT]':
         "self + other"
 
         assert isinstance(other, Vector), \
             f"Cannot add {type(other)} to {type(self)}"
 
-        for a, b in zip(self.space.base_units, other.space.base_units):
+        for a, b in zip(self.frame.space.base_units, other.frame.space.base_units):
             SumDimensionsMismatchError.check(a, "==", b) # type: ignore
 
-        assert self.space is other.space, \
-            f"Cannot add vectors of different VectorSpaces: {self.space} + {other.space}"
+        assert self.frame.space is other.frame.space, \
+            f"Cannot add vectors of different VectorSpaces: {self.frame.space} + {other.frame.space}"
         
         # convert matrixsymbols to explicit beforehand because sympy can't tell that
         # a + b == O[a[0] + b[0], a[1] + b[1], ...]
         # this appears to be because there is no link between a as a matrix symbol and a[0] as a matrix element
         # self_mat = self.val.as_explicit() if isinstance(self.val, MatrixSymbol) else self.val
         # other_mat = other.val.as_explicit() if isinstance(other.val, MatrixSymbol) else other.val
         
-        return self.__class__(self.space, self.expr + other.expr) # type: ignore
+        return self.__class__(self.frame, self.expr + other.expr) # type: ignore
     
     def __sub__(self, other: Self) -> Self:
         "self - other"
         
-        for a, b in zip(self.space.base_units, other.space.base_units):
+        for a, b in zip(self.frame.space.base_units, other.frame.space.base_units):
             SumDimensionsMismatchError.check(a, "==", b)
 
-        assert self.space is other.space, \
-            f"Cannot subtract vectors of different VectorSpaces: {self.space} - {other.space}"
+        assert self.frame.space is other.frame.space, \
+            f"Cannot subtract vectors of different VectorSpaces: {self.frame.space} - {other.frame.space}"
+
+        return self.__class__(self.frame, self.expr - other.expr) # type: ignore
+
+    def in_units(self, units: Union[Literal["SI"], Sequence[Val]]) -> Self:
+        
+        if isinstance(units, str):
+            assert units == "SI", f"Only 'SI' is supported. Got {units}"
+            target_units = [
+                UnitSystem.get_unit_system(unit)._base_units
+                for unit in units
+            ]
+
+        else:
+            assert all(unit.expr == 1 for unit in units), \
+                f"valid units must have an expr == 1. Got {units}"
+            
+            target_units = units
+        
+        scaling_factors, new_units = zip(*(
+            _split_coeff_and_units(
+                convert_to(self_unit.units, target_units.units)  # type: ignore
+            )
+            for self_unit, target_units in zip(self.frame.space.base_units, target_units)
+        ))
+
+        if all(sf == 1 for sf in scaling_factors):
+            return self.__class__(self.frame, self.expr)
+
+        scaling_factors_vec = Matrix(scaling_factors)
 
-        return self.__class__(self.space, self.expr - other.expr) # type: ignore
+        new_expr = scaling_factors_vec * self.expr
+
+        new_space = VectorSpace(
+            self.frame.space.name,
+            self.frame.space.base_names,
+            new_units
+        )
+        
+        frame = new_space(self.frame.name)
+
+        return self.__class__(frame, new_expr)
     
     def _repr_latex_(self, wrapped: bool = True):
 
         # TODO: get vlatex() to display the MatrixSymbol as a \vec{} always
-        # vlatex(self.expr) if isinstance(self.expr, MatrixSymbol) else
+        # vlatex(self.expr) if isinstance(self.expr, MatrixSymbol) else``
         
         if isinstance(self.expr, Derivative):
             # workaround for vlatex() crashing on vector derivatives.
             orig_expr_variables = self.expr.__class__.variables
             self.expr.__class__.variables = self.expr._wrt_variables # type: ignore
         else:
             orig_expr_variables = None
@@ -129,129 +153,130 @@
             + " \\end{bmatrix}"
         ) if isinstance(self.expr, Matrix) else vlatex(self.expr)
     
         if orig_expr_variables:
             # undo temp monkeypatch
             self.expr.__class__.variables = orig_expr_variables # type: ignore
 
-        vectorspace_ltx = self.space._repr_latex_(wrapped=False)
+        frame_ltx = self.frame._repr_latex_(wrapped=False)
         
         spacer_ltx = "\\hspace{1.25em}"
 
-        full_ltx = f"{expr_ltx} {spacer_ltx} {vectorspace_ltx}"
+        full_ltx = f"{expr_ltx} {spacer_ltx} {frame_ltx}"
 
         return f"$$ {full_ltx} $$" if wrapped else full_ltx
     
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Val]:
         return (
-            Val(unit.units, val)
-            for unit, val
-            in zip(self.space.base_units, self.expr) # type: ignore
+            self[index] for index in range(len(self)) # type: ignore
         )
     
     def __len__(self):
         return self.expr.shape[0] # type: ignore
     
     def __getitem__(self, index: int) -> Val:
-        return Val(
-            self.space.base_units[index].units,
-            self.expr[index] # type: ignore
-        )
+        unit = self.frame.space.base_units[index].units
+        # base_name = self.frame.space.base_names[index]
+
+        # expr: Basic = Symbol(f"{self.expr.name}_{base_name}") \
+        #     if getattr(self.expr, 'is_symbol', False) \
+        #     else self.expr[index] # type: ignore
+        
+        return Val(unit, self.expr[index]) # type: ignore
     
     def __neg__(self) -> Self:
-        return self.__class__(self.space, -self.expr) # type: ignore
+        return self.__class__(self.frame.space, -self.expr) # type: ignore
         
     def norm(self) -> Val:
         """
         Returns the norm / magnitude of this vector
 
         Raises:
             ValueError: if the vector does not have uniform dimensionality (each base_unit in the vector space must be equivalent)
         """
-        from mathpad.functions import sqrt
+        from mathpad.math.functions import sqrt
 
-        try:
-            norm_squared = sum(val ** 2 for val in self)
-        except SumDimensionsMismatchError:
-            raise ValueError("Cannot take the norm of a vector with non-uniform units")
+        assert len(set(self.frame.space.base_units)) == 1, "Cannot take the norm of a vector with non-uniform units"
 
-        return sqrt(norm_squared) # type: ignore
+        return Val(
+            self.frame.space.base_units[0].units,
+            self.expr.norm() if isinstance(self.expr, MatrixSymbol) \
+                else sqrt(sum(el ** 2 for el in self)).expr
+        )
     
     def __mul__(self, other: Q[Val]):
         return Vector(
-            (self.space * other) if isinstance(other, Val) else self.space,
+            (self.frame * other) if isinstance(other, Val) else self.frame,
             self.expr * (
                 other.expr if isinstance(other, Val) else other # type: ignore
             )
         )
     
     def __rmul__(self, other: Q[Val]):
         return self * other
     
     def __truediv__(self, other: Q[Val]):
         return Vector(
-            (self.space / other) if isinstance(other, Val) else self.space,
+            (self.frame / other) if isinstance(other, Val) else self.frame,
             self.expr / (other.expr if isinstance(other, Val) else other)
         )
     
     def __str__(self) -> str:
         # TODO: make this output more readable for MatrixExpr's
         nl = "\n"
         nltab = "\n\t"
         val_str = f'{str(self.expr).replace(nl, nltab)}' \
             if isinstance(self.expr, Expr) \
             else str([val for val in self.expr])
 
-        return f"{val_str} wrt. {self.space.name}" if self.space.name else val_str
+        return f"{val_str} wrt. {self.frame.name}" if self.frame.name else val_str
     
     def _repr(self, _with_units: bool) -> str:
         return repr(self)
 
     def __repr__(self) -> str:
         return str(self)
     
     def eval(self, precision: int = 6):
         "Return a new Vec with consts evaluated to their floating point equivalent with given precision"
-        return self.__class__(self.space, self.expr.evalf(precision))
+        return self.__class__(self.frame.space, self.expr.evalf(precision))
     
     # TODO: extend this to higher dimensions and other bases somehow
     # PS: technically cross product is only defined for 3D and 7D, but the concept of orthogonal basis vectors is more general
     # TODO: should this only be defined for R3?
-    def cross(self, other: Self) -> 'Vector':
+    def cross(self, other: Self) -> 'Vector[Any]':
         """
         Cross product of two vectors.
 
         Args:
             other: The other vector to take the cross product with.
                 Must contain the same number of dimensions as this vector.
 
-            out_space: The space to put the result in. Can be a string or a VectorSpace.
-                If a string, a new VectorSpace subclass will be created and instantiated with that name.
-
         Returns:
             A new vector of the output space containing the cross product of the two vectors.
             
         """
         assert len(self) == len(other) == 3, "Cross product is only defined for 3D vectors"
 
-        out_space = self.space * other.space # type: ignore
+        out_space = self.frame.space * other.frame.space # type: ignore
+        out_frame = out_space(self.frame.name)
 
         # MatrixSymbol doesn't have the .cross() method - convert to explicit (MatrixExpr) first
         self_val = self.expr.as_explicit() if isinstance(self.expr, MatrixSymbol) else self.expr
 
         return Vector(
-            out_space,
+            out_frame,
             self.Cross(self_val, other.expr) # type: ignore
         )
     
     def dot(self, other: 'Vector[Any]') -> Val:
         "dot product"
 
         out_units = (
-            self.space.base_units[0] * other.space.base_units[0]
+            self.frame.space.base_units[0] * other.frame.space.base_units[0]
         ).units
 
         self_val_matrix = self.expr if isinstance(self.expr, Matrix) else Matrix(self.expr)
         other_val_matrix = other.expr if isinstance(other.expr, Matrix) else Matrix(other.expr)
 
         return Val(
             out_units,
@@ -271,40 +296,32 @@
         >>> R3.j == R3[0, 1, 0]
         True
 
         etc.
 
         """
 
-        if name in self.space.base_names:
-            idx = self.space.base_names.index(name)
-
-            if isinstance(self.expr, Function):
-                raise
-
-            assert not isinstance(self.expr, Function), \
-                "Cannot yet access components of a symbolic function vector.\n" \
-                "For a temporary workaround, construct the vector explicitly with a list of symbolic values.\n" \
-                "For example:\n" \
-                ">>> v = R3('O')['v_i' * m, 'v_j' * m, 'v_k' * m]\n" \
-                ">>> v.i # this should then work"
-
-
-            return Val(
-                self.space.base_units[idx].units,
-                self.expr[idx] # type: ignore
-            )
+        if name in self.frame.space.base_names:
+            idx = self.frame.space.base_names.index(name)
+            return self[idx]
             
         else:
             raise AttributeError(
                 f"{self.__class__.__name__} has no attribute {name}. "
-                f" (base names are {self.space.base_names})"
+                f" (base names are {self.frame.space.base_names})"
             )
+    
+    def homogeneous(self, name: Optional[str] = None) -> 'Vector[Homogeneous[VectorSpaceT]]':
+        "Return a new vector with an extra dimension of 1"
+        return Vector(
+            Frame(self.frame.space.homogeneous(name), f"self.frame.name", wrt=None),
+            self.expr.row_insert(len(self.frame.space), Matrix([1])) # type: ignore
+        )
         
-    class Cross(Vector):
+    class Cross(SympyVector):
         """
         A custom Cross product class that works with matrices instead of vectors.
         Also gets rid of some weird negation behaviour (see sympy.vector.vector.Cross's __new__ method)
         """
             
         def __new__(cls, expr1, expr2):
             obj = Expr.__new__(cls, expr1, expr2)
@@ -312,23 +329,27 @@
             obj._expr2 = expr2 # type: ignore
             return obj
 
         def doit(self, **hints):
             a, b = self.args # type: ignore
             return a.cross(b, **hints) # type: ignore
 
+
     class Dot(Dot):
         """
         A custom Dot product class that works with matrices instead of vectors
         """
 
         def doit(self, **hints):
             return self._expr1.dot(self._expr2, **hints) # type: ignore
 
 
+
 VecT = TypeVar('VecT', bound=Vector)
 
-def _broken_rtruediv(_self: Vector, other: Q[Val]):
-    "Make it obvious that this is impossible, but don't let the type checker know this method is implemented"
-    assert isinstance(other, Vector), "Can only divide vectors by vectors. Got {other} / {self}"
+from mathpad.sympy_extensions.monkeypatch import monkeypatch_method
+
+@monkeypatch_method(Vector)
+def __rtruediv__(self: Vector[Any], other: Q[Val]):
+    "[UNAVAILABLE] Display helfpul error message, without letting the type checker know"
+    assert isinstance(other, Vector), f"Can only divide vectors by vectors. Got {other} / {self}"
 
-setattr(Vector, '__rtruediv__', _broken_rtruediv)
```

### Comparing `mathpad-1.2.0/pyproject.toml` & `mathpad-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mathpad"
-version = "1.2.0"
+version = "2.0.0"
 description = "Simplified interface to Sympy for solving physics, engineering and maths problems"
 authors = ["Callum J Hays <callumjhays@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CallumJHays/mathpad"
 documentation = "https://mathpad.readthedocs.io"
 classifiers = [
@@ -26,19 +26,15 @@
 python = ">=3.7,<3.10" # < 3.10 required by scipy currently
 typing-extensions = "^4.0.0"
 numpy = "^1.20"
 sympy = "^1.8"
 tqdm = "^4.62.3"
 scipy = "^1.7.1"
 plotly = "^5.3.1"
-
-
-[tool.poetry.extras]
-# kaleido doesn't work on jupyterlite yet
-static_plots = ["kaleido==0.2.1"]
+k3d = "^2.15.2"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

