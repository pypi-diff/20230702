# Comparing `tmp/sweep-2.0.0.2-py3.10.egg` & `tmp/sweep-2.0.1.0-py3.10.egg`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 16087 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat     6446 b- defN 23-Jun-30 21:10 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      671 b- defN 23-Jun-30 21:10 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-30 21:10 EGG-INFO/dependency_links.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-30 20:02 EGG-INFO/not-zip-safe
--rw-rw-rw-  2.0 fat       32 b- defN 23-Jun-30 21:10 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-30 21:10 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat      316 b- defN 23-Jun-30 21:10 sweep/__init__.pyc
--rw-rw-rw-  2.0 fat      698 b- defN 23-Jun-30 21:10 sweep/calc_proj_mat_size.pyc
--rw-rw-rw-  2.0 fat     3244 b- defN 23-Jun-30 21:10 sweep/default_proj_mat_ope.pyc
--rw-rw-rw-  2.0 fat     5282 b- defN 23-Jun-30 21:10 sweep/fas2sweep.pyc
--rw-rw-rw-  2.0 fat      515 b- defN 23-Jun-30 21:10 sweep/fastaread.pyc
--rw-rw-rw-  2.0 fat      565 b- defN 23-Jun-30 21:10 sweep/is_orthonormal.pyc
--rw-rw-rw-  2.0 fat      662 b- defN 23-Jun-30 21:10 sweep/orthbase.pyc
--rw-rw-rw-  2.0 fat      350 b- defN 23-Jun-30 21:10 sweep/sweep_support/__init__.pyc
--rw-rw-rw-  2.0 fat      601 b- defN 23-Jun-30 21:10 sweep/sweep_support/aa2idx.pyc
--rw-rw-rw-  2.0 fat      807 b- defN 23-Jun-30 21:10 sweep/sweep_support/aa2int.pyc
--rw-rw-rw-  2.0 fat      578 b- defN 23-Jun-30 21:10 sweep/sweep_support/generate_chunk.pyc
--rw-rw-rw-  2.0 fat      301 b- defN 23-Jun-30 21:10 sweep/sweep_support/ij2inds.pyc
--rw-rw-rw-  2.0 fat      764 b- defN 23-Jun-30 21:10 sweep/sweep_support/mask2vec_bin.pyc
--rw-rw-rw-  2.0 fat      843 b- defN 23-Jun-30 21:10 sweep/sweep_support/mask2vec_count.pyc
--rw-rw-rw-  2.0 fat      762 b- defN 23-Jun-30 21:10 sweep/sweep_support/nt2int.pyc
--rw-rw-rw-  2.0 fat      451 b- defN 23-Jun-30 21:10 sweep/sweep_support/orth.pyc
--rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-30 21:10 sweep/sweep_support/seq2list.pyc
-23 files, 24380 bytes uncompressed, 13095 bytes compressed:  46.3%
+Zip file size: 16081 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat     6204 b- defN 23-Jul-02 02:14 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      671 b- defN 23-Jul-02 02:14 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-02 02:14 EGG-INFO/dependency_links.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-02 02:14 EGG-INFO/not-zip-safe
+-rw-rw-rw-  2.0 fat       32 b- defN 23-Jul-02 02:14 EGG-INFO/requires.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-02 02:14 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Jul-02 02:14 sweep/__init__.pyc
+-rw-rw-rw-  2.0 fat      698 b- defN 23-Jul-02 02:14 sweep/calc_proj_mat_size.pyc
+-rw-rw-rw-  2.0 fat     3244 b- defN 23-Jul-02 02:14 sweep/default_proj_mat_ope.pyc
+-rw-rw-rw-  2.0 fat     5282 b- defN 23-Jul-02 02:14 sweep/fas2sweep.pyc
+-rw-rw-rw-  2.0 fat      515 b- defN 23-Jul-02 02:14 sweep/fastaread.pyc
+-rw-rw-rw-  2.0 fat      565 b- defN 23-Jul-02 02:14 sweep/is_orthonormal.pyc
+-rw-rw-rw-  2.0 fat      662 b- defN 23-Jul-02 02:14 sweep/orthbase.pyc
+-rw-rw-rw-  2.0 fat      350 b- defN 23-Jul-02 02:14 sweep/sweep_support/__init__.pyc
+-rw-rw-rw-  2.0 fat      601 b- defN 23-Jul-02 02:14 sweep/sweep_support/aa2idx.pyc
+-rw-rw-rw-  2.0 fat      807 b- defN 23-Jul-02 02:14 sweep/sweep_support/aa2int.pyc
+-rw-rw-rw-  2.0 fat      578 b- defN 23-Jul-02 02:14 sweep/sweep_support/generate_chunk.pyc
+-rw-rw-rw-  2.0 fat      301 b- defN 23-Jul-02 02:14 sweep/sweep_support/ij2inds.pyc
+-rw-rw-rw-  2.0 fat      815 b- defN 23-Jul-02 02:14 sweep/sweep_support/mask2vec_bin.pyc
+-rw-rw-rw-  2.0 fat      894 b- defN 23-Jul-02 02:14 sweep/sweep_support/mask2vec_count.pyc
+-rw-rw-rw-  2.0 fat      762 b- defN 23-Jul-02 02:14 sweep/sweep_support/nt2int.pyc
+-rw-rw-rw-  2.0 fat      451 b- defN 23-Jul-02 02:14 sweep/sweep_support/orth.pyc
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Jul-02 02:14 sweep/sweep_support/seq2list.pyc
+23 files, 24240 bytes uncompressed, 13089 bytes compressed:  46.0%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweep
-Version: 2.0.0.2
+Version: 2.0.1.0
 Summary: SWeeP is a tool for representing large biological sequences datasets in compact vectors
 Home-page: https://github.com/diogomachado-bioinfo/sweep
 Author: Diogo de J. S. Machado
 Author-email: diogomachado.bioinfo@gmail.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 
@@ -82,27 +82,26 @@
 
 | Function                            | Description                                                                      | Input                                                          | Output                                          |
 |-------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------|-------------------------------------------------|
 | ``fastaread``                       | Reads a FASTA file and returns a list of sequence records                        | ``fastaname`` (str): Path to the FASTA file                    | ``records`` (list): List of sequence records    |
 | ``fas2sweep``                       | Converts a list of sequences into SWeeP vectors                                  | ``fasta`` (list): List of sequence records                     | ``vect`` (numpy.ndarray): SWeeP vectors         |
 | ``orthbase``                        | Generates an orthonormal projection matrix of the specified size                 | ``lin`` (int): Number of rows                                  | ``mret`` (numpy.ndarray): Orthonormal matrix    |
 | ``calc_proj_mat_size``              | Calculates the number of lines in the projection matrix for a given mask         | ``mask`` (list): Mask specifying dimensions                    | ``lines`` (int): Number of lines in the matrix  |
