# Comparing `tmp/mbc_unicode_input-0.1.0.tar.gz` & `tmp/mbc_unicode_input-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbc_unicode_input-0.1.0.tar", max compression
+gzip compressed data, was "mbc_unicode_input-0.2.0.tar", max compression
```

## Comparing `mbc_unicode_input-0.1.0.tar` & `mbc_unicode_input-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9497 2023-07-02 12:38:23.040427 mbc_unicode_input-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-02 11:21:48.877806 mbc_unicode_input-0.1.0/mbc_unicode_input/__init__.py
--rw-r--r--   0        0        0     1235 2023-07-02 12:33:56.549796 mbc_unicode_input-0.1.0/mbc_unicode_input/main.py
--rw-r--r--   0        0        0      467 2023-07-02 11:23:08.659842 mbc_unicode_input-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10378 1970-01-01 00:00:00.000000 mbc_unicode_input-0.1.0/setup.py
--rw-r--r--   0        0        0     9849 1970-01-01 00:00:00.000000 mbc_unicode_input-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9497 2023-07-02 12:38:23.040427 mbc_unicode_input-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-02 11:21:48.877806 mbc_unicode_input-0.2.0/mbc_unicode_input/__init__.py
+-rw-r--r--   0        0        0     1716 2023-07-02 15:03:13.428299 mbc_unicode_input-0.2.0/mbc_unicode_input/main.py
+-rw-r--r--   0        0        0      467 2023-07-02 15:04:06.240597 mbc_unicode_input-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10378 1970-01-01 00:00:00.000000 mbc_unicode_input-0.2.0/setup.py
+-rw-r--r--   0        0        0     9849 1970-01-01 00:00:00.000000 mbc_unicode_input-0.2.0/PKG-INFO
```

### Comparing `mbc_unicode_input-0.1.0/README.md` & `mbc_unicode_input-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mbc_unicode_input-0.1.0/mbc_unicode_input/main.py` & `mbc_unicode_input-0.2.0/mbc_unicode_input/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from typing import Dict, List
 import subprocess
 import pathlib
+import argparse
 
 
 def _flatten_keys(contents: List) -> List:
     new_contents = []
     for item in contents:
         value = item["value"]
         name = item["name"]
@@ -26,21 +27,38 @@
     subprocess.run(["wtype", text])
 
 
 def _parse_output(output: str) -> str:
     return output.strip().split(" ")[0]
 
 
+def _parse_args():
+    """Parse command line arguments"""
+    # optional argument for indicating matching mode
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-m",
+        "--matching",
+        default="fuzzy",
+        choices=["fuzzy", "normal", "regex", "glob", "prefix"],
+        help="Rofi matching mode, see rofi -h",
+    )
+    return parser.parse_args()
+
+
 def main():
+    args = _parse_args()
     with open(
         pathlib.Path.home().joinpath(
             ".local", "share", "mbc-unicode-input", "symbols.json"
         )
     ) as f:
         json_raw = f.read()
         contents = _flatten_keys(json.loads(json_raw))
         formatted = _format_contents(contents)
         output = subprocess.run(
-            ["rofi", "-dmenu"], input=str.encode(formatted), stdout=subprocess.PIPE
+            ["rofi", "-dmenu", "-matching", args.matching],
+            input=str.encode(formatted),
+            stdout=subprocess.PIPE,
         ).stdout.decode("utf-8")
         if len(output) > 0:
             _wtype(_parse_output(output))
