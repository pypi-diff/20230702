# Comparing `tmp/qepy-0.0.3.tar.gz` & `tmp/qepy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qepy-0.0.3.tar", last modified: Sun Jun  4 21:50:20 2023, max compression
+gzip compressed data, was "qepy-0.0.4.tar", last modified: Sun Jul  2 15:33:56 2023, max compression
```

## Comparing `qepy-0.0.3.tar` & `qepy-0.0.4.tar`

### file list

```diff
@@ -1,258 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.179441 qepy-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.143441 qepy-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-04 21:49:50.000000 qepy-0.0.3/.github/workflows/linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-04 21:49:50.000000 qepy-0.0.3/.github/workflows/macos_arm64.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-04 21:49:50.000000 qepy-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-04 21:49:50.000000 qepy-0.0.3/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-04 21:49:50.000000 qepy-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-04 21:49:50.000000 qepy-0.0.3/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-04 21:49:50.000000 qepy-0.0.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-04 21:50:20.179441 qepy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-04 21:49:50.000000 qepy-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/QEpy.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/contact.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/development/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/development/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/development/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/qepy/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/qepy/calculator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/qepy/driver.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/qepy/io.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/qepy/qepy.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/static/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/doc/source/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.151441 qepy-0.0.3/doc/source/tutorials/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/dirac_exchange.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/dos_band_graphene.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/qepy_scf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/qepy_scf_iterative.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/test_ecutwfc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/test_eos_vc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/jupyter/test_kpoints.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-04 21:49:50.000000 qepy-0.0.3/doc/source/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.151441 qepy-0.0.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.151441 qepy-0.0.3/examples/ase/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/ase/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/ase/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/ase/test_ase_nvt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3360 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/ase/test_ase_scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/clean.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.143441 qepy-0.0.3/examples/develop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.151441 qepy-0.0.3/examples/develop/pw/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/test_pwscf_scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/tmp2energy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/develop/pw/tmp2energy_pw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/examples/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/DATA/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/C.pbe-rrkjus.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/H_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/DATA/O_ONCV_PBE-1.2.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/band/
--rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/band/C.pbe-rrkjus.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/band/dos_band_graphene.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/colab/
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/colab/qepy_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/eos/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/eos/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/eos/test_eos_slow.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/eos/test_eos_vc.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/ext/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/ext/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/ext/dftpy_xc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/ext/dirac_exchange.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.155441 qepy-0.0.3/examples/jupyter/nvt/
--rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/nvt/H_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/nvt/O_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/nvt/ase_nvt.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/nvt/qe_in.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.159441 qepy-0.0.3/examples/jupyter/pp/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/pp.in
--rw-r--r--   0 runner    (1001) docker     (123)    33477 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/qepy_elf_rdg.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/qepy_parse_output.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    28575 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/pp/qepy_potentials.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.159441 qepy-0.0.3/examples/jupyter/scf/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/dftpy_mixer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qe_in.in
--rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qepy_iterative.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qepy_qeinput.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qepy_scf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/scf/qepy_scf_iterative.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.159441 qepy-0.0.3/examples/jupyter/testing/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/testing/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/testing/test_degauss.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/testing/test_ecutwfc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/jupyter/testing/test_kpoints.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/examples/opt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/opt/ase/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/opt/ase/out/
--rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/out/ase.out
--rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/out/qepy.out
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/si_pbe_v1.uspp.F.UPF
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/test_ase_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/ase/vcrelax.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/opt/qe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/opt/qe/out/
--rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/out/qepy.out
--rw-r--r--   0 runner    (1001) docker     (123)    90822 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/out/ref.out
--rwxr-xr-x   0 runner    (1001) docker     (123)     2171 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/qe_relax.py
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/si_pbe_v1.uspp.F.UPF
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/opt/qe/vcrelax.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/examples/original/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/original/6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.5/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.5/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.5/run_pwscf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.163441 qepy-0.0.3/examples/original/6.8/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.8/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.8/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/original/6.8/run_pwscf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/scf/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/test_pwscf_iterative.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/test_readfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/scf/test_readfile_pw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/tddft/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/tddft/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/tddft/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      743 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/tddft/test_ce_tddft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/tddft/test_ce_tddft_restart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/al_md_3.traj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/oldxml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/Al_ONCV_PBE-1.2.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/K00001/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/K00001/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/charge-density.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.save/data-file.xml
--rw-r--r--   0 runner    (1001) docker     (123)   804960 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml/al_oldxml.wfc1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/examples/test/DATA/oldxml_collect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.167441 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/Al_ONCV_PBE-1.2.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   808502 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    32091 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/gkvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/charge-density.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/data-file.xml
--rw-r--r--   0 runner    (1001) docker     (123)   185540 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/oldxml_collect/al_oldxml.save/gvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/qe_fake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/DATA/qe_in.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/examples/test/qe-6.5/
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_ce_tddft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_comm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1461 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_oldxml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1360 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1364 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_pwscf_scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/qe-6.5/test_readfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_ase_md.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_ce_tddft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_oldxml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_pwscf_iterative.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-06-04 21:49:50.000000 qepy-0.0.3/examples/test/test_readfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/install/
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-04 21:49:50.000000 qepy-0.0.3/install/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-04 21:49:50.000000 qepy-0.0.3/install/Makefile.cetddft
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-04 21:49:50.000000 qepy-0.0.3/install/kind_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-04 21:49:50.000000 qepy-0.0.3/install/make.depend
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-04 21:49:50.000000 qepy-0.0.3/install/make.depend.cetddft
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-04 21:49:50.000000 qepy-0.0.3/install/make.qe.inc
--rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-06-04 21:49:50.000000 qepy-0.0.3/install/makedeps.sh
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-04 21:49:50.000000 qepy-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/qepy/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/__new__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/qepy/cui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/cui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/cui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/cui/pwx.py
--rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-06-04 21:49:50.000000 qepy-0.0.3/qepy/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/qepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:50:19.000000 qepy-0.0.3/qepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 21:50:20.000000 qepy-0.0.3/qepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 21:50:20.179441 qepy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-04 21:49:50.000000 qepy-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.147441 qepy-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.171441 qepy-0.0.3/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-06-04 21:49:50.000000 qepy-0.0.3/src/api/qepy_common.f90
--rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-04 21:49:50.000000 qepy-0.0.3/src/api/qepy_mod.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-06-04 21:49:50.000000 qepy-0.0.3/src/cmd/command_line_options.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-04 21:49:50.000000 qepy-0.0.3/src/cmd/pwscf.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/fix/
--rw-r--r--   0 runner    (1001) docker     (123)    66035 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/funct.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/potinit.f90
--rw-r--r--   0 runner    (1001) docker     (123)    56596 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/pw_restart_new.f90
--rw-r--r--   0 runner    (1001) docker     (123)   360829 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/qes_read_module.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/read_file_new.f90
--rw-r--r--   0 runner    (1001) docker     (123)    50735 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/scatter_mod.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-04 21:49:50.000000 qepy-0.0.3/src/fix/wfcinit.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/ldau/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-04 21:49:50.000000 qepy-0.0.3/src/ldau/qepy_econf.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     6276 2023-06-04 21:49:50.000000 qepy-0.0.3/src/ldau/qepy_ldau_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/oldxml/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_io_rho_xml.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_potinit.f90
--rw-r--r--   0 runner    (1001) docker     (123)   105084 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_pw_restart.f90
--rw-r--r--   0 runner    (1001) docker     (123)   176393 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_qexml.f90
--rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_read_file.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_wfcinit.f90
--rw-r--r--   0 runner    (1001) docker     (123)    40621 2023-06-04 21:49:50.000000 qepy-0.0.3/src/oldxml/oldxml_xml_io_base.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.175441 qepy-0.0.3/src/qe/
--rw-r--r--   0 runner    (1001) docker     (123)    61363 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_electrons.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_electrons_nscf.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_hinit1.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_init_run.f90
--rw-r--r--   0 runner    (1001) docker     (123)    61917 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_pw2casino_write.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_pwscf.f90
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_run_pwscf.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_setlocal.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_stop_run.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_stress.f90
--rw-r--r--   0 runner    (1001) docker     (123)    38870 2023-06-04 21:49:50.000000 qepy-0.0.3/src/qe/qepy_v_of_rho.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:50:20.179441 qepy-0.0.3/src/tddft/
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_molecule_optical_absorption.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_common.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_main.f90
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_mod.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_routines.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_tddft_setup.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-04 21:49:50.000000 qepy-0.0.3/src/tddft/qepy_update_ham.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:33:56.891496 qepy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-02 15:33:56.891496 qepy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-02 15:33:28.000000 qepy-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-02 15:33:28.000000 qepy-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:33:56.887496 qepy-0.0.4/qepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/__new__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:33:56.887496 qepy-0.0.4/qepy/cui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/cui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/cui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/cui/pwx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36869 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-07-02 15:33:28.000000 qepy-0.0.4/qepy/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:33:56.887496 qepy-0.0.4/qepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-02 15:33:56.000000 qepy-0.0.4/qepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-02 15:33:56.000000 qepy-0.0.4/qepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:33:56.000000 qepy-0.0.4/qepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:33:56.000000 qepy-0.0.4/qepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-02 15:33:56.000000 qepy-0.0.4/qepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-02 15:33:56.000000 qepy-0.0.4/qepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:33:56.891496 qepy-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-07-02 15:33:28.000000 qepy-0.0.4/setup.py
```

### Comparing `qepy-0.0.3/PKG-INFO` & `qepy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qepy
-Version: 0.0.3
+Version: 0.0.4
 Summary: QEpy: Quantum ESPRESSO Python interface
 Home-page: https://gitlab.com/shaoxc/qepy
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qepy-0.0.3/README.md` & `qepy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy/__init__.py` & `qepy-0.0.4/qepy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,25 @@
                     attr = mod + '.' + item
                     operator.attrgetter(attr)(qepy).clear()
 
 
 qepy_clean_saved()
 __author__ = "Pavanello Research Group"
 __contact__ = "m.pavanello@rutgers.edu"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __license__ = "GPL"