-| ``md5``                             | Calculates the MD5 hash of a file                                                | ``fname`` (str): Path to the file                              | ``hash_md5`` (str): MD5 hash of the file        |
 | ``down_proj_mat``                   | Downloads the default projection matrix file                                     | ``destination`` (str): Path to the destination file (optional) | None                                            |
 | ``return_proj_mat_not_found_error`` | Raises an exception indicating that the default projection matrix is not found   | None                                                           | None                                            |
 | ``check_default_proj_mat``          | Checks if the default projection matrix exists and matches the expected MD5 hash | ``file`` (str): Path to the projection matrix file             | None                                            |
 | ``get_default_proj_mat``            | Retrieves the default projection matrix                                          | None                                                           | ``orth_mat`` (numpy.ndarray): Projection matrix |
 
 ## Article Reference
 
 If you use the SWeeP algorithm or this Python package in your research work, please cite the
 following article:
 
 ```
-@article{De Pierri2020,
+@article{Pierri2020,
   title={SWeeP: representing large biological sequences datasets in compact vectors},
   author={De Pierri, Camilla Reginatto and Voyceik, Ricardo and Santos de Mattos, LetÃ­cia Graziela Costa and Kulik, Mariane GonÃ§alves and Camargo, JosuÃ© Oliveira and Repula de Oliveira, Aryel Marlus and de Lima Nichio, Bruno Thiago and Marchaukoski, Jeroniza Nunes and da Silva Filho, Antonio Camilo and Guizelini, Dieval and Ortega, J. Miguel and Pedrosa, Fabio O. and Raittz, Roberto Tadeu},
   journal={Scientific Reports},
   volume={10},
   number={1},
   pages={91},
   year={2020},
```

## sweep/__init__.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 20:09:36 2023 UTC, .py size: 252 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8036 9f64 fc00 0000  o........6.d....
+00000000: 6f0d 0d0a 0000 0000 4103 a164 ff00 0000  o.......A..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6401 6c03 5400 6400  d.l.T.d.d.l.T.d.
 00000050: 6401 6c04 5400 6400 6401 6c05 5400 6400  d.l.T.d.d.l.T.d.
 00000060: 6401 6c06 5400 6402 5300 2903 e901 0000  d.l.T.d.S.).....
 00000070: 0029 01da 012a 4e29 075a 0d73 7765 6570  .)...*N).Z.sweep
@@ -12,9 +12,9 @@
 000000b0: 6173 655a 0966 6173 7461 7265 6164 5a0e  aseZ.fastareadZ.
 000000c0: 6973 5f6f 7274 686f 6e6f 726d 616c 5a12  is_orthonormalZ.
 000000d0: 6361 6c63 5f70 726f 6a5f 6d61 745f 7369  calc_proj_mat_si
 000000e0: 7a65 a900 7203 0000 0072 0300 0000 fa2b  ze..r....r.....+
 000000f0: 6275 696c 645c 6264 6973 742e 7769 6e2d  build\bdist.win-
 00000100: 616d 6436 345c 6567 675c 7377 6565 705c  amd64\egg\sweep\
 00000110: 5f5f 696e 6974 5f5f 2e70 79da 083c 6d6f  __init__.py..<mo
-00000120: 6475 6c65 3e01 0000 0073 0e00 0000 0802  dule>....s......
+00000120: 6475 6c65 3e01 0000 0073 0e00 0000 0803  dule>....s......
 00000130: 0801 0801 0801 0801 0801 0c01            ............
```

## sweep/calc_proj_mat_size.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 20:43:35 2023 UTC, .py size: 564 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 773e 9f64 3402 0000  o.......w>.d4...
+00000000: 6f0d 0d0a 0000 0000 4403 a164 6302 0000  o.......D..dc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 0e00 0000 6404  .....@...s....d.
 00000030: 6401 6402 8401 5a00 6403 5300 2905 da02  d.d...Z.d.S.)...
 00000040: 4141 6302 0000 0000 0000 0000 0000 0004  AAc.............
 00000050: 0000 0004 0000 0043 0000 0073 4000 0000  .......C...s@...
 00000060: 7c01 6401 6b02 7207 6402 7d02 6e0b 7c01  |.d.k.r.d.}.n.|.
 00000070: 6403 6b02 720e 6404 7d02 6e04 7400 6405  d.k.r.d.}.n.t.d.
@@ -32,13 +32,13 @@
 000001f0: 6545 7272 6f72 2904 da04 6d61 736b 5a0a  eError)...maskZ.
 00000200: 6661 7374 615f 7479 7065 da01 78da 056c  fasta_type..x..l
 00000210: 696e 6573 a900 720a 0000 00fa 3562 7569  ines..r.....5bui
 00000220: 6c64 5c62 6469 7374 2e77 696e 2d61 6d64  ld\bdist.win-amd
 00000230: 3634 5c65 6767 5c73 7765 6570 5c63 616c  64\egg\sweep\cal
 00000240: 635f 7072 6f6a 5f6d 6174 5f73 697a 652e  c_proj_mat_size.
 00000250: 7079 da12 6361 6c63 5f70 726f 6a5f 6d61  py..calc_proj_ma
-00000260: 745f 7369 7a65 0100 0000 730e 0000 0008  t_size....s.....
+00000260: 745f 7369 7a65 0400 0000 730e 0000 0008  t_size....s.....
 00000270: 0c06 0108 0106 0108 0218 0204 0172 0c00  .............r..
 00000280: 0000 4e29 0172 0100 0000 2901 720c 0000  ..N).r....).r...
 00000290: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
 000002a0: 720b 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000002b0: 0000 0073 0200 0000 0e00                 ...s......
+000002b0: 0000 0073 0200 0000 0e03                 ...s......
```

## sweep/default_proj_mat_ope.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 22:27:17 2023 UTC, .py size: 3278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c556 9f64 ce0c 0000  o........V.d....
+00000000: 6f0d 0d0a 0000 0000 5303 a164 cf0c 0000  o.......S..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 8400 5a05 640c  d.l.Z.d.d...Z.d.
 00000060: 6404 6405 8401 5a06 6406 6407 8400 5a07  d.d...Z.d.d...Z.
 00000070: 6408 6409 8400 5a08 640a 640b 8400 5a09  d.d...Z.d.d...Z.