```

### Comparing `mbc_unicode_input-0.1.0/setup.py` & `mbc_unicode_input-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['mbc-unicode-input = mbc_unicode_input.main:main']}
 
 setup_kwargs = {
     'name': 'mbc-unicode-input',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': '# mbc-unicode-input\n\nUses rofi to show a character selection string, with metadata. The characters\nare loaded from `"$HOME/.local/share/mbc-unicode-input/symbols.json"`.\n\nThe selected character is sent as virtual keyboard input using\n[wtype](https://github.com/atx/wtype).\n\n## Usage\n\nSimply add your desired characters to `"$HOME/.local/share/mbc-unicode-input/symbols.json"`\nand run\n\n```bash\nmbc-unicode-input\n```\n\nAn example `symbols.json` file is:\n\n```json\n[\n  { "value": "\\\\", "keys": ["\\\\"], "name": "Backslash" },\n  { "value": "ℕ", "keys": ["bN"], "name": "Double-Struck Capital N" },\n  { "value": "⟨", "keys": ["<"], "name": "Mathematical Left Angle Bracket" },\n  { "value": "⟩", "keys": [">"], "name": "Mathematical Right Angle Bracket" },\n  { "value": "∎", "keys": ["qed", "blacksquare"], "name": "End Of Proof" },\n  { "value": "∀", "keys": ["forall", "all"], "name": "For All" },\n  { "value": "∃", "keys": ["exists", "ex"], "name": "There Exists" },\n  { "value": "∈", "keys": ["in"], "name": "Element Of" },\n  { "value": "∋", "keys": ["ni", "contains"], "name": "Contains As Member" },\n  { "value": "∉", "keys": ["notin"], "name": "Not An Element Of" },\n  { "value": "∅", "keys": ["emptyset", "0"], "name": "Empty Set" },\n  { "value": "′", "keys": ["\'"], "name": "Prime" },\n  { "value": "″", "keys": ["\'\'"], "name": "Double Prime" },\n  { "value": "‴", "keys": ["\'\'\'"], "name": "Triple Prime" },\n  { "value": "⁗", "keys": ["\'\'\'\'"], "name": "Quadruple Prime" },\n  { "value": "∘", "keys": ["o", "circ", "comp"], "name": "Ring Operator" },\n  { "value": "≃", "keys": ["~-", "simeq"], "name": "Asymptotically Equal To" },\n  { "value": "×", "keys": ["x", "times"], "name": "Multiplication Sign" },\n  { "value": "⊎", "keys": ["u+"], "name": "Multiset Union" },\n  { "value": "⊤", "keys": ["top"], "name": "Down Tack" },\n  { "value": "⊥", "keys": ["bot"], "name": "Up Tack" },\n  { "value": "⊢", "keys": ["vdash", "|-"], "name": "Right Tack" },\n  { "value": "¬", "keys": ["neg", "not"], "name": "Not Sign" },\n  { "value": "★", "keys": ["star"], "name": "Black Star" },\n  {\n    "value": "ƛ",\n    "keys": ["Gl-", "lambda-"],\n    "name": "Latin Small Letter Lambda With Stroke"\n  },\n  { "value": "·", "keys": ["cdot"], "name": "Middle Dot" },\n  { "value": "—", "keys": ["em", "--"], "name": "Em Dash" },\n  { "value": "∷", "keys": ["::"], "name": "Proportion" },\n  { "value": "⦂", "keys": [":"], "name": "Z Notation Type Colon" },\n  { "value": "｡", "keys": ["."], "name": "Halfwidth Ideographic Full Stop" },\n  { "value": "⊗", "keys": ["otimes", "ox"], "name": "Circled Times" },\n  { "value": "⊕", "keys": ["oplus", "o+"], "name": "Circled Plus" },\n  {\n    "value": "⨁",\n    "keys": ["bigoplus", "O+"],\n    "name": "N-Ary Circled Plus Operator"\n  },\n  { "value": "∥", "keys": ["||", "parallel"], "name": "Parallel To" },\n  {\n    "value": "▷",\n    "keys": ["|>", "vartriangleright"],\n    "name": "White Right-Pointing Triangle"\n  },\n  { "value": "□", "keys": ["|=|", "square"], "name": "White Square" },\n  {\n    "value": "⋯",\n    "keys": ["cdots", "^..."],\n    "name": "Midline Horizontal Ellipsis"\n  },\n  { "value": "∸", "keys": [".-"], "name": "Dot Minus" },\n  { "value": "∔", "keys": [".+"], "name": "Dot Plus" },\n  { "value": "≟", "keys": ["?="], "name": "Questioned Equal To" },\n  { "value": "≢", "keys": ["==n", "neq", "!=="], "name": "Not Identical To" },\n  { "value": "≡", "keys": ["=="], "name": "Identical To" },\n  { "value": "≈", "keys": ["approx", "~~"], "name": "Almost Equal To" },\n  { "value": "≤", "keys": ["<=", "le", "leq"], "name": "Less-Than Or Equal" },\n  {\n    "value": "≥",\n    "keys": [">=", "ge", "geq"],\n    "name": "Greater-Than Or Equal"\n  },\n  { "value": "≲", "keys": ["<~"], "name": "Less-Than or Equivalent To" },\n  { "value": "⊏", "keys": ["sqsubset"], "name": "Square Image Of" },\n  { "value": "⊐", "keys": ["sqsupset"], "name": "Square Original Of" },\n  {\n    "value": "⊑",\n    "keys": ["sqsubseteq"],\n    "name": "Square Image of or Equal To"\n  },\n  {\n    "value": "⊒",\n    "keys": ["sqsupseteq"],\n    "name": "Square Original of or Equal To"\n  },\n  { "value": "⊔", "keys": ["sqcup"], "name": "Square Cup" },\n  { "value": "†", "keys": ["dagger", "t"], "name": "Dagger" },\n  {\n    "value": "⟦",\n    "keys": ["[["],\n    "name": "Mathematical Left White Square Bracket"\n  },\n  {\n    "value": "⟧",\n    "keys": ["]]"],\n    "name": "Mathematical Right White Square Bracket"\n  },\n  {\n    "value": "⇒",\n    "keys": ["=>", "implies"],\n    "name": "Rightwards Double Arrow"\n  },\n  { "value": "⤇", "keys": ["|=>"], "name": "Rightwards Double Arrow From Bar" },\n  {\n    "value": "⇝",\n    "keys": ["/->", "squig", "rightsquigarrow"],\n    "name": "Rightwards Squiggle Arrow"\n  },\n  { "value": "⇔", "keys": ["<=>", "iff"], "name": "Left Right Double Arrow" },\n  { "value": "↠", "keys": ["rr-"], "name": "Rightwards Two Headed Arrow" },\n  { "value": "→", "keys": ["->", "to", "r"], "name": "Rightwards Arrow" },\n  {\n    "value": "←",\n    "keys": ["<-", "gets", "l", "leftarrow"],\n    "name": "Leftwards Arrow"\n  },\n  {\n    "value": "↦",\n    "keys": ["|->", "mapsto"],\n    "name": "Rightwards Arrow from Bar"\n  },\n  { "value": "↑", "keys": ["u", "uparrow"], "name": "Upwards Arrow" },\n  { "value": "↓", "keys": ["d", "downarrow"], "name": "Downwards Arrow" },\n  { "value": "⌊", "keys": ["clL"], "name": "Left Floor" },\n  { "value": "⌋", "keys": ["clR"], "name": "Right Floor" },\n  { "value": "∧", "keys": ["and", "wedge"], "name": "Logical And" },\n  { "value": "∨", "keys": ["or", "vee"], "name": "Logical Or" },\n  { "value": "⊃", "keys": ["sup"], "name": "Superset Of" },\n  { "value": "⊆", "keys": ["subseteq"], "name": "Subset Of or Equal To" },\n  { "value": "⊂", "keys": ["subset"], "name": "Subset Of" },\n  { "value": "α", "keys": ["alpha", "Ga"], "name": "Greek Small Letter Alpha" },\n  { "value": "β", "keys": ["beta", "Gb"], "name": "Greek Small Letter Beta" },\n  { "value": "γ", "keys": ["gamma", "Gg"], "name": "Greek Small Letter Gamma" },\n  { "value": "δ", "keys": ["delta", "Gd"], "name": "Greek Small Letter Delta" },\n  {\n    "value": "ε",\n    "keys": ["epsilon", "Ge"],\n    "name": "Greek Small Letter Epsilon"\n  },\n  { "value": "ζ", "keys": ["zeta", "Gz"], "name": "Greek Small Letter Zeta" },\n  { "value": "η", "keys": ["eta"], "name": "Greek Small Letter Eta" },\n  { "value": "θ", "keys": ["theta"], "name": "Greek Small Letter Theta" },\n  { "value": "ι", "keys": ["iota", "Gi"], "name": "Greek Small Letter Iota" },\n  { "value": "κ", "keys": ["kappa", "Gk"], "name": "Greek Small Letter Kappa" },\n  {\n    "value": "λ",\n    "keys": ["lambda", "Gl"],\n    "name": "Greek Small Letter Lambda"\n  },\n  { "value": "μ", "keys": ["mu"], "name": "Greek Small Letter Mu" },\n  { "value": "ν", "keys": ["nu"], "name": "Greek Small Letter Nu" },\n  { "value": "ξ", "keys": ["xi", "Gx"], "name": "Greek Small Letter Xi" },\n  {\n    "value": "ο",\n    "keys": ["omicron", "Go"],\n    "name": "Greek Small Letter Omicron"\n  },\n  { "value": "π", "keys": ["pi", "Gp"], "name": "Greek Small Letter Pi" },\n  { "value": "ρ", "keys": ["rho", "Gr"], "name": "Greek Small Letter Rho" },\n  {\n    "value": "ς",\n    "keys": ["finalsigma"],\n    "name": "Greek Small Letter Final Sigma"\n  },\n  { "value": "σ", "keys": ["sigma"], "name": "Greek Small Letter Sigma" },\n  { "value": "τ", "keys": ["tau"], "name": "Greek Small Letter Tau" },\n  { "value": "υ", "keys": ["upsilon"], "name": "Greek Small Letter Upsilon" },\n  { "value": "φ", "keys": ["phi"], "name": "Greek Small Letter Phi" },\n  { "value": "χ", "keys": ["chi"], "name": "Greek Small Letter Chi" },\n  { "value": "ψ", "keys": ["psi"], "name": "Greek Small Letter Psi" },\n  { "value": "ω", "keys": ["omega"], "name": "Greek Small Letter Omega" },\n  { "value": "Σ", "keys": ["Sigma"], "name": "Greek Capital Letter Sigma" },\n  { "value": "Π", "keys": ["Pi"], "name": "Greek Capital Letter Pi" },\n  {\n    "value": "Δ",\n    "keys": ["Delta", "GD"],\n    "name": "Greek Capital Letter Delta"\n  },\n  {\n    "value": "Γ",\n    "keys": ["Gamma", "GG"],\n    "name": "Greek Capital Letter Gamma"\n  },\n  { "value": "ℬ", "keys": ["sB"], "name": "Script Capital B" },\n  { "value": "𝓁", "keys": ["sl"], "name": "Mathematical Script Small L" },\n  { "value": "ᵇ", "keys": ["^b"], "name": "Modifier Letter Small B" },\n  { "value": "ˡ", "keys": ["^l"], "name": "Modifier Letter Small L" },\n  { "value": "ʳ", "keys": ["^r"], "name": "Modifier Letter Small R" },\n  { "value": "ˢ", "keys": ["^s"], "name": "Modifier Letter Small S" },\n  { "value": "ᵗ", "keys": ["^t"], "name": "Modifier Letter Small T" },\n  { "value": "⁺", "keys": ["^+"], "name": "Superscript Plus Sign" },\n  { "value": "⁻", "keys": ["^-"], "name": "Superscript Minus" },\n  { "value": "₀", "keys": ["_0"], "name": "Subscript Zero" },\n  { "value": "₁", "keys": ["_1"], "name": "Subscript One" },\n  { "value": "₂", "keys": ["_2"], "name": "Subscript Two" },\n  { "value": "₃", "keys": ["_3"], "name": "Subscript Three" },\n  { "value": "₄", "keys": ["_4"], "name": "Subscript Four" },\n  { "value": "₅", "keys": ["_5"], "name": "Subscript Five" },\n  { "value": "₆", "keys": ["_6"], "name": "Subscript Six" },\n  { "value": "₇", "keys": ["_7"], "name": "Subscript Seven" },\n  { "value": "₈", "keys": ["_8"], "name": "Subscript Eight" },\n  { "value": "₉", "keys": ["_9"], "name": "Subscript Nine" }\n]\n```\n',
     'author': 'Manuel Brea',
     'author_email': 'm.brea.carreras@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mbc_unicode_input-0.1.0/PKG-INFO` & `mbc_unicode_input-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbc-unicode-input
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Manuel Brea
 Author-email: m.brea.carreras@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