-__date__ = "2023-06-03"
+__date__ = "2023-07-02"
 
 try:
     from importlib.metadata import version # python >= 3.8
 except Exception :
     try:
         from importlib_metadata import version
     except Exception :
         pass
 
 try:
     __version__ = version("qepy")
 except Exception :
     pass
+
+from qepy.driver import Driver
```

### Comparing `qepy-0.0.3/qepy/__new__.py` & `qepy-0.0.4/qepy/__new__.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy/calculator.py` & `qepy-0.0.4/qepy/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,17 +259,17 @@
     def get_potential_energy(self, atoms = None, **kwargs):
         """See :func:`qepy.driver.Driver.get_potential_energy`"""
         self.update_optimizer(atoms)
         return self.driver.get_energy(**kwargs) * units['Ry']
 
     def get_forces(self, atoms = None, icalc = 0):
         """See :func:`qepy.driver.Driver.get_forces`"""
-        if self.update_optimizer(atoms) or self._forces is None:
-            self._forces = self.driver.get_forces(icalc=icalc)* units['Ry'] / units['Bohr']
-        return self._forces
+        if self.update_optimizer(atoms) or 'forces' not in self.results :
+            self.results['forces'] = self.driver.get_forces(icalc=icalc)* units['Ry'] / units['Bohr']
+        return self.results['forces']
 
     def get_dos(self, qe_options = None, spin = None, inputfile = None, **kwargs):
         """ calculate density of states (DOS) and return the tuple (energies, dos)
 
         Parameters
         ----------
         qe_options : dict
@@ -339,20 +339,20 @@
         self.driver.non_scf()
 
         band = get_band_structure(calc = self, path = kpts, reference=reference)
         return band
 
     def get_stress(self, atoms = None):
         """Return the stress tensor in the Voigt order (xx, yy, zz, yz, xz, xy)"""
-        if self.update_optimizer(atoms) or self._stress is None:
+        if self.update_optimizer(atoms) or 'stress' not in self.results :
             stress = self.driver.get_stress()
-            self._stress = np.array(
+            self.results['stress'] = np.array(
                 [stress[0, 0], stress[1, 1], stress[2, 2],
                  stress[1, 2], stress[0, 2], stress[0, 1]]) * -1 * units['Ry'] / (units['Bohr'] ** 3)
-        return self._stress
+        return self.results['stress']
 
     def get_number_of_bands(self):
         """See :func:`qepy.driver.Driver.get_number_of_bands`"""
         return self.driver.get_number_of_bands()
 
     def get_xc_functional(self):
         """See :func:`qepy.driver.Driver.get_xc_functional`"""
```

### Comparing `qepy-0.0.3/qepy/core.py` & `qepy-0.0.4/qepy/core.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy/cui/main.py` & `qepy-0.0.4/qepy/cui/main.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy/cui/pwx.py` & `qepy-0.0.4/qepy/cui/pwx.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy/driver.py` & `qepy-0.0.4/qepy/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
              + energy : Ry
              + forces : Ry/Bohr
              + stress : Ry/Bohr**3
              + potential : Ry
              + density : 1.0/Bohr**3
 
     """