```

## sweep/fas2sweep.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 23:00:54 2023 UTC, .py size: 6492 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a65e 9f64 5c19 0000  o........^.d\...
+00000000: 6f0d 0d0a 0000 0000 5503 a164 5d19 0000  o.......U..d]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6404  ..d.d.l.m.Z...d.
 00000060: 6405 6c09 5a09 6404 6405 6c0a 5a0a 6404  d.l.Z.d.d.l.Z.d.
 00000070: 6405 6c0b 5a0b 6404 6405 6c0c 5a0d 6404  d.l.Z.d.d.l.Z.d.
```

## sweep/fastaread.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 20:42:58 2023 UTC, .py size: 378 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 523e 9f64 7a01 0000  o.......R>.dz...
+00000000: 6f0d 0d0a 0000 0000 5803 a164 7b01 0000  o.......X..d{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 8400  d.l.m.Z...d.d...
 00000040: 5a02 6404 5300 2905 e900 0000 0029 01da  Z.d.S.)......)..
 00000050: 0553 6571 494f 6301 0000 0000 0000 0000  .SeqIOc.........
 00000060: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
 00000070: 1400 0000 7400 7401 a002 7c00 6401 a102  ....t.t...|.d...
```

## sweep/is_orthonormal.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  1 15:18:50 2023 UTC, .py size: 637 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5ad8 4f64 7d02 0000  o.......Z.Od}...
+00000000: 6f0d 0d0a 0000 0000 5b03 a164 9302 0000  o.......[..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
 00000040: 5300 2904 e900 0000 004e 6301 0000 0000  S.)......Nc.....
 00000050: 0000 0000 0000 0009 0000 0008 0000 0043  ...............C
 00000060: 0000 0073 a800 0000 7c00 6a00 5c02 7d01  ...s....|.j.\.}.
 00000070: 7d02 7401 7c02 8301 4400 5d1b 7d03 7c00  }.t.|...D.].}.|.
@@ -22,15 +22,15 @@
 00000150: 095a 066d 6174 7269 78da 016d da01 6eda  .Z.matrix..m..n.
 00000160: 016a da03 636f 6c72 0600 0000 da02 6a31  .j..colr......j1
 00000170: da02 6a32 5a0b 646f 745f 7072 6f64 7563  ..j2Z.dot_produc
 00000180: 74a9 0072 0f00 0000 fa31 6275 696c 645c  t..r.....1build\
 00000190: 6264 6973 742e 7769 6e2d 616d 6436 345c  bdist.win-amd64\
 000001a0: 6567 675c 7377 6565 705c 6973 5f6f 7274  egg\sweep\is_ort
 000001b0: 686f 6e6f 726d 616c 2e70 79da 0e69 735f  honormal.py..is_
-000001c0: 6f72 7468 6f6e 6f72 6d61 6c04 0000 0073  orthonormal....s
+000001c0: 6f72 7468 6f6e 6f72 6d61 6c06 0000 0073  orthonormal....s
 000001d0: 1e00 0000 0a02 0c03 1001 0c01 1001 0601  ................
 000001e0: 02ff 0c04 1201 2401 0c01 0801 02ff 02fe  ......$.........
 000001f0: 0406 7211 0000 0029 03da 056e 756d 7079  ..r....)...numpy
 00000200: 7205 0000 0072 1100 0000 720f 0000 0072  r....r....r....r
 00000210: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
 00000220: 3c6d 6f64 756c 653e 0100 0000 7304 0000  <module>....s...
-00000230: 0008 010c 02                             .....
+00000230: 0008 030c 02                             .....
```

## sweep/orthbase.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 20:41:58 2023 UTC, .py size: 546 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 163e 9f64 2202 0000  o........>.d"...
+00000000: 6f0d 0d0a 0000 0000 6503 a164 2302 0000  o.......e..d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6404 6405 8400 5a04 6403 5300 2906  Z.d.d...Z.d.S.).
 00000050: e901 0000 0029 01da 046f 7274 68e9 0000  .....)...orth...
 00000060: 0000 4e63 0200 0000 0000 0000 0000 0000  ..Nc............
 00000070: 0400 0000 0600 0000 4300 0000 7350 0000  ........C...sP..
```

## sweep/sweep_support/__init__.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 30 20:09:39 2023 UTC, .py size: 303 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8336 9f64 2f01 0000  o........6.d/...
+00000000: 6f0d 0d0a 0000 0000 7203 a164 3201 0000  o.......r..d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6401 6c03 5400 6400  d.l.T.d.d.l.T.d.
 00000050: 6401 6c04 5400 6400 6401 6c05 5400 6400  d.l.T.d.d.l.T.d.
 00000060: 6401 6c06 5400 6400 6401 6c07 5400 6400  d.l.T.d.d.l.T.d.
 00000070: 6401 6c04 5400 6400 6401 6c08 5400 6402  d.l.T.d.d.l.T.d.
@@ -14,9 +14,9 @@
 000000d0: 736b 3276 6563 5f62 696e 5a0e 6d61 736b  sk2vec_binZ.mask
 000000e0: 3276 6563 5f63 6f75 6e74 5a04 6f72 7468  2vec_countZ.orth
 000000f0: a900 7203 0000 0072 0300 0000 fa39 6275  ..r....r.....9bu
 00000100: 696c 645c 6264 6973 742e 7769 6e2d 616d  ild\bdist.win-am
 00000110: 6436 345c 6567 675c 7377 6565 705c 7377  d64\egg\sweep\sw
 00000120: 6565 705f 7375 7070 6f72 745c 5f5f 696e  eep_support\__in
 00000130: 6974 5f5f 2e70 79da 083c 6d6f 6475 6c65  it__.py..<module
-00000140: 3e01 0000 0073 1400 0000 0802 0801 0801  >....s..........
+00000140: 3e01 0000 0073 1400 0000 0803 0801 0801  >....s..........
 00000150: 0801 0801 0801 0801 0801 0801 0c01       ..............
```

## sweep/sweep_support/aa2idx.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 01:10:27 2023 UTC, .py size: 443 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 03c0 4d64 bb01 0000  o.........Md....
+00000000: 6f0d 0d0a 0000 0000 7b03 a164 c001 0000  o.......{..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d01 5a01 0100 6403 6404 6c02 5a03 6405  m.Z...d.d.l.Z.d.
 00000050: 6406 8400 5a04 6404 5300 2907 e901 0000  d...Z.d.S.).....
 00000060: 0029 01da 0661 6132 696e 7429 01da 066e  .)...aa2int)...n
 00000070: 7432 696e 74e9 0000 0000 4e63 0200 0000  t2int.....Nc....
