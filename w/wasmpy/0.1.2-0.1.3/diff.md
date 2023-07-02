# Comparing `tmp/wasmpy-0.1.2.tar.gz` & `tmp/wasmpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmpy-0.1.2.tar", last modified: Sat Jun 24 23:33:09 2023, max compression
+gzip compressed data, was "dist/wasmpy-0.1.3.tar", last modified: Sun Jul  2 16:43:58 2023, max compression
```

## Comparing `wasmpy-0.1.2.tar` & `wasmpy-0.1.3.tar`

### file list

```diff
@@ -1,158 +1,156 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.427096 wasmpy-0.1.2/
--rw-rw-rw-   0        0        0     1068 2023-06-15 12:12:24.000000 wasmpy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      143 2023-06-24 18:22:33.000000 wasmpy-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2445 2023-06-24 23:33:09.427096 wasmpy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1568 2023-06-24 18:50:52.000000 wasmpy-0.1.2/README.md
--rw-rw-rw-   0        0        0     4975 2023-06-24 22:12:53.000000 wasmpy-0.1.2/opcodes.py
--rw-rw-rw-   0        0        0       42 2023-06-24 23:33:09.427096 wasmpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     5360 2023-06-24 23:32:18.000000 wasmpy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.270573 wasmpy-0.1.2/wasmpy/
--rw-rw-rw-   0        0        0      106 2023-06-23 12:23:39.000000 wasmpy-0.1.2/wasmpy/__init__.py
--rw-rw-rw-   0        0        0     1689 2023-06-23 11:11:55.000000 wasmpy-0.1.2/wasmpy/hooks.py
--rw-rw-rw-   0        0        0    14893 2023-06-24 07:42:57.000000 wasmpy-0.1.2/wasmpy/instructions.py
--rw-rw-rw-   0        0        0     3097 2023-06-24 21:59:04.000000 wasmpy-0.1.2/wasmpy/module.py
--rw-rw-rw-   0        0        0     1085 2023-06-22 15:47:07.000000 wasmpy-0.1.2/wasmpy/native.py
--rw-rw-rw-   0        0        0     5286 2023-06-23 11:12:14.000000 wasmpy-0.1.2/wasmpy/sections.py
--rw-rw-rw-   0        0        0     2421 2023-06-21 19:25:53.000000 wasmpy-0.1.2/wasmpy/types.py
--rw-rw-rw-   0        0        0     2029 2023-06-23 11:12:52.000000 wasmpy-0.1.2/wasmpy/values.py
--rw-rw-rw-   0        0        0     8283 2023-06-24 23:27:15.000000 wasmpy-0.1.2/wasmpy/win_x86.cpp
-drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.287310 wasmpy-0.1.2/wasmpy/x86/
--rw-rw-rw-   0        0        0      217 2023-06-24 06:23:55.000000 wasmpy-0.1.2/wasmpy/x86/helpers.cpp
--rw-rw-rw-   0        0        0      128 2023-06-24 23:03:29.000000 wasmpy-0.1.2/wasmpy/x86/helpers.h
-drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.413246 wasmpy-0.1.2/wasmpy/x86/instructions/
--rw-rw-rw-   0        0        0       16 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/drop
--rw-rw-rw-   0        0        0       76 2023-06-24 05:34:10.000000 wasmpy-0.1.2/wasmpy/x86/instructions/drop.asm
--rw-rw-rw-   0        0        0       16 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f32.const
--rw-rw-rw-   0        0        0       81 2023-06-24 22:35:34.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f32.const.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f32.eq
--rw-rw-rw-   0        0        0      210 2023-06-24 22:35:42.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f32.eq.asm
--rw-rw-rw-   0        0        0       28 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f64.const
--rw-rw-rw-   0        0        0      131 2023-06-24 22:35:50.000000 wasmpy-0.1.2/wasmpy/x86/instructions/f64.const.asm
--rw-rw-rw-   0        0        0       31 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.add
--rw-rw-rw-   0        0        0      150 2023-06-24 22:29:16.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.add.asm
--rw-rw-rw-   0        0        0       31 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.and
--rw-rw-rw-   0        0        0      150 2023-06-24 22:35:57.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.and.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.clz
--rw-rw-rw-   0        0        0      199 2023-06-24 22:36:17.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.clz.asm
--rw-rw-rw-   0        0        0       16 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.const
--rw-rw-rw-   0        0        0       81 2023-06-24 22:36:20.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.const.asm
--rw-rw-rw-   0        0        0       33 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ctz
--rw-rw-rw-   0        0        0      175 2023-06-24 22:36:23.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ctz.asm
--rw-rw-rw-   0        0        0       41 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.div_s
--rw-rw-rw-   0        0        0      184 2023-06-24 22:36:28.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.div_s.asm
--rw-rw-rw-   0        0        0       41 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.div_u
--rw-rw-rw-   0        0        0      183 2023-06-24 22:36:32.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.div_u.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.eq
--rw-rw-rw-   0        0        0      210 2023-06-24 22:37:09.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.eq.asm
--rw-rw-rw-   0        0        0       32 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.eqz
--rw-rw-rw-   0        0        0      171 2023-06-24 22:37:12.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.eqz.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ge_s
--rw-rw-rw-   0        0        0      211 2023-06-24 22:37:16.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ge_s.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ge_u
--rw-rw-rw-   0        0        0      211 2023-06-24 22:37:19.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ge_u.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.gt_s
--rw-rw-rw-   0        0        0      210 2023-06-24 22:39:10.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.gt_s.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.gt_u
--rw-rw-rw-   0        0        0      210 2023-06-24 22:39:15.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.gt_u.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.le_s
--rw-rw-rw-   0        0        0      211 2023-06-24 22:39:18.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.le_s.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.le_u
--rw-rw-rw-   0        0        0      211 2023-06-24 22:39:22.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.le_u.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.lt_s
--rw-rw-rw-   0        0        0      210 2023-06-24 22:39:26.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.lt_s.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.lt_u
--rw-rw-rw-   0        0        0      210 2023-06-24 22:39:29.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.lt_u.asm
--rw-rw-rw-   0        0        0       32 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.mul
--rw-rw-rw-   0        0        0      151 2023-06-24 22:39:33.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.mul.asm
--rw-rw-rw-   0        0        0       40 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ne
--rw-rw-rw-   0        0        0      212 2023-06-24 22:39:36.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.ne.asm
--rw-rw-rw-   0        0        0       31 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.or
--rw-rw-rw-   0        0        0      149 2023-06-24 22:39:40.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.or.asm
--rw-rw-rw-   0        0        0       23 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.popcnt
--rw-rw-rw-   0        0        0      114 2023-06-24 22:39:43.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.popcnt.asm
--rw-rw-rw-   0        0        0       43 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rem_s
--rw-rw-rw-   0        0        0      198 2023-06-24 22:39:46.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rem_s.asm
--rw-rw-rw-   0        0        0       43 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rem_u
--rw-rw-rw-   0        0        0      197 2023-06-24 22:39:50.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rem_u.asm
--rw-rw-rw-   0        0        0       31 2023-06-24 23:32:53.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rotl
--rw-rw-rw-   0        0        0      149 2023-06-24 22:39:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rotl.asm
--rw-rw-rw-   0        0        0       31 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rotr
--rw-rw-rw-   0        0        0      149 2023-06-24 22:39:57.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.rotr.asm
--rw-rw-rw-   0        0        0       37 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shl
--rw-rw-rw-   0        0        0      169 2023-06-24 22:40:01.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shl.asm
--rw-rw-rw-   0        0        0       37 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shr_s
--rw-rw-rw-   0        0        0      169 2023-06-24 22:40:05.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shr_s.asm
--rw-rw-rw-   0        0        0       37 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shr_u
--rw-rw-rw-   0        0        0      169 2023-06-24 22:40:10.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.shr_u.asm
--rw-rw-rw-   0        0        0       31 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.sub
--rw-rw-rw-   0        0        0      150 2023-06-24 22:40:14.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.sub.asm
--rw-rw-rw-   0        0        0       10 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.wrap_i64
--rw-rw-rw-   0        0        0       55 2023-06-24 22:40:17.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.wrap_i64.asm
--rw-rw-rw-   0        0        0       31 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.xor
--rw-rw-rw-   0        0        0      150 2023-06-24 22:40:21.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i32.xor.asm
--rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.add
--rw-rw-rw-   0        0        0      253 2023-06-24 22:40:33.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.add.asm
--rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.and
--rw-rw-rw-   0        0        0      253 2023-06-24 22:40:36.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.and.asm
--rw-rw-rw-   0        0        0       74 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.clz
--rw-rw-rw-   0        0        0      366 2023-06-24 22:40:40.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.clz.asm
--rw-rw-rw-   0        0        0       28 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.const
--rw-rw-rw-   0        0        0      131 2023-06-24 22:40:42.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.const.asm
--rw-rw-rw-   0        0        0       64 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ctz
--rw-rw-rw-   0        0        0      330 2023-06-24 22:40:48.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ctz.asm
--rw-rw-rw-   0        0        0       58 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.eq
--rw-rw-rw-   0        0        0      296 2023-06-24 22:40:51.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.eq.asm
--rw-rw-rw-   0        0        0       43 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.eqz
--rw-rw-rw-   0        0        0      228 2023-06-24 22:40:55.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.eqz.asm
--rw-rw-rw-   0        0        0       38 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.extend_i32_s
--rw-rw-rw-   0        0        0      204 2023-06-24 22:40:58.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.extend_i32_s.asm
--rw-rw-rw-   0        0        0       14 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.extend_i32_u
--rw-rw-rw-   0        0        0       79 2023-06-24 22:41:02.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.extend_i32_u.asm
--rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ge_s
--rw-rw-rw-   0        0        0      310 2023-06-24 22:41:05.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ge_s.asm
--rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ge_u
--rw-rw-rw-   0        0        0      310 2023-06-24 22:41:09.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ge_u.asm
--rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.gt_s
--rw-rw-rw-   0        0        0      309 2023-06-24 22:41:13.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.gt_s.asm
--rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.gt_u
--rw-rw-rw-   0        0        0      309 2023-06-24 22:41:16.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.gt_u.asm
--rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.le_s
--rw-rw-rw-   0        0        0      310 2023-06-24 22:41:20.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.le_s.asm
--rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.le_u
--rw-rw-rw-   0        0        0      310 2023-06-24 22:41:23.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.le_u.asm
--rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.lt_s
--rw-rw-rw-   0        0        0      309 2023-06-24 22:41:27.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.lt_s.asm
--rw-rw-rw-   0        0        0       60 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.lt_u
--rw-rw-rw-   0        0        0      309 2023-06-24 22:41:31.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.lt_u.asm
--rw-rw-rw-   0        0        0       58 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ne
--rw-rw-rw-   0        0        0      293 2023-06-24 22:41:34.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.ne.asm
--rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.or
--rw-rw-rw-   0        0        0      251 2023-06-24 22:41:37.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.or.asm
--rw-rw-rw-   0        0        0       44 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.popcnt
--rw-rw-rw-   0        0        0      214 2023-06-24 22:41:41.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.popcnt.asm
--rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.sub
--rw-rw-rw-   0        0        0      253 2023-06-24 22:41:44.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.sub.asm
--rw-rw-rw-   0        0        0       54 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.xor
--rw-rw-rw-   0        0        0      253 2023-06-24 22:41:48.000000 wasmpy-0.1.2/wasmpy/x86/instructions/i64.xor.asm
--rw-rw-rw-   0        0        0      108 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/select
--rw-rw-rw-   0        0        0      502 2023-06-24 22:41:51.000000 wasmpy-0.1.2/wasmpy/x86/instructions/select.asm
-drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.417137 wasmpy-0.1.2/wasmpy/x86/instructions/x64/
--rw-rw-rw-   0        0        0       89 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.get
--rw-rw-rw-   0        0        0      412 2023-06-24 22:35:15.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.get.asm
--rw-rw-rw-   0        0        0      102 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.set
--rw-rw-rw-   0        0        0      467 2023-06-24 22:35:21.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.set.asm
--rw-rw-rw-   0        0        0      137 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.tee
--rw-rw-rw-   0        0        0      642 2023-06-24 22:35:25.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x64/local.tee.asm
-drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.427096 wasmpy-0.1.2/wasmpy/x86/instructions/x86/
--rw-rw-rw-   0        0        0       83 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.get
--rw-rw-rw-   0        0        0      412 2023-06-24 22:42:10.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.get.asm
--rw-rw-rw-   0        0        0       92 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.set
--rw-rw-rw-   0        0        0      467 2023-06-24 22:42:13.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.set.asm
--rw-rw-rw-   0        0        0      127 2023-06-24 23:32:54.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.tee
--rw-rw-rw-   0        0        0      642 2023-06-24 22:42:17.000000 wasmpy-0.1.2/wasmpy/x86/instructions/x86/local.tee.asm
--rw-rw-rw-   0        0        0     1193 2023-06-24 07:47:40.000000 wasmpy-0.1.2/wasmpy/x86/opcodes.h
-drwxrwxrwx   0        0        0        0 2023-06-24 23:33:09.285804 wasmpy-0.1.2/wasmpy.egg-info/
--rw-rw-rw-   0        0        0     2445 2023-06-24 23:33:09.000000 wasmpy-0.1.2/wasmpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4933 2023-06-24 23:33:09.000000 wasmpy-0.1.2/wasmpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 23:33:09.000000 wasmpy-0.1.2/wasmpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 23:33:09.000000 wasmpy-0.1.2/wasmpy.egg-info/top_level.txt
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2023-07-02 16:43:58.000000 wasmpy-0.1.3/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1068 2023-07-02 16:43:51.000000 wasmpy-0.1.3/LICENSE
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      183 2023-07-02 16:43:51.000000 wasmpy-0.1.3/MANIFEST.in
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2469 2023-07-02 16:43:58.000000 wasmpy-0.1.3/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1600 2023-07-02 16:43:51.000000 wasmpy-0.1.3/README.md
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5272 2023-07-02 16:43:51.000000 wasmpy-0.1.3/opcodes.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       38 2023-07-02 16:43:58.000000 wasmpy-0.1.3/setup.cfg
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     8719 2023-07-02 16:43:51.000000 wasmpy-0.1.3/setup.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2023-07-02 16:43:58.000000 wasmpy-0.1.3/wasmpy/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      106 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/__init__.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1689 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/hooks.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    14893 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/instructions.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2995 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/module.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1187 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/native.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     1209 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/opcodes.hpp
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     5286 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/sections.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2421 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/types.py
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2029 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/values.py
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2023-07-02 16:43:58.000000 wasmpy-0.1.3/wasmpy/x86/
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2023-07-02 16:43:58.000000 wasmpy-0.1.3/wasmpy/x86/32/
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       81 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/32/local.get
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      415 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/32/local.get.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       90 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/32/local.set
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      477 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/32/local.set.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)      123 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/32/local.tee
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      639 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/32/local.tee.s
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2023-07-02 16:43:58.000000 wasmpy-0.1.3/wasmpy/x86/64/
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       87 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/64/local.get
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      415 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/64/local.get.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)      100 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/64/local.set
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      477 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/64/local.set.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)      133 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/64/local.tee
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      639 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/64/local.tee.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       16 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/drop
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       86 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/drop.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       15 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/f32.const
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       85 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/f32.const.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/f32.eq
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      176 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/f32.eq.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       27 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/f64.const
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      139 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/f64.const.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       30 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.add
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      154 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.add.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       30 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.and
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      154 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.and.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       37 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.clz
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      179 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.clz.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       15 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i32.const
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       85 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.const.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       30 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.ctz
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      152 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.ctz.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       40 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i32.div_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      188 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.div_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       40 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i32.div_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      187 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.div_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.eq
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      176 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.eq.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       28 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.eqz
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      136 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.eqz.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.ge_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      177 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.ge_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i32.ge_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      177 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.ge_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.gt_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      176 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.gt_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.gt_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      176 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.gt_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.le_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      177 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.le_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.le_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      177 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.le_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.lt_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      176 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.lt_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i32.lt_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      176 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.lt_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       31 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.mul
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      155 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.mul.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.ne
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      178 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.ne.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       30 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.or
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      153 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.or.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       21 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.popcnt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      105 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.popcnt.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       42 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.rem_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      204 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.rem_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       42 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.rem_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      203 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.rem_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       30 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.rotl
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      153 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.rotl.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       30 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.rotr
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      153 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.rotr.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.shl
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      176 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.shl.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.shr_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      176 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.shr_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       36 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i32.shr_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      176 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.shr_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       30 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i32.sub
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      154 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.sub.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        9 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i32.wrap_i64
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       55 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.wrap_i64.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       30 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i32.xor
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      154 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i32.xor.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       53 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.add
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      261 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.add.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       53 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.and
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      261 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.and.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       69 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i64.clz
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      327 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.clz.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       27 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.const
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      139 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.const.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       59 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.ctz
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      286 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.ctz.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       54 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.eq
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      264 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.eq.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       39 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.eqz
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      194 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.eqz.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       33 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i64.extend_i32_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      158 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.extend_i32_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       11 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.extend_i32_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)       57 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.extend_i32_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       56 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.ge_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      276 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.ge_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       56 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.ge_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      276 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.ge_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       56 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.gt_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      275 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.gt_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       56 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.gt_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      275 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.gt_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       56 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i64.le_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      276 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.le_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       56 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i64.le_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      276 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.le_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       56 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i64.lt_s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      275 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.lt_s.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       56 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i64.lt_u
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      275 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.lt_u.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       54 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/i64.ne
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      261 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.ne.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       53 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.or
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      259 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.or.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       40 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.popcnt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      186 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.popcnt.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       53 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.sub
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      261 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.sub.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)       53 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy/x86/i64.xor
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      261 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/i64.xor.s
+-rwxr-xr-x   0 appveyor  (1000) appveyor  (1000)      106 2023-07-02 16:43:56.000000 wasmpy-0.1.3/wasmpy/x86/select
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      492 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86/select.s
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)    12547 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86.cpp
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)      343 2023-07-02 16:43:51.000000 wasmpy-0.1.3/wasmpy/x86.hpp
+drwxr-xr-x   0 appveyor  (1000) appveyor  (1000)        0 2023-07-02 16:43:58.000000 wasmpy-0.1.3/wasmpy.egg-info/
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     2469 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy.egg-info/PKG-INFO
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)     3094 2023-07-02 16:43:58.000000 wasmpy-0.1.3/wasmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        1 2023-07-02 16:43:57.000000 wasmpy-0.1.3/wasmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 appveyor  (1000) appveyor  (1000)        7 2023-07-02 16:43:58.000000 wasmpy-0.1.3/wasmpy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `wasmpy-0.1.2/LICENSE` & `wasmpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.2/PKG-INFO` & `wasmpy-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,87 @@
-Metadata-Version: 2.1
-Name: wasmpy
-Version: 0.1.2
-Summary: Interactions between WebAssembly and Python
-Home-page: https://github.com/olivi-r/wasmpy
-Author: Olivia Ryan
-Author-email: olivia.r.dev@gmail.com
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Assembly
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# WasmPy
-Interacting with WebAssembly code from python.
-
-Wasmpy is a fairly lightweight layer that sits between Python and the WebAssembly code. When attempting to import a WebAssembly file, the file is read and it is converted into native machine code for native speeds.
-
-This project is intended to be used in conjunction with [wasmpy-build](https://github.com/olivi-r/wasmpy-build), although it does support regular WebAssembly files too.
-
-## Installing
-
-Install the latest version:
-
-```
-$ python -m pip install wasmpy
-```
-
-Or build and install from source (the `assemble` step requires having [NASM](https://www.nasm.us/) on path):
-
-
-```
-$ git clone https://github.com/olivi-r/wasmpy.git
-$ cd wasmpy
-$ python setup.py assemble
-$ python setup.py install
-```
-
-# Usage
-WasmPy defines import hooks to make the loading of WebAssembly binary files much easier! Just import the `WasmPy` library then you are good to go!
-### Example:
-If you have the following project setup:
-
-```
-|- my_wasm_file.wasm
-|- main.py
-```
-Then in `main.py` the following code will load the WebAssembly file:
-```py
-import wasmpy
-import my_wasm_file
-```
-The hook also allows importing the files from submodules, eg:
-```
-|- main.py
-|- my_module
-|  |- my_wasm_file.wasm
-```
-Then 
-```py
-import wasmpy
-from my_module import my_wasm_file
-```
-
-Functions can be called with the call function from the imported module:
-
-```py
-import wasmpy
-import wasm_math
-
-wasm_math.call("add")(...)
-```
-
-This is due to WebAssembly supporting exported names that may not be valid Python names, such as `add two numbers`
+Metadata-Version: 2.1
+Name: wasmpy
+Version: 0.1.3
+Summary: Interactions between WebAssembly and Python
+Home-page: https://github.com/olivi-r/wasmpy
+Author: Olivia Ryan
+Author-email: olivia.r.dev@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: WebAssembly
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Assembly
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![AppVeyor](https://img.shields.io/appveyor/build/olivi-r/wasmpy)](https://ci.appveyor.com/project/olivi-r/wasmpy)
+
+# wasmpy
+Interacting with WebAssembly code from python.
+
+Wasmpy is a fairly lightweight layer that sits between Python and the WebAssembly code. When attempting to import a WebAssembly file, the file is read and it is converted into native machine code for native speeds.
+
+This project is intended to be used in conjunction with [wasmpy-build](https://github.com/olivi-r/wasmpy-build), although it does support regular WebAssembly files too.
+
+## Installing
+
+Install the latest version:
+
+```
+python -m pip install wasmpy
+```
+
+Or build and install from source:
+
+
+```
+git clone https://github.com/olivi-r/wasmpy.git
+cd wasmpy
+python setup.py assemble
+python -m pip install .
+```
+
+# Usage
+WasmPy defines import hooks to make the loading of WebAssembly binary files much easier! Just import the `wasmpy` library then you are good to go!
+### Example:
+If you have the following project setup:
+
+```
+|- my_wasm_file.wasm
+|- main.py
+```
+Then in `main.py` the following code will load the WebAssembly file:
+```py
+import wasmpy
+import my_wasm_file
+```
+The hook also allows importing the files from submodules, eg:
+```
+|- main.py
+|- my_module
+|  |- my_wasm_file.wasm
+```
+Then 
+```py
+import wasmpy
+from my_module import my_wasm_file
+```
+
+Functions can be called with the call function from the imported module:
+
+```py
+import wasmpy
+import wasm_math
+
+wasm_math.call("add")(...)
+```
+
+This is due to WebAssembly supporting exported names that may not be valid Python names, such as `add two numbers`
```