+    POTNAMES = {'external' : 0, 'localpp' : 1, 'hartree' : 2, 'xc' : 4}
+    FORCENAMES = {'ewald' : 1, 'localpp' : 2, 'nlcc' : 4}
 
     def __init__(self, inputfile = None, comm = None, ldescf = False, iterative = False,
              task = 'scf', embed = None, prefix = None, outdir = None, logfile = None,
              qe_options = None, prog = 'pw', progress = False, atoms = None, needwf = True,
              **kwargs):
         if embed is None :
             embed = qepy.qepy_common.embed_base()
@@ -112,14 +114,16 @@
         self.qe_options = qe_options
         self.prog = prog
         self.progress = progress
         self.atoms = atoms
         self.needwf = needwf
         #
         self.embed.ldescf = ldescf
+        self.embed.iterative = iterative
+        self.embed.tddft.iterative = iterative
         #
         self.comm = comm
         self.qepy = qepy
         self.qeinput = QEInput()
         #
         self.driver_initialize()
 
@@ -188,16 +192,14 @@
 
         Parameters
         ----------
         inputfile : str
             Name of QE input file
         commf : object
             Parallel communicator (Fortran)
-        iterative : bool
-            Iteratively run the scf or tddft
         task : str
             Task of the driver :
 
               - 'scf' : scf task
               - 'optical' : Optical absorption spectrum (TDDFT)
               - 'nscf' : read file from scf
 