@@ -24,15 +24,15 @@
 00000170: 0572 616e 6765 da03 7375 6d29 085a 0478  .range..sum).Z.x
 00000180: 7365 715a 0764 6566 5369 7a65 da01 6eda  seqZ.defSize..n.
 00000190: 016d 5a03 766c 735a 0370 6f74 da01 745a  .mZ.vlsZ.pot..tZ
 000001a0: 046d 7265 74a9 0072 1000 0000 fa37 6275  .mret..r.....7bu
 000001b0: 696c 645c 6264 6973 742e 7769 6e2d 616d  ild\bdist.win-am
 000001c0: 6436 345c 6567 675c 7377 6565 705c 7377  d64\egg\sweep\sw
 000001d0: 6565 705f 7375 7070 6f72 745c 6161 3269  eep_support\aa2i
-000001e0: 6478 2e70 79da 0661 6132 6964 7806 0000  dx.py..aa2idx...
+000001e0: 6478 2e70 79da 0661 6132 6964 7808 0000  dx.py..aa2idx...
 000001f0: 0073 1200 0000 1001 0801 1601 0801 1401  .s..............
 00000200: 1801 1001 1a01 0401 7212 0000 0029 0572  ........r....).r
 00000210: 0200 0000 7203 0000 00da 056e 756d 7079  ....r......numpy
 00000220: 7207 0000 0072 1200 0000 7210 0000 0072  r....r....r....r
 00000230: 1000 0000 7210 0000 0072 1100 0000 da08  ....r....r......
 00000240: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-00000250: 000c 020c 0108 010c 01                   .........
+00000250: 000c 030c 0108 010c 02                   .........
```

## sweep/sweep_support/aa2int.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 00:25:49 2023 UTC, .py size: 825 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8db5 4d64 3903 0000  o.........Md9...
+00000000: 6f0d 0d0a 0000 0000 8803 a164 3e03 0000  o..........d>...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
 00000040: 5300 2904 e900 0000 004e 6301 0000 0000  S.)......Nc.....
 00000050: 0000 0000 0000 0003 0000 000e 0000 0043  ...............C
 00000060: 0000 0073 ac00 0000 6900 6401 6402 9301  ...s....i.d.d...
 00000070: 6403 6404 9301 6405 6406 9301 6407 6408  d.d...d.d...d.d.
@@ -33,19 +33,19 @@
 00000200: 6c6f 7765 725a 0976 6563 746f 7269 7a65  lowerZ.vectorize
 00000210: da03 6765 7429 035a 0761 615f 6c69 7374  ..get).Z.aa_list
 00000220: da03 6d61 705a 086d 6170 5f66 756e 63a9  ..mapZ.map_func.
 00000230: 0072 3d00 0000 fa37 6275 696c 645c 6264  .r=....7build\bd
 00000240: 6973 742e 7769 6e2d 616d 6436 345c 6567  ist.win-amd64\eg
 00000250: 675c 7377 6565 705c 7377 6565 705f 7375  g\sweep\sweep_su
 00000260: 7070 6f72 745c 6161 3269 6e74 2e70 79da  pport\aa2int.py.
-00000270: 0661 6132 696e 7404 0000 0073 6400 0000  .aa2int....sd...
+00000270: 0661 6132 696e 7406 0000 0073 6400 0000  .aa2int....sd...
 00000280: 0801 0401 02ff 0402 02fe 0403 02fd 0404  ................
 00000290: 02fc 0405 02fb 0406 02fa 0407 02f9 0408  ................
 000002a0: 02f8 0409 02f7 040a 02f6 040b 02f5 040c  ................
 000002b0: 02f4 040d 02f3 040e 02f2 040f 02f1 0410  ................
 000002c0: 02f0 0211 0201 0201 0201 0201 0201 0201  ................
 000002d0: 0201 0201 0201 0201 0201 08e4 0c1e 0c01  ................
 000002e0: 0801 0401 723f 0000 0029 03da 056e 756d  ....r?...)...num
 000002f0: 7079 7238 0000 0072 3f00 0000 723d 0000  pyr8...r?...r=..
 00000300: 0072 3d00 0000 723d 0000 0072 3e00 0000  .r=...r=...r>...
 00000310: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
-00000320: 0000 0008 020c 01                        .......
+00000320: 0000 0008 030c 02                        .......
```

## sweep/sweep_support/generate_chunk.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 00:57:52 2023 UTC, .py size: 438 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 10bd 4d64 b601 0000  o.........Md....
+00000000: 6f0d 0d0a 0000 0000 8f03 a164 bb01 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a03 6401 5300 2904 e900 0000  d...Z.d.S.).....
 00000050: 004e 6302 0000 0000 0000 0000 0000 0004  .Nc.............
 00000060: 0000 0009 0000 0043 0000 0073 7800 0000  .......C...sx...
 00000070: 7400 a001 7c01 7c00 1b00 a101 7d02 7402  t...|.|.....}.t.
@@ -23,15 +23,15 @@
 00000160: 6b73 5a08 6669 6c65 5f6c 656e da0a 6368  ksZ.file_len..ch
 00000170: 756e 6b5f 7369 7a65 5a0d 6368 756e 6b5f  unk_sizeZ.chunk_
 00000180: 696e 6469 6365 73a9 0072 0e00 0000 fa3f  indices..r.....?
 00000190: 6275 696c 645c 6264 6973 742e 7769 6e2d  build\bdist.win-
 000001a0: 616d 6436 345c 6567 675c 7377 6565 705c  amd64\egg\sweep\
 000001b0: 7377 6565 705f 7375 7070 6f72 745c 6765  sweep_support\ge
 000001c0: 6e65 7261 7465 5f63 6875 6e6b 2e70 79da  nerate_chunk.py.
-000001d0: 0e67 656e 6572 6174 655f 6368 756e 6b05  .generate_chunk.
+000001d0: 0e67 656e 6572 6174 655f 6368 756e 6b07  .generate_chunk.
 000001e0: 0000 0073 1000 0000 0e01 0e01 2601 02ff  ...s........&...
 000001f0: 2402 04fe 0803 0401 7210 0000 0029 0472  $.......r....).r
 00000200: 0500 0000 da05 6e75 6d70 7972 0700 0000  ......numpyr....
 00000210: 7210 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
 00000220: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
