# Comparing `tmp/phonopy-2.9.2.tar.gz` & `tmp/phonopy-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonopy-2.9.2.tar", last modified: Wed Mar 17 03:06:09 2021, max compression
+gzip compressed data, was "phonopy-2.9.3.tar", last modified: Wed Mar 17 03:54:44 2021, max compression
```

## Comparing `phonopy-2.9.2.tar` & `phonopy-2.9.3.tar`

### file list

```diff
@@ -1,630 +1,635 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.641527 phonopy-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-03-17 03:06:02.000000 phonopy-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-03-17 03:06:02.000000 phonopy-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-03-17 03:06:09.641527 phonopy-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-03-17 03:06:02.000000 phonopy-2.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-17 03:06:05.000000 phonopy-2.9.2/__nanoversion__.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.573522 phonopy-2.9.2/c/
--rw-r--r--   0 runner    (1001) docker     (121)    39498 2021-03-17 03:06:02.000000 phonopy-2.9.2/c/_phonopy.c
--rw-r--r--   0 runner    (1001) docker     (121)    12750 2021-03-17 03:06:02.000000 phonopy-2.9.2/c/derivative_dynmat.c
--rw-r--r--   0 runner    (1001) docker     (121)    20318 2021-03-17 03:06:02.000000 phonopy-2.9.2/c/dynmat.c
--rw-r--r--   0 runner    (1001) docker     (121)     5387 2021-03-17 03:06:02.000000 phonopy-2.9.2/c/kgrid.c
--rw-r--r--   0 runner    (1001) docker     (121)    34883 2021-03-17 03:06:02.000000 phonopy-2.9.2/c/phonopy.c
--rw-r--r--   0 runner    (1001) docker     (121)    37326 2021-03-17 03:06:02.000000 phonopy-2.9.2/c/tetrahedron_method.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.573522 phonopy-2.9.2/example/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.573522 phonopy-2.9.2/example/Al-Fleur/
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-Fleur/FORCES
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.577522 phonopy-2.9.2/example/Al-Fleur/IO/
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-Fleur/IO/inp.xml
--rw-r--r--   0 runner    (1001) docker     (121)    29458 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-Fleur/IO/kpts.xml
--rw-r--r--   0 runner    (1001) docker     (121)   320633 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-Fleur/IO/out
--rw-r--r--   0 runner    (1001) docker     (121)      739 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-Fleur/IO/sym.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-Fleur/README
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-Fleur/fleur_inpgen
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-Fleur/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      775 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-Fleur/supercell-001.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.577522 phonopy-2.9.2/example/Al-QHA/
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/Al-QHA.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR--1
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR--2
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR--3
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR--4
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR--5
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR-0
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR-1
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR-2
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR-3
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR-4
--rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/POSCAR-5
--rw-r--r--   0 runner    (1001) docker     (121)      559 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/README
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/e-v.dat
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--1
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--2
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--3
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--4
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--5
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-0
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-1
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-2
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-3
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-4
--rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-5
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.577522 phonopy-2.9.2/example/Al-hiphive/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-hiphive/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.581522 phonopy-2.9.2/example/Al-hiphive/reference_data/
--rw-r--r--   0 runner    (1001) docker     (121)     7872 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-hiphive/reference_data/POSCAR-001
--rw-r--r--   0 runner    (1001) docker     (121)     7872 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-hiphive/reference_data/POSCAR-002
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-hiphive/reference_data/POSCAR_prim
--rw-r--r--   0 runner    (1001) docker     (121)     8335 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-hiphive/reference_data/vasprun.xml-001
--rw-r--r--   0 runner    (1001) docker     (121)     8335 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al-hiphive/reference_data/vasprun.xml-002
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.581522 phonopy-2.9.2/example/Al2O3/
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al2O3/Al2O3.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al2O3/BORN
--rw-r--r--   0 runner    (1001) docker     (121)    29161 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al2O3/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al2O3/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      503 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al2O3/README
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al2O3/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)    26516 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al2O3/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    36124 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Al2O3/vaspruns.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.581522 phonopy-2.9.2/example/CaTiO3/
--rw-r--r--   0 runner    (1001) docker     (121)     7971 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/CaTiO3/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      550 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/CaTiO3/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)     8808 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/CaTiO3/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    15918 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/CaTiO3/vaspruns.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.581522 phonopy-2.9.2/example/Cr/
--rw-r--r--   0 runner    (1001) docker     (121)      849 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      863 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr/README
--rw-r--r--   0 runner    (1001) docker     (121)     4333 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    18816 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr/vasprun.xml.xz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.581522 phonopy-2.9.2/example/Cr-castep/
--rw-r--r--   0 runner    (1001) docker     (121)      849 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr-castep/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr-castep/README
--rw-r--r--   0 runner    (1001) docker     (121)    11524 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr-castep/band.pdf
--rw-r--r--   0 runner    (1001) docker     (121)      644 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr-castep/make_displ_dirs.sh
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr-castep/tail.cell
--rw-r--r--   0 runner    (1001) docker     (121)     6308 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cr-castep/unitcell.cell
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.585523 phonopy-2.9.2/example/Cu-QHA/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-00
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-01
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-02
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-03
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-04
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-05
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-06
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-07
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-08
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-09
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/POSCAR-10
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/README
--rw-r--r--   0 runner    (1001) docker     (121)      518 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/e-v.dat
--rw-r--r--   0 runner    (1001) docker     (121)    28604 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/fe-v.dat
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-00
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-01
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-02
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-03
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-04
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-05
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-06
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-07
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-08
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-09
--rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-10
--rw-r--r--   0 runner    (1001) docker     (121)   176164 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Cu-QHA/vasprun.xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.585523 phonopy-2.9.2/example/Graphene-siesta/
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Graphene-siesta/Gr.fdf
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Graphene-siesta/README
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.585523 phonopy-2.9.2/example/Graphene-siesta/disp-001/
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Graphene-siesta/disp-001/Gr.FA
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Graphene-siesta/run_example.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.585523 phonopy-2.9.2/example/LiF-nosym/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/LiF-nosym/BORN
--rw-r--r--   0 runner    (1001) docker     (121)   150828 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/LiF-nosym/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/LiF-nosym/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/LiF-nosym/README
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.585523 phonopy-2.9.2/example/MgB2/
--rw-r--r--   0 runner    (1001) docker     (121)     5335 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgB2/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgB2/MgB2.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgB2/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgB2/README
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgB2/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)     9982 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgB2/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    48627 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgB2/vaspruns.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.585523 phonopy-2.9.2/example/MgO/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgO/BORN
--rw-r--r--   0 runner    (1001) docker     (121)     6295 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgO/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgO/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      406 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgO/README
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgO/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)    12692 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgO/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5002 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/MgO/vaspruns.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.589523 phonopy-2.9.2/example/NaCl/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/BORN
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/NaCl-band-gv.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/NaCl-band.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/NaCl-dynmat.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/NaCl-gv.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/NaCl-read_write_fc.py
--rw-r--r--   0 runner    (1001) docker     (121)      704 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/NaCl-yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)     4239 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/NaCl.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/README
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/band-pdos.conf
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)     7932 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/pdos.conf
--rw-r--r--   0 runner    (1001) docker     (121)    12203 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    46150 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/vasprun.xml-001
--rw-r--r--   0 runner    (1001) docker     (121)    45042 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl/vasprun.xml-002
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.589523 phonopy-2.9.2/example/NaCl-CP2K/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CP2K/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CP2K/NaCl-supercell-001-forces-1_0.xyz
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CP2K/NaCl-supercell-002-forces-1_0.xyz
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CP2K/NaCl.inp
--rw-r--r--   0 runner    (1001) docker     (121)      989 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CP2K/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CP2K/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)    12733 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CP2K/phonopy_disp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.589523 phonopy-2.9.2/example/NaCl-CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CRYSTAL/README
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CRYSTAL/TEMPLATE
--rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CRYSTAL/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)    96429 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CRYSTAL/crystal.o
--rw-r--r--   0 runner    (1001) docker     (121)   356364 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CRYSTAL/supercell-001.o
--rw-r--r--   0 runner    (1001) docker     (121)   356364 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-CRYSTAL/supercell-002.o
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.593523 phonopy-2.9.2/example/NaCl-QE/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/BORN
--rw-r--r--   0 runner    (1001) docker     (121)     4864 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/NaCl-001.in
--rw-r--r--   0 runner    (1001) docker     (121)    24732 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/NaCl-001.out
--rw-r--r--   0 runner    (1001) docker     (121)     4864 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/NaCl-002.in
--rw-r--r--   0 runner    (1001) docker     (121)    24765 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/NaCl-002.out
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/NaCl.in
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/NaCl.ph.in
--rw-r--r--   0 runner    (1001) docker     (121)    27798 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/NaCl.ph.out
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/README
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)     7932 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE/header.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.593523 phonopy-2.9.2/example/NaCl-QE-q2r/
--rw-r--r--   0 runner    (1001) docker     (121)      799 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE-q2r/NaCl.in
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE-q2r/NaCl.ph-gamma.in
--rw-r--r--   0 runner    (1001) docker     (121)      249 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE-q2r/NaCl.ph.in
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE-q2r/README
--rw-r--r--   0 runner    (1001) docker     (121)    58693 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE-q2r/output888.tar.lzma
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-QE-q2r/q2r.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.597524 phonopy-2.9.2/example/NaCl-VASPdfpt/
--rw-r--r--   0 runner    (1001) docker     (121)   860165 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-VASPdfpt/FORCE_CONSTANTS
--rw-r--r--   0 runner    (1001) docker     (121)  1744162 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-VASPdfpt/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (121)     4138 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-VASPdfpt/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-VASPdfpt/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      626 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-VASPdfpt/README
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-VASPdfpt/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)  1298012 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-VASPdfpt/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.597524 phonopy-2.9.2/example/NaCl-abinit/
--rw-r--r--   0 runner    (1001) docker     (121)      728 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-abinit/NaCl.in
--rw-r--r--   0 runner    (1001) docker     (121)      863 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-abinit/README
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-abinit/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)     6433 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-abinit/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    95557 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-abinit/supercell-001.out
--rw-r--r--   0 runner    (1001) docker     (121)    96285 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-abinit/supercell-002.out
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.597524 phonopy-2.9.2/example/NaCl-castep/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-castep/BORN
--rw-r--r--   0 runner    (1001) docker     (121)     6295 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-castep/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-castep/README
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-castep/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)      644 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-castep/make_displ_dirs.sh
--rw-r--r--   0 runner    (1001) docker     (121)      851 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-castep/supercell.param
--rw-r--r--   0 runner    (1001) docker     (121)      585 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-castep/tail.cell
--rw-r--r--   0 runner    (1001) docker     (121)    64061 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-castep/unitcell.cell
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.597524 phonopy-2.9.2/example/NaCl-gruneisen/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.597524 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-0.995/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-0.995/BORN
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-0.995/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      736 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-0.995/POSCAR-unitcell
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.601524 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.00/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.00/BORN
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.00/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      736 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.00/POSCAR-unitcell
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.601524 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.005/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.005/BORN
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.005/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      736 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.005/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-gruneisen/README
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.601524 phonopy-2.9.2/example/NaCl-wien2k/
--rw-r--r--   0 runner    (1001) docker     (121)   847258 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k/NaCl-001.scf
--rw-r--r--   0 runner    (1001) docker     (121)   847258 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k/NaCl-002.scf
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k/NaCl.struct
--rw-r--r--   0 runner    (1001) docker     (121)      398 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k/README
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)     6433 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k/disp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.605524 phonopy-2.9.2/example/NaCl-wien2k-P1/
--rw-r--r--   0 runner    (1001) docker     (121)  2593810 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k-P1/NaCl-001.scf
--rw-r--r--   0 runner    (1001) docker     (121)  1044972 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k-P1/NaCl-002.scf
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k-P1/NaCl.struct
--rw-r--r--   0 runner    (1001) docker     (121)      490 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k-P1/README
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/NaCl-wien2k-P1/band.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.605524 phonopy-2.9.2/example/Si/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      442 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si/README
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si/mesh.conf
--rw-r--r--   0 runner    (1001) docker     (121)     4592 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    61197 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.605524 phonopy-2.9.2/example/Si-CP2K/
--rw-r--r--   0 runner    (1001) docker     (121)      833 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-CP2K/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-CP2K/Si-supercell-001-forces-1_0.xyz
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-CP2K/Si.inp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.605524 phonopy-2.9.2/example/Si-CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-CRYSTAL/README
--rw-r--r--   0 runner    (1001) docker     (121)      815 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-CRYSTAL/TEMPLATE
--rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-CRYSTAL/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)    46643 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-CRYSTAL/crystal.o
--rw-r--r--   0 runner    (1001) docker     (121)   355271 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-CRYSTAL/supercell-001.o
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.609525 phonopy-2.9.2/example/Si-QE/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QE/README
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QE/Si.in
--rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QE/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    64863 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QE/supercell-001.out
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.609525 phonopy-2.9.2/example/Si-QHA/
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR--1
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR--2
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR--3
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR--4
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR--5
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR-0
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR-1
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR-2
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR-3
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR-4
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/POSCAR-5
--rw-r--r--   0 runner    (1001) docker     (121)      751 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/README
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/Si.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      264 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/e-v.dat
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--1
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--2
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--3
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--4
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--5
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-0
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-1
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-2
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-3
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-4
--rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-5
--rw-r--r--   0 runner    (1001) docker     (121)    29920 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-QHA/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.609525 phonopy-2.9.2/example/Si-TURBOMOLE/
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/README
--rw-r--r--   0 runner    (1001) docker     (121)      257 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/control
--rw-r--r--   0 runner    (1001) docker     (121)      493 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/coord
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-TURBOMOLE/example-001/
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/example-001/auxbasis
--rw-r--r--   0 runner    (1001) docker     (121)      775 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/example-001/basis
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/example-001/control
--rw-r--r--   0 runner    (1001) docker     (121)    11676 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/example-001/coord
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/example-001/energy
--rw-r--r--   0 runner    (1001) docker     (121)    30357 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/example-001/gradient
--rw-r--r--   0 runner    (1001) docker     (121)   109958 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-TURBOMOLE/example-001/supercell-001.out
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-abinit/
--rw-r--r--   0 runner    (1001) docker     (121)      808 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-abinit/README
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-abinit/Si.in
--rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-abinit/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    99730 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-abinit/supercell-001.out
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-elk/
--rw-r--r--   0 runner    (1001) docker     (121)   144478 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-elk/INFO.OUT
--rw-r--r--   0 runner    (1001) docker     (121)      840 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-elk/README
--rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-elk/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-elk/elk-unitcell.in
--rw-r--r--   0 runner    (1001) docker     (121)     4245 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-elk/elk.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-gruneisen/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/README
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/Si-gruneisen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-gruneisen/minus/
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/minus/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/minus/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/minus/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   105506 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/minus/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-gruneisen/orig/
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/orig/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/orig/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/orig/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   105506 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/orig/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-gruneisen/plus/
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/plus/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/plus/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/plus/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   105506 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-gruneisen/plus/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-nosym/
--rw-r--r--   0 runner    (1001) docker     (121)      366 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-nosym/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-nosym/README
--rw-r--r--   0 runner    (1001) docker     (121)     4300 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-nosym/disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-nosym/mesh.conf
--rw-r--r--   0 runner    (1001) docker     (121)    28696 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-nosym/vasprun_xmls.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-siesta/
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-siesta/README
--rw-r--r--   0 runner    (1001) docker     (121)      881 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-siesta/Si.fdf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.613525 phonopy-2.9.2/example/Si-siesta/disp-001/
--rw-r--r--   0 runner    (1001) docker     (121)     4273 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-siesta/disp-001/Si.FA
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/Si-siesta/run_example.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.617525 phonopy-2.9.2/example/SiO2-HP/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SiO2-HP/BORN
--rw-r--r--   0 runner    (1001) docker     (121)     7133 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SiO2-HP/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SiO2-HP/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)      948 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SiO2-HP/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      639 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SiO2-HP/README
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SiO2-HP/anime.conf
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SiO2-HP/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)    10059 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SiO2-HP/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    10275 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SiO2-HP/vaspruns.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.617525 phonopy-2.9.2/example/SnO2/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SnO2/BORN
--rw-r--r--   0 runner    (1001) docker     (121)    10589 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SnO2/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SnO2/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SnO2/README
--rw-r--r--   0 runner    (1001) docker     (121)    13427 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SnO2/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    24635 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/SnO2/vaspruns.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.617525 phonopy-2.9.2/example/TiO2-anatase/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/TiO2-anatase/BORN
--rw-r--r--   0 runner    (1001) docker     (121)    37155 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/TiO2-anatase/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      977 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/TiO2-anatase/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/TiO2-anatase/README
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/TiO2-anatase/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)    31890 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/TiO2-anatase/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    21593 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/TiO2-anatase/vaspruns.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.617525 phonopy-2.9.2/example/ZnO/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/ZnO/BORN
--rw-r--r--   0 runner    (1001) docker     (121)     9647 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/ZnO/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/ZnO/POSCAR-unitcell
--rw-r--r--   0 runner    (1001) docker     (121)      240 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/ZnO/README
--rw-r--r--   0 runner    (1001) docker     (121)     7641 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/ZnO/phonopy_disp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    21254 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/ZnO/vaspruns.tar.lzma
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.617525 phonopy-2.9.2/example/ase/
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/ase/8Si-phonon.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.617525 phonopy-2.9.2/example/diamond-FHI-aims/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-FHI-aims/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-FHI-aims/band.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.617525 phonopy-2.9.2/example/diamond-FHI-aims/disp-001/
--rw-r--r--   0 runner    (1001) docker     (121)   255918 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-FHI-aims/disp-001/aims.out
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-FHI-aims/disp-001/control.in
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-FHI-aims/disp-001/geometry.in
--rw-r--r--   0 runner    (1001) docker     (121)      997 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-FHI-aims/geometry.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.617525 phonopy-2.9.2/example/diamond-dftb/
--rw-r--r--   0 runner    (1001) docker     (121)      713 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-dftb/README
--rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-dftb/band.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-dftb/dftb_in.hsd
--rw-r--r--   0 runner    (1001) docker     (121)      801 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-dftb/geo.gen
--rw-r--r--   0 runner    (1001) docker     (121)   100237 2021-03-17 03:06:02.000000 phonopy-2.9.2/example/diamond-dftb/results.tag
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.621525 phonopy-2.9.2/phonopy/
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6545 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/api_gruneisen.py
--rw-r--r--   0 runner    (1001) docker     (121)   120527 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/api_phonopy.py
--rw-r--r--   0 runner    (1001) docker     (121)    13084 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/api_qha.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.621525 phonopy-2.9.2/phonopy/cui/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/cui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11289 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/cui/collect_cell_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     6724 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/cui/create_force_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)    12076 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/cui/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     9860 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/cui/load_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    21738 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/cui/phonopy_argparse.py
--rw-r--r--   0 runner    (1001) docker     (121)    66582 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/cui/phonopy_script.py
--rw-r--r--   0 runner    (1001) docker     (121)    86800 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/cui/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5713 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/cui/show_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)    25491 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/file_IO.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.621525 phonopy-2.9.2/phonopy/gruneisen/
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/gruneisen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10858 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/gruneisen/band_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     5273 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/gruneisen/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     9468 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/gruneisen/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     4462 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/gruneisen/thermal_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.621525 phonopy-2.9.2/phonopy/harmonic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/harmonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10727 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/harmonic/derivative_dynmat.py
--rw-r--r--   0 runner    (1001) docker     (121)     9777 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/harmonic/displacement.py
--rw-r--r--   0 runner    (1001) docker     (121)    28794 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/harmonic/dynamical_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    16638 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/harmonic/dynmat_to_fc.py
--rw-r--r--   0 runner    (1001) docker     (121)    32326 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/harmonic/force_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.625526 phonopy-2.9.2/phonopy/interface/
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9634 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/abinit.py
--rw-r--r--   0 runner    (1001) docker     (121)     7975 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/aims.py
--rw-r--r--   0 runner    (1001) docker     (121)    11388 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/alm.py
--rw-r--r--   0 runner    (1001) docker     (121)    29163 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9124 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/castep.py
--rw-r--r--   0 runner    (1001) docker     (121)     3465 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/cif.py
--rw-r--r--   0 runner    (1001) docker     (121)     9425 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/cp2k.py
--rw-r--r--   0 runner    (1001) docker     (121)    13126 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/crystal.py
--rw-r--r--   0 runner    (1001) docker     (121)     6833 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/dftbp.py
--rw-r--r--   0 runner    (1001) docker     (121)     8000 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/elk.py
--rw-r--r--   0 runner    (1001) docker     (121)     4603 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/fc_calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8452 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/fleur.py
--rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/hiphive_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    23602 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/phonopy_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)    21043 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/qe.py
--rw-r--r--   0 runner    (1001) docker     (121)     9197 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/siesta.py
--rw-r--r--   0 runner    (1001) docker     (121)     8593 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/turbomole.py
--rw-r--r--   0 runner    (1001) docker     (121)    41790 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/vasp.py
--rw-r--r--   0 runner    (1001) docker     (121)    14731 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/interface/wien2k.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.625526 phonopy-2.9.2/phonopy/phonon/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9107 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/animation.py
--rw-r--r--   0 runner    (1001) docker     (121)    31525 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/band_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)    64066 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/character_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/degeneracy.py
--rw-r--r--   0 runner    (1001) docker     (121)    18812 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/dos.py
--rw-r--r--   0 runner    (1001) docker     (121)    10161 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/group_velocity.py
--rw-r--r--   0 runner    (1001) docker     (121)    23111 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/irreps.py
--rw-r--r--   0 runner    (1001) docker     (121)    15414 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)    10564 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/modulation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3731 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/moment.py
--rw-r--r--   0 runner    (1001) docker     (121)     9091 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/qpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)    16018 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/random_displacements.py
--rw-r--r--   0 runner    (1001) docker     (121)    10059 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/tetrahedron_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)    14596 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/thermal_displacement.py
--rw-r--r--   0 runner    (1001) docker     (121)    17080 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/phonon/thermal_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.625526 phonopy-2.9.2/phonopy/qha/
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/qha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31960 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/qha/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     5999 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/qha/electron.py
--rw-r--r--   0 runner    (1001) docker     (121)     4242 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/qha/eos.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.625526 phonopy-2.9.2/phonopy/spectrum/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/spectrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9660 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/spectrum/dynamic_structure_factor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6831 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/spectrum/velocity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.625526 phonopy-2.9.2/phonopy/structure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29223 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/structure/atoms.py
--rw-r--r--   0 runner    (1001) docker     (121)     4516 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/structure/brillouin_zone.py
--rw-r--r--   0 runner    (1001) docker     (121)    48165 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/structure/cells.py
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/structure/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    23251 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/structure/grid_points.py
--rw-r--r--   0 runner    (1001) docker     (121)    10525 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/structure/snf.py
--rw-r--r--   0 runner    (1001) docker     (121)    20680 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/structure/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)    19503 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/structure/tetrahedron_method.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.629526 phonopy-2.9.2/phonopy/unfolding/
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/unfolding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12833 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/unfolding/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/units.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-03-17 03:06:02.000000 phonopy-2.9.2/phonopy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.621525 phonopy-2.9.2/phonopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-03-17 03:06:09.000000 phonopy-2.9.2/phonopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16407 2021-03-17 03:06:09.000000 phonopy-2.9.2/phonopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-17 03:06:09.000000 phonopy-2.9.2/phonopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-03-17 03:06:09.000000 phonopy-2.9.2/phonopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-17 03:06:09.000000 phonopy-2.9.2/phonopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-03-17 03:06:02.000000 phonopy-2.9.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.629526 phonopy-2.9.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1845 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy
--rwxr-xr-x   0 runner    (1001) docker     (121)    21767 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-bandplot
--rwxr-xr-x   0 runner    (1001) docker     (121)     3945 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-calc-convert
--rwxr-xr-x   0 runner    (1001) docker     (121)     5809 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-crystal-born
--rwxr-xr-x   0 runner    (1001) docker     (121)    13054 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-gruneisen
--rwxr-xr-x   0 runner    (1001) docker     (121)     9132 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-gruneisenplot
--rwxr-xr-x   0 runner    (1001) docker     (121)     1888 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-load
--rwxr-xr-x   0 runner    (1001) docker     (121)     7314 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-pdosplot
--rwxr-xr-x   0 runner    (1001) docker     (121)     7363 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-propplot
--rwxr-xr-x   0 runner    (1001) docker     (121)     9899 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-qha
--rwxr-xr-x   0 runner    (1001) docker     (121)     7398 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-tdplot
--rwxr-xr-x   0 runner    (1001) docker     (121)     5911 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-vasp-born
--rwxr-xr-x   0 runner    (1001) docker     (121)     5131 2021-03-17 03:06:02.000000 phonopy-2.9.2/scripts/phonopy-vasp-efe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-17 03:06:09.641527 phonopy-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5131 2021-03-17 03:06:02.000000 phonopy-2.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.629526 phonopy-2.9.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/BORN_NaCl
--rw-r--r--   0 runner    (1001) docker     (121)      411 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/BORN_SnO2
--rw-r--r--   0 runner    (1001) docker     (121)      408 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/BORN_TiO2
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/FORCE_SETS_NaCl
--rw-r--r--   0 runner    (1001) docker     (121)    17642 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/FORCE_SETS_SnO2
--rw-r--r--   0 runner    (1001) docker     (121)    31536 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/FORCE_SETS_TiO2
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/POSCAR_NaCl
--rw-r--r--   0 runner    (1001) docker     (121)     7154 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.629526 phonopy-2.9.2/test/harmonic/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/harmonic/comm_points.dat
--rw-r--r--   0 runner    (1001) docker     (121)     5635 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/harmonic/test_dynamical_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     3931 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/harmonic/test_dynmat_to_fc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/harmonic/test_force_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.633526 phonopy-2.9.2/test/interface/
--rw-r--r--   0 runner    (1001) docker     (121)      591 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/BaGa2-wien2k.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/BaGa2.struct
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/FORCE_SETS_NaCl
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/NaCl-abinit-pwscf.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      728 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/NaCl-abinit.in
--rw-r--r--   0 runner    (1001) docker     (121)    64061 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/NaCl-castep.cell
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/NaCl-castep.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/NaCl-pwscf.in
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/NaCl-vasp.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/Si-CP2K.inp
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/Si-CP2K.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    46643 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/Si-CRYSTAL.o
--rw-r--r--   0 runner    (1001) docker     (121)      477 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/Si-CRYSTAL.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/Si-TURBOMOLE-control
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/Si-TURBOMOLE.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    12534 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/phonopy.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/test_CP2K.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/test_CRYSTAL.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/test_TURBOMOLE.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/test_abinit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/test_castep.py
--rw-r--r--   0 runner    (1001) docker     (121)     3438 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/test_phonopy_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/test_pwscf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/test_vasp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/test_wien2k.py
--rw-r--r--   0 runner    (1001) docker     (121)     6310 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/interface/vasprun.xml.tar.bz2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.641527 phonopy-2.9.2/test/phonon/
--rw-r--r--   0 runner    (1001) docker     (121)    99122 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_Amm2
--rw-r--r--   0 runner    (1001) docker     (121)    46792 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_I4_1a
--rw-r--r--   0 runner    (1001) docker     (121)    35132 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P-3m1
--rw-r--r--   0 runner    (1001) docker     (121)    90224 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P-4
--rw-r--r--   0 runner    (1001) docker     (121)    42114 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P-42_1m
--rw-r--r--   0 runner    (1001) docker     (121)    15722 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P-43m
--rw-r--r--   0 runner    (1001) docker     (121)    90520 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P-6
--rw-r--r--   0 runner    (1001) docker     (121)    45134 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P-6m2
--rw-r--r--   0 runner    (1001) docker     (121)   279292 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P2
--rw-r--r--   0 runner    (1001) docker     (121)   261420 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P222_1
--rw-r--r--   0 runner    (1001) docker     (121)    28080 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P2_13
--rw-r--r--   0 runner    (1001) docker     (121)    74580 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P3m1
--rw-r--r--   0 runner    (1001) docker     (121)   298284 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P4_1
--rw-r--r--   0 runner    (1001) docker     (121)    38624 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P4_332
--rw-r--r--   0 runner    (1001) docker     (121)    57082 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P4mm
--rw-r--r--   0 runner    (1001) docker     (121)   174912 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P6
--rw-r--r--   0 runner    (1001) docker     (121)    69832 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_P6_222
--rw-r--r--   0 runner    (1001) docker     (121)    14046 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_Pa-3
--rw-r--r--   0 runner    (1001) docker     (121)   298284 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/FORCE_SETS_Pc
--rw-r--r--   0 runner    (1001) docker     (121)      866 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_Amm2
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_I4_1a
--rw-r--r--   0 runner    (1001) docker     (121)      560 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P-3m1
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P-4
--rw-r--r--   0 runner    (1001) docker     (121)      746 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P-42_1m
--rw-r--r--   0 runner    (1001) docker     (121)      744 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P-43m
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P-6
--rw-r--r--   0 runner    (1001) docker     (121)      696 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P-6m2
--rw-r--r--   0 runner    (1001) docker     (121)      992 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P2
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P222_1
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P2_13
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P3m1
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P4_1
--rw-r--r--   0 runner    (1001) docker     (121)     3720 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P4_332
--rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P4mm
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P6
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_P6_222
--rw-r--r--   0 runner    (1001) docker     (121)      982 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_Pa-3
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/POSCAR_Pc
--rw-r--r--   0 runner    (1001) docker     (121)    22923 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/eigvecs_ii_TiPN3.txt
--rw-r--r--   0 runner    (1001) docker     (121)    73570 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/eigvecs_ij_TiPN3.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_band_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     4740 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_dos.py
--rw-r--r--   0 runner    (1001) docker     (121)    50951 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_irreps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_moment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_qpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)    12099 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_random_displacements.py
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_tetrahedron_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     4977 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_thermal_displacement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonon/test_thermal_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)    12203 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonopy_disp_NaCl.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13647 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonopy_disp_SnO2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19499 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonopy_disp_TiO2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    10056 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonopy_params_TiPN3.yaml.xz
--rw-r--r--   0 runner    (1001) docker     (121)    22776 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/phonopy_params_Zr3N4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.641527 phonopy-2.9.2/test/qha/
--rw-r--r--   0 runner    (1001) docker     (121)    10460 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/qha/test_electron.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.641527 phonopy-2.9.2/test/spectrum/
--rw-r--r--   0 runner    (1001) docker     (121)    17225 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/spectrum/XDATCAR
--rw-r--r--   0 runner    (1001) docker     (121)     8367 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/spectrum/test_dynamic_structure_factor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/spectrum/test_velocity.py
--rw-r--r--   0 runner    (1001) docker     (121)    30564 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/spectrum/velocities.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.641527 phonopy-2.9.2/test/structure/
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/structure/Si-conv.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4345 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/structure/SiO2-123.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/structure/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/structure/test_brillouin_zone.py
--rw-r--r--   0 runner    (1001) docker     (121)     4590 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/structure/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (121)    11228 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/structure/test_grid_points.py
--rw-r--r--   0 runner    (1001) docker     (121)     6171 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/structure/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     7929 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/structure/test_tetrahedron_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     2469 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/structure/tio2_qpoints.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:06:09.641527 phonopy-2.9.2/test/unfolding/
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/unfolding/FORCE_SETS
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/unfolding/bin-unfolding.dat
--rw-r--r--   0 runner    (1001) docker     (121)      971 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/unfolding/bin-unfolding_to_atoms.dat
--rw-r--r--   0 runner    (1001) docker     (121)      338 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/unfolding/plot_band.py
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2021-03-17 03:06:02.000000 phonopy-2.9.2/test/unfolding/test_unfolding.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.529753 phonopy-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-03-17 03:54:36.000000 phonopy-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2021-03-17 03:54:36.000000 phonopy-2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2021-03-17 03:54:44.529753 phonopy-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-03-17 03:54:36.000000 phonopy-2.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-03-17 03:54:39.000000 phonopy-2.9.3/__nanoversion__.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.417753 phonopy-2.9.3/c/
+-rw-r--r--   0 runner    (1001) docker     (121)    39498 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/_phonopy.c
+-rw-r--r--   0 runner    (1001) docker     (121)    12750 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/derivative_dynmat.c
+-rw-r--r--   0 runner    (1001) docker     (121)     2638 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/derivative_dynmat.h
+-rw-r--r--   0 runner    (1001) docker     (121)    20318 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/dynmat.c
+-rw-r--r--   0 runner    (1001) docker     (121)     5036 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/dynmat.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5387 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/kgrid.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4540 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/kgrid.h
+-rw-r--r--   0 runner    (1001) docker     (121)    34883 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/phonopy.c
+-rw-r--r--   0 runner    (1001) docker     (121)    11825 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/phonopy.h
+-rw-r--r--   0 runner    (1001) docker     (121)    37326 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/tetrahedron_method.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3543 2021-03-17 03:54:36.000000 phonopy-2.9.3/c/tetrahedron_method.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.413753 phonopy-2.9.3/example/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.421753 phonopy-2.9.3/example/Al-Fleur/
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-Fleur/FORCES
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.421753 phonopy-2.9.3/example/Al-Fleur/IO/
+-rw-r--r--   0 runner    (1001) docker     (121)     4471 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-Fleur/IO/inp.xml
+-rw-r--r--   0 runner    (1001) docker     (121)    29458 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-Fleur/IO/kpts.xml
+-rw-r--r--   0 runner    (1001) docker     (121)   320633 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-Fleur/IO/out
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-Fleur/IO/sym.xml
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-Fleur/README
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-Fleur/fleur_inpgen
+-rw-r--r--   0 runner    (1001) docker     (121)     3059 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-Fleur/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-Fleur/supercell-001.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.425753 phonopy-2.9.3/example/Al-QHA/
+-rw-r--r--   0 runner    (1001) docker     (121)     1468 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/Al-QHA.py
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR--1
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR--2
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR--3
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR--4
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR--5
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR-0
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR-1
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR-2
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR-3
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR-4
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/POSCAR-5
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/README
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/e-v.dat
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--1
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--2
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--3
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--4
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--5
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-0
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-1
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-2
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-3
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-4
+-rw-r--r--   0 runner    (1001) docker     (121)   133379 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-5
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.425753 phonopy-2.9.3/example/Al-hiphive/
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-hiphive/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.425753 phonopy-2.9.3/example/Al-hiphive/reference_data/
+-rw-r--r--   0 runner    (1001) docker     (121)     7872 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-hiphive/reference_data/POSCAR-001
+-rw-r--r--   0 runner    (1001) docker     (121)     7872 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-hiphive/reference_data/POSCAR-002
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-hiphive/reference_data/POSCAR_prim
+-rw-r--r--   0 runner    (1001) docker     (121)     8335 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-hiphive/reference_data/vasprun.xml-001
+-rw-r--r--   0 runner    (1001) docker     (121)     8335 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al-hiphive/reference_data/vasprun.xml-002
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.429753 phonopy-2.9.3/example/Al2O3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al2O3/Al2O3.py
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al2O3/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)    29161 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al2O3/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     3603 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al2O3/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      503 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al2O3/README
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al2O3/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    26516 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al2O3/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    36124 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Al2O3/vaspruns.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.429753 phonopy-2.9.3/example/CaTiO3/
+-rw-r--r--   0 runner    (1001) docker     (121)     7971 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/CaTiO3/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/CaTiO3/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)     8808 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/CaTiO3/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    15918 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/CaTiO3/vaspruns.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.429753 phonopy-2.9.3/example/Cr/
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      863 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr/README
+-rw-r--r--   0 runner    (1001) docker     (121)     4333 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    18816 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr/vasprun.xml.xz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.429753 phonopy-2.9.3/example/Cr-castep/
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr-castep/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr-castep/README
+-rw-r--r--   0 runner    (1001) docker     (121)    11524 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr-castep/band.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr-castep/make_displ_dirs.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr-castep/tail.cell
+-rw-r--r--   0 runner    (1001) docker     (121)     6308 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cr-castep/unitcell.cell
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.433753 phonopy-2.9.3/example/Cu-QHA/
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-00
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-01
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-02
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-03
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-04
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-05
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-06
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-07
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-08
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-09
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/POSCAR-10
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/README
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/e-v.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    28604 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/fe-v.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-00
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-01
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-02
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-03
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-04
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-05
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-06
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-07
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-08
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-09
+-rw-r--r--   0 runner    (1001) docker     (121)    41986 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-10
+-rw-r--r--   0 runner    (1001) docker     (121)   176164 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Cu-QHA/vasprun.xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.433753 phonopy-2.9.3/example/Graphene-siesta/
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Graphene-siesta/Gr.fdf
+-rw-r--r--   0 runner    (1001) docker     (121)     1038 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Graphene-siesta/README
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.433753 phonopy-2.9.3/example/Graphene-siesta/disp-001/
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Graphene-siesta/disp-001/Gr.FA
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Graphene-siesta/run_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.437753 phonopy-2.9.3/example/LiF-nosym/
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/LiF-nosym/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)   150828 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/LiF-nosym/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/LiF-nosym/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/LiF-nosym/README
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.437753 phonopy-2.9.3/example/MgB2/
+-rw-r--r--   0 runner    (1001) docker     (121)     5335 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgB2/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgB2/MgB2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgB2/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgB2/README
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgB2/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     9982 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgB2/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    48627 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgB2/vaspruns.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.437753 phonopy-2.9.3/example/MgO/
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgO/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)     6295 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgO/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgO/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgO/README
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgO/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    12692 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgO/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5002 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/MgO/vaspruns.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.441753 phonopy-2.9.3/example/NaCl/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/NaCl-band-gv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/NaCl-band.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/NaCl-dynmat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/NaCl-gv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/NaCl-read_write_fc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/NaCl-yaml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4239 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/NaCl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/README
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/band-pdos.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     7932 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/pdos.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    12203 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    46150 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/vasprun.xml-001
+-rw-r--r--   0 runner    (1001) docker     (121)    45042 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl/vasprun.xml-002
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.441753 phonopy-2.9.3/example/NaCl-CP2K/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CP2K/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     4853 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CP2K/NaCl-supercell-001-forces-1_0.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)     4853 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CP2K/NaCl-supercell-002-forces-1_0.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)     3660 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CP2K/NaCl.inp
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CP2K/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CP2K/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    12733 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CP2K/phonopy_disp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.441753 phonopy-2.9.3/example/NaCl-CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CRYSTAL/README
+-rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CRYSTAL/TEMPLATE
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CRYSTAL/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    96429 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CRYSTAL/crystal.o
+-rw-r--r--   0 runner    (1001) docker     (121)   356364 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CRYSTAL/supercell-001.o
+-rw-r--r--   0 runner    (1001) docker     (121)   356364 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-CRYSTAL/supercell-002.o
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.445753 phonopy-2.9.3/example/NaCl-QE/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)     4864 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/NaCl-001.in
+-rw-r--r--   0 runner    (1001) docker     (121)    24732 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/NaCl-001.out
+-rw-r--r--   0 runner    (1001) docker     (121)     4864 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/NaCl-002.in
+-rw-r--r--   0 runner    (1001) docker     (121)    24765 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/NaCl-002.out
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/NaCl.in
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/NaCl.ph.in
+-rw-r--r--   0 runner    (1001) docker     (121)    27798 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/NaCl.ph.out
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/README
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     7932 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE/header.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.445753 phonopy-2.9.3/example/NaCl-QE-q2r/
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE-q2r/NaCl.in
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE-q2r/NaCl.ph-gamma.in
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE-q2r/NaCl.ph.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE-q2r/README
+-rw-r--r--   0 runner    (1001) docker     (121)    58693 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE-q2r/output888.tar.lzma
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-QE-q2r/q2r.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.449753 phonopy-2.9.3/example/NaCl-VASPdfpt/
+-rw-r--r--   0 runner    (1001) docker     (121)   860165 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-VASPdfpt/FORCE_CONSTANTS
+-rw-r--r--   0 runner    (1001) docker     (121)  1744162 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-VASPdfpt/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     4138 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-VASPdfpt/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-VASPdfpt/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-VASPdfpt/README
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-VASPdfpt/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)  1298012 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-VASPdfpt/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.453753 phonopy-2.9.3/example/NaCl-abinit/
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-abinit/NaCl.in
+-rw-r--r--   0 runner    (1001) docker     (121)      863 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-abinit/README
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-abinit/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     6433 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-abinit/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    95557 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-abinit/supercell-001.out
+-rw-r--r--   0 runner    (1001) docker     (121)    96285 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-abinit/supercell-002.out
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.453753 phonopy-2.9.3/example/NaCl-castep/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-castep/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)     6295 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-castep/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-castep/README
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-castep/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-castep/make_displ_dirs.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-castep/supercell.param
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-castep/tail.cell
+-rw-r--r--   0 runner    (1001) docker     (121)    64061 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-castep/unitcell.cell
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.453753 phonopy-2.9.3/example/NaCl-gruneisen/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.453753 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-0.995/
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-0.995/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-0.995/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-0.995/POSCAR-unitcell
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.453753 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.00/
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.00/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.00/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.00/POSCAR-unitcell
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.453753 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.005/
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.005/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.005/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.005/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-gruneisen/README
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.457753 phonopy-2.9.3/example/NaCl-wien2k/
+-rw-r--r--   0 runner    (1001) docker     (121)   847258 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k/NaCl-001.scf
+-rw-r--r--   0 runner    (1001) docker     (121)   847258 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k/NaCl-002.scf
+-rw-r--r--   0 runner    (1001) docker     (121)     2556 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k/NaCl.struct
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k/README
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     6433 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k/disp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.465753 phonopy-2.9.3/example/NaCl-wien2k-P1/
+-rw-r--r--   0 runner    (1001) docker     (121)  2593810 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k-P1/NaCl-001.scf
+-rw-r--r--   0 runner    (1001) docker     (121)  1044972 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k-P1/NaCl-002.scf
+-rw-r--r--   0 runner    (1001) docker     (121)     2556 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k-P1/NaCl.struct
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k-P1/README
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/NaCl-wien2k-P1/band.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.465753 phonopy-2.9.3/example/Si/
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si/README
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si/mesh.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     4592 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    61197 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.465753 phonopy-2.9.3/example/Si-CP2K/
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-CP2K/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4853 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-CP2K/Si-supercell-001-forces-1_0.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-CP2K/Si.inp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.465753 phonopy-2.9.3/example/Si-CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-CRYSTAL/README
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-CRYSTAL/TEMPLATE
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-CRYSTAL/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    46643 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-CRYSTAL/crystal.o
+-rw-r--r--   0 runner    (1001) docker     (121)   355271 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-CRYSTAL/supercell-001.o
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.465753 phonopy-2.9.3/example/Si-QE/
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QE/README
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QE/Si.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QE/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    64863 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QE/supercell-001.out
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.473753 phonopy-2.9.3/example/Si-QHA/
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR--1
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR--2
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR--3
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR--4
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR--5
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR-0
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR-1
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR-2
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR-3
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR-4
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/POSCAR-5
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/README
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/Si.py
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/e-v.dat
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--1
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--2
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--3
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--4
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--5
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-0
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-1
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-2
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-3
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-4
+-rw-r--r--   0 runner    (1001) docker     (121)    35319 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-5
+-rw-r--r--   0 runner    (1001) docker     (121)    29920 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-QHA/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.473753 phonopy-2.9.3/example/Si-TURBOMOLE/
+-rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/README
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/control
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/coord
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.473753 phonopy-2.9.3/example/Si-TURBOMOLE/example-001/
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/example-001/auxbasis
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/example-001/basis
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/example-001/control
+-rw-r--r--   0 runner    (1001) docker     (121)    11676 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/example-001/coord
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/example-001/energy
+-rw-r--r--   0 runner    (1001) docker     (121)    30357 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/example-001/gradient
+-rw-r--r--   0 runner    (1001) docker     (121)   109958 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-TURBOMOLE/example-001/supercell-001.out
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.473753 phonopy-2.9.3/example/Si-abinit/
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-abinit/README
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-abinit/Si.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-abinit/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    99730 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-abinit/supercell-001.out
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.477753 phonopy-2.9.3/example/Si-elk/
+-rw-r--r--   0 runner    (1001) docker     (121)   144478 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-elk/INFO.OUT
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-elk/README
+-rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-elk/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-elk/elk-unitcell.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4245 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-elk/elk.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.477753 phonopy-2.9.3/example/Si-gruneisen/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/README
+-rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/Si-gruneisen.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.477753 phonopy-2.9.3/example/Si-gruneisen/minus/
+-rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/minus/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     1123 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/minus/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/minus/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   105506 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/minus/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.477753 phonopy-2.9.3/example/Si-gruneisen/orig/
+-rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/orig/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/orig/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/orig/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   105506 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/orig/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.477753 phonopy-2.9.3/example/Si-gruneisen/plus/
+-rw-r--r--   0 runner    (1001) docker     (121)     3154 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/plus/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     1123 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/plus/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)     6249 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/plus/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   105506 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-gruneisen/plus/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.481753 phonopy-2.9.3/example/Si-nosym/
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-nosym/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-nosym/README
+-rw-r--r--   0 runner    (1001) docker     (121)     4300 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-nosym/disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-nosym/mesh.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    28696 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-nosym/vasprun_xmls.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.481753 phonopy-2.9.3/example/Si-siesta/
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-siesta/README
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-siesta/Si.fdf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.481753 phonopy-2.9.3/example/Si-siesta/disp-001/
+-rw-r--r--   0 runner    (1001) docker     (121)     4273 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-siesta/disp-001/Si.FA
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/Si-siesta/run_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.481753 phonopy-2.9.3/example/SiO2-HP/
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SiO2-HP/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)     7133 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SiO2-HP/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SiO2-HP/INCAR
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SiO2-HP/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SiO2-HP/README
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SiO2-HP/anime.conf
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SiO2-HP/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    10059 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SiO2-HP/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    10275 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SiO2-HP/vaspruns.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.481753 phonopy-2.9.3/example/SnO2/
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SnO2/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)    10589 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SnO2/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SnO2/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SnO2/README
+-rw-r--r--   0 runner    (1001) docker     (121)    13427 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SnO2/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    24635 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/SnO2/vaspruns.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.485753 phonopy-2.9.3/example/TiO2-anatase/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/TiO2-anatase/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)    37155 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/TiO2-anatase/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      977 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/TiO2-anatase/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/TiO2-anatase/README
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/TiO2-anatase/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    31890 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/TiO2-anatase/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    21593 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/TiO2-anatase/vaspruns.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.485753 phonopy-2.9.3/example/ZnO/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/ZnO/BORN
+-rw-r--r--   0 runner    (1001) docker     (121)     9647 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/ZnO/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/ZnO/POSCAR-unitcell
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/ZnO/README
+-rw-r--r--   0 runner    (1001) docker     (121)     7641 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/ZnO/phonopy_disp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    21254 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/ZnO/vaspruns.tar.lzma
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.485753 phonopy-2.9.3/example/ase/
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/ase/8Si-phonon.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.485753 phonopy-2.9.3/example/diamond-FHI-aims/
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-FHI-aims/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-FHI-aims/band.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.485753 phonopy-2.9.3/example/diamond-FHI-aims/disp-001/
+-rw-r--r--   0 runner    (1001) docker     (121)   255918 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-FHI-aims/disp-001/aims.out
+-rw-r--r--   0 runner    (1001) docker     (121)     2536 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-FHI-aims/disp-001/control.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4454 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-FHI-aims/disp-001/geometry.in
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-FHI-aims/geometry.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.489753 phonopy-2.9.3/example/diamond-dftb/
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-dftb/README
+-rw-r--r--   0 runner    (1001) docker     (121)      239 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-dftb/band.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-dftb/dftb_in.hsd
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-dftb/geo.gen
+-rw-r--r--   0 runner    (1001) docker     (121)   100237 2021-03-17 03:54:36.000000 phonopy-2.9.3/example/diamond-dftb/results.tag
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.489753 phonopy-2.9.3/phonopy/
+-rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6545 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/api_gruneisen.py
+-rw-r--r--   0 runner    (1001) docker     (121)   120527 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/api_phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13084 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/api_qha.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.493753 phonopy-2.9.3/phonopy/cui/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/cui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11289 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/cui/collect_cell_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6724 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/cui/create_force_sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12076 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/cui/load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9860 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/cui/load_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21738 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/cui/phonopy_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (121)    66582 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/cui/phonopy_script.py
+-rw-r--r--   0 runner    (1001) docker     (121)    86800 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/cui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5713 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/cui/show_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25491 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/file_IO.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.493753 phonopy-2.9.3/phonopy/gruneisen/
+-rw-r--r--   0 runner    (1001) docker     (121)     1724 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/gruneisen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10858 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/gruneisen/band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5273 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/gruneisen/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9468 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/gruneisen/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4462 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/gruneisen/thermal_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.493753 phonopy-2.9.3/phonopy/harmonic/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/harmonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10727 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/harmonic/derivative_dynmat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9777 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/harmonic/displacement.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28794 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/harmonic/dynamical_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16638 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/harmonic/dynmat_to_fc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32326 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/harmonic/force_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.497753 phonopy-2.9.3/phonopy/interface/
+-rw-r--r--   0 runner    (1001) docker     (121)     1581 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9634 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/abinit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7975 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/aims.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11388 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/alm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29163 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9124 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/castep.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3465 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/cif.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9425 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/cp2k.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13126 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/crystal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6833 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/dftbp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8000 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/elk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4603 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/fc_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8452 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/fleur.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/hiphive_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23602 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/phonopy_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21043 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/qe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9197 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/siesta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8593 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/turbomole.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41790 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14731 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/interface/wien2k.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.501753 phonopy-2.9.3/phonopy/phonon/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9107 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/animation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31525 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    64066 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/character_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3947 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/degeneracy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18812 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/dos.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10161 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/group_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23111 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/irreps.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15414 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10564 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/modulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3731 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/moment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9091 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/qpoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16018 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/random_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10059 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/tetrahedron_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14596 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/thermal_displacement.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17080 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/phonon/thermal_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.501753 phonopy-2.9.3/phonopy/qha/
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/qha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31960 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/qha/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5999 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/qha/electron.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4242 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/qha/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.501753 phonopy-2.9.3/phonopy/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/spectrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9660 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/spectrum/dynamic_structure_factor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6831 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/spectrum/velocity.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.501753 phonopy-2.9.3/phonopy/structure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29223 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/structure/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4516 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/structure/brillouin_zone.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48165 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/structure/cells.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3623 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/structure/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23251 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/structure/grid_points.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10525 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/structure/snf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20680 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/structure/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19503 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/structure/tetrahedron_method.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.505753 phonopy-2.9.3/phonopy/unfolding/
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/unfolding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12833 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/unfolding/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3547 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/units.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-03-17 03:54:36.000000 phonopy-2.9.3/phonopy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.489753 phonopy-2.9.3/phonopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2021-03-17 03:54:44.000000 phonopy-2.9.3/phonopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    16485 2021-03-17 03:54:44.000000 phonopy-2.9.3/phonopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-17 03:54:44.000000 phonopy-2.9.3/phonopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-03-17 03:54:44.000000 phonopy-2.9.3/phonopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-03-17 03:54:44.000000 phonopy-2.9.3/phonopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-03-17 03:54:36.000000 phonopy-2.9.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.505753 phonopy-2.9.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1845 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy
+-rwxr-xr-x   0 runner    (1001) docker     (121)    21767 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-bandplot
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3945 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-calc-convert
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5809 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-crystal-born
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13054 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-gruneisen
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9132 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-gruneisenplot
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1888 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-load
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7314 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-pdosplot
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7363 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-propplot
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9899 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-qha
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7398 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-tdplot
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5911 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-vasp-born
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5131 2021-03-17 03:54:36.000000 phonopy-2.9.3/scripts/phonopy-vasp-efe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-17 03:54:44.529753 phonopy-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5131 2021-03-17 03:54:36.000000 phonopy-2.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.509753 phonopy-2.9.3/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/BORN_NaCl
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/BORN_SnO2
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/BORN_TiO2
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/FORCE_SETS_NaCl
+-rw-r--r--   0 runner    (1001) docker     (121)    17642 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/FORCE_SETS_SnO2
+-rw-r--r--   0 runner    (1001) docker     (121)    31536 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/FORCE_SETS_TiO2
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/POSCAR_NaCl
+-rw-r--r--   0 runner    (1001) docker     (121)     7154 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.509753 phonopy-2.9.3/test/harmonic/
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/harmonic/comm_points.dat
+-rw-r--r--   0 runner    (1001) docker     (121)     5635 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/harmonic/test_dynamical_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3931 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/harmonic/test_dynmat_to_fc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/harmonic/test_force_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.513753 phonopy-2.9.3/test/interface/
+-rw-r--r--   0 runner    (1001) docker     (121)      591 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/BaGa2-wien2k.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2559 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/BaGa2.struct
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/FORCE_SETS_NaCl
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/NaCl-abinit-pwscf.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/NaCl-abinit.in
+-rw-r--r--   0 runner    (1001) docker     (121)    64061 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/NaCl-castep.cell
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/NaCl-castep.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/NaCl-pwscf.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/NaCl-vasp.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/Si-CP2K.inp
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/Si-CP2K.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    46643 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/Si-CRYSTAL.o
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/Si-CRYSTAL.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/Si-TURBOMOLE-control
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/Si-TURBOMOLE.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    12534 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/phonopy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1313 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/test_CP2K.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/test_CRYSTAL.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/test_TURBOMOLE.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/test_abinit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/test_castep.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3438 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/test_phonopy_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1212 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/test_pwscf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/test_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/test_wien2k.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6310 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/interface/vasprun.xml.tar.bz2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.525753 phonopy-2.9.3/test/phonon/
+-rw-r--r--   0 runner    (1001) docker     (121)    99122 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_Amm2
+-rw-r--r--   0 runner    (1001) docker     (121)    46792 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_I4_1a
+-rw-r--r--   0 runner    (1001) docker     (121)    35132 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P-3m1
+-rw-r--r--   0 runner    (1001) docker     (121)    90224 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P-4
+-rw-r--r--   0 runner    (1001) docker     (121)    42114 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P-42_1m
+-rw-r--r--   0 runner    (1001) docker     (121)    15722 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P-43m
+-rw-r--r--   0 runner    (1001) docker     (121)    90520 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P-6
+-rw-r--r--   0 runner    (1001) docker     (121)    45134 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P-6m2
+-rw-r--r--   0 runner    (1001) docker     (121)   279292 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P2
+-rw-r--r--   0 runner    (1001) docker     (121)   261420 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P222_1
+-rw-r--r--   0 runner    (1001) docker     (121)    28080 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P2_13
+-rw-r--r--   0 runner    (1001) docker     (121)    74580 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P3m1
+-rw-r--r--   0 runner    (1001) docker     (121)   298284 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P4_1
+-rw-r--r--   0 runner    (1001) docker     (121)    38624 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P4_332
+-rw-r--r--   0 runner    (1001) docker     (121)    57082 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P4mm
+-rw-r--r--   0 runner    (1001) docker     (121)   174912 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P6
+-rw-r--r--   0 runner    (1001) docker     (121)    69832 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_P6_222
+-rw-r--r--   0 runner    (1001) docker     (121)    14046 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_Pa-3
+-rw-r--r--   0 runner    (1001) docker     (121)   298284 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/FORCE_SETS_Pc
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_Amm2
+-rw-r--r--   0 runner    (1001) docker     (121)     1736 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_I4_1a
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P-3m1
+-rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P-4
+-rw-r--r--   0 runner    (1001) docker     (121)      746 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P-42_1m
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P-43m
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P-6
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P-6m2
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P2
+-rw-r--r--   0 runner    (1001) docker     (121)     1984 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P222_1
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P2_13
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P3m1
+-rw-r--r--   0 runner    (1001) docker     (121)     2230 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P4_1
+-rw-r--r--   0 runner    (1001) docker     (121)     3720 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P4_332
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P4mm
+-rw-r--r--   0 runner    (1001) docker     (121)     2098 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P6
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_P6_222
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_Pa-3
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/POSCAR_Pc
+-rw-r--r--   0 runner    (1001) docker     (121)    22923 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/eigvecs_ii_TiPN3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    73570 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/eigvecs_ij_TiPN3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4740 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_dos.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50951 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_irreps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2757 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3397 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_moment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_qpoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12099 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_random_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2891 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_tetrahedron_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4977 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_thermal_displacement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonon/test_thermal_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12203 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonopy_disp_NaCl.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    13647 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonopy_disp_SnO2.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    19499 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonopy_disp_TiO2.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    10056 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonopy_params_TiPN3.yaml.xz
+-rw-r--r--   0 runner    (1001) docker     (121)    22776 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/phonopy_params_Zr3N4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.525753 phonopy-2.9.3/test/qha/
+-rw-r--r--   0 runner    (1001) docker     (121)    10460 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/qha/test_electron.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.525753 phonopy-2.9.3/test/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (121)    17225 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/spectrum/XDATCAR
+-rw-r--r--   0 runner    (1001) docker     (121)     8367 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/spectrum/test_dynamic_structure_factor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/spectrum/test_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30564 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/spectrum/velocities.dat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.525753 phonopy-2.9.3/test/structure/
+-rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/structure/Si-conv.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4345 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/structure/SiO2-123.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/structure/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2343 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/structure/test_brillouin_zone.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4590 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/structure/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11228 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/structure/test_grid_points.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6171 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/structure/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7929 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/structure/test_tetrahedron_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2469 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/structure/tio2_qpoints.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-17 03:54:44.529753 phonopy-2.9.3/test/unfolding/
+-rw-r--r--   0 runner    (1001) docker     (121)     6296 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/unfolding/FORCE_SETS
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/unfolding/bin-unfolding.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/unfolding/bin-unfolding_to_atoms.dat
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/unfolding/plot_band.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4753 2021-03-17 03:54:36.000000 phonopy-2.9.3/test/unfolding/test_unfolding.py
```

### Comparing `phonopy-2.9.2/LICENSE` & `phonopy-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/README.md` & `phonopy-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/c/_phonopy.c` & `phonopy-2.9.3/c/_phonopy.c`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/c/derivative_dynmat.c` & `phonopy-2.9.3/c/derivative_dynmat.c`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/c/dynmat.c` & `phonopy-2.9.3/c/dynmat.c`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/c/kgrid.c` & `phonopy-2.9.3/c/kgrid.c`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/c/phonopy.c` & `phonopy-2.9.3/c/phonopy.c`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/c/tetrahedron_method.c` & `phonopy-2.9.3/c/tetrahedron_method.c`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-Fleur/FORCES` & `phonopy-2.9.3/example/Al-Fleur/FORCES`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-Fleur/IO/inp.xml` & `phonopy-2.9.3/example/Al-Fleur/IO/inp.xml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-Fleur/IO/kpts.xml` & `phonopy-2.9.3/example/Al-Fleur/IO/kpts.xml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-Fleur/IO/out` & `phonopy-2.9.3/example/Al-Fleur/IO/out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-Fleur/IO/sym.xml` & `phonopy-2.9.3/example/Al-Fleur/IO/sym.xml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-Fleur/README` & `phonopy-2.9.3/example/Al-Fleur/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-Fleur/phonopy_disp.yaml` & `phonopy-2.9.3/example/Al-Fleur/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-Fleur/supercell-001.in` & `phonopy-2.9.3/example/Al-Fleur/supercell-001.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/Al-QHA.py` & `phonopy-2.9.3/example/Al-QHA/Al-QHA.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR--1` & `phonopy-2.9.3/example/Al-QHA/POSCAR--1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR--2` & `phonopy-2.9.3/example/Al-QHA/POSCAR--2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR--3` & `phonopy-2.9.3/example/Al-QHA/POSCAR--3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR--4` & `phonopy-2.9.3/example/Al-QHA/POSCAR--4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR--5` & `phonopy-2.9.3/example/Al-QHA/POSCAR--5`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR-0` & `phonopy-2.9.3/example/Al-QHA/POSCAR-0`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR-1` & `phonopy-2.9.3/example/Al-QHA/POSCAR-1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR-2` & `phonopy-2.9.3/example/Al-QHA/POSCAR-2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR-3` & `phonopy-2.9.3/example/Al-QHA/POSCAR-3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR-4` & `phonopy-2.9.3/example/Al-QHA/POSCAR-4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/POSCAR-5` & `phonopy-2.9.3/example/Al-QHA/POSCAR-5`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/README` & `phonopy-2.9.3/example/Al-QHA/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--1` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--2` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--3` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--4` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml--5` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml--5`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-0` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-0`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-1` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-2` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-3` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-4` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-QHA/thermal_properties.yaml-5` & `phonopy-2.9.3/example/Al-QHA/thermal_properties.yaml-5`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-hiphive/README.md` & `phonopy-2.9.3/example/Al-hiphive/README.md`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-hiphive/reference_data/POSCAR-001` & `phonopy-2.9.3/example/Al-hiphive/reference_data/POSCAR-001`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-hiphive/reference_data/POSCAR-002` & `phonopy-2.9.3/example/Al-hiphive/reference_data/POSCAR-002`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-hiphive/reference_data/vasprun.xml-001` & `phonopy-2.9.3/example/Al-hiphive/reference_data/vasprun.xml-001`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al-hiphive/reference_data/vasprun.xml-002` & `phonopy-2.9.3/example/Al-hiphive/reference_data/vasprun.xml-002`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al2O3/Al2O3.py` & `phonopy-2.9.3/example/Al2O3/Al2O3.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al2O3/FORCE_SETS` & `phonopy-2.9.3/example/Al2O3/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al2O3/POSCAR-unitcell` & `phonopy-2.9.3/example/Al2O3/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al2O3/phonopy_disp.yaml` & `phonopy-2.9.3/example/Al2O3/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Al2O3/vaspruns.tar.lzma` & `phonopy-2.9.3/example/Al2O3/vaspruns.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/CaTiO3/FORCE_SETS` & `phonopy-2.9.3/example/CaTiO3/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/CaTiO3/POSCAR-unitcell` & `phonopy-2.9.3/example/CaTiO3/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/CaTiO3/phonopy_disp.yaml` & `phonopy-2.9.3/example/CaTiO3/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/CaTiO3/vaspruns.tar.lzma` & `phonopy-2.9.3/example/CaTiO3/vaspruns.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr/FORCE_SETS` & `phonopy-2.9.3/example/Cr/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr/README` & `phonopy-2.9.3/example/Cr/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr/phonopy_disp.yaml` & `phonopy-2.9.3/example/Cr/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr/vasprun.xml.xz` & `phonopy-2.9.3/example/Cr/vasprun.xml.xz`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr-castep/FORCE_SETS` & `phonopy-2.9.3/example/Cr-castep/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr-castep/README` & `phonopy-2.9.3/example/Cr-castep/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr-castep/band.pdf` & `phonopy-2.9.3/example/Cr-castep/band.pdf`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr-castep/make_displ_dirs.sh` & `phonopy-2.9.3/example/Cr-castep/make_displ_dirs.sh`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr-castep/tail.cell` & `phonopy-2.9.3/example/Cr-castep/tail.cell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cr-castep/unitcell.cell` & `phonopy-2.9.3/example/Cr-castep/unitcell.cell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/README` & `phonopy-2.9.3/example/Cu-QHA/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/e-v.dat` & `phonopy-2.9.3/example/Cu-QHA/e-v.dat`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/fe-v.dat` & `phonopy-2.9.3/example/Cu-QHA/fe-v.dat`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-00` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-00`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-01` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-01`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-02` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-02`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-03` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-03`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-04` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-04`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-05` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-05`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-06` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-06`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-07` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-07`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-08` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-08`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-09` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-09`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/thermal_properties.yaml-10` & `phonopy-2.9.3/example/Cu-QHA/thermal_properties.yaml-10`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Cu-QHA/vasprun.xmls.tar.lzma` & `phonopy-2.9.3/example/Cu-QHA/vasprun.xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Graphene-siesta/Gr.fdf` & `phonopy-2.9.3/example/Graphene-siesta/Gr.fdf`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Graphene-siesta/README` & `phonopy-2.9.3/example/Graphene-siesta/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Graphene-siesta/disp-001/Gr.FA` & `phonopy-2.9.3/example/Graphene-siesta/disp-001/Gr.FA`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Graphene-siesta/run_example.sh` & `phonopy-2.9.3/example/Graphene-siesta/run_example.sh`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/LiF-nosym/FORCE_SETS` & `phonopy-2.9.3/example/LiF-nosym/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/LiF-nosym/POSCAR` & `phonopy-2.9.3/example/LiF-nosym/POSCAR`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/LiF-nosym/README` & `phonopy-2.9.3/example/LiF-nosym/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/MgB2/FORCE_SETS` & `phonopy-2.9.3/example/MgB2/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/MgB2/phonopy_disp.yaml` & `phonopy-2.9.3/example/MgB2/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/MgB2/vaspruns.tar.lzma` & `phonopy-2.9.3/example/MgB2/vaspruns.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/MgO/FORCE_SETS` & `phonopy-2.9.3/example/MgO/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/MgO/POSCAR-unitcell` & `phonopy-2.9.3/example/MgO/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/MgO/phonopy_disp.yaml` & `phonopy-2.9.3/example/MgO/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/MgO/vaspruns.tar.lzma` & `phonopy-2.9.3/example/MgO/vaspruns.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/FORCE_SETS` & `phonopy-2.9.3/example/NaCl/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/NaCl-band-gv.py` & `phonopy-2.9.3/example/NaCl/NaCl-band-gv.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/NaCl-band.py` & `phonopy-2.9.3/example/NaCl/NaCl-band.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/NaCl-dynmat.py` & `phonopy-2.9.3/example/NaCl/NaCl-dynmat.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/NaCl-gv.py` & `phonopy-2.9.3/example/NaCl/NaCl-gv.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/NaCl-read_write_fc.py` & `phonopy-2.9.3/example/NaCl/NaCl-read_write_fc.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/NaCl-yaml.py` & `phonopy-2.9.3/example/NaCl/NaCl-yaml.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/NaCl.py` & `phonopy-2.9.3/example/NaCl/NaCl.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/POSCAR-unitcell` & `phonopy-2.9.3/example/NaCl/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/README` & `phonopy-2.9.3/example/NaCl/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/disp.yaml` & `phonopy-2.9.3/example/NaCl/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/phonopy_disp.yaml` & `phonopy-2.9.3/example/NaCl/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/vasprun.xml-001` & `phonopy-2.9.3/example/NaCl/vasprun.xml-001`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl/vasprun.xml-002` & `phonopy-2.9.3/example/NaCl/vasprun.xml-002`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CP2K/NaCl-supercell-001-forces-1_0.xyz` & `phonopy-2.9.3/example/NaCl-CP2K/NaCl-supercell-001-forces-1_0.xyz`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CP2K/NaCl-supercell-002-forces-1_0.xyz` & `phonopy-2.9.3/example/NaCl-CP2K/NaCl-supercell-002-forces-1_0.xyz`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CP2K/NaCl.inp` & `phonopy-2.9.3/example/NaCl-CP2K/NaCl.inp`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CP2K/README.md` & `phonopy-2.9.3/example/NaCl-CP2K/README.md`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CP2K/phonopy_disp.yaml` & `phonopy-2.9.3/example/NaCl-CP2K/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CRYSTAL/README` & `phonopy-2.9.3/example/NaCl-CRYSTAL/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CRYSTAL/TEMPLATE` & `phonopy-2.9.3/example/NaCl-CRYSTAL/TEMPLATE`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CRYSTAL/crystal.o` & `phonopy-2.9.3/example/NaCl-CRYSTAL/crystal.o`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CRYSTAL/supercell-001.o` & `phonopy-2.9.3/example/NaCl-CRYSTAL/supercell-001.o`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-CRYSTAL/supercell-002.o` & `phonopy-2.9.3/example/NaCl-CRYSTAL/supercell-002.o`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE/NaCl-001.in` & `phonopy-2.9.3/example/NaCl-QE/NaCl-001.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE/NaCl-001.out` & `phonopy-2.9.3/example/NaCl-QE/NaCl-001.out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE/NaCl-002.in` & `phonopy-2.9.3/example/NaCl-QE/NaCl-002.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE/NaCl-002.out` & `phonopy-2.9.3/example/NaCl-QE/NaCl-002.out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE/NaCl.in` & `phonopy-2.9.3/example/NaCl-QE/NaCl.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE/NaCl.ph.out` & `phonopy-2.9.3/example/NaCl-QE/NaCl.ph.out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE/README` & `phonopy-2.9.3/example/NaCl-QE/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE/disp.yaml` & `phonopy-2.9.3/example/NaCl-QE/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE-q2r/NaCl.in` & `phonopy-2.9.3/example/NaCl-QE-q2r/NaCl.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE-q2r/README` & `phonopy-2.9.3/example/NaCl-QE-q2r/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-QE-q2r/output888.tar.lzma` & `phonopy-2.9.3/example/NaCl-QE-q2r/output888.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-VASPdfpt/FORCE_CONSTANTS` & `phonopy-2.9.3/example/NaCl-VASPdfpt/FORCE_CONSTANTS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-VASPdfpt/OUTCAR` & `phonopy-2.9.3/example/NaCl-VASPdfpt/OUTCAR`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-VASPdfpt/POSCAR` & `phonopy-2.9.3/example/NaCl-VASPdfpt/POSCAR`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-VASPdfpt/POSCAR-unitcell` & `phonopy-2.9.3/example/NaCl-VASPdfpt/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-VASPdfpt/README` & `phonopy-2.9.3/example/NaCl-VASPdfpt/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-VASPdfpt/vasprun.xml` & `phonopy-2.9.3/example/NaCl-VASPdfpt/vasprun.xml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-abinit/NaCl.in` & `phonopy-2.9.3/example/NaCl-abinit/NaCl.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-abinit/README` & `phonopy-2.9.3/example/NaCl-abinit/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-abinit/disp.yaml` & `phonopy-2.9.3/example/NaCl-abinit/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-abinit/supercell-001.out` & `phonopy-2.9.3/example/NaCl-abinit/supercell-001.out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-abinit/supercell-002.out` & `phonopy-2.9.3/example/NaCl-abinit/supercell-002.out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-castep/FORCE_SETS` & `phonopy-2.9.3/example/NaCl-castep/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-castep/README` & `phonopy-2.9.3/example/NaCl-castep/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-castep/make_displ_dirs.sh` & `phonopy-2.9.3/example/NaCl-castep/make_displ_dirs.sh`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-castep/supercell.param` & `phonopy-2.9.3/example/NaCl-castep/supercell.param`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-castep/tail.cell` & `phonopy-2.9.3/example/NaCl-castep/tail.cell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-castep/unitcell.cell` & `phonopy-2.9.3/example/NaCl-castep/unitcell.cell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-gruneisen/NaCl-0.995/FORCE_SETS` & `phonopy-2.9.3/example/NaCl-gruneisen/NaCl-0.995/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-gruneisen/NaCl-0.995/POSCAR-unitcell` & `phonopy-2.9.3/example/NaCl-gruneisen/NaCl-0.995/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.00/FORCE_SETS` & `phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.00/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.00/POSCAR-unitcell` & `phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.00/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.005/FORCE_SETS` & `phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.005/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-gruneisen/NaCl-1.005/POSCAR-unitcell` & `phonopy-2.9.3/example/NaCl-gruneisen/NaCl-1.005/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-wien2k/NaCl-001.scf` & `phonopy-2.9.3/example/NaCl-wien2k/NaCl-001.scf`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-wien2k/NaCl-002.scf` & `phonopy-2.9.3/example/NaCl-wien2k/NaCl-002.scf`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-wien2k/NaCl.struct` & `phonopy-2.9.3/example/NaCl-wien2k/NaCl.struct`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-wien2k/disp.yaml` & `phonopy-2.9.3/example/NaCl-wien2k/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-wien2k-P1/NaCl-001.scf` & `phonopy-2.9.3/example/NaCl-wien2k-P1/NaCl-001.scf`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-wien2k-P1/NaCl-002.scf` & `phonopy-2.9.3/example/NaCl-wien2k-P1/NaCl-002.scf`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/NaCl-wien2k-P1/NaCl.struct` & `phonopy-2.9.3/example/NaCl-wien2k-P1/NaCl.struct`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si/phonopy_disp.yaml` & `phonopy-2.9.3/example/Si/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si/vasprun.xml` & `phonopy-2.9.3/example/Si/vasprun.xml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-CP2K/README.md` & `phonopy-2.9.3/example/Si-CP2K/README.md`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-CP2K/Si-supercell-001-forces-1_0.xyz` & `phonopy-2.9.3/example/Si-CP2K/Si-supercell-001-forces-1_0.xyz`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-CP2K/Si.inp` & `phonopy-2.9.3/example/Si-CP2K/Si.inp`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-CRYSTAL/README` & `phonopy-2.9.3/example/Si-CRYSTAL/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-CRYSTAL/TEMPLATE` & `phonopy-2.9.3/example/Si-CRYSTAL/TEMPLATE`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-CRYSTAL/crystal.o` & `phonopy-2.9.3/example/Si-CRYSTAL/crystal.o`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-CRYSTAL/supercell-001.o` & `phonopy-2.9.3/example/Si-CRYSTAL/supercell-001.o`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QE/README` & `phonopy-2.9.3/example/Si-QE/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QE/Si.in` & `phonopy-2.9.3/example/Si-QE/Si.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QE/disp.yaml` & `phonopy-2.9.3/example/Si-QE/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QE/supercell-001.out` & `phonopy-2.9.3/example/Si-QE/supercell-001.out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR--1` & `phonopy-2.9.3/example/Si-QHA/POSCAR--1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR--2` & `phonopy-2.9.3/example/Si-QHA/POSCAR--2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR--3` & `phonopy-2.9.3/example/Si-QHA/POSCAR--3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR--4` & `phonopy-2.9.3/example/Si-QHA/POSCAR--4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR--5` & `phonopy-2.9.3/example/Si-QHA/POSCAR--5`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR-0` & `phonopy-2.9.3/example/Si-QHA/POSCAR-0`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR-1` & `phonopy-2.9.3/example/Si-QHA/POSCAR-1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR-2` & `phonopy-2.9.3/example/Si-QHA/POSCAR-2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR-3` & `phonopy-2.9.3/example/Si-QHA/POSCAR-3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR-4` & `phonopy-2.9.3/example/Si-QHA/POSCAR-4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/POSCAR-5` & `phonopy-2.9.3/example/Si-QHA/POSCAR-5`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/README` & `phonopy-2.9.3/example/Si-QHA/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/Si.py` & `phonopy-2.9.3/example/Si-QHA/Si.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--1` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--2` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--3` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--4` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml--5` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml--5`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-0` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-0`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-1` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-2` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-3` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-4` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/thermal_properties.yaml-5` & `phonopy-2.9.3/example/Si-QHA/thermal_properties.yaml-5`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-QHA/vasprun_xmls.tar.lzma` & `phonopy-2.9.3/example/Si-QHA/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-TURBOMOLE/README` & `phonopy-2.9.3/example/Si-TURBOMOLE/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-TURBOMOLE/example-001/auxbasis` & `phonopy-2.9.3/example/Si-TURBOMOLE/example-001/auxbasis`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-TURBOMOLE/example-001/basis` & `phonopy-2.9.3/example/Si-TURBOMOLE/example-001/basis`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-TURBOMOLE/example-001/control` & `phonopy-2.9.3/example/Si-TURBOMOLE/example-001/control`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-TURBOMOLE/example-001/coord` & `phonopy-2.9.3/example/Si-TURBOMOLE/example-001/coord`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-TURBOMOLE/example-001/gradient` & `phonopy-2.9.3/example/Si-TURBOMOLE/example-001/gradient`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-TURBOMOLE/example-001/supercell-001.out` & `phonopy-2.9.3/example/Si-TURBOMOLE/example-001/supercell-001.out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-abinit/README` & `phonopy-2.9.3/example/Si-abinit/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-abinit/Si.in` & `phonopy-2.9.3/example/Si-abinit/Si.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-abinit/disp.yaml` & `phonopy-2.9.3/example/Si-abinit/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-abinit/supercell-001.out` & `phonopy-2.9.3/example/Si-abinit/supercell-001.out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-elk/INFO.OUT` & `phonopy-2.9.3/example/Si-elk/INFO.OUT`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-elk/README` & `phonopy-2.9.3/example/Si-elk/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-elk/disp.yaml` & `phonopy-2.9.3/example/Si-elk/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-elk/elk-unitcell.in` & `phonopy-2.9.3/example/Si-elk/elk-unitcell.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-elk/elk.in` & `phonopy-2.9.3/example/Si-elk/elk.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/Si-gruneisen.py` & `phonopy-2.9.3/example/Si-gruneisen/Si-gruneisen.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/minus/FORCE_SETS` & `phonopy-2.9.3/example/Si-gruneisen/minus/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/minus/POSCAR-unitcell` & `phonopy-2.9.3/example/Si-gruneisen/minus/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/minus/disp.yaml` & `phonopy-2.9.3/example/Si-gruneisen/minus/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/minus/vasprun.xml` & `phonopy-2.9.3/example/Si-gruneisen/minus/vasprun.xml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/orig/FORCE_SETS` & `phonopy-2.9.3/example/Si-gruneisen/orig/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/orig/POSCAR-unitcell` & `phonopy-2.9.3/example/Si-gruneisen/orig/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/orig/disp.yaml` & `phonopy-2.9.3/example/Si-gruneisen/orig/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/orig/vasprun.xml` & `phonopy-2.9.3/example/Si-gruneisen/orig/vasprun.xml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/plus/FORCE_SETS` & `phonopy-2.9.3/example/Si-gruneisen/plus/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/plus/POSCAR-unitcell` & `phonopy-2.9.3/example/Si-gruneisen/plus/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/plus/disp.yaml` & `phonopy-2.9.3/example/Si-gruneisen/plus/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-gruneisen/plus/vasprun.xml` & `phonopy-2.9.3/example/Si-gruneisen/plus/vasprun.xml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-nosym/README` & `phonopy-2.9.3/example/Si-nosym/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-nosym/disp.yaml` & `phonopy-2.9.3/example/Si-nosym/disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-nosym/vasprun_xmls.tar.lzma` & `phonopy-2.9.3/example/Si-nosym/vasprun_xmls.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-siesta/README` & `phonopy-2.9.3/example/Si-siesta/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-siesta/Si.fdf` & `phonopy-2.9.3/example/Si-siesta/Si.fdf`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-siesta/disp-001/Si.FA` & `phonopy-2.9.3/example/Si-siesta/disp-001/Si.FA`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/Si-siesta/run_example.sh` & `phonopy-2.9.3/example/Si-siesta/run_example.sh`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SiO2-HP/FORCE_SETS` & `phonopy-2.9.3/example/SiO2-HP/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SiO2-HP/POSCAR-unitcell` & `phonopy-2.9.3/example/SiO2-HP/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SiO2-HP/README` & `phonopy-2.9.3/example/SiO2-HP/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SiO2-HP/phonopy_disp.yaml` & `phonopy-2.9.3/example/SiO2-HP/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SiO2-HP/vaspruns.tar.lzma` & `phonopy-2.9.3/example/SiO2-HP/vaspruns.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SnO2/FORCE_SETS` & `phonopy-2.9.3/example/SnO2/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SnO2/POSCAR-unitcell` & `phonopy-2.9.3/example/SnO2/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SnO2/README` & `phonopy-2.9.3/example/SnO2/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SnO2/phonopy_disp.yaml` & `phonopy-2.9.3/example/SnO2/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/SnO2/vaspruns.tar.lzma` & `phonopy-2.9.3/example/SnO2/vaspruns.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/TiO2-anatase/FORCE_SETS` & `phonopy-2.9.3/example/TiO2-anatase/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/TiO2-anatase/POSCAR-unitcell` & `phonopy-2.9.3/example/TiO2-anatase/POSCAR-unitcell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/TiO2-anatase/phonopy_disp.yaml` & `phonopy-2.9.3/example/TiO2-anatase/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/TiO2-anatase/vaspruns.tar.lzma` & `phonopy-2.9.3/example/TiO2-anatase/vaspruns.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/ZnO/FORCE_SETS` & `phonopy-2.9.3/example/ZnO/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/ZnO/phonopy_disp.yaml` & `phonopy-2.9.3/example/ZnO/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/ZnO/vaspruns.tar.lzma` & `phonopy-2.9.3/example/ZnO/vaspruns.tar.lzma`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/ase/8Si-phonon.py` & `phonopy-2.9.3/example/ase/8Si-phonon.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/diamond-FHI-aims/README.md` & `phonopy-2.9.3/example/diamond-FHI-aims/README.md`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/diamond-FHI-aims/disp-001/aims.out` & `phonopy-2.9.3/example/diamond-FHI-aims/disp-001/aims.out`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/diamond-FHI-aims/disp-001/control.in` & `phonopy-2.9.3/example/diamond-FHI-aims/disp-001/control.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/diamond-FHI-aims/disp-001/geometry.in` & `phonopy-2.9.3/example/diamond-FHI-aims/disp-001/geometry.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/diamond-FHI-aims/geometry.in` & `phonopy-2.9.3/example/diamond-FHI-aims/geometry.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/diamond-dftb/README` & `phonopy-2.9.3/example/diamond-dftb/README`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/diamond-dftb/dftb_in.hsd` & `phonopy-2.9.3/example/diamond-dftb/dftb_in.hsd`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/diamond-dftb/geo.gen` & `phonopy-2.9.3/example/diamond-dftb/geo.gen`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/example/diamond-dftb/results.tag` & `phonopy-2.9.3/example/diamond-dftb/results.tag`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/__init__.py` & `phonopy-2.9.3/phonopy/__init__.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/api_gruneisen.py` & `phonopy-2.9.3/phonopy/api_gruneisen.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/api_phonopy.py` & `phonopy-2.9.3/phonopy/api_phonopy.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/api_qha.py` & `phonopy-2.9.3/phonopy/api_qha.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/cui/collect_cell_info.py` & `phonopy-2.9.3/phonopy/cui/collect_cell_info.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/cui/create_force_sets.py` & `phonopy-2.9.3/phonopy/cui/create_force_sets.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/cui/load.py` & `phonopy-2.9.3/phonopy/cui/load.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/cui/load_helper.py` & `phonopy-2.9.3/phonopy/cui/load_helper.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/cui/phonopy_argparse.py` & `phonopy-2.9.3/phonopy/cui/phonopy_argparse.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/cui/phonopy_script.py` & `phonopy-2.9.3/phonopy/cui/phonopy_script.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/cui/settings.py` & `phonopy-2.9.3/phonopy/cui/settings.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/cui/show_symmetry.py` & `phonopy-2.9.3/phonopy/cui/show_symmetry.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/file_IO.py` & `phonopy-2.9.3/phonopy/file_IO.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/gruneisen/__init__.py` & `phonopy-2.9.3/phonopy/gruneisen/__init__.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/gruneisen/band_structure.py` & `phonopy-2.9.3/phonopy/gruneisen/band_structure.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/gruneisen/core.py` & `phonopy-2.9.3/phonopy/gruneisen/core.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/gruneisen/mesh.py` & `phonopy-2.9.3/phonopy/gruneisen/mesh.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/gruneisen/thermal_properties.py` & `phonopy-2.9.3/phonopy/gruneisen/thermal_properties.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/harmonic/derivative_dynmat.py` & `phonopy-2.9.3/phonopy/harmonic/derivative_dynmat.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/harmonic/displacement.py` & `phonopy-2.9.3/phonopy/harmonic/displacement.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/harmonic/dynamical_matrix.py` & `phonopy-2.9.3/phonopy/harmonic/dynamical_matrix.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/harmonic/dynmat_to_fc.py` & `phonopy-2.9.3/phonopy/harmonic/dynmat_to_fc.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/harmonic/force_constants.py` & `phonopy-2.9.3/phonopy/harmonic/force_constants.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/__init__.py` & `phonopy-2.9.3/phonopy/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/abinit.py` & `phonopy-2.9.3/phonopy/interface/abinit.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/aims.py` & `phonopy-2.9.3/phonopy/interface/aims.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/alm.py` & `phonopy-2.9.3/phonopy/interface/alm.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/calculator.py` & `phonopy-2.9.3/phonopy/interface/calculator.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/castep.py` & `phonopy-2.9.3/phonopy/interface/castep.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/cif.py` & `phonopy-2.9.3/phonopy/interface/cif.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/cp2k.py` & `phonopy-2.9.3/phonopy/interface/cp2k.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/crystal.py` & `phonopy-2.9.3/phonopy/interface/crystal.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/dftbp.py` & `phonopy-2.9.3/phonopy/interface/dftbp.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/elk.py` & `phonopy-2.9.3/phonopy/interface/elk.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/fc_calculator.py` & `phonopy-2.9.3/phonopy/interface/fc_calculator.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/fleur.py` & `phonopy-2.9.3/phonopy/interface/fleur.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/hiphive_interface.py` & `phonopy-2.9.3/phonopy/interface/hiphive_interface.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/phonopy_yaml.py` & `phonopy-2.9.3/phonopy/interface/phonopy_yaml.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/qe.py` & `phonopy-2.9.3/phonopy/interface/qe.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/siesta.py` & `phonopy-2.9.3/phonopy/interface/siesta.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/turbomole.py` & `phonopy-2.9.3/phonopy/interface/turbomole.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/vasp.py` & `phonopy-2.9.3/phonopy/interface/vasp.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/interface/wien2k.py` & `phonopy-2.9.3/phonopy/interface/wien2k.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/animation.py` & `phonopy-2.9.3/phonopy/phonon/animation.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/band_structure.py` & `phonopy-2.9.3/phonopy/phonon/band_structure.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/character_table.py` & `phonopy-2.9.3/phonopy/phonon/character_table.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/degeneracy.py` & `phonopy-2.9.3/phonopy/phonon/degeneracy.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/dos.py` & `phonopy-2.9.3/phonopy/phonon/dos.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/group_velocity.py` & `phonopy-2.9.3/phonopy/phonon/group_velocity.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/irreps.py` & `phonopy-2.9.3/phonopy/phonon/irreps.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/mesh.py` & `phonopy-2.9.3/phonopy/phonon/mesh.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/modulation.py` & `phonopy-2.9.3/phonopy/phonon/modulation.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/moment.py` & `phonopy-2.9.3/phonopy/phonon/moment.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/qpoints.py` & `phonopy-2.9.3/phonopy/phonon/qpoints.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/random_displacements.py` & `phonopy-2.9.3/phonopy/phonon/random_displacements.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/tetrahedron_mesh.py` & `phonopy-2.9.3/phonopy/phonon/tetrahedron_mesh.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/thermal_displacement.py` & `phonopy-2.9.3/phonopy/phonon/thermal_displacement.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/phonon/thermal_properties.py` & `phonopy-2.9.3/phonopy/phonon/thermal_properties.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/qha/__init__.py` & `phonopy-2.9.3/phonopy/qha/__init__.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/qha/core.py` & `phonopy-2.9.3/phonopy/qha/core.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/qha/electron.py` & `phonopy-2.9.3/phonopy/qha/electron.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/qha/eos.py` & `phonopy-2.9.3/phonopy/qha/eos.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/spectrum/dynamic_structure_factor.py` & `phonopy-2.9.3/phonopy/spectrum/dynamic_structure_factor.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/spectrum/velocity.py` & `phonopy-2.9.3/phonopy/spectrum/velocity.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/structure/atoms.py` & `phonopy-2.9.3/phonopy/structure/atoms.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/structure/brillouin_zone.py` & `phonopy-2.9.3/phonopy/structure/brillouin_zone.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/structure/cells.py` & `phonopy-2.9.3/phonopy/structure/cells.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/structure/dataset.py` & `phonopy-2.9.3/phonopy/structure/dataset.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/structure/grid_points.py` & `phonopy-2.9.3/phonopy/structure/grid_points.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/structure/snf.py` & `phonopy-2.9.3/phonopy/structure/snf.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/structure/symmetry.py` & `phonopy-2.9.3/phonopy/structure/symmetry.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/structure/tetrahedron_method.py` & `phonopy-2.9.3/phonopy/structure/tetrahedron_method.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/unfolding/__init__.py` & `phonopy-2.9.3/phonopy/unfolding/__init__.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/unfolding/core.py` & `phonopy-2.9.3/phonopy/unfolding/core.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/units.py` & `phonopy-2.9.3/phonopy/units.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/phonopy/version.py` & `phonopy-2.9.3/phonopy/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 # BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.9.2"
+__version__ = "2.9.3"
```

### Comparing `phonopy-2.9.2/phonopy.egg-info/SOURCES.txt` & `phonopy-2.9.3/phonopy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 MANIFEST.in
 README.md
 __nanoversion__.txt
 pyproject.toml
 setup.py
 c/_phonopy.c
 c/derivative_dynmat.c