@@ -241,15 +243,14 @@
                     qepy.read_file()
                 else :
                     qepy.read_file_new(False)
             if self.needwf :
                 qepy.qepy_mod.qepy_open_files()
         else :
             qepy.qepy_pwscf(inputfile, commf)
-            self.embed.iterative = self.iterative
             if self.embed.iterative :
                 qepy.control_flags.set_niter(1)
         #
         self.density = np.zeros((1, 1))
         self.iter = 0
 
     def tddft_initialize(self, inputfile = None, commf = None, **kwargs):
@@ -268,27 +269,29 @@
         if self.progress :
             qepy.wvfct.get_array_g2kin()
             qepy.qepy_tddft_readin(inputfile)
         else :
             qepy.qepy_tddft_main_initial(inputfile, commf)
             qepy.read_file()
         qepy.qepy_tddft_main_setup()
-        self.embed.tddft.iterative = self.iterative
 
-    def diagonalize(self, print_level = 2, **kwargs):
+    def diagonalize(self, print_level = 2, nscf = False, **kwargs):
         """Diagonalize the hamiltonian
 
         Parameters
         ----------
         print_level :
             The level of output of QE
         """
+        self.embed.lmovecell = False
         self.iter += 1
         if self.task == 'optical' :
             qepy.qepy_molecule_optical_absorption()