-00000230: 6c65 3e01 0000 0073 0600 0000 0802 0801  le>....s........
-00000240: 0c01                                     ..
+00000230: 6c65 3e01 0000 0073 0600 0000 0803 0801  le>....s........
+00000240: 0c02                                     ..
```

## sweep/sweep_support/ij2inds.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 22 02:38:19 2022 UTC, .py size: 118 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,19 +1,19 @@
-00000000: 6f0d 0d0a 0000 0000 9b36 3962 7600 0000  o........69bv...
+00000000: 6f0d 0d0a 0000 0000 9203 a164 7900 0000  o..........dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 6401 8400 5a00 6402 5300 2903 6302 0000  d...Z.d.S.).c...
 00000040: 0000 0000 0000 0000 0002 0000 0004 0000  ................
 00000050: 0043 0000 0073 2800 0000 7c00 6400 6400  .C...s(...|.d.d.
 00000060: 8502 6401 6602 1900 6401 1800 7c01 1400  ..d.f...d...|...
 00000070: 7c00 6400 6400 8502 6402 6602 1900 1700  |.d.d...d.f.....
 00000080: 5300 2903 4ee9 0100 0000 e900 0000 00a9  S.).N...........
 00000090: 0029 025a 0369 6a73 5a05 746d 636f 6c72  .).Z.ijsZ.tmcolr
 000000a0: 0300 0000 7203 0000 00fa 3862 7569 6c64  ....r.....8build
 000000b0: 5c62 6469 7374 2e77 696e 2d61 6d64 3634  \bdist.win-amd64
 000000c0: 5c65 6767 5c73 7765 6570 5c73 7765 6570  \egg\sweep\sweep
 000000d0: 5f73 7570 706f 7274 5c69 6a32 696e 6473  _support\ij2inds
-000000e0: 2e70 79da 0769 6a32 696e 6473 0300 0000  .py..ij2inds....
+000000e0: 2e70 79da 0769 6a32 696e 6473 0400 0000  .py..ij2inds....
 000000f0: 7302 0000 0028 0172 0500 0000 4e29 0172  s....(.r....N).r
 00000100: 0500 0000 7203 0000 0072 0300 0000 7203  ....r....r....r.
 00000110: 0000 0072 0400 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000120: 653e 0100 0000 7302 0000 000c 02         e>....s......
+00000120: 653e 0100 0000 7302 0000 000c 03         e>....s......
```

## sweep/sweep_support/mask2vec_bin.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 29 20:21:03 2023 UTC, .py size: 677 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,48 +1,51 @@
-00000000: 6f0d 0d0a 0000 0000 afe7 9d64 a502 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 9903 a164 aa02 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d01 5a01 0100 6400 6403 6c02 6d02 5a02  m.Z...d.d.l.m.Z.
 00000050: 0100 6404 6405 6c03 5a04 6700 6406 a201  ..d.d.l.Z.g.d...
 00000060: 6407 6602 6408 6409 8401 5a05 6405 5300  d.f.d.d...Z.d.S.
 00000070: 290a e901 0000 0029 01da 0873 6571 326c  )......)...seq2l
 00000080: 6973 7429 01da 0661 6132 6964 7829 01da  ist)...aa2idx)..
 00000090: 0769 6a32 696e 6473 e900 0000 004e 2903  .ij2inds.....N).
 000000a0: e902 0000 0072 0100 0000 7206 0000 00e9  .....r....r.....
 000000b0: 1400 0000 6303 0000 0000 0000 0000 0000  ....c...........
-000000c0: 000a 0000 0009 0000 0043 0000 0073 c800  .........C...s..
+000000c0: 000b 0000 0009 0000 0043 0000 0073 ec00  .........C...s..
 000000d0: 0000 7c01 6401 1900 7c01 6402 1900 1700  ..|.d...|.d.....
 000000e0: 7c01 6403 1900 1700 7d03 7400 7c00 7401  |.d.....}.t.|.t.
 000000f0: 7c03 8301 8302 7d04 7402 a003 7404 7c04  |.....}.t...t.|.
 00000100: 6400 6400 8502 6401 7c01 6401 1900 8502  d.d...d.|.d.....
 00000110: 6602 1900 7c02 8302 7404 7c04 6400 6400  f...|...t.|.d.d.
 00000120: 8502 7c03 7c01 6403 1900 1800 7c03 8502  ..|.|.d.....|...
 00000130: 6602 1900 7c02 8302 6702 a101 6a05 7d05  f...|...g...j.}.
 00000140: 7402 6a06 7c05 6401 6404 8d02 7d05 7c02  t.j.|.d.d...}.|.
 00000150: 7c01 6401 1900 1300 7d06 7407 7c05 7c06  |.d.....}.t.|.|.
 00000160: 8302 7d07 7c02 7c01 6403 1900 1300 7d08  ..}.|.|.d.....}.
 00000170: 7402 6a08 6402 7c06 7c08 1400 6602 7401  t.j.d.|.|...f.t.