+c/derivative_dynmat.h
 c/dynmat.c
+c/dynmat.h
 c/kgrid.c
+c/kgrid.h
 c/phonopy.c
+c/phonopy.h
 c/tetrahedron_method.c
+c/tetrahedron_method.h
 example/Al-Fleur/FORCES
 example/Al-Fleur/README
 example/Al-Fleur/fleur_inpgen
 example/Al-Fleur/phonopy_disp.yaml
 example/Al-Fleur/supercell-001.in
 example/Al-Fleur/IO/inp.xml
 example/Al-Fleur/IO/kpts.xml
```

### Comparing `phonopy-2.9.2/scripts/phonopy` & `phonopy-2.9.3/scripts/phonopy`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-bandplot` & `phonopy-2.9.3/scripts/phonopy-bandplot`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-calc-convert` & `phonopy-2.9.3/scripts/phonopy-calc-convert`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-crystal-born` & `phonopy-2.9.3/scripts/phonopy-crystal-born`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-gruneisen` & `phonopy-2.9.3/scripts/phonopy-gruneisen`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-gruneisenplot` & `phonopy-2.9.3/scripts/phonopy-gruneisenplot`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-load` & `phonopy-2.9.3/scripts/phonopy-load`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-pdosplot` & `phonopy-2.9.3/scripts/phonopy-pdosplot`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-propplot` & `phonopy-2.9.3/scripts/phonopy-propplot`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-qha` & `phonopy-2.9.3/scripts/phonopy-qha`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-tdplot` & `phonopy-2.9.3/scripts/phonopy-tdplot`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-vasp-born` & `phonopy-2.9.3/scripts/phonopy-vasp-born`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/scripts/phonopy-vasp-efe` & `phonopy-2.9.3/scripts/phonopy-vasp-efe`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/setup.py` & `phonopy-2.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/FORCE_SETS_NaCl` & `phonopy-2.9.3/test/FORCE_SETS_NaCl`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/FORCE_SETS_SnO2` & `phonopy-2.9.3/test/FORCE_SETS_SnO2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/FORCE_SETS_TiO2` & `phonopy-2.9.3/test/FORCE_SETS_TiO2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/POSCAR_NaCl` & `phonopy-2.9.3/test/POSCAR_NaCl`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/conftest.py` & `phonopy-2.9.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/harmonic/comm_points.dat` & `phonopy-2.9.3/test/harmonic/comm_points.dat`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/harmonic/test_dynamical_matrix.py` & `phonopy-2.9.3/test/harmonic/test_dynamical_matrix.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/harmonic/test_dynmat_to_fc.py` & `phonopy-2.9.3/test/harmonic/test_dynmat_to_fc.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/harmonic/test_force_constants.py` & `phonopy-2.9.3/test/harmonic/test_force_constants.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/BaGa2-wien2k.yaml` & `phonopy-2.9.3/test/interface/BaGa2-wien2k.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/BaGa2.struct` & `phonopy-2.9.3/test/interface/BaGa2.struct`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/FORCE_SETS_NaCl` & `phonopy-2.9.3/test/interface/FORCE_SETS_NaCl`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/NaCl-abinit-pwscf.yaml` & `phonopy-2.9.3/test/interface/NaCl-abinit-pwscf.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/NaCl-abinit.in` & `phonopy-2.9.3/test/interface/NaCl-abinit.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/NaCl-castep.cell` & `phonopy-2.9.3/test/interface/NaCl-castep.cell`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/NaCl-castep.yaml` & `phonopy-2.9.3/test/interface/NaCl-castep.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/NaCl-pwscf.in` & `phonopy-2.9.3/test/interface/NaCl-pwscf.in`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/NaCl-vasp.yaml` & `phonopy-2.9.3/test/interface/NaCl-vasp.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/Si-CP2K.yaml` & `phonopy-2.9.3/test/interface/Si-CP2K.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/Si-CRYSTAL.o` & `phonopy-2.9.3/test/interface/Si-CRYSTAL.o`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/Si-TURBOMOLE-control` & `phonopy-2.9.3/test/interface/Si-TURBOMOLE-control`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/Si-TURBOMOLE.yaml` & `phonopy-2.9.3/test/interface/Si-TURBOMOLE.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/phonopy.yaml` & `phonopy-2.9.3/test/interface/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/test_CP2K.py` & `phonopy-2.9.3/test/interface/test_CP2K.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/test_CRYSTAL.py` & `phonopy-2.9.3/test/interface/test_CRYSTAL.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/test_TURBOMOLE.py` & `phonopy-2.9.3/test/interface/test_TURBOMOLE.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/test_abinit.py` & `phonopy-2.9.3/test/interface/test_abinit.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/test_castep.py` & `phonopy-2.9.3/test/interface/test_castep.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/test_phonopy_yaml.py` & `phonopy-2.9.3/test/interface/test_phonopy_yaml.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/test_pwscf.py` & `phonopy-2.9.3/test/interface/test_pwscf.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/test_vasp.py` & `phonopy-2.9.3/test/interface/test_vasp.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/test_wien2k.py` & `phonopy-2.9.3/test/interface/test_wien2k.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/interface/vasprun.xml.tar.bz2` & `phonopy-2.9.3/test/interface/vasprun.xml.tar.bz2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_Amm2` & `phonopy-2.9.3/test/phonon/FORCE_SETS_Amm2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_I4_1a` & `phonopy-2.9.3/test/phonon/FORCE_SETS_I4_1a`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P-3m1` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P-3m1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P-4` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P-4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P-42_1m` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P-42_1m`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P-43m` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P-43m`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P-6` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P-6`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P-6m2` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P-6m2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P2` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P222_1` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P222_1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P2_13` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P2_13`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P3m1` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P3m1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P4_1` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P4_1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P4_332` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P4_332`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P4mm` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P4mm`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P6` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P6`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_P6_222` & `phonopy-2.9.3/test/phonon/FORCE_SETS_P6_222`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_Pa-3` & `phonopy-2.9.3/test/phonon/FORCE_SETS_Pa-3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/FORCE_SETS_Pc` & `phonopy-2.9.3/test/phonon/FORCE_SETS_Pc`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_Amm2` & `phonopy-2.9.3/test/phonon/POSCAR_Amm2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_I4_1a` & `phonopy-2.9.3/test/phonon/POSCAR_I4_1a`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P-3m1` & `phonopy-2.9.3/test/phonon/POSCAR_P-3m1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P-4` & `phonopy-2.9.3/test/phonon/POSCAR_P-4`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P-42_1m` & `phonopy-2.9.3/test/phonon/POSCAR_P-42_1m`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P-43m` & `phonopy-2.9.3/test/phonon/POSCAR_P-43m`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P-6` & `phonopy-2.9.3/test/phonon/POSCAR_P-6`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P-6m2` & `phonopy-2.9.3/test/phonon/POSCAR_P-6m2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P2` & `phonopy-2.9.3/test/phonon/POSCAR_P2`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P222_1` & `phonopy-2.9.3/test/phonon/POSCAR_P222_1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P2_13` & `phonopy-2.9.3/test/phonon/POSCAR_P2_13`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P4_1` & `phonopy-2.9.3/test/phonon/POSCAR_P4_1`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P4_332` & `phonopy-2.9.3/test/phonon/POSCAR_P4_332`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P4mm` & `phonopy-2.9.3/test/phonon/POSCAR_P4mm`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P6` & `phonopy-2.9.3/test/phonon/POSCAR_P6`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_P6_222` & `phonopy-2.9.3/test/phonon/POSCAR_P6_222`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_Pa-3` & `phonopy-2.9.3/test/phonon/POSCAR_Pa-3`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/POSCAR_Pc` & `phonopy-2.9.3/test/phonon/POSCAR_Pc`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/eigvecs_ii_TiPN3.txt` & `phonopy-2.9.3/test/phonon/eigvecs_ii_TiPN3.txt`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/eigvecs_ij_TiPN3.txt` & `phonopy-2.9.3/test/phonon/eigvecs_ij_TiPN3.txt`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_band_structure.py` & `phonopy-2.9.3/test/phonon/test_band_structure.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_dos.py` & `phonopy-2.9.3/test/phonon/test_dos.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_irreps.py` & `phonopy-2.9.3/test/phonon/test_irreps.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_mesh.py` & `phonopy-2.9.3/test/phonon/test_mesh.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_moment.py` & `phonopy-2.9.3/test/phonon/test_moment.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_qpoints.py` & `phonopy-2.9.3/test/phonon/test_qpoints.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_random_displacements.py` & `phonopy-2.9.3/test/phonon/test_random_displacements.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_tetrahedron_mesh.py` & `phonopy-2.9.3/test/phonon/test_tetrahedron_mesh.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_thermal_displacement.py` & `phonopy-2.9.3/test/phonon/test_thermal_displacement.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonon/test_thermal_properties.py` & `phonopy-2.9.3/test/phonon/test_thermal_properties.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonopy_disp_NaCl.yaml` & `phonopy-2.9.3/test/phonopy_disp_NaCl.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonopy_disp_SnO2.yaml` & `phonopy-2.9.3/test/phonopy_disp_SnO2.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonopy_disp_TiO2.yaml` & `phonopy-2.9.3/test/phonopy_disp_TiO2.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonopy_params_TiPN3.yaml.xz` & `phonopy-2.9.3/test/phonopy_params_TiPN3.yaml.xz`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/phonopy_params_Zr3N4.yaml` & `phonopy-2.9.3/test/phonopy_params_Zr3N4.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/qha/test_electron.py` & `phonopy-2.9.3/test/qha/test_electron.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/spectrum/XDATCAR` & `phonopy-2.9.3/test/spectrum/XDATCAR`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/spectrum/test_dynamic_structure_factor.py` & `phonopy-2.9.3/test/spectrum/test_dynamic_structure_factor.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/spectrum/test_velocity.py` & `phonopy-2.9.3/test/spectrum/test_velocity.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/spectrum/velocities.dat` & `phonopy-2.9.3/test/spectrum/velocities.dat`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/structure/Si-conv.yaml` & `phonopy-2.9.3/test/structure/Si-conv.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/structure/SiO2-123.yaml` & `phonopy-2.9.3/test/structure/SiO2-123.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/structure/test_atoms.py` & `phonopy-2.9.3/test/structure/test_atoms.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/structure/test_brillouin_zone.py` & `phonopy-2.9.3/test/structure/test_brillouin_zone.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/structure/test_cells.py` & `phonopy-2.9.3/test/structure/test_cells.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/structure/test_grid_points.py` & `phonopy-2.9.3/test/structure/test_grid_points.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/structure/test_symmetry.py` & `phonopy-2.9.3/test/structure/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/structure/test_tetrahedron_method.py` & `phonopy-2.9.3/test/structure/test_tetrahedron_method.py`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/structure/tio2_qpoints.yaml` & `phonopy-2.9.3/test/structure/tio2_qpoints.yaml`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/unfolding/FORCE_SETS` & `phonopy-2.9.3/test/unfolding/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/unfolding/bin-unfolding.dat` & `phonopy-2.9.3/test/unfolding/bin-unfolding.dat`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/unfolding/bin-unfolding_to_atoms.dat` & `phonopy-2.9.3/test/unfolding/bin-unfolding_to_atoms.dat`

 * *Files identical despite different names*

### Comparing `phonopy-2.9.2/test/unfolding/test_unfolding.py` & `phonopy-2.9.3/test/unfolding/test_unfolding.py`

 * *Files identical despite different names*