+        elif nscf :
+            qepy.qepy_electrons_nscf(print_level, 0)
         else :
             self.embed.mix_coef = -1.0
             qepy.qepy_electrons_scf(print_level, 0)
 
     def mix(self, mix_coef = 0.7, print_level = 2):
         """Mixing the density
 
@@ -317,23 +320,25 @@
     def get_scf_steps(self, **kwargs):
         """Return the number of steps of scf"""
         if self.embed.iterative :
             return self.iter
         else :
             return qepy.control_flags.get_n_scf_steps()
 
-    def scf(self, print_level = 2, maxiter = None, original = False, **kwargs):
+    def scf(self, print_level = 2, maxiter = None, original = False, nscf = False, **kwargs):
         """Run the scf/tddft until converged or maximum number of iterations"""
         if maxiter is not None and not self.embed.iterative :
             qepy.control_flags.set_niter(maxiter)
         if self.task == 'optical' :
             qepy.qepy_molecule_optical_absorption()
         elif not self.embed.iterative and self.embed.exttype < 2 :
             # Use electrons to support hybrid xc functional
             return self.electrons(original=original)
+        elif nscf :
+            qepy.qepy_electrons_nscf(print_level, 0)
         else :
             qepy.qepy_electrons_scf(print_level, 0)
         return self.embed.etotal
 
     def non_scf(self, **kwargs):
         # fix some saved variables from last scf calculations
         qepy.control_flags.set_lscf(0)
@@ -347,60 +352,65 @@
     def electrons(self, original = False, **kwargs):
         if original :
             qepy.electrons()
         else :
             qepy.qepy_electrons()
         return qepy.ener.get_etot()
 
-    def end_scf(self, **kwargs):
+    def end_scf(self, nscf = False, **kwargs):
         """End the scf and clean the scf workspace. Only need run it in iterative mode"""
         if self.embed.iterative :
-            self.embed.finish = True
-            qepy.qepy_electrons_scf(0, 0)
+            if self.task == 'optical' :
+                self.embed.tddft.finish = True
+                qepy.qepy_molecule_optical_absorption()
+            elif nscf :
+                self.embed.finish = True
+                qepy.qepy_electrons_nscf(0, 0)
+            else :
+                self.embed.finish = True
+                qepy.qepy_electrons_scf(0, 0)
 
     def stop(self, exit_status = 0, what = 'all', print_flag = 0, **kwargs):
-        """stop.
+        """stop the driver.
 
         Parameters
         ----------
         exit_status : int
             0 : QE will remove it temporary files
         print_flag : int
             0 : Not print time informations
         what : str
              see :func:`qepy.driver.Driver.save`.
         """
         if self.task == 'optical' :
             self.tddft_stop(exit_status, print_flag = print_flag, what = what, **kwargs)
         else :
+            if not self.embed.initial : self.end_scf()
             qepy.qepy_stop_run(exit_status, print_flag = print_flag, what = what, finalize = False)
 
         if hasattr(self.fileobj, 'close'): self.fileobj.close()
         qepy.qepy_clean_saved()
         #
         env['DRIVER'] = None
         env['STDOUT'] = None
-        #
 
     def tddft_restart(self, istep=None, **kwargs):
         """Restart the tddft from previous interrupted run.
 
         Parameters
         ----------
         istep : int
             Start number of steps, just for output.
         """
         qepy.qepy_tddft_mod.qepy_cetddft_wfc2rho()
         if istep is not None :
             self.embed.tddft.istep = istep
 
     def tddft_stop(self, exit_status = 0, what = 'no', print_flag = 0, **kwargs):
-        if self.embed.tddft.iterative :
-            self.embed.tddft.finish = True
-            qepy.qepy_molecule_optical_absorption()
+        if not self.embed.tddft.initial : self.end_scf()
         #! Do not save the PW files, otherwise the initial wfcs will be overwritten.
         qepy.qepy_stop_run(exit_status, print_flag = print_flag, what = 'no', finalize = False)
         qepy.qepy_stop_tddft(exit_status)
 
     def save(self, what = 'all', **kwargs):
         """
         Save the QE data to the disk
@@ -419,14 +429,15 @@
                            (save density);
           * what = 'config-init' : write xml data file only excluding final results
                                    (for dry run, can be called at early stages).
 
           see PW/src/punch.f90
         """
         qepy.punch(what)