-00000180: 6405 8d02 7d09 6402 7c09 6401 7c07 6402  d...}.d.|.d.|.d.
-00000190: 1800 6602 3c00 7c09 5300 2906 4e72 0500  ..f.<.|.S.).Nr..
-000001a0: 0000 7201 0000 0072 0600 0000 2901 5a04  ..r....r....).Z.
-000001b0: 6178 6973 2901 5a05 6474 7970 6529 0972  axis).Z.dtype).r
-000001c0: 0200 0000 da03 696e 74da 026e 70da 0561  ......int..np..a
-000001d0: 7272 6179 7203 0000 00da 0154 da06 756e  rrayr......T..un
-000001e0: 6971 7565 7204 0000 005a 057a 6572 6f73  iquer....Z.zeros
-000001f0: 290a 5a04 7873 6571 da04 6d61 736b 5a07  ).Z.xseq..maskZ.
-00000200: 6465 6653 697a 65da 0174 da05 736c 6963  defSize..t..slic
-00000210: 655a 0278 79da 056c 696e 6573 5a04 696e  eZ.xy..linesZ.in
-00000220: 6473 da04 636f 6c73 da01 4da9 0072 1300  ds..cols..M..r..
-00000230: 0000 fa3d 6275 696c 645c 6264 6973 742e  ...=build\bdist.
-00000240: 7769 6e2d 616d 6436 345c 6567 675c 7377  win-amd64\egg\sw
-00000250: 6565 705c 7377 6565 705f 7375 7070 6f72  eep\sweep_suppor
-00000260: 745c 6d61 736b 3276 6563 5f62 696e 2e70  t\mask2vec_bin.p
-00000270: 79da 0c6d 6173 6b32 7665 635f 6269 6e07  y..mask2vec_bin.
-00000280: 0000 0073 1c00 0000 1801 0e01 2001 2001  ...s........ . .
-00000290: 04ff 0201 02ff 0e02 0c01 0a01 0c01 1601  ................
-000002a0: 1003 0401 7215 0000 0029 0672 0200 0000  ....r....).r....
-000002b0: 7203 0000 0072 0400 0000 da05 6e75 6d70  r....r......nump
-000002c0: 7972 0900 0000 7215 0000 0072 1300 0000  yr....r....r....
-000002d0: 7213 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
-000002e0: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
-000002f0: 0000 0c02 0c01 0c01 0801 1601            ............
+00000180: 6405 8d02 7d09 7c02 7c01 6401 1900 1300  d...}.|.|.d.....
+00000190: 7c02 7c01 6403 1900 1300 1400 7d0a 7c07  |.|.d.......}.|.
+000001a0: 7c07 7c0a 6b01 1900 7d07 6402 7c09 6401  |.|.k...}.d.|.d.
+000001b0: 7c07 6402 1800 6602 3c00 7c09 5300 2906  |.d...f.<.|.S.).
+000001c0: 4e72 0500 0000 7201 0000 0072 0600 0000  Nr....r....r....
+000001d0: 2901 5a04 6178 6973 2901 5a05 6474 7970  ).Z.axis).Z.dtyp
+000001e0: 6529 0972 0200 0000 da03 696e 74da 026e  e).r......int..n
+000001f0: 70da 0561 7272 6179 7203 0000 00da 0154  p..arrayr......T
+00000200: da06 756e 6971 7565 7204 0000 005a 057a  ..uniquer....Z.z
+00000210: 6572 6f73 290b 5a04 7873 6571 da04 6d61  eros).Z.xseq..ma
+00000220: 736b 5a07 6465 6653 697a 65da 0174 da05  skZ.defSize..t..
+00000230: 736c 6963 655a 0278 79da 056c 696e 6573  sliceZ.xy..lines
+00000240: 5a04 696e 6473 da04 636f 6c73 da01 4d5a  Z.inds..cols..MZ
+00000250: 0972 6f77 735f 7369 7a65 a900 7213 0000  .rows_size..r...
+00000260: 00fa 3d62 7569 6c64 5c62 6469 7374 2e77  ..=build\bdist.w
+00000270: 696e 2d61 6d64 3634 5c65 6767 5c73 7765  in-amd64\egg\swe
+00000280: 6570 5c73 7765 6570 5f73 7570 706f 7274  ep\sweep_support
+00000290: 5c6d 6173 6b32 7665 635f 6269 6e2e 7079  \mask2vec_bin.py
+000002a0: da0c 6d61 736b 3276 6563 5f62 696e 0900  ..mask2vec_bin..
+000002b0: 0000 7320 0000 0018 010e 0120 0120 0104  ..s ....... . ..
+000002c0: ff02 0102 ff0e 020c 010a 010c 0116 0118  ................
+000002d0: 010c 0110 0104 0172 1500 0000 2906 7202  .......r....).r.
+000002e0: 0000 0072 0300 0000 7204 0000 00da 056e  ...r....r......n
+000002f0: 756d 7079 7209 0000 0072 1500 0000 7213  umpyr....r....r.
+00000300: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
+00000310: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000320: 730a 0000 000c 030c 010c 0108 0116 02    s..............
```

## sweep/sweep_support/mask2vec_count.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 29 20:21:00 2023 UTC, .py size: 867 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,53 +1,56 @@
-00000000: 6f0d 0d0a 0000 0000 ace7 9d64 6303 0000  o..........dc...
+00000000: 6f0d 0d0a 0000 0000 9f03 a164 6803 0000  o..........dh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d01 5a01 0100 6400 6403 6c02 6d02 5a02  m.Z...d.d.l.m.Z.
 00000050: 0100 6404 6405 6c03 5a04 6700 6406 a201  ..d.d.l.Z.g.d...
 00000060: 6407 6602 6408 6409 8401 5a05 6405 5300  d.f.d.d...Z.d.S.
 00000070: 290a e901 0000 0029 01da 0873 6571 326c  )......)...seq2l
 00000080: 6973 7429 01da 0661 6132 6964 7829 01da  ist)...aa2idx)..
 00000090: 0769 6a32 696e 6473 e900 0000 004e 2903  .ij2inds.....N).
 000000a0: e902 0000 0072 0100 0000 7206 0000 00e9  .....r....r.....
 000000b0: 1400 0000 6303 0000 0000 0000 0000 0000  ....c...........
-000000c0: 000b 0000 0009 0000 0043 0000 0073 d200  .........C...s..
+000000c0: 000c 0000 0009 0000 0043 0000 0073 f600  .........C...s..
 000000d0: 0000 7c01 6401 1900 7c01 6402 1900 1700  ..|.d...|.d.....
 000000e0: 7c01 6403 1900 1700 7d03 7400 7c00 7401  |.d.....}.t.|.t.
 000000f0: 7c03 8301 8302 7d04 7402 a003 7404 7c04  |.....}.t...t.|.
 00000100: 6400 6400 8502 6401 7c01 6401 1900 8502  d.d...d.|.d.....
 00000110: 6602 1900 7c02 8302 7404 7c04 6400 6400  f...|...t.|.d.d.
 00000120: 8502 7c03 7c01 6403 1900 1800 7c03 8502  ..|.|.d.....|...
 00000130: 6602 1900 7c02 8302 6702 a101 6a05 7d05  f...|...g...j.}.
 00000140: 7c02 7c01 6401 1900 1300 7d06 7406 7c05  |.|.d.....}.t.|.
 00000150: 7c06 8302 7d07 7c02 7c01 6403 1900 1300  |...}.|.|.d.....
 00000160: 7d08 7402 6a07 6402 7c06 7c08 1400 6602  }.t.j.d.|.|...f.
-00000170: 7401 6404 8d02 7d09 7402 6a08 7c07 6405  t.d...}.t.j.|.d.
-00000180: 6405 6406 6400 6407 8d05 5c02 7d07 7d0a  d.d.d.d...\.}.}.
-00000190: 7c0a 7c09 6401 7c07 6402 1800 6602 3c00  |.|.d.|.d...f.<.
-000001a0: 7c09 5300 2908 4e72 0500 0000 7201 0000  |.S.).Nr....r...
-000001b0: 0072 0600 0000 2901 5a05 6474 7970 6546  .r....).Z.dtypeF
-000001c0: 5429 045a 0c72 6574 7572 6e5f 696e 6465  T).Z.return_inde
-000001d0: 785a 0e72 6574 7572 6e5f 696e 7665 7273  xZ.return_invers
-000001e0: 655a 0d72 6574 7572 6e5f 636f 756e 7473  eZ.return_counts
-000001f0: 5a04 6178 6973 2909 7202 0000 00da 0369  Z.axis).r......i
-00000200: 6e74 da02 6e70 da05 6172 7261 7972 0300  nt..np..arrayr..
-00000210: 0000 da01 5472 0400 0000 5a05 7a65 726f  ....Tr....Z.zero
-00000220: 73da 0675 6e69 7175 6529 0b5a 0478 7365  s..unique).Z.xse
-00000230: 71da 046d 6173 6b5a 0764 6566 5369 7a65  q..maskZ.defSize
-00000240: da01 74da 0573 6c69 6365 5a02 7879 da05  ..t..sliceZ.xy..
-00000250: 6c69 6e65 735a 0469 6e64 73da 0463 6f6c  linesZ.inds..col
-00000260: 73da 014d da06 636f 756e 7473 a900 7214  s..M..counts..r.
-00000270: 0000 00fa 3f62 7569 6c64 5c62 6469 7374  ....?build\bdist
-00000280: 2e77 696e 2d61 6d64 3634 5c65 6767 5c73  .win-amd64\egg\s
-00000290: 7765 6570 5c73 7765 6570 5f73 7570 706f  weep\sweep_suppo
-000002a0: 7274 5c6d 6173 6b32 7665 635f 636f 756e  rt\mask2vec_coun
-000002b0: 742e 7079 da0e 6d61 736b 3276 6563 5f63  t.py..mask2vec_c
-000002c0: 6f75 6e74 0700 0000 7326 0000 0018 010e  ount....s&......
-000002d0: 0120 0120 0104 ff02 0102 ff0c 020a 010c  . . ............
-000002e0: 0116 0106 0302 0102 0102 0102 010a fc10  ................
-000002f0: 0504 0172 1600 0000 2906 7202 0000 0072  ...r....).r....r
-00000300: 0300 0000 7204 0000 00da 056e 756d 7079  ....r......numpy
-00000310: 7209 0000 0072 1600 0000 7214 0000 0072  r....r....r....r
-00000320: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
-00000330: 3c6d 6f64 756c 653e 0100 0000 730a 0000  <module>....s...
-00000340: 000c 020c 010c 0108 0116 01              ...........
+00000170: 7401 6404 8d02 7d09 7c02 7c01 6401 1900  t.d...}.|.|.d...
+00000180: 1300 7c02 7c01 6403 1900 1300 1400 7d0a  ..|.|.d.......}.
+00000190: 7c07 7c07 7c0a 6b01 1900 7d07 7402 6a08  |.|.|.k...}.t.j.
+000001a0: 7c07 6405 6405 6406 6400 6407 8d05 5c02  |.d.d.d.d.d...\.
+000001b0: 7d07 7d0b 7c0b 7c09 6401 7c07 6402 1800  }.}.|.|.d.|.d...
+000001c0: 6602 3c00 7c09 5300 2908 4e72 0500 0000  f.<.|.S.).Nr....
+000001d0: 7201 0000 0072 0600 0000 2901 5a05 6474  r....r....).Z.dt
+000001e0: 7970 6546 5429 045a 0c72 6574 7572 6e5f  ypeFT).Z.return_
+000001f0: 696e 6465 785a 0e72 6574 7572 6e5f 696e  indexZ.return_in
+00000200: 7665 7273 655a 0d72 6574 7572 6e5f 636f  verseZ.return_co
+00000210: 756e 7473 5a04 6178 6973 2909 7202 0000  untsZ.axis).r...
+00000220: 00da 0369 6e74 da02 6e70 da05 6172 7261  ...int..np..arra
+00000230: 7972 0300 0000 da01 5472 0400 0000 5a05  yr......Tr....Z.
+00000240: 7a65 726f 73da 0675 6e69 7175 6529 0c5a  zeros..unique).Z
+00000250: 0478 7365 71da 046d 6173 6b5a 0764 6566  .xseq..maskZ.def
+00000260: 5369 7a65 da01 74da 0573 6c69 6365 5a02  Size..t..sliceZ.
+00000270: 7879 da05 6c69 6e65 735a 0469 6e64 73da  xy..linesZ.inds.
+00000280: 0463 6f6c 73da 014d 5a09 726f 7773 5f73  .cols..MZ.rows_s
+00000290: 697a 65da 0663 6f75 6e74 73a9 0072 1400  ize..counts..r..
+000002a0: 0000 fa3f 6275 696c 645c 6264 6973 742e  ...?build\bdist.
+000002b0: 7769 6e2d 616d 6436 345c 6567 675c 7377  win-amd64\egg\sw
+000002c0: 6565 705c 7377 6565 705f 7375 7070 6f72  eep\sweep_suppor
+000002d0: 745c 6d61 736b 3276 6563 5f63 6f75 6e74  t\mask2vec_count
+000002e0: 2e70 79da 0e6d 6173 6b32 7665 635f 636f  .py..mask2vec_co
+000002f0: 756e 7409 0000 0073 2a00 0000 1801 0e01  unt....s*.......
+00000300: 2001 2001 04ff 0201 02ff 0c02 0a01 0c01   . .............
+00000310: 1601 1801 0c01 0601 0201 0201 0201 0201  ................
+00000320: 0afc 1005 0401 7216 0000 0029 0672 0200  ......r....).r..
+00000330: 0000 7203 0000 0072 0400 0000 da05 6e75  ..r....r......nu
+00000340: 6d70 7972 0900 0000 7216 0000 0072 1400  mpyr....r....r..
+00000350: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00000360: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000370: 0a00 0000 0c03 0c01 0c01 0801 1602       ..............
```