### Comparing `wasmpy-0.1.2/README.md` & `wasmpy-0.1.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-# WasmPy
+[![AppVeyor](https://img.shields.io/appveyor/build/olivi-r/wasmpy)](https://ci.appveyor.com/project/olivi-r/wasmpy)
+
+# wasmpy
 Interacting with WebAssembly code from python.
 
 Wasmpy is a fairly lightweight layer that sits between Python and the WebAssembly code. When attempting to import a WebAssembly file, the file is read and it is converted into native machine code for native speeds.
 
 This project is intended to be used in conjunction with [wasmpy-build](https://github.com/olivi-r/wasmpy-build), although it does support regular WebAssembly files too.
 
 ## Installing
 
 Install the latest version:
 
 ```
-$ python -m pip install wasmpy
+python -m pip install wasmpy
 ```
 
-Or build and install from source (the `assemble` step requires having [NASM](https://www.nasm.us/) on path):
+Or build and install from source:
 
 
 ```
-$ git clone https://github.com/olivi-r/wasmpy.git
-$ cd wasmpy
-$ python setup.py assemble
-$ python setup.py install
+git clone https://github.com/olivi-r/wasmpy.git
+cd wasmpy
+python setup.py assemble
+python -m pip install .
 ```
 
 # Usage
-WasmPy defines import hooks to make the loading of WebAssembly binary files much easier! Just import the `WasmPy` library then you are good to go!
+WasmPy defines import hooks to make the loading of WebAssembly binary files much easier! Just import the `wasmpy` library then you are good to go!
 ### Example:
 If you have the following project setup:
 
 ```
 |- my_wasm_file.wasm
 |- main.py
 ```
```

### Comparing `wasmpy-0.1.2/wasmpy/hooks.py` & `wasmpy-0.1.3/wasmpy/hooks.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.2/wasmpy/instructions.py` & `wasmpy-0.1.3/wasmpy/instructions.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.2/wasmpy/module.py` & `wasmpy-0.1.3/wasmpy/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,19 +97,17 @@
     module["funcs"] += tuple(
         {
             "type": module["types"][typeidx[i]],
             "locals": t,
             "body": e,
             "obj": create_function(
                 module["types"][typeidx[i]][1][0],
-                "".join("".join(chr(k) for k in j[1:]) for j in e).encode(
-                    "ansi"
-                ),
+                bytes(k for j in e for k in j[1:]),
                 bytes(module["types"][typeidx[i]][0]),
-                "".join(chr(j) for j in t).encode("ansi"),
+                bytes(t),
             ),
         }
         for i, (t, e) in enumerate(code)
     )
 
     for e in module["exports"]:
         if e["desc"][0] == "func":
```

### Comparing `wasmpy-0.1.2/wasmpy/native.py` & `wasmpy-0.1.3/wasmpy/native.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from . import win_x86
+import platform
 import struct
 import ctypes
 
 
+if platform.machine() in ("x86", "i386", "i686", "AMD64", "x86_64"):
+    from . import x86 as nativelib
+
+
 def create_function(ret, code, arg=b"", local=b""):
-    func, ret = win_x86.create_function(
+    func, ret = nativelib.create_function(
         struct.calcsize("P"), ret, code, arg, local
     )
 
     params = []
     param_doc = []
     for i, a in enumerate(arg):
         if a == 0x7F:
```

### Comparing `wasmpy-0.1.2/wasmpy/sections.py` & `wasmpy-0.1.3/wasmpy/sections.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.2/wasmpy/types.py` & `wasmpy-0.1.3/wasmpy/types.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.2/wasmpy/values.py` & `wasmpy-0.1.3/wasmpy/values.py`

 * *Files identical despite different names*

### Comparing `wasmpy-0.1.2/wasmpy/x86/opcodes.h` & `wasmpy-0.1.3/wasmpy/opcodes.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-#include "helpers.h"
+#ifndef OPCODES_H
+#define OPCODES_H
+
+#include "x86.hpp"
 
 #define PUSH(x) 0x66, 0x68, (uint8_t)(x & 255), (uint8_t)(x >> 8)
 
 #define JMP(x) 0xEB, (uint8_t)x
 #define JE(x) 0x74, (uint8_t)x
 #define JNE(x) 0x75, (uint8_t)x
 
 #define V32 PUSH(2)
 #define V64 PUSH(4)
 
-#define MOV_AX 0x66, 0xB8
-
 #define PUSH_AX 0x66, 0x50
 #define PUSH_CX 0x66, 0x51
 #define PUSH_DX 0x66, 0x52
 #define PUSH_BX 0x66, 0x53
 
 #define POP_AX 0x66, 0x58
 #define POP_CX 0x66, 0x59
@@ -41,7 +42,9 @@
 #define POP_V64A POP_AX, POP_EAX, POP_ECX
 #define POP_V64B POP_DX, POP_EDX, POP_EBX
 
 #define PUSH_V32 PUSH_AX, SHR_EAX, PUSH_AX, V32
 #define PUSH_V64 PUSH_CX, SHR_ECX, PUSH_CX, PUSH_AX, SHR_EAX, PUSH_AX, V64
 
 bytes decodeFunc(bytes buf, char plat);
+
+#endif
```

### Comparing `wasmpy-0.1.2/wasmpy.egg-info/PKG-INFO` & `wasmpy-0.1.3/wasmpy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,87 @@
-Metadata-Version: 2.1
-Name: wasmpy
-Version: 0.1.2
-Summary: Interactions between WebAssembly and Python
-Home-page: https://github.com/olivi-r/wasmpy
-Author: Olivia Ryan
-Author-email: olivia.r.dev@gmail.com
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Assembly
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# WasmPy
-Interacting with WebAssembly code from python.
-
-Wasmpy is a fairly lightweight layer that sits between Python and the WebAssembly code. When attempting to import a WebAssembly file, the file is read and it is converted into native machine code for native speeds.
-
-This project is intended to be used in conjunction with [wasmpy-build](https://github.com/olivi-r/wasmpy-build), although it does support regular WebAssembly files too.
-
-## Installing
-
-Install the latest version:
-
-```
-$ python -m pip install wasmpy
-```
-
-Or build and install from source (the `assemble` step requires having [NASM](https://www.nasm.us/) on path):
-
-
-```
-$ git clone https://github.com/olivi-r/wasmpy.git
-$ cd wasmpy
-$ python setup.py assemble
-$ python setup.py install
-```
-
-# Usage
-WasmPy defines import hooks to make the loading of WebAssembly binary files much easier! Just import the `WasmPy` library then you are good to go!
-### Example:
-If you have the following project setup:
-
-```
-|- my_wasm_file.wasm
-|- main.py
-```
-Then in `main.py` the following code will load the WebAssembly file:
-```py
-import wasmpy
-import my_wasm_file
-```
-The hook also allows importing the files from submodules, eg:
-```
-|- main.py
-|- my_module
-|  |- my_wasm_file.wasm
-```
-Then 
-```py
-import wasmpy
-from my_module import my_wasm_file
-```
-
-Functions can be called with the call function from the imported module:
-
-```py
-import wasmpy
-import wasm_math
-
-wasm_math.call("add")(...)
-```
-
-This is due to WebAssembly supporting exported names that may not be valid Python names, such as `add two numbers`
+Metadata-Version: 2.1
+Name: wasmpy
+Version: 0.1.3
+Summary: Interactions between WebAssembly and Python
+Home-page: https://github.com/olivi-r/wasmpy
+Author: Olivia Ryan
+Author-email: olivia.r.dev@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: WebAssembly
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Assembly
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![AppVeyor](https://img.shields.io/appveyor/build/olivi-r/wasmpy)](https://ci.appveyor.com/project/olivi-r/wasmpy)
+
+# wasmpy
+Interacting with WebAssembly code from python.
+
+Wasmpy is a fairly lightweight layer that sits between Python and the WebAssembly code. When attempting to import a WebAssembly file, the file is read and it is converted into native machine code for native speeds.
+
+This project is intended to be used in conjunction with [wasmpy-build](https://github.com/olivi-r/wasmpy-build), although it does support regular WebAssembly files too.
+
+## Installing
+
+Install the latest version:
+
+```
+python -m pip install wasmpy
+```
+
+Or build and install from source:
+
+
+```
+git clone https://github.com/olivi-r/wasmpy.git
+cd wasmpy
+python setup.py assemble
+python -m pip install .
+```
+
+# Usage
+WasmPy defines import hooks to make the loading of WebAssembly binary files much easier! Just import the `wasmpy` library then you are good to go!
+### Example:
+If you have the following project setup:
+
+```
+|- my_wasm_file.wasm
+|- main.py
+```
+Then in `main.py` the following code will load the WebAssembly file:
+```py
+import wasmpy
+import my_wasm_file
+```
+The hook also allows importing the files from submodules, eg:
+```
+|- main.py
+|- my_module
+|  |- my_wasm_file.wasm
+```
+Then 
+```py
+import wasmpy
+from my_module import my_wasm_file
+```
+
+Functions can be called with the call function from the imported module:
+
+```py
+import wasmpy
+import wasm_math
+
+wasm_math.call("add")(...)
+```
+
+This is due to WebAssembly supporting exported names that may not be valid Python names, such as `add two numbers`
```