+        # qepy.close_files(False)
 
     def update_run_options(self, qe_options = {}, **kwargs):
         pass
 
     def get_energy(self, **kwargs):
         """Return the total energy."""
         if abs(qepy.ener.get_etot()) > 1E-16 :
@@ -515,14 +526,20 @@
 
     def get_density(self, gather = True, out = None):
         """Return density array in real space."""
         if out is None : out = self.create_array(gather=gather, kind='rho')
         qepy.qepy_mod.qepy_get_rho(out, gather = gather)
         return out
 
+    def get_core_density(self, gather = True, out = None):
+        """Return density array in real space."""
+        if out is None : out = self.create_array(gather=gather, kind='rho')
+        qepy.qepy_mod.qepy_get_rho_core(out, gather = gather)
+        return out
+
     def get_kinetic_energy_density(self, gather = True, out = None):
         """Return density array in real space."""
         if out is None : out = self.create_array(gather=gather, kind='rho')
         qepy.qepy_mod.qepy_get_tau(out, gather = gather)
         return out
 
     def get_wave_function(self, band=None, kpt=0):
@@ -554,32 +571,30 @@
     def set_external_potential(self, potential, exttype = None, gather = True, extene  = None, **kwargs):
         """Set the external potential.
 
         Parameters
         ----------
         potential : (nnr, nspin)
             The external potential
-        exttype : int
-            The type of external potential
+        exttype : list or int
+            The type of external potential. It can be a list of name or a integer.
+            e.g.  `exttype = ('localpp', 'xc')` or `exttype = 5`
 
                  ==== ============================== ===
                  type potential                      bin
                  ==== ============================== ===
                   0   external                       000
-                  1   pseudo                         001
+                  1   localpp                        001
                   2   hartree                        010
-                  3   pseudo + hartree               011
                   4   xc                             100
-                  5   pseudo + xc                    101
-                  6   hartree + xc                   110
-                  7   pseudo + hartree + xc          111
                  ==== ============================== ===
 
         """
         if exttype is not None :
+            if not isinstance(exttype, int): exttype = self.potname2type(exttype)
             self.embed.exttype = exttype
         if extene is not None :
             self.embed.extene = extene
         else :
             self.embed.extene = 0.0
         #
         if potential is None : potential = np.zeros((1, 1))
@@ -700,34 +715,37 @@
 
 #-----------------------------------------------------------------------
     #ASE Calculator
     def get_potential_energy(self, **kwargs):
         """Return the potential energy."""
         return self.get_energy()
 
-    def get_forces(self, icalc = 0, **kwargs):
+    def get_forces(self, icalc = 0, ignore = (), **kwargs):
         """Return the total forces. (n, 3)
 
         Parameters
         ----------
         icalc : int
 
             ===== ============================= ===
             icalc without                       bin
             ===== ============================= ===
               0   all                           000
               1   no ewald                      001
-              2   no local                      010
-              3   no ewald + local              011
+              2   no localpp                    010
               4   no nlcc                       100
-              5   no ewald + nlcc               101
-              6   no local + nlcc               110
-              7   no ewald + local + nlcc       111
             ===== ============================= ===
+        ignore : list
+            ignore some forces, which does same job as `icalc`.
+
+              - ewald (1)
+              - localpp (2)
+              - nlcc (4)
         """
+        if len(ignore) > 0 : icalc = self.forcename2type(ignore)
         qepy.qepy_forces(icalc)
         forces = qepy.force_mod.get_array_force().T
         return forces
 
     @classmethod
     def get_stress(cls, **kwargs):
         """Return the stress (3, 3)."""