## sweep/sweep_support/nt2int.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 00:35:21 2023 UTC, .py size: 817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c9b7 4d64 3103 0000  o.........Md1...
+00000000: 6f0d 0d0a 0000 0000 a403 a164 3603 0000  o..........d6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
 00000040: 5300 2904 e900 0000 004e 6301 0000 0000  S.)......Nc.....
 00000050: 0000 0000 0000 0003 0000 000e 0000 0043  ...............C
 00000060: 0000 0073 ac00 0000 6900 6401 6402 9301  ...s....i.d.d...
 00000070: 6403 6404 9301 6405 6406 9301 6407 6408  d.d...d.d...d.d.
@@ -30,19 +30,19 @@
 000001d0: 72da 056c 6f77 6572 5a09 7665 6374 6f72  r..lowerZ.vector
 000001e0: 697a 65da 0367 6574 2903 5a07 6e74 5f6c  ize..get).Z.nt_l
 000001f0: 6973 74da 036d 6170 5a08 6d61 705f 6675  ist..mapZ.map_fu
 00000200: 6e63 a900 7234 0000 00fa 3762 7569 6c64  nc..r4....7build
 00000210: 5c62 6469 7374 2e77 696e 2d61 6d64 3634  \bdist.win-amd64
 00000220: 5c65 6767 5c73 7765 6570 5c73 7765 6570  \egg\sweep\sweep
 00000230: 5f73 7570 706f 7274 5c6e 7432 696e 742e  _support\nt2int.