@@ -804,20 +822,20 @@
             return evc
         else :
             return evc[:, band]
 
     @classmethod
     def get_eigenvalues(cls, kpt=0, spin=0):
         """Return eigenvalue array."""
-        return qepy.wvfct.get_array_et()[:, kpt]
+        return qepy.wvfct.get_array_et().T[kpt]
 
     @classmethod
     def get_occupation_numbers(cls, kpt=0, spin=0):
         """Return occupation number array."""
-        return qepy.wvfct.get_array_wg()[:, kpt]
+        return qepy.wvfct.get_array_wg().T[kpt]
 
     @classmethod
     def get_fermi_level(cls):
         """Return the Fermi level."""
         return qepy.ener.get_ef()
 
     # def initial_wannier(self, initialwannier, kpointgrid, fixedstates,
@@ -847,15 +865,15 @@
         return nr
     #ASE DFTCalculator END
 #-----------------------------------------------------------------------
 
     @classmethod
     def get_number_of_k_points(cls):
         """Return the number of kpoints."""
-        return qepy.klist.get_nks()
+        return qepy.klist.get_nkstot()
 
     @classmethod
     def get_volume(cls):
         """Return the volume."""
         return qepy.cell_base.get_omega()
 
     @classmethod
@@ -998,7 +1016,36 @@
 
         return pp_options
 
     @classmethod
     def update_exchange_correlation(cls, xc=None, libxc=None, **kwargs):
         if libxc : xc = None
         qepy.qepy_mod.qepy_set_dft(xc)
+
+    @classmethod
+    def sum_band(cls, occupations = None, **kwargs):
+        qepy.qepy_mod.qepy_sum_band(occupations)
+
+    @staticmethod
+    def name2type(dictionary, name):
+        if isinstance(name, int):
+            value = []
+            for k, v in dictionary.items():
+                if name & v == v : value.append(k)
+        else :
+            if isinstance(name, str): name = [name]
+            value = 0
+            for key in name :
+                i = dictionary.get(key, None)
+                if i is None :
+                    raise AttributeError(f"The key '{key}' not in the given dictionary.")
+                value += i
+            return value
+        return value
+
+    @classmethod
+    def potname2type(cls, name):
+        return cls.name2type(cls.POTNAMES, name)
+
+    @classmethod
+    def forcename2type(cls, name = None):
+        return cls.name2type(cls.FORCENAMES, name)
```

### Comparing `qepy-0.0.3/qepy/io.py` & `qepy-0.0.4/qepy/io.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.3/qepy.egg-info/PKG-INFO` & `qepy-0.0.4/qepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qepy
-Version: 0.0.3
+Version: 0.0.4
 Summary: QEpy: Quantum ESPRESSO Python interface
 Home-page: https://gitlab.com/shaoxc/qepy
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qepy-0.0.3/setup.py` & `qepy-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,33 +130,41 @@
 extensions_qepy = Extension(
         "qepy._qepy",
         sources = [],
         )
 
 ext_modules = [extensions_qepy, ]
 
+release = 1
+if release :
+    VERSION = {'version' : __version__}
+else :
+    VERSION = {
+            'use_scm_version': {'version_scheme': 'post-release'},
+            'setup_requires': [
+                'setuptools_scm',
+                'importlib-metadata>=0.12;python_version<"3.8"'],
+            }
+
 if __name__ == "__main__":
     setup(
             name=name,
             url='https://gitlab.com/shaoxc/qepy',
             description=description,
-            version=__version__,
-            # use_scm_version={'version_scheme': 'post-release'},
             author=__author__,
             author_email=__contact__,
             license=__license__,
+            **VERSION,
             long_description=long_description,
             long_description_content_type='text/markdown',
             python_requires = '>=3.7',
             install_requires=[
-                'setuptools_scm',
                 'setuptools<=59.8.0',
                 'numpy>=1.18.0',
                 'f90wrap>=0.2.8',
-                'importlib-metadata>=0.12;python_version<"3.8"'
                 ],
             extras_require={
                 'mpi': [
                     'mpi4py>=3.0.2',
                     ],
                 },
             packages=find_packages('./'),
```