-00000240: 7079 da06 6e74 3269 6e74 0400 0000 7364  py..nt2int....sd
+00000240: 7079 da06 6e74 3269 6e74 0600 0000 7364  py..nt2int....sd
 00000250: 0000 0008 0104 0102 ff04 0202 fe04 0302  ................
 00000260: fd04 0402 fc04 0502 fb04 0602 fa04 0702  ................
 00000270: f904 0802 f804 0902 f704 0a02 f604 0b02  ................
 00000280: f504 0c02 f404 0d02 f304 0e02 f204 0f02  ................
 00000290: f104 1002 f002 1102 0102 0102 0102 0102  ................
 000002a0: 0102 0102 0102 0102 0102 0102 0108 e40c  ................
 000002b0: 1e0c 0108 0104 0172 3600 0000 2903 da05  .......r6...)...
 000002c0: 6e75 6d70 7972 2f00 0000 7236 0000 0072  numpyr/...r6...r
 000002d0: 3400 0000 7234 0000 0072 3400 0000 7235  4...r4...r4...r5
 000002e0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000002f0: 0073 0400 0000 0802 0c01                 .s........
+000002f0: 0073 0400 0000 0803 0c02                 .s........
```

## sweep/sweep_support/orth.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  1 14:09:27 2023 UTC, .py size: 242 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 17c8 4f64 f200 0000  o.........Od....
+00000000: 6f0d 0d0a 0000 0000 a703 a164 f400 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
 00000040: 5300 2904 e900 0000 004e 6301 0000 0000  S.)......Nc.....
 00000050: 0000 0000 0000 0006 0000 0004 0000 0043  ...............C
 00000060: 0000 0073 5800 0000 7400 6a01 6a02 7c00  ...sX...t.j.j.|.
 00000070: 6401 6402 8d02 5c03 7d01 7d02 7d03 7403  d.d...\.}.}.}.t.
@@ -16,14 +16,14 @@
 000000f0: 5a03 7376 64da 036d 6178 da05 7368 6170  Z.svd..max..shap
 00000100: 655a 0566 696e 666f da03 6570 73da 0373  eZ.finfo..eps..s
 00000110: 756d 2906 da01 41da 0151 da01 535a 0256  um)...A..Q..SZ.V
 00000120: 745a 0374 6f6c da01 72a9 0072 0b00 0000  tZ.tol..r..r....
 00000130: fa35 6275 696c 645c 6264 6973 742e 7769  .5build\bdist.wi
 00000140: 6e2d 616d 6436 345c 6567 675c 7377 6565  n-amd64\egg\swee
 00000150: 705c 7377 6565 705f 7375 7070 6f72 745c  p\sweep_support\
-00000160: 6f72 7468 2e70 79da 046f 7274 6805 0000  orth.py..orth...
+00000160: 6f72 7468 2e70 79da 046f 7274 6806 0000  orth.py..orth...
 00000170: 0073 0a00 0000 1601 1e01 0c01 1401 0401  .s..............
 00000180: 720d 0000 0029 03da 056e 756d 7079 7202  r....)...numpyr.
 00000190: 0000 0072 0d00 0000 720b 0000 0072 0b00  ...r....r....r..
 000001a0: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
 000001b0: 6f64 756c 653e 0100 0000 7304 0000 0008  odule>....s.....
-000001c0: 020c 02                                  ...
+000001c0: 030c 02                                  ...
```

## sweep/sweep_support/seq2list.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 00:16:47 2023 UTC, .py size: 317 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6fb3 4d64 3d01 0000  o.......o.Md=...
+00000000: 6f0d 0d0a 0000 0000 ac03 a164 4101 0000  o..........dA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
 00000040: 5300 2904 e900 0000 004e 6302 0000 0000  S.)......Nc.....
 00000050: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
 00000060: 0000 0073 7c00 0000 7400 a001 7402 7c00  ...s|...t...t.|.
 00000070: 8301 a101 7d00 7c00 6a03 6401 1900 7d02  ....}.|.j.d...}.
@@ -18,14 +18,14 @@
 00000110: 6861 7065 5a05 7a65 726f 7372 0300 0000  hapeZ.zerosr....
 00000120: da05 7261 6e67 6529 055a 0473 646e 61da  ..range).Z.sdna.
 00000130: 0171 da01 6eda 0162 da01 69a9 0072 0d00  .q..n..b..i..r..
 00000140: 0000 fa39 6275 696c 645c 6264 6973 742e  ...9build\bdist.
 00000150: 7769 6e2d 616d 6436 345c 6567 675c 7377  win-amd64\egg\sw
 00000160: 6565 705c 7377 6565 705f 7375 7070 6f72  eep\sweep_suppor
 00000170: 745c 7365 7132 6c69 7374 2e70 79da 0873  t\seq2list.py..s
-00000180: 6571 326c 6973 7404 0000 0073 1000 0000  eq2list....s....
+00000180: 6571 326c 6973 7406 0000 0073 1000 0000  eq2list....s....
 00000190: 0e01 0a01 0801 0a01 1c01 0c01 2601 0401  ............&...
 000001a0: 720f 0000 0029 03da 056e 756d 7079 7204  r....)...numpyr.
 000001b0: 0000 0072 0f00 0000 720d 0000 0072 0d00  ...r....r....r..
 000001c0: 0000 720d 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
 000001d0: 6f64 756c 653e 0100 0000 7304 0000 0008  odule>....s.....
-000001e0: 020c 01                                  ...
+000001e0: 030c 02                                  ...
```

