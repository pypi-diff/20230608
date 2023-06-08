# Comparing `tmp/aiida_nanotech_empa-1.0.0b0.tar.gz` & `tmp/aiida_nanotech_empa-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_nanotech_empa-1.0.0b0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_nanotech_empa-1.0.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_nanotech_empa-1.0.0b0.tar` & `aiida_nanotech_empa-1.0.0b1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0       13 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.codecov.yml
--rw-r--r--   0        0        0       33 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.coveragerc
--rw-r--r--   0        0        0       52 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.flake8
--rw-r--r--   0        0        0      200 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.github/install_cp2k.sh
--rw-r--r--   0        0        0      289 2023-05-15 10:57:56.989751 aiida_nanotech_empa-1.0.0b0/.github/install_qe.sh
--rw-r--r--   0        0        0     1737 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      795 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      135 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/.gitignore
--rw-r--r--   0        0        0     1628 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/LICENSE
--rw-r--r--   0        0        0     2125 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/README.md
--rw-r--r--   0        0        0      189 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/__init__.py
--rw-r--r--   0        0        0       51 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/helpers.py
--rw-r--r--   0        0        0      273 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/__init__.py
--rw-r--r--   0        0        0     9867 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cp2k_gw_parser.py
--rw-r--r--   0        0        0     4706 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cp2k_neb_parser.py
--rw-r--r--   0        0        0     2542 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py
--rw-r--r--   0        0        0     1678 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py
--rw-r--r--   0        0        0     1379 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/pp_parser.py
--rw-r--r--   0        0        0      230 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/__init__.py
--rw-r--r--   0        0        0     3023 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/afm.py
--rw-r--r--   0        0        0     2951 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/hrstm.py
--rw-r--r--   0        0        0     3542 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/overlap.py
--rw-r--r--   0        0        0     2863 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/stm.py
--rw-r--r--   0        0        0      168 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/schedulers/__init__.py
--rw-r--r--   0        0        0     1523 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py
--rw-r--r--   0        0        0     1599 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py
--rw-r--r--   0        0        0        0 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/__init__.py
--rw-r--r--   0        0        0    15829 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/analyze_structure.py
--rw-r--r--   0        0        0     1375 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/common_utils.py
--rw-r--r--   0        0        0     2736 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/cube_utils.py
--rw-r--r--   0        0        0     9994 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py
--rw-r--r--   0        0        0    10034 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/igor.py
--rw-r--r--   0        0        0     5427 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/pymol_render.py
--rw-r--r--   0        0        0     8560 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/stm_tools.py
--rw-r--r--   0        0        0      103 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/version.py
--rw-r--r--   0        0        0        0 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/__init__.py
--rw-r--r--   0        0        0     1147 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/__init__.py
--rw-r--r--   0        0        0    12242 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py
--rw-r--r--   0        0        0     5908 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py
--rw-r--r--   0        0        0    30468 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py
--rw-r--r--   0        0        0     2627 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS
--rw-r--r--   0        0        0     2333 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT
--rw-r--r--   0        0        0   135679 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT
--rw-r--r--   0        0        0   114564 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET
--rw-r--r--   0        0        0   172445 2023-05-15 10:57:56.993751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS
--rw-r--r--   0        0        0   135561 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL
--rw-r--r--   0        0        0      378 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/POTENTIALS_DEFAULT
--rw-r--r--   0        0        0   154582 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all
--rw-r--r--   0        0        0     8385 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml
--rw-r--r--   0        0        0    10869 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini
--rw-r--r--   0        0        0    10601 2023-05-15 10:57:56.997751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini
--rw-r--r--   0        0        0  1959318 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat
--rw-r--r--   0        0        0    10100 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py
--rw-r--r--   0        0        0    13286 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py
--rw-r--r--   0        0        0     8261 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py
--rw-r--r--   0        0        0     5417 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py
--rw-r--r--   0        0        0    12131 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py
--rw-r--r--   0        0        0     6432 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py
--rw-r--r--   0        0        0     9959 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py
--rw-r--r--   0        0        0     3893 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py
--rw-r--r--   0        0        0     6771 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py
--rw-r--r--   0        0        0     5579 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py
--rw-r--r--   0        0        0     1252 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml
--rw-r--r--   0        0        0    12253 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml
--rw-r--r--   0        0        0    11446 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml
--rw-r--r--   0        0        0     7983 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml
--rw-r--r--   0        0        0     9918 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml
--rw-r--r--   0        0        0     1966 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml
--rw-r--r--   0        0        0     7603 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml
--rw-r--r--   0        0        0    14363 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py
--rw-r--r--   0        0        0     4085 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py
--rw-r--r--   0        0        0      812 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/__init__.py
--rw-r--r--   0        0        0     9185 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py
--rw-r--r--   0        0        0     8919 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py
--rw-r--r--   0        0        0     6083 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/common.py
--rw-r--r--   0        0        0     6708 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py
--rw-r--r--   0        0        0     7953 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py
--rw-r--r--   0        0        0     5234 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py
--rw-r--r--   0        0        0    11073 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py
--rw-r--r--   0        0        0    12134 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py
--rw-r--r--   0        0        0    11760 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py
--rw-r--r--   0        0        0    11519 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py
--rw-r--r--   0        0        0       80 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/qe/__init__.py
--rw-r--r--   0        0        0    22418 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/qe/nanoribbon.py
--rw-r--r--   0        0        0     3369 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/conftest.py
--rw-r--r--   0        0        0       96 2023-05-15 10:57:57.005751 aiida_nanotech_empa-1.0.0b0/examples/__init__.py
--rw-r--r--   0        0        0   921233 2023-05-15 10:57:57.009751 aiida_nanotech_empa-1.0.0b0/examples/data/sssp_minimal/C.upf
--rw-r--r--   0        0        0   366195 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/data/sssp_minimal/H.upf
--rw-r--r--   0        0        0       13 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/.gitignore
--rwxr-xr-x   0        0        0     9833 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/aa
--rw-r--r--   0        0        0      558 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/benzene-diradical.xyz
--rw-r--r--   0        0        0      402 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2.xyz
--rw-r--r--   0        0        0      422 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2_no_spin.xyz
--rw-r--r--   0        0        0     2959 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2_on_au111.xyz
--rw-r--r--   0        0        0      467 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2_spin.xyz
--rw-r--r--   0        0        0      572 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h4.xyz
--rw-r--r--   0        0        0     2533 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_ads_gw_ic.py
--rw-r--r--   0        0        0     4739 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_afm.py
--rw-r--r--   0        0        0     2725 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_diag.py
--rw-r--r--   0        0        0     3169 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_fragment_separation.py
--rw-r--r--   0        0        0     4118 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_geo_opt.py
--rw-r--r--   0        0        0     3177 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_gw.py
--rw-r--r--   0        0        0     5394 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_hrstm.py
--rw-r--r--   0        0        0     1934 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_mol_opt_gw.py
--rw-r--r--   0        0        0     5582 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_neb.py
--rw-r--r--   0        0        0     3513 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_orb.py
--rw-r--r--   0        0        0     4089 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_pdos.py
--rw-r--r--   0        0        0     2742 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_phonons.py
--rw-r--r--   0        0        0     2622 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_replica_chain.py
--rw-r--r--   0        0        0     3446 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_stm.py
--rw-r--r--   0        0        0     2145 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_gaussian_casscf.py
--rw-r--r--   0        0        0     1393 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_gaussian_spin.py
--rw-r--r--   0        0        0     2776 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/example_nanoribbon.py
--rw-r--r--   0        0        0      251 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/h2.xyz
--rw-r--r--   0        0        0     2483 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/h2_on_au111.xyz
--rw-r--r--   0        0        0     1568 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/h2_on_hbn.xyz
--rw-r--r--   0        0        0      679 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/examples/workflows/si_bulk.xyz
--rw-r--r--   0        0        0     4743 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/pyproject.toml
--rw-r--r--   0        0        0      253 2023-05-15 10:57:57.013752 aiida_nanotech_empa-1.0.0b0/pytest.ini
--rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 aiida_nanotech_empa-1.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.codecov.yml
+-rw-r--r--   0        0        0       33 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.coveragerc
+-rw-r--r--   0        0        0       52 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.flake8
+-rw-r--r--   0        0        0      200 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.github/install_cp2k.sh
+-rw-r--r--   0        0        0      289 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.github/install_qe.sh
+-rw-r--r--   0        0        0     1737 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      795 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      135 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.gitignore
+-rw-r--r--   0        0        0     1628 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     2277 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/README.md
+-rw-r--r--   0        0        0      189 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/__init__.py
+-rw-r--r--   0        0        0       51 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/helpers.py
+-rw-r--r--   0        0        0      273 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/__init__.py
+-rw-r--r--   0        0        0     9867 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cp2k_gw_parser.py
+-rw-r--r--   0        0        0     4846 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cp2k_neb_parser.py
+-rw-r--r--   0        0        0     2542 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py
+-rw-r--r--   0        0        0     1678 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py
+-rw-r--r--   0        0        0     1379 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/pp_parser.py
+-rw-r--r--   0        0        0      230 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/__init__.py
+-rw-r--r--   0        0        0     3023 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/afm.py
+-rw-r--r--   0        0        0     2951 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/hrstm.py
+-rw-r--r--   0        0        0     3542 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/overlap.py
+-rw-r--r--   0        0        0     2863 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/stm.py
+-rw-r--r--   0        0        0      168 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/__init__.py
+-rw-r--r--   0        0        0     1523 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py
+-rw-r--r--   0        0        0     1599 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/__init__.py
+-rw-r--r--   0        0        0    15829 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/analyze_structure.py
+-rw-r--r--   0        0        0     1375 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/common_utils.py
+-rw-r--r--   0        0        0     2736 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/cube_utils.py
+-rw-r--r--   0        0        0     9994 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py
+-rw-r--r--   0        0        0    10034 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/igor.py
+-rw-r--r--   0        0        0     5427 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/pymol_render.py
+-rw-r--r--   0        0        0     8560 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/stm_tools.py
+-rw-r--r--   0        0        0      103 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/version.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/__init__.py
+-rw-r--r--   0        0        0    11867 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py
+-rw-r--r--   0        0        0     6154 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py
+-rw-r--r--   0        0        0    31717 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py
+-rw-r--r--   0        0        0     2627 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS
+-rw-r--r--   0        0        0     2333 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT
+-rw-r--r--   0        0        0   135679 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT
+-rw-r--r--   0        0        0   114564 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET
+-rw-r--r--   0        0        0   172445 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS
+-rw-r--r--   0        0        0   135561 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL
+-rw-r--r--   0        0        0      378 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/POTENTIALS_DEFAULT
+-rw-r--r--   0        0        0   154582 2023-06-08 15:09:59.614987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all
+-rw-r--r--   0        0        0     8385 2023-06-08 15:09:59.614987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml
+-rw-r--r--   0        0        0    10869 2023-06-08 15:09:59.614987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini
+-rw-r--r--   0        0        0    10601 2023-06-08 15:09:59.614987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini
+-rw-r--r--   0        0        0  1959318 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat
+-rw-r--r--   0        0        0     9698 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py
+-rw-r--r--   0        0        0    13166 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py
+-rw-r--r--   0        0        0     7700 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py
+-rw-r--r--   0        0        0     5666 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py
+-rw-r--r--   0        0        0    11952 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py
+-rw-r--r--   0        0        0     6348 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py
+-rw-r--r--   0        0        0     9953 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py
+-rw-r--r--   0        0        0     4169 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py
+-rw-r--r--   0        0        0     6973 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py
+-rw-r--r--   0        0        0     5592 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py
+-rw-r--r--   0        0        0     1252 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml
+-rw-r--r--   0        0        0    12253 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml
+-rw-r--r--   0        0        0    11446 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml
+-rw-r--r--   0        0        0     7983 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml
+-rw-r--r--   0        0        0     9918 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml
+-rw-r--r--   0        0        0     1966 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml
+-rw-r--r--   0        0        0     7603 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml
+-rw-r--r--   0        0        0    14942 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py
+-rw-r--r--   0        0        0     4369 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py
+-rw-r--r--   0        0        0      812 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/__init__.py
+-rw-r--r--   0        0        0     9185 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py
+-rw-r--r--   0        0        0     8919 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py
+-rw-r--r--   0        0        0     6083 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/common.py
+-rw-r--r--   0        0        0     6708 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py
+-rw-r--r--   0        0        0     7953 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py
+-rw-r--r--   0        0        0     5234 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py
+-rw-r--r--   0        0        0    11073 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py
+-rw-r--r--   0        0        0    12134 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py
+-rw-r--r--   0        0        0    11760 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py
+-rw-r--r--   0        0        0    11519 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py
+-rw-r--r--   0        0        0       80 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/qe/__init__.py
+-rw-r--r--   0        0        0    22418 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/qe/nanoribbon.py
+-rw-r--r--   0        0        0     3369 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/conftest.py
+-rw-r--r--   0        0        0       96 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/examples/__init__.py
+-rw-r--r--   0        0        0   921233 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/data/sssp_minimal/C.upf
+-rw-r--r--   0        0        0   366195 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/data/sssp_minimal/H.upf
+-rw-r--r--   0        0        0       13 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/.gitignore
+-rwxr-xr-x   0        0        0     9833 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/aa
+-rw-r--r--   0        0        0      558 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/benzene-diradical.xyz
+-rw-r--r--   0        0        0      402 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2.xyz
+-rw-r--r--   0        0        0      422 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2_no_spin.xyz
+-rw-r--r--   0        0        0     2959 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2_on_au111.xyz
+-rw-r--r--   0        0        0      467 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2_spin.xyz
+-rw-r--r--   0        0        0      572 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h4.xyz
+-rw-r--r--   0        0        0     2533 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_ads_gw_ic.py
+-rw-r--r--   0        0        0     5271 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_afm.py
+-rw-r--r--   0        0        0     3527 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_diag.py
+-rw-r--r--   0        0        0     3702 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_fragment_separation.py
+-rw-r--r--   0        0        0     4654 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_geo_opt.py
+-rw-r--r--   0        0        0     3177 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_gw.py
+-rw-r--r--   0        0        0     5825 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_hrstm.py
+-rw-r--r--   0        0        0     1934 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_mol_opt_gw.py
+-rw-r--r--   0        0        0     6194 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_neb.py
+-rw-r--r--   0        0        0     3893 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_orb.py
+-rw-r--r--   0        0        0     4486 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_pdos.py
+-rw-r--r--   0        0        0     3057 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_phonons.py
+-rw-r--r--   0        0        0     3163 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_replica_chain.py
+-rw-r--r--   0        0        0     3831 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_stm.py
+-rw-r--r--   0        0        0     2145 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_gaussian_casscf.py
+-rw-r--r--   0        0        0     1393 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_gaussian_spin.py
+-rw-r--r--   0        0        0     2776 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_nanoribbon.py
+-rw-r--r--   0        0        0      251 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/h2.xyz
+-rw-r--r--   0        0        0     2483 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/h2_on_au111.xyz
+-rw-r--r--   0        0        0     1568 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/h2_on_hbn.xyz
+-rw-r--r--   0        0        0      679 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/si_bulk.xyz
+-rw-r--r--   0        0        0     4743 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      253 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/pytest.ini
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 aiida_nanotech_empa-1.0.0b1/PKG-INFO
```

### Comparing `aiida_nanotech_empa-1.0.0b0/.github/workflows/ci.yml` & `aiida_nanotech_empa-1.0.0b1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/.github/workflows/publish.yml` & `aiida_nanotech_empa-1.0.0b1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/.pre-commit-config.yaml` & `aiida_nanotech_empa-1.0.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/LICENSE` & `aiida_nanotech_empa-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/README.md` & `aiida_nanotech_empa-1.0.0b1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 
 ```shell
 pip install aiida-nanotech-empa
 ```
 
 ## For maintainers
 
-To create a new release, clone the repository, install development dependencies with `pip install '.[dev]'`, and then execute `bumpver update --major/--minor/--patch`.
+To create a new release, clone the repository, install development dependencies with `pip install '.[dev]'`, and then execute `bumpver update --dry --major (--minor/--patch)`.
+This will display the changes that will be made to the repository - check them carefully.
+
+Once you are happy with the changes, remove the `--dry` option and re-execute the command.
 This will:
 
   1. Create a tagged release with bumped version and push it to the repository.
   2. Trigger a GitHub actions workflow that creates a GitHub release.
 
 Additional notes:
 
-  - Use the `--dry` option to preview the release change.
   - The release tag (e.g. a/b/rc) is determined from the last release.
-    Use the `--tag` option to switch the release tag.
+    Use the `--tag beta (alpha/gamma)`  option to switch the release tag.
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cp2k_gw_parser.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cp2k_gw_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cp2k_neb_parser.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cp2k_neb_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -83,17 +83,15 @@
         self.out("replica_distances", distances_arr_data)
 
         return None
 
     def _parse_trajectory(self):
         """CP2K trajectory parser."""
 
-        fname = (
-            self.node.process_class._DEFAULT_RESTART_FILE_NAME
-        )  # pylint: disable=protected-access
+        fname = self.node.process_class._DEFAULT_RESTART_FILE_NAME
 
         # Check if the restart file is present.
         if fname not in self.retrieved.list_object_names():
             raise common.NotExistent(
                 "No restart file available, so the output trajectory can't be extracted"
             )
 
@@ -118,15 +116,24 @@
         coord_set_with_elements = coord_line_sets[-1]
         replica_coord_line_sets = coord_line_sets[:-1]
 
         # Remove integers from element names and create tags.
         element_list = [
             re.sub(r"[0-9]+", "", line[0]) for line in coord_set_with_elements
         ]
-        tags = [int(re.findall(r"\d+", line[0])[0]) for line in coord_set_with_elements]
+
+        # Extract tags from the element labels
+        tags = []
+        for line in coord_set_with_elements:
+            try:
+                to_append = re.findall(r"\d+", line[0])[0]
+            except IndexError:
+                to_append = 0
+
+            tags.append(int(to_append))
 
         for i_rep, rep_coord_lines in enumerate(replica_coord_line_sets):
             positions = np.array(rep_coord_lines, np.float64)
             ase_atoms = ase.Atoms(symbols=element_list, positions=positions, cell=cell)
             ase_atoms.set_tags(tags)
             replica_label = f"opt_replica_{str(i_rep).zfill(3)}"
             self.out(replica_label, StructureData(ase=ase_atoms, label=replica_label))
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/parsers/pp_parser.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/pp_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/afm.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/afm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/hrstm.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/hrstm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/overlap.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/overlap.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/plugins/stm.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/stm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/analyze_structure.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/analyze_structure.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/common_utils.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/cube_utils.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/cube_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/igor.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/igor.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/pymol_render.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/pymol_render.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/utils/stm_tools.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/stm_tools.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/__init__.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             help="Substrate type, determines the image charge plane.",
         )
         spec.input(
             "protocol",
             valid_type=orm.Str,
             default=lambda: orm.Str("gpw_std"),
             required=False,
-            help="Protocol supported by the GW workchain.",
+            help="Protocol supported by the Cp2kMoleculeGwWorkChain.",
         )
         spec.input(
             "multiplicity",
             valid_type=orm.Int,
             default=lambda: orm.Int(0),
             required=False,
         )
@@ -188,22 +188,14 @@
             "options.ic",
             valid_type=dict,
             non_db=True,
             required=False,
             help="Define options for the GW cacluation: walltime, memory, CPUs, etc.",
         )
         spec.input(
-            "debug",
-            valid_type=orm.Bool,
-            default=lambda: orm.Bool(False),
-            required=False,
-            help="Run with fast parameters for debugging.",
-        )
-
-        spec.input(
             "geometry_mode",
             valid_type=orm.Str,
             default=lambda: orm.Str("ads_geo"),
             required=False,
             help="Possibilities: ads_geo, gas_opt",
         )
 
@@ -268,16 +260,14 @@
         builder = Cp2kGeoOptWorkChain.get_builder()
         builder.code = self.inputs.code
         builder.structure = self.ctx.mol_struct
         builder.multiplicity = self.inputs.multiplicity
         builder.magnetization_per_site = self.ctx.mol_mag_per_site
         builder.vdw = orm.Bool(True)
         builder.protocol = orm.Str("standard")
-        if self.inputs.debug.value:
-            builder.protocol = orm.Str("debug")
         builder.options = self.inputs.options.scf
         builder.metadata.description = "gas_opt"
         submitted_node = self.submit(builder)
         return engine.ToContext(gas_opt=submitted_node)
 
     def check_gas_opt(self):
         if not self.ctx.gas_opt.is_finished_ok:
@@ -298,15 +288,14 @@
 
         builder = Cp2kMoleculeGwWorkChain.get_builder()
         builder.code = self.inputs.code
         builder.protocol = self.inputs.protocol
         builder.structure = self.ctx.mol_struct
         builder.magnetization_per_site = self.ctx.mol_mag_per_site
         builder.multiplicity = self.inputs.multiplicity
-        builder.debug = self.inputs.debug
         builder.run_image_charge = orm.Bool(True)
         builder.z_ic_plane = self.ctx.image_plane_z
         builder.options.scf = self.inputs.options.scf
         builder.options.gw = self.inputs.options.ic
         builder.metadata.description = "ic"
         submitted_node = self.submit(builder)
         return engine.ToContext(ic=submitted_node)
@@ -319,15 +308,14 @@
 
         builder = Cp2kMoleculeGwWorkChain.get_builder()
         builder.code = self.inputs.code
         builder.protocol = self.inputs.protocol
         builder.structure = self.ctx.mol_struct
         builder.magnetization_per_site = self.ctx.mol_mag_per_site
         builder.multiplicity = self.inputs.multiplicity
-        builder.debug = self.inputs.debug
         builder.options.scf = self.inputs.options.scf
         builder.options.gw = self.inputs.options.gw
         builder.metadata.description = "gw"
         submitted_node = self.submit(builder)
         return engine.ToContext(gw=submitted_node)
 
     def finalize(self):
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,31 @@
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
         spec.input("cp2k_code", valid_type=orm.Code)
         spec.input("structure", valid_type=orm.StructureData)
         spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the Cp2kDiagWorkChain.",
+        )
         spec.input("dft_params", valid_type=orm.Dict)
         spec.input(
             "options",
             valid_type=dict,
             non_db=True,
             help="Define options for the cacluations: walltime, memory, CPUs, etc.",
         )
 
         spec.input("afm_pp_code", valid_type=orm.Code)
         spec.input("afm_pp_params", valid_type=orm.Dict)
-
         spec.input("afm_2pp_code", valid_type=orm.Code)
         spec.input("afm_2pp_params", valid_type=orm.Dict)
 
         spec.outline(
             cls.setup,
             cls.run_diag_scf,
             cls.run_afms,
@@ -78,28 +84,29 @@
         }
 
     def run_diag_scf(self):
         self.report("Running CP2K diagonalization SCF")
         builder = Cp2kDiagWorkChain.get_builder()
         builder.cp2k_code = self.inputs.cp2k_code
         builder.structure = self.inputs.structure
+        builder.protocol = self.inputs.protocol
         builder.dft_params = orm.Dict(self.ctx.dft_params)
         builder.options = orm.Dict(self.inputs.options)
 
         # Restart wfn.
         if "parent_calc_folder" in self.inputs:
             builder.parent_calc_folder = self.inputs.parent_calc_folder
 
         future = self.submit(builder)
         self.to_context(diag_scf=future)
 
     def run_afms(self):
         self.report("Running PP")
         if not common_utils.check_if_calc_ok(self, self.ctx.diag_scf):
-            return self.exit_codes.ERROR_TERMINATION  # pylint: disable=no-member
+            return self.exit_codes.ERROR_TERMINATION
         afm_pp_inputs = {}
 
         afm_pp_inputs["geo_no_labels"] = self.ctx.files["geo_no_labels"]
         afm_pp_inputs["metadata"] = {}
         afm_pp_inputs["metadata"]["label"] = "afm_pp"
         afm_pp_inputs["code"] = self.inputs.afm_pp_code
         afm_pp_inputs["parameters"] = self.inputs.afm_pp_params
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import collections
-import copy
 import io
 import numbers
 import os
 import pathlib
 import re
 import shutil
 import tempfile
@@ -163,15 +162,24 @@
         pathlib.Path(__file__).parent / "./data/atomic_kinds.yml", encoding="utf-8"
     ) as fhandle:
         atom_data = yaml.safe_load(fhandle)
     elements = structure.get_symbols_set()
     return max([atom_data["cutoff"][element] for element in elements])
 
 
-def get_dft_inputs(dft_params, structure, template):
+def load_protocol(fname, protocol=None):
+    """Load a protocol from a file."""
+    with open(
+        pathlib.Path(__file__).parent / "protocols" / fname, encoding="utf-8"
+    ) as fhandle:
+        protocols = yaml.safe_load(fhandle)
+        return protocols[protocol] if protocol else protocols
+
+
+def get_dft_inputs(dft_params, structure, template, protocol):
     ase_atoms = structure.get_ase()
     files = {
         "basis": orm.SinglefileData(
             file=os.path.join(
                 os.path.dirname(os.path.realpath(__file__)),
                 ".",
                 "data",
@@ -183,22 +191,17 @@
                 os.path.dirname(os.path.realpath(__file__)),
                 ".",
                 "data",
                 "POTENTIAL",
             )
         ),
     }
-    # load input template
-    protocol = "./protocols/" + template
-    with open(
-        pathlib.Path(__file__).parent / protocol,
-        encoding="utf-8",
-    ) as handle:
-        protocols = yaml.safe_load(handle)
-        input_dict = copy.deepcopy(protocols[dft_params["protocol"]])
+
+    # Load input template.
+    input_dict = load_protocol(template, protocol)
 
     # vdW section
     if "vdw" in dft_params:
         if not dft_params["vdw"]:
             input_dict["FORCE_EVAL"]["DFT"]["XC"].pop("VDW_POTENTIAL")
     else:
         input_dict["FORCE_EVAL"]["DFT"]["XC"].pop("VDW_POTENTIAL")
@@ -220,15 +223,15 @@
 
     ase_atoms = structure_with_tags.get_ase()
 
     # non periodic systems only NONE and XYZ implemented: TO BE CHECKED FOR NEB!!!!
     if "periodic" in dft_params:
         if dft_params["periodic"] == "NONE":
             # make sure cell is big enough for MT poisson solver and center molecule
-            if dft_params["protocol"] == "debug":
+            if protocol == "debug":
                 extra_cell = 5.0
             else:
                 extra_cell = 15.0
             ase_atoms.cell = 2 * (np.ptp(ase_atoms.positions, axis=0)) + extra_cell
             ase_atoms.center()
 
             # Poisson solver
@@ -739,14 +742,40 @@
         ]  # shift -1 atom indexes
         return ["angle", atoms.get_angle(ids[0], ids[1], ids[2], mic=True)]
     # else:
     points_xyz = get_points_coords(the_cv["ANGLE"]["POINT"], atoms)
     return ["angle", points_xyz.get_angle(0, 1, 2, mic=True)]
 
 
+def cv_torsion(details):
+    """Returns the CP2K dictionary input section for the angle CV  between atoms or points.
+    cv_torsion('angle point atoms 2 3  point fix_point 8.36 6.78 5.0 point atoms 3 4 end'.split())
+    returns
+    {'TORSION': {'POINT': [{'TYPE': 'GEO_CENTER', 'ATOMS': '2 3 '}, {'TYPE': 'FIX_POINT', 'XYZ': '8.36 6.78 5.0 '},
+    {'TYPE': 'GEO_CENTER', 'ATOMS': '3 4 '}], 'ATOMS': '1 2 3'}}
+    """
+    # WEIGHTS NOT IMPLEMENTED
+    # case ATOMS and no points not implemented
+
+    points = get_points(details)
+    return_dict = {"TORSION": {}}
+    if points:
+        return_dict["TORSION"].update(points)
+    return_dict["TORSION"]["ATOMS"] = "1 2 3 4"
+
+    return return_dict
+
+
+def eval_cv_torsion(details, atoms):
+    """Evaluates the CV angle between the atoms defined in the CV."""
+    the_cv = cv_torsion(details)
+    points_xyz = get_points_coords(the_cv["TORSION"]["POINT"], atoms)
+    return ["angle", points_xyz.get_dihedral(0, 1, 2, 3, mic=True)]
+
+
 def cv_angle_plane_plane(details):
     """CV anagle between two planes.
     cv_angle_plane_plane('angle_plane_plane point fix_point 12.1 7.5  5.
     point atoms 1..6 point fix_point 7.1 7.5   7. plane atoms 1 2 3 plane vector 0 0 1 end'.split())
     returns
     {'ANGLE_PLANE_PLANE': {'POINT': [{'TYPE': 'FIX_POINT', 'XYZ': '12.1 7.5 5. '},
     {'TYPE': 'GEO_CENTER', 'ATOMS': '1..6 '},
@@ -846,14 +875,16 @@
             allcvs.append(cv_dist(details))
         elif details[0].lower() == "angle":
             allcvs.append(cv_angle(details))
         elif details[0].lower() == "angle_plane_plane":
             allcvs.append(cv_angle_plane_plane(details))
         elif details[0].lower() == "bond_rotation":
             allcvs.append(cv_bond_rotation(details))
+        elif details[0].lower() == "torsion":
+            allcvs.append(cv_torsion(details))
 
     return {"COLVAR": allcvs}
 
 
 def get_constraints_section(constraints):
     """Creates the CONSTRAINTS CP2K input dictionary."""
     constraints_dict = {}
@@ -894,9 +925,11 @@
             allcvs.append(eval_cv_dist(details, atoms))
         elif details[0].lower() == "angle":
             allcvs.append(eval_cv_angle(details, atoms))
         elif details[0].lower() == "angle_plane_plane":
             allcvs.append(eval_cv_angle_plane_plane(details, atoms))
         elif details[0].lower() == "bond_rotation":
             allcvs.append(eval_cv_bond_rotation(details, atoms))
+        elif details[0].lower() == "torsion":
+            allcvs.append(eval_cv_torsion(details, atoms))
 
     return allcvs
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
 import pathlib
 
 import numpy as np
-import yaml
 from aiida import engine, orm, plugins
 
 from ...utils import common_utils
 from . import cp2k_utils
 
 Cp2kBaseWorkChain = plugins.WorkflowFactory("cp2k.base")
 
@@ -16,14 +15,21 @@
     def define(cls, spec):
         super().define(spec)
 
         spec.input("cp2k_code", valid_type=orm.Code)
         spec.input("structure", valid_type=orm.StructureData)
         spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
         spec.input("dft_params", valid_type=orm.Dict, default=lambda: orm.Dict(dict={}))
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the Cp2kBaseWorkChain.",
+        )
         spec.input("pdos_lists", valid_type=orm.List, required=False)
         spec.input("settings", valid_type=orm.Dict, required=False)
         spec.input(
             "options",
             valid_type=orm.Dict,
             default=lambda: orm.Dict(
                 dict={
@@ -69,23 +75,14 @@
 
         # Set up mol UKS parameters.
 
         self.ctx.dft_params = copy.deepcopy(self.inputs.dft_params.get_dict())
 
         # Resources.
         self.ctx.options = self.inputs.options.get_dict()
-        if self.ctx.dft_params["protocol"] == "debug":
-            self.ctx.options = {
-                "max_wallclock_seconds": 600,
-                "resources": {
-                    "num_machines": 1,
-                    "num_mpiprocs_per_machine": 1,
-                    "num_cores_per_mpiproc": 1,
-                },
-            }
 
         if not self.ctx.dft_params["uks"]:
             self.ctx.dft_params["spin_up_guess"] = []
             self.ctx.dft_params["spin_dw_guess"] = []
 
         # Get cutoff.
         self.ctx.cutoff = cp2k_utils.get_cutoff(structure=structure)
@@ -103,40 +100,38 @@
         ]
         structure_with_tags, kinds_dict = cp2k_utils.determine_kinds(
             structure, magnetization_per_site
         )
 
         ase_atoms = structure_with_tags.get_ase()
 
-        # PERIODIC: only NONE and XYZ are supported
+        # Periodic: only NONE and XYZ are supported.
         if self.ctx.dft_params["periodic"] == "NONE":
-            # Make sure cell is big enough for MT poisson solver and center positions
-            if self.ctx.dft_params["protocol"] == "debug":
-                extra_cell = 9.0  # Angstrom
+            # Make sure cell is big enough for MT poisson solver and center positions.
+            if self.inputs.protocol == "debug":
+                extra_cell = 9.0  # Angstrom.
             else:
-                extra_cell = 15.0
+                extra_cell = 15.0  # Angstrom.
             ase_atoms.cell = 2 * (np.ptp(ase_atoms.positions, axis=0)) + extra_cell
             ase_atoms.center()
 
         self.ctx.structure_with_tags = ase_atoms
         self.ctx.kinds_section = cp2k_utils.get_kinds_section(
             kinds_dict, protocol="gpw"
         )
 
     def run_ot_scf(self):
         self.report("Running CP2K OT SCF")
 
         # Load input template.
-        with open(
-            pathlib.Path(__file__).parent / "protocols" / "scf_ot_protocol.yml",
-            encoding="utf-8",
-        ) as handle:
-            protocols = yaml.safe_load(handle)
-            input_dict = copy.deepcopy(protocols[self.ctx.dft_params["protocol"]])
+        input_dict = cp2k_utils.load_protocol(
+            "scf_ot_protocol.yml", self.inputs.protocol.value
+        )
 
+        # Set workflow inputs.
         builder = Cp2kBaseWorkChain.get_builder()
         builder.cp2k.code = self.inputs.cp2k_code
         builder.cp2k.structure = orm.StructureData(ase=self.ctx.structure_with_tags)
 
         builder.cp2k.file = self.ctx.files
         # restart wfn
         if "parent_calc_folder" in self.inputs:
@@ -154,61 +149,58 @@
         # UKS
         if self.ctx.dft_params["uks"]:
             input_dict["FORCE_EVAL"]["DFT"]["UKS"] = ".TRUE."
             input_dict["FORCE_EVAL"]["DFT"]["MULTIPLICITY"] = self.ctx.dft_params[
                 "multiplicity"
             ]
 
-        # cutoff
+        # CUTOFF.
         input_dict["FORCE_EVAL"]["DFT"]["MGRID"]["CUTOFF"] = self.ctx.cutoff
 
         # KINDS section
         cp2k_utils.dict_merge(input_dict, self.ctx.kinds_section)
 
         # Setup walltime.
         input_dict["GLOBAL"]["WALLTIME"] = 86000
 
         builder.cp2k.metadata.options = self.ctx.options
 
-        # parser
+        # Parser.
         builder.cp2k.metadata.options.parser_name = "cp2k_advanced_parser"
 
-        # cp2k input dictionary
+        # CP2K input dictionary.
         builder.cp2k.parameters = orm.Dict(input_dict)
         self.ctx.input_dict = copy.deepcopy(input_dict)
 
         future = self.submit(builder)
         self.to_context(ot_scf=future)
 
     def run_diag_scf(self):
         self.report("Running CP2K diagonalization SCF")
         if not common_utils.check_if_calc_ok(self, self.ctx.ot_scf):
             return self.exit_codes.ERROR_TERMINATION
 
-        # load input template
-        with open(
-            pathlib.Path(__file__).parent / "./protocols/scf_diag_protocol.yml",
-            encoding="utf-8",
-        ) as handle:
-            protocols = yaml.safe_load(handle)
-            scf_dict = copy.deepcopy(protocols[self.ctx.dft_params["protocol"]])
+        # Load input template.
+        scf_dict = cp2k_utils.load_protocol(
+            "scf_diag_protocol.yml", self.inputs.protocol.value
+        )
 
         input_dict = copy.deepcopy(self.ctx.input_dict)
         if self.ctx.dft_params["elpa_switch"]:
             input_dict["GLOBAL"]["PREFERRED_DIAG_LIBRARY"] = "ELPA"
             input_dict["GLOBAL"]["ELPA_KERNEL"] = "AUTO"
             input_dict["GLOBAL"]["DBCSR"] = {"USE_MPI_ALLOCATOR": ".FALSE."}
         input_dict["FORCE_EVAL"]["DFT"].pop("SCF")
         input_dict["FORCE_EVAL"]["DFT"]["SCF"] = scf_dict
         if "added_mos" in self.ctx.dft_params:
             input_dict["FORCE_EVAL"]["DFT"]["SCF"]["ADDED_MOS"] = self.ctx.dft_params[
                 "added_mos"
             ]
 
-        # pdos
+        # PDOS
         if "pdos_lists" in self.inputs:
             pdos_list_dicts = [
                 {"COMPONENTS": "", "LIST": e} for e in self.inputs.pdos_lists
             ]
             input_dict["FORCE_EVAL"]["DFT"]["PRINT"]["PDOS"] = {
                 "NLUMO": self.ctx.dft_params["added_mos"],
                 "LDOS": pdos_list_dicts,
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 import pathlib
 
 import numpy as np
-import yaml
 from aiida import engine, orm, plugins
 
 from ...utils import analyze_structure, common_utils
 from . import cp2k_utils
 
 StructureData = plugins.DataFactory("core.structure")
 Cp2kBaseWorkChain = plugins.WorkflowFactory("cp2k.base")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute() / "data"
 
 
-def load_protocol(fname, protocol):
-    """Load a protocol from a file."""
-    with open(
-        pathlib.Path(__file__).parent / "protocols" / fname, encoding="utf-8"
-    ) as fhandle:
-        protocols = yaml.safe_load(fhandle)
-        return protocols[protocol]
-
-
 # @engine.calcfunction
 def split_structure(structure, fixed_atoms, magnetization_per_site, fragments):
     ase_geo = structure.get_ase()
 
     allfixed = [0 for i in ase_geo]
     mps = []
     fixed = ""
@@ -89,25 +79,31 @@
 
         spec.input_namespace(
             "fragments",
             valid_type=orm.List,
             help="List of indices of atoms defining individual fragments.",
         )
 
-        # dft parameters
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol used by the work chain (geo_opt_protocol).",
+        )
+
         spec.input(
             "dft_params",
             valid_type=orm.Dict,
             help="""
         multiplicities, dictionary: multiplicity of each fragment. Use 'all' to specify the multiplicity of the whole system.
         magnetization_per_site: Magnetization per site of the whole system.
             Magnetization per site of the fragments will be extracted automatically.
         charges, dictionary: Charges of each fragment. No need to specify the charge of the full system
             as it would be computed automatically.
-        protocol: Protocol to use for the calculation.
         uks: Use unrestricted Kohn-Sham.
         """,
         )
 
         # Fixed atoms and magnetization per site defined for the whole system. Information for the fragments will extracted automatically.
         spec.input(
             "fixed_atoms",
@@ -181,17 +177,17 @@
             fixed_atoms=self.inputs.fixed_atoms,
             magnetization_per_site=self.inputs.dft_params["magnetization_per_site"]
             if "magnetization_per_site" in self.inputs.dft_params
             else None,
             fragments=self.inputs.fragments,
         ):
             # Re-loading the input dictionary for the given protocol.
-            input_dict = load_protocol(
+            input_dict = cp2k_utils.load_protocol(
                 fname="geo_opt_protocol.yml",
-                protocol=self.inputs.dft_params["protocol"],
+                protocol=self.inputs.protocol.value,
             )
 
             self.report(
                 f"""Running SCF for the fragment '{inputs['label']}' consisting of {len(inputs['structure'].sites)} atoms, """
                 f"""where {analyze_structure.list_to_string_range(inputs['fixed_atoms']) or 'None'} atoms are fixed."""
             )
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import copy
 import pathlib
 
 import numpy as np
-import yaml
 from aiida import engine, orm, plugins
 
 from ...utils import common_utils
 from . import cp2k_utils
 
 Cp2kBaseWorkChain = plugins.WorkflowFactory("cp2k.base")
 
@@ -14,14 +12,21 @@
 class Cp2kGeoOptWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
         spec.input("code", valid_type=orm.Code)
         spec.input("structure", valid_type=orm.StructureData)
         spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the work chain (geo_opt_protocol).",
+        )
         spec.input("dft_params", valid_type=orm.Dict)
         spec.input("sys_params", valid_type=orm.Dict)
         spec.input(
             "options",
             valid_type=dict,
             non_db=True,
             help="Define options for the cacluations: walltime, memory, CPUs, etc.",
@@ -47,26 +52,18 @@
             "pseudo": orm.SinglefileData(
                 file=pathlib.Path(__file__).parent / "data" / "POTENTIAL"
             ),
         }
 
         self.ctx.sys_params = self.inputs.sys_params.get_dict()
         self.ctx.dft_params = self.inputs.dft_params.get_dict()
-
         self.ctx.n_atoms = len(self.inputs.structure.sites)
-
-        # Load input template.
-        with open(
-            pathlib.Path(__file__).parent / "protocols" / "geo_opt_protocol.yml",
-            encoding="utf-8",
-        ) as handle:
-            protocols = yaml.safe_load(handle)
-            self.ctx.input_dict = copy.deepcopy(
-                protocols[self.ctx.dft_params["protocol"]]
-            )
+        self.ctx.input_dict = cp2k_utils.load_protocol(
+            "geo_opt_protocol.yml", self.inputs.protocol.value
+        )
 
         # vdW section.
         if "vdw" in self.ctx.dft_params:
             if not self.ctx.dft_params["vdw"]:
                 self.ctx.input_dict["FORCE_EVAL"]["DFT"]["XC"].pop("VDW_POTENTIAL")
         else:
             self.ctx.input_dict["FORCE_EVAL"]["DFT"]["XC"].pop("VDW_POTENTIAL")
@@ -93,16 +90,16 @@
         )
 
         ase_atoms = structure_with_tags.get_ase()
 
         # Non-periodic systems only NONE and XYZ implemented:
         if "periodic" in self.ctx.dft_params:
             if self.ctx.dft_params["periodic"] == "NONE":
-                # make sure cell is big enough for MT poisson solver and center molecule
-                if self.ctx.dft_params["protocol"] == "debug":
+                # Make sure cell is big enough for MT poisson solver and center molecule.
+                if self.inputs.protocol.value == "debug":
                     extra_cell = 5.0
                 else:
                     extra_cell = 15.0
                 ase_atoms.cell = 2 * (np.ptp(ase_atoms.positions, axis=0)) + extra_cell
                 ase_atoms.center()
 
                 # Poisson solver
@@ -130,22 +127,17 @@
         if "symmetry" in self.ctx.sys_params:
             self.ctx.input_dict["FORCE_EVAL"]["SUBSYS"]["CELL"][
                 "SYMMETRY"
             ] = self.ctx.sys_params["symmetry"]
 
         # Cell optimization.
         if "cell_opt" in self.ctx.sys_params:
-            with open(
-                pathlib.Path(__file__).parent / "protocols" / "cell_opt_protocol.yml",
-                encoding="utf-8",
-            ) as handle:
-                protocols = yaml.safe_load(handle)
-                cell_input_dict = copy.deepcopy(
-                    protocols[self.ctx.dft_params["protocol"]]
-                )
+            cell_input_dict = cp2k_utils.load_protocol(
+                "cell_opt_protocol.yml", self.inputs.protocol.value
+            )
             self.ctx.input_dict["GLOBAL"]["RUN_TYPE"] = "CELL_OPT"
             self.ctx.input_dict["MOTION"] = cell_input_dict["MOTION"]
             self.ctx.input_dict["FORCE_EVAL"]["STRESS_TENSOR"] = "ANALYTICAL"
             if "cell_opt_constraint" in self.ctx.sys_params:
                 self.ctx.input_dict["MOTION"]["CELL_OPT"][
                     "CONSTRAINT"
                 ] = self.ctx.sys_params["cell_opt_constraint"]
@@ -162,23 +154,14 @@
         if "colvars" in self.ctx.sys_params:
             self.ctx.input_dict["FORCE_EVAL"]["SUBSYS"].update(
                 cp2k_utils.get_colvars_section(self.ctx.sys_params["colvars"])
             )
 
         # Resources.
         self.ctx.options = self.inputs.options
-        if self.ctx.dft_params["protocol"] == "debug":
-            self.ctx.options = {
-                "max_wallclock_seconds": 600,
-                "resources": {
-                    "num_machines": 1,
-                    "num_mpiprocs_per_machine": 1,
-                    "num_cores_per_mpiproc": 1,
-                },
-            }
         self.ctx.input_dict["GLOBAL"]["WALLTIME"] = self.ctx.options[
             "max_wallclock_seconds"
         ]
 
     def submit_calc(self):
         self.report("Submitting geometry optimization")
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,21 @@
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
         spec.input("cp2k_code", valid_type=orm.Code)
         spec.input("structure", valid_type=orm.StructureData)
         spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the Cp2kDiagWorkChain.",
+        )
         spec.input("dft_params", valid_type=orm.Dict)
         spec.input(
             "options",
             valid_type=dict,
             non_db=True,
             help="Define options for the cacluations: walltime, memory, CPUs, etc.",
         )
@@ -67,36 +74,37 @@
         }
 
     def run_diag_scf(self):
         self.report("Running CP2K diagonalization SCF")
         builder = Cp2kDiagWorkChain.get_builder()
         builder.cp2k_code = self.inputs.cp2k_code
         builder.structure = self.inputs.structure
+        builder.protocol = self.inputs.protocol
         builder.dft_params = orm.Dict(self.ctx.dft_params)
         builder.options = orm.Dict(self.ctx.options)
 
-        # restart wfn
+        # Restart WFN.
         if "parent_calc_folder" in self.inputs:
             builder.parent_calc_folder = self.inputs.parent_calc_folder
 
         future = self.submit(builder)
         self.to_context(diag_scf=future)
 
     def run_ppm(self):
         self.report("Running PPM")
         if not common_utils.check_if_calc_ok(self, self.ctx.diag_scf):
-            return self.exit_codes.ERROR_TERMINATION  # pylint: disable=no-member
+            return self.exit_codes.ERROR_TERMINATION
         inputs = {}
         inputs["geo_no_labels"] = self.ctx.files["geo_no_labels"]
         inputs["metadata"] = {}
         inputs["metadata"]["label"] = "hrstm_ppm"
         inputs["code"] = self.inputs.ppm_code
         inputs["parameters"] = self.inputs.ppm_params
         inputs["parent_calc_folder"] = self.ctx.diag_scf.outputs.remote_folder
-        # TODO set atom types properly
+        # TODO set atom types properly.
         inputs["atomtypes"] = self.ctx.files["2pp"]
         inputs["metadata"]["options"] = {
             "max_wallclock_seconds": 21600,
             "resources": {
                 "num_machines": 1,
                 "num_mpiprocs_per_machine": 1,
                 "num_cores_per_mpiproc": 1,
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
 import pathlib
 
 import numpy as np
-import yaml
 from aiida import engine, orm
 from aiida_cp2k.calculations import Cp2kCalculation
 
 from . import cp2k_utils
 
 ALLOWED_PROTOCOLS = ["gapw_std", "gapw_hq", "gpw_std"]
 
@@ -116,21 +115,15 @@
     def setup(self):
         self.report("Inspecting input and setting up things")
 
         if self.inputs.protocol not in ALLOWED_PROTOCOLS:
             self.report("Error: protocol not supported.")
             return self.exit_codes.ERROR_TERMINATION
 
-        # Load protocol templates.
-        with open(
-            pathlib.Path(__file__).parent.joinpath("./protocols/gw_protocols.yml"),
-            encoding="utf-8",
-        ) as handle:
-            self.ctx.protocols = yaml.safe_load(handle)
-
+        self.ctx.protocols = cp2k_utils.load_cp2k_protocol("gw_protocols.yml")
         structure = self.inputs.structure
         self.ctx.cutoff = cp2k_utils.get_cutoff(structure=structure)
         magnetization_per_site = copy.deepcopy(self.inputs.magnetization_per_site)
         ghost_per_site = None
 
         # Add ghost atoms in case of gw-ic.
         if self.inputs.run_image_charge:
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,16 +139,14 @@
         builder = Cp2kGeoOptWorkChain.get_builder()
         builder.code = self.inputs.code
         builder.structure = self.ctx.mol_struct
         builder.multiplicity = self.inputs.multiplicity
         builder.magnetization_per_site = self.ctx.mol_mag_per_site
         builder.vdw = orm.Bool(True)
         builder.protocol = orm.Str("standard")
-        if self.inputs.debug.value:
-            builder.protocol = orm.Str("debug")
         builder.options = self.inputs.options.geo_opt
         builder.metadata.description = "Submitted by Cp2kMoleculeOptGwWorkChain."
         builder.metadata.label = "Cp2kGeoOptWorkChain"
         return engine.ToContext(gas_opt=self.submit(builder))
 
     def check_gas_opt(self):
         if not self.ctx.gas_opt.is_finished_ok:
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,21 @@
             "replicas",
             valid_type=orm.StructureData,
             required=False,
             help="nodes of input replicas",
         )
         spec.input("wfn_cp_commands", valid_type=orm.Str, required=False)
         spec.input("restart_from", valid_type=orm.Str, required=False)
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the Cp2kDiagWorkChain.",
+        )
         spec.input("dft_params", valid_type=orm.Dict)
         spec.input("sys_params", valid_type=orm.Dict)
         spec.input("neb_params", valid_type=orm.Dict)
         spec.input(
             "options",
             valid_type=dict,
             non_db=True,
@@ -63,15 +70,18 @@
             dft_params = self.inputs.dft_params.get_dict()
 
         (
             self.ctx.files,
             self.ctx.input_dict,
             self.ctx.structure_with_tags,
         ) = cp2k_utils.get_dft_inputs(
-            dft_params, self.inputs.structure, "neb_protocol.yml"
+            dft_params,
+            self.inputs.structure,
+            "neb_protocol.yml",
+            self.inputs.protocol.value,
         )
         self.ctx.sys_params = self.inputs.sys_params.get_dict()
         self.ctx.neb_params = self.inputs.neb_params.get_dict()
 
         # The input structure is the  NEB replica 0 if we do not continue from previous NEB.
         all_replica_nodes = [self.inputs.structure]
 
@@ -151,23 +161,14 @@
         if "optimize_end_points" in self.ctx.neb_params:
             self.ctx.input_dict["MOTION"]["BAND"]["OPTIMIZE_BAND"][
                 "OPTIMIZE_END_POINTS"
             ] = self.ctx.neb_params["optimize_end_points"]
 
         # Resources
         self.ctx.options = self.inputs.options
-        if self.inputs.dft_params["protocol"] == "debug":
-            self.ctx.options = {
-                "max_wallclock_seconds": 600,
-                "resources": {
-                    "num_machines": 3,
-                    "num_mpiprocs_per_machine": 1,
-                    "num_cores_per_mpiproc": 1,
-                },
-            }
         self.ctx.scf_options = copy.deepcopy(self.ctx.options)
 
         # Number of mpi processes for scf derived from nproc_replica
         self.ctx.scf_options["resources"]["num_machines"] = int(
             self.ctx.neb_params["nproc_rep"]
             / self.ctx.options["resources"]["num_mpiprocs_per_machine"]
         )
@@ -182,14 +183,15 @@
     def first_scf(self):
         """Run scf on the initial geometry."""
 
         files, input_dict, structure_with_tags = cp2k_utils.get_dft_inputs(
             self.inputs.dft_params.get_dict(),
             self.inputs.structure,
             "scf_ot_protocol.yml",
+            self.inputs.protocol.value,
         )
 
         builder = Cp2kCalculation.get_builder()
         builder.structure = orm.StructureData(ase=structure_with_tags)
         builder.code = self.inputs.code
         builder.file = files
         builder.metadata.options = self.ctx.scf_options
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,21 @@
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
         spec.input("cp2k_code", valid_type=orm.Code)
         spec.input("structure", valid_type=orm.StructureData)
         spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the Cp2kDiagWorkChain.",
+        )
         spec.input("dft_params", valid_type=orm.Dict)
         spec.input("spm_code", valid_type=orm.Code)
         spec.input("spm_params", valid_type=orm.Dict)
         spec.input(
             "options",
             valid_type=dict,
             non_db=True,
@@ -49,14 +56,15 @@
 
     def run_diag_scf(self):
         self.report("Running CP2K diagonalization SCF")
         builder = Cp2kDiagWorkChain.get_builder()
         builder.cp2k_code = self.inputs.cp2k_code
         builder.structure = self.inputs.structure
         builder.dft_params = orm.Dict(self.ctx.dft_params)
+        builder.protocol = self.inputs.protocol
 
         # Restart wfn.
         if "parent_calc_folder" in self.inputs:
             builder.parent_calc_folder = self.inputs.parent_calc_folder
         builder.settings = orm.Dict(
             {
                 "additional_retrieve_list": [
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,21 @@
         super().define(spec)
 
         spec.input("cp2k_code", valid_type=orm.Code)
         spec.input("slabsys_structure", valid_type=orm.StructureData)
         spec.input("mol_structure", valid_type=orm.StructureData)
         spec.input("pdos_lists", valid_type=orm.List)
         spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the Cp2kDiagWorkChain workchain.",
+        )
         spec.input("dft_params", valid_type=orm.Dict)
         spec.input("overlap_code", valid_type=orm.Code)
         spec.input("overlap_params", valid_type=orm.Dict)
         spec.input_namespace(
             "options",
             valid_type=int,
             non_db=True,
@@ -101,14 +108,15 @@
     def run_diags(self):
         # Slab part.
         self.report("Running Diag Workchain for slab")
 
         builder = Cp2kDiagWorkChain.get_builder()
         builder.cp2k_code = self.inputs.cp2k_code
         builder.structure = self.inputs.slabsys_structure
+        builder.protocol = self.inputs.protocol
         builder.dft_params = orm.Dict(self.ctx.slab_dft_params)
         builder.settings = orm.Dict({"additional_retrieve_list": ["*.pdos"]})
         builder.options = orm.Dict(self.ctx.slab_options)
 
         # Restart WFN.
         if "parent_calc_folder" in self.inputs:
             builder.parent_calc_folder = self.inputs.parent_calc_folder
@@ -122,14 +130,15 @@
 
         # Molecule part.
         self.report("Running Diag Workchain for molecule")
 
         builder = Cp2kDiagWorkChain.get_builder()
         builder.cp2k_code = self.inputs.cp2k_code
         builder.structure = self.inputs.mol_structure
+        builder.protocol = self.inputs.protocol
         builder.dft_params = orm.Dict(self.ctx.mol_dft_params)
         builder.options = orm.Dict(self.ctx.mol_options)
 
         mol_future = self.submit(builder)
         self.to_context(mol_diag_scf=mol_future)
         # End molecule part.
 
@@ -149,17 +158,14 @@
 
         n_machines = 4 if self.ctx.n_slab_atoms < 2000 else 8
 
         inputs["metadata"]["options"] = {
             "resources": {"num_machines": n_machines},
             "max_wallclock_seconds": 86400,
         }
-
-        if self.inputs.dft_params["protocol"] == "debug":
-            inputs["metadata"]["options"]["max_wallclock_seconds"] = 600
         settings = orm.Dict({"additional_retrieve_list": ["overlap.npz"]})
         inputs["settings"] = settings
         future = self.submit(OverlapCalculation, **inputs)
         return engine.ToContext(overlap=future)
 
     def finalize(self):
         if "overlap.npz" not in [
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 class Cp2kPhononsWorkChain(engine.WorkChain):
     @classmethod
     def define(cls, spec):
         super().define(spec)
         spec.input("code", valid_type=orm.Code)
         spec.input("structure", valid_type=orm.StructureData)
         spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the Cp2kGeoOptWorkChain.",
+        )
         spec.input("dft_params", valid_type=orm.Dict)
         spec.input("sys_params", valid_type=orm.Dict)
         spec.input("phonons_params", valid_type=orm.Dict)
         spec.input(
             "options",
             valid_type=dict,
             non_db=True,
@@ -46,15 +53,18 @@
         dft_params = self.inputs.dft_params.get_dict()
 
         (
             self.ctx.files,
             self.ctx.input_dict,
             self.ctx.structure_with_tags,
         ) = cp2k_utils.get_dft_inputs(
-            dft_params, self.inputs.structure, "phonons_protocol.yml"
+            dft_params,
+            self.inputs.structure,
+            "phonons_protocol.yml",
+            protocol=self.inputs.protocol.value,
         )
         self.ctx.sys_params = self.inputs.sys_params.get_dict()
         self.ctx.phonons_params = self.inputs.phonons_params.get_dict()
         self.ctx.input_dict["VIBRATIONAL_ANALYSIS"][
             "NPROC_REP"
         ] = self.ctx.phonons_params["nproc_rep"]
 
@@ -75,23 +85,14 @@
         if "colvars" in self.ctx.sys_params:
             self.ctx.input_dict["FORCE_EVAL"]["SUBSYS"].update(
                 cp2k_utils.get_colvars_section(self.ctx.sys_params["colvars"])
             )
 
         # Resources.
         self.ctx.options = self.inputs.options
-        if self.inputs.dft_params["protocol"] == "debug":
-            self.ctx.options = {
-                "max_wallclock_seconds": 600,
-                "resources": {
-                    "num_machines": 3,
-                    "num_mpiprocs_per_machine": 1,
-                    "num_cores_per_mpiproc": 1,
-                },
-            }
         self.ctx.geo_options = copy.deepcopy(self.ctx.options)
         self.ctx.geo_options["resources"]["num_machines"] = int(
             self.ctx.phonons_params["nproc_rep"]
             / self.ctx.options["resources"]["num_mpiprocs_per_machine"]
         )
         self.ctx.input_dict["GLOBAL"]["WALLTIME"] = max(
             600, self.ctx.options["max_wallclock_seconds"] - 600
@@ -104,14 +105,15 @@
 
         builder.code = self.inputs.code
         builder.structure = self.inputs.structure
 
         # Restart WFN.
         if "parent_calc_folder" in self.inputs:
             builder.parent_calc_folder = self.inputs.parent_calc_folder
+        builder.protocol = self.inputs.protocol
         builder.dft_params = self.inputs.dft_params
         builder.sys_params = self.inputs.sys_params
         builder.options = self.ctx.geo_options
         builder.structure = orm.StructureData(ase=self.ctx.structure_with_tags)
         builder.code = self.inputs.code
 
         future = self.submit(builder)
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,21 @@
         super().define(spec)
 
         # Define the inputs of the workflow.
         spec.input("code", valid_type=orm.Code)
         spec.input("structure", valid_type=orm.StructureData)
         spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
         spec.input("restart_from", valid_type=orm.Str, required=False)
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the Cp2kBaseWorkChain.",
+        )
         spec.input("dft_params", valid_type=orm.Dict)
         spec.input("sys_params", valid_type=orm.Dict)
         spec.input(
             "options",
             valid_type=dict,
             non_db=True,
             help="Define options for the cacluations: walltime, memory, CPUs, etc.",
@@ -157,25 +164,27 @@
     def first_scf(self):
         """Run scf on the initial geometry."""
 
         files, input_dict, structure_with_tags = cp2k_utils.get_dft_inputs(
             self.inputs.dft_params.get_dict(),
             self.ctx.lowest_energy_structure,
             "scf_ot_protocol.yml",
+            self.inputs.protocol.value,
         )
 
         builder = Cp2kCalculation.get_builder()
         builder.structure = orm.StructureData(ase=structure_with_tags)
         builder.code = self.inputs.code
         builder.file = files
         if "parent_calc_folder" in self.inputs:
             builder.parent_calc_folder = self.inputs.parent_calc_folder
         builder.metadata.options = self.inputs.options
         builder.metadata.label = "scf"
         builder.metadata.options.parser_name = "cp2k_advanced_parser"
+        input_dict["GLOBAL"]["WALLTIME"] = self.inputs.options["max_wallclock_seconds"]
         builder.parameters = orm.Dict(input_dict)
 
         future = self.submit(builder)
         self.report(f"Submitted scf of the initial geometry: {future.pk}")
         self.to_context(initial_scf=future)
 
     def update_colvars_values(self):
@@ -189,15 +198,15 @@
         self.report(f"actual CVs values: {self.ctx.colvars_values}")
         if self.ctx.propagation_step == 0:
             self.ctx.CVs_to_increment = self.ctx.colvars_values
         else:
             self.ctx.CVs_to_increment = self.ctx.CVs_cases[self.ctx.lowest_energy_calc]
 
     def update_colvars_increments(self):
-        """Computes teh increments for the CVs according to deviation from target.
+        """Computes the increments for the CVs according to deviation from target.
         If the target value is reached wihtin the increment, set increment to 0.
         Deviation from target is computed wrt actual value of CVs while new CVs
         are computed as previous target plus increment to avoid slow diverging deviations
         from targets"""
         self.ctx.colvars_increments = []
         for index, colvar in enumerate(self.ctx.colvars_values):
             if (
@@ -219,15 +228,18 @@
         """Run a constrained geometry optimization for each non 0 increment of colvars."""
         self.ctx.CVs_cases = []
         for index in range(len(self.ctx.CVs_to_increment)):
             if self.ctx.colvars_increments[index] != 0:
                 structure = self.ctx.lowest_energy_structure
 
                 files, input_dict, structure_with_tags = cp2k_utils.get_dft_inputs(
-                    self.inputs.dft_params, structure, "geo_opt_protocol.yml"
+                    self.inputs.dft_params,
+                    structure,
+                    "geo_opt_protocol.yml",
+                    self.inputs.protocol.value,
                 )
 
                 builder = Cp2kBaseWorkChain.get_builder()
                 builder.cp2k.code = self.inputs.code
                 builder.cp2k.structure = orm.StructureData(ase=structure_with_tags)
                 builder.cp2k.file = files
                 builder.cp2k.metadata.options = self.inputs.options
@@ -266,14 +278,17 @@
                         target += self.ctx.colvars_increments[icv]
                     current_cvs_targets.append(target)
                     input_dict["MOTION"]["CONSTRAINT"]["COLLECTIVE"][icv]["TARGET"] = (
                         units + " " + str(target)
                     )
                     submitted_cvs += " " + str(target)
                 self.ctx.CVs_cases.append(current_cvs_targets)
+                input_dict["GLOBAL"]["WALLTIME"] = self.inputs.options[
+                    "max_wallclock_seconds"
+                ]
                 builder.cp2k.parameters = orm.Dict(input_dict)
 
                 submitted_calculation = self.submit(builder)
                 self.report(
                     f"Submitted geo opt: {submitted_calculation.pk}, with {submitted_cvs}"
                 )
                 self.to_context(
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,21 @@
     @classmethod
     def define(cls, spec):
         super().define(spec)
 
         spec.input("cp2k_code", valid_type=orm.Code)
         spec.input("structure", valid_type=orm.StructureData)
         spec.input("parent_calc_folder", valid_type=orm.RemoteData, required=False)
+        spec.input(
+            "protocol",
+            valid_type=orm.Str,
+            default=lambda: orm.Str("standard"),
+            required=False,
+            help="Protocol supported by the Cp2kDiagWorkChain.",
+        )
         spec.input("dft_params", valid_type=orm.Dict)
         spec.input("spm_code", valid_type=orm.Code)
         spec.input("spm_params", valid_type=orm.Dict)
         spec.input(
             "options",
             valid_type=dict,
             non_db=True,
@@ -50,17 +57,19 @@
         self.ctx.dft_params["added_mos"] = added_mos
 
     def run_diag_scf(self):
         self.report("Running CP2K diagonalization SCF")
         builder = Cp2kDiagWorkChain.get_builder()
         builder.cp2k_code = self.inputs.cp2k_code
         builder.structure = self.inputs.structure
+        builder.protocol = self.inputs.protocol
         builder.dft_params = orm.Dict(self.ctx.dft_params)
         builder.options = orm.Dict(self.inputs.options)
-        # restart wfn
+
+        # Restart wfn, if requested.
         if "parent_calc_folder" in self.inputs:
             builder.parent_calc_folder = self.inputs.parent_calc_folder
 
         future = self.submit(builder)
         self.to_context(diag_scf=future)
 
     def run_stm(self):
@@ -84,15 +93,15 @@
         if self.ctx.n_atoms > 4000:
             n_machines = 30
 
         inputs["metadata"]["options"] = {
             "resources": {"num_machines": n_machines},
             "max_wallclock_seconds": 36000,
         }
-        if self.inputs.dft_params["protocol"] == "debug":
+        if self.inputs.protocol.value == "debug":
             inputs["metadata"]["options"]["max_wallclock_seconds"] = 600
 
         # Need to make an explicit instance for the node to be stored to AiiDA.
         settings = orm.Dict({"additional_retrieve_list": ["stm.npz"]})
         inputs["settings"] = settings
 
         future = self.submit(StmCalculation, **inputs)
```

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/__init__.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/common.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/common.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/aiida_nanotech_empa/workflows/qe/nanoribbon.py` & `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/qe/nanoribbon.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/conftest.py` & `aiida_nanotech_empa-1.0.0b1/conftest.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/data/sssp_minimal/C.upf` & `aiida_nanotech_empa-1.0.0b1/examples/data/sssp_minimal/C.upf`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/data/sssp_minimal/H.upf` & `aiida_nanotech_empa-1.0.0b1/examples/data/sssp_minimal/H.upf`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/aa` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/aa`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/benzene-diradical.xyz` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/benzene-diradical.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h2_on_au111.xyz` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2_on_au111.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/c2h4.xyz` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h4.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_ads_gw_ic.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_ads_gw_ic.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_afm.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_afm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import pathlib
 
 import ase.io
+import click
 import numpy as np
 from aiida import engine, orm, plugins
 
 Cp2kAfmWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.afm")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 GEO_FILE = "c2h2_on_au111.xyz"
 
 
 def _example_cp2k_afm(
-    cp2k_code, afm_code1, afm_code2, sc_diag, force_multiplicity, uks
+    cp2k_code,
+    afm_code1,
+    afm_code2,
+    sc_diag,
+    force_multiplicity,
+    uks,
+    n_nodes,
+    n_cores_per_node,
 ):
     # Check test geometry is already in database
     qb = orm.QueryBuilder()
     qb.append(orm.Node, filters={"label": {"in": ["auto_test_c2h2_au_structure"]}})
     structure = None
     for node_tuple in qb.iterall():
         node = node_tuple[0]
@@ -25,42 +33,41 @@
     else:
         structure = orm.StructureData(ase=ase.io.read(DATA_DIR / GEO_FILE))
         structure.label = "auto_test_c2h2_au_structure"
         structure.store()
         print(f"Created new structure: {structure.pk}")
     builder = Cp2kAfmWorkChain.get_builder()
 
-    builder.metadata.label = "Cp2kAfmWorkChain"
+    builder.metadata.label = "CP2K_AFM"
     builder.metadata.description = "test description"
     builder.cp2k_code = cp2k_code
     ase_geom = ase.io.read(DATA_DIR / GEO_FILE)
     builder.structure = orm.StructureData(ase=ase_geom)
     builder.options = {
         "resources": {
-            "num_machines": 1,
-            "num_mpiprocs_per_machine": 1,
+            "num_machines": n_nodes,
+            "num_mpiprocs_per_machine": n_cores_per_node,
         },
         "max_wallclock_seconds": 600,
     }
 
+    builder.protocol = orm.Str("debug")
     builder.dft_params = orm.Dict(
         {
-            "protocol": "debug",
             "sc_diag": sc_diag,
             "force_multiplicity": force_multiplicity,
             "elpa_switch": False,
             "periodic": "XYZ",
             "uks": uks,
             "smear_t": 150,
         }
     )
     if uks:
         builder.dft_params = orm.Dict(
             {
-                "protocol": "debug",
                 "sc_diag": sc_diag,
                 "force_multiplicity": force_multiplicity,
                 "elpa_switch": False,
                 "periodic": "XYZ",
                 "uks": uks,
                 "multiplicity": 1,
                 "smear_t": 150,
@@ -139,17 +146,29 @@
     _example_cp2k_afm(cp2k_code, afm_code1, afm_code2, False, True, False)
 
 
 def example_cp2k_afm_sc_diag(cp2k_code, afm_code1, afm_code2):
     _example_cp2k_afm(cp2k_code, afm_code1, afm_code2, True, True, True)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.argument("ppafm_code", default="ppafm@localhost")
+@click.argument("ppafm2_code", default="2ppafm@localhost")
+@click.option("-n", "--n-nodes", default=1)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, ppafm_code, ppafm2_code, n_nodes, n_cores_per_node):
     print("#### no sc_diag UKS no force")
     _example_cp2k_afm(
-        orm.load_code("cp2k@localhost"),
-        orm.load_code("py_afm_pp_@localhost"),
-        orm.load_code("py_afm_2pp_@localhost"),
-        False,
-        False,
-        True,
+        cp2k_code=orm.load_code(cp2k_code),
+        afm_code1=orm.load_code(ppafm_code),
+        afm_code2=orm.load_code(ppafm2_code),
+        sc_diag=False,
+        force_multiplicity=False,
+        uks=True,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
     )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_fragment_separation.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_fragment_separation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pathlib
 
 import ase.io
+import click
 from aiida import engine, orm, plugins
 
 StructureData = plugins.DataFactory("core.structure")
 Cp2kFragmentSeparationWorkChain = plugins.WorkflowFactory(
     "nanotech_empa.cp2k.fragment_separation"
 )
 
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 GEO_FILE = "h2_on_hbn.xyz"
 
 
-def _example_cp2k_ads_ene(cp2k_code, mult):
+def _example_cp2k_ads_ene(cp2k_code, mult, n_nodes, n_cores_per_node):
     """Example of running a workflow to compute the adsorption energy of a molecule on substrate."""
     # Check test geometry is already in database.
     qb = orm.QueryBuilder()
     qb.append(orm.Node, filters={"label": {"in": [GEO_FILE]}})
     structure = None
     for node_tuple in qb.iterall():
         node = node_tuple[0]
@@ -56,39 +57,39 @@
         "uks": uks,
         "multiplicities": {
             "all": mult,
             "molecule": mult,
             "slab": mult,
         },
         "magnetization_per_site": mag,
-        "protocol": "debug",
     }
 
     builder.dft_params = orm.Dict(dft_params)
+    builder.protocol = orm.Str("debug")
 
     builder.options = {
         "all": {
             "max_wallclock_seconds": 1200,
             "resources": {
-                "num_machines": 1,
-                "num_mpiprocs_per_machine": 1,
+                "num_machines": n_nodes,
+                "num_mpiprocs_per_machine": n_cores_per_node,
             },
         },
         "molecule": {
             "max_wallclock_seconds": 1200,
             "resources": {
-                "num_machines": 1,
-                "num_mpiprocs_per_machine": 1,
+                "num_machines": n_nodes,
+                "num_mpiprocs_per_machine": n_cores_per_node,
             },
         },
         "slab": {
             "max_wallclock_seconds": 1200,
             "resources": {
-                "num_machines": 1,
-                "num_mpiprocs_per_machine": 1,
+                "num_machines": n_nodes,
+                "num_mpiprocs_per_machine": n_cores_per_node,
             },
         },
     }
 
     _, calc_node = engine.run_get_node(builder)
 
     assert calc_node.is_finished_ok
@@ -103,13 +104,31 @@
     _example_cp2k_ads_ene(cp2k_code, 0)
 
 
 def example_cp2k_slabopt_uks(cp2k_code):
     _example_cp2k_ads_ene(cp2k_code, 1)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.option("-n", "--n-nodes", default=1)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, n_nodes, n_cores_per_node):
     print("#### RKS")
-    _example_cp2k_ads_ene(orm.load_code("cp2k@localhost"), 0)
+    _example_cp2k_ads_ene(
+        orm.load_code(cp2k_code),
+        mult=0,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
+    )
 
     print("#### UKS")
-    _example_cp2k_ads_ene(orm.load_code("cp2k@localhost"), 1)
+    _example_cp2k_ads_ene(
+        orm.load_code(cp2k_code),
+        mult=1,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
+    )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_geo_opt.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_geo_opt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import pathlib
 
 import ase.io
+import click
 from aiida import engine, orm, plugins
 
 Cp2kGeoOptWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.geo_opt")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 GEOS = ["h2_on_hbn.xyz", "si_bulk.xyz", "c2h2.xyz"]
 
 
-def _example_cp2k_geo_opt(cp2k_code, sys_type, uks):
+def _example_cp2k_geo_opt(cp2k_code, sys_type, uks, n_nodes, n_cores_per_node):
     # Check test geometries are already in database.
     qb = orm.QueryBuilder()
     qb.append(
         orm.Node,
         filters={"label": {"in": GEOS}},
     )
     structures = {}
@@ -33,50 +34,47 @@
     builder = Cp2kGeoOptWorkChain.get_builder()
 
     builder.metadata.description = "test description"
     builder.code = cp2k_code
     builder.options = {
         "max_wallclock_seconds": 600,
         "resources": {
-            "num_machines": 1,
-            "num_mpiprocs_per_machine": 1,
+            "num_machines": n_nodes,
+            "num_mpiprocs_per_machine": n_cores_per_node,
             "num_cores_per_mpiproc": 1,
         },
     }
+    builder.protocol = orm.Str("debug")
 
     # define structure
     if sys_type == "SlabXY":
         structure = structures["h2_on_hbn.xyz"]
         builder.metadata.label = "CP2K_GeoOpt"
     elif sys_type == "Molecule":
         structure = structures["c2h2.xyz"]
         builder.metadata.label = "CP2K_GeoOpt"
     elif sys_type == "Bulk":
         structure = structures["si_bulk.xyz"]
         builder.metadata.label = "CP2K_CellOpt"
 
-    dft_params = {
-        "protocol": "debug",
-        "cutoff": 300,
-    }
-
     if uks:
         magnetization_per_site = [0 for i in range(len(structure.sites))]
         magnetization_per_site[0] = 1
         magnetization_per_site[1] = -1
         dft_params = {
-            "protocol": "debug",
             "uks": uks,
             "magnetization_per_site": magnetization_per_site,
             "charge": 0,
             "periodic": "XYZ",
             "vdw": False,
             "multiplicity": 1,
             "cutoff": 300,
         }
+    else:
+        dft_params = {"cutoff": 300}
 
     sys_params = {}
 
     # adapt parameters to structure
     if sys_type == "SlabXY":
         sys_params[
             "constraints"
@@ -115,14 +113,34 @@
     _example_cp2k_geo_opt(cp2k_code, "SlabXY", False)
 
 
 def example_cp2k_slab_opt_uks(cp2k_code):
     _example_cp2k_geo_opt(cp2k_code, "SlabXY", True)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.option("-n", "--n-nodes", default=1)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, n_nodes, n_cores_per_node):
     for sys_type in ["SlabXY", "Molecule", "Bulk"]:
         print("#### ", sys_type, " RKS")
-        _example_cp2k_geo_opt(orm.load_code("cp2k@localhost"), sys_type, False)
+        _example_cp2k_geo_opt(
+            orm.load_code(cp2k_code),
+            sys_type=sys_type,
+            uks=False,
+            n_nodes=n_nodes,
+            n_cores_per_node=n_cores_per_node,
+        )
 
         print("#### ", sys_type, " UKS")
-        _example_cp2k_geo_opt(orm.load_code("cp2k@localhost"), sys_type, True)
+        _example_cp2k_geo_opt(
+            orm.load_code(cp2k_code),
+            sys_type=sys_type,
+            uks=True,
+            n_nodes=n_nodes,
+            n_cores_per_node=n_cores_per_node,
+        )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_gw.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_gw.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_hrstm.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_hrstm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import os
 import pathlib
 
 import ase.io
+import click
 import numpy as np
 from aiida import engine, orm, plugins
 
 Cp2kHrstmWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.hrstm")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 GEO_FILE = "c2h2_on_au111.xyz"
 
 
 def _example_cp2k_hrstm(
-    cp2k_code, afm_code, hrstm_code, sc_diag, force_multiplicity, uks
+    cp2k_code,
+    afm_code,
+    hrstm_code,
+    sc_diag,
+    force_multiplicity,
+    uks,
+    n_nodes,
+    n_cores_per_node,
 ):
     # Check test geometry is already in database.
     qb = orm.QueryBuilder()
     qb.append(orm.Node, filters={"label": {"in": [GEO_FILE]}})
     structure = None
     for node_tuple in qb.iterall():
         node = node_tuple[0]
@@ -38,42 +46,38 @@
     builder.options = {
         "resources": {
             "num_machines": 1,
             "num_mpiprocs_per_machine": 1,
         },
         "max_wallclock_seconds": 600,
     }
+    builder.protocol = orm.Str("debug")
 
-    builder.dft_params = orm.Dict(
-        {
-            "protocol": "debug",
+    if uks:
+        dft_params = {
             "sc_diag": sc_diag,
             "force_multiplicity": force_multiplicity,
             "elpa_switch": False,
             "periodic": "XYZ",
             "uks": uks,
+            "multiplicity": 1,
             "smear_t": 150,
+            "spin_up_guess": [0],
+            "spin_dw_guess": [1],
         }
-    )
-    if uks:
-        builder.dft_params = orm.Dict(
-            {
-                "protocol": "debug",
-                "sc_diag": sc_diag,
-                "force_multiplicity": force_multiplicity,
-                "elpa_switch": False,
-                "periodic": "XYZ",
-                "uks": uks,
-                "multiplicity": 1,
-                "smear_t": 150,
-                "spin_up_guess": [0],
-                "spin_dw_guess": [1],
-            }
-        )
-
+    else:
+        dft_params = {
+            "sc_diag": sc_diag,
+            "force_multiplicity": force_multiplicity,
+            "elpa_switch": False,
+            "periodic": "XYZ",
+            "uks": uks,
+            "smear_t": 150,
+        }
+    builder.dft_params = orm.Dict(dft_params)
     builder.ppm_code = afm_code
 
     cell = ase_geom.cell
     top_z = np.max(ase_geom.positions[:, 2])
     dx = 0.2
     scanminz = 3.5
     scanmaxz = 5.5
@@ -157,17 +161,29 @@
     _example_cp2k_hrstm(cp2k_code, afm_code, hrstm_code, False, True, False)
 
 
 def example_cp2k_hrstm_sc_diag(cp2k_code, afm_code, hrstm_code):
     _example_cp2k_hrstm(cp2k_code, afm_code, hrstm_code, True, True, True)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.argument("ppafm2_code", default="2ppafm@localhost")
+@click.argument("hrstm_code", default="hrstm@localhost")
+@click.option("-n", "--n-nodes", default=1)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, ppafm2_code, hrstm_code, n_nodes, n_cores_per_node):
     print("#### no sc_diag UKS no force")
     _example_cp2k_hrstm(
-        orm.load_code("cp2k@localhost"),
-        orm.load_code("py_afm_2pp_@localhost"),
-        orm.load_code("py_hrstm_4576cd@localhost"),
-        False,
-        False,
-        True,
+        orm.load_code(cp2k_code),
+        orm.load_code(ppafm2_code),
+        orm.load_code(hrstm_code),
+        sc_diag=False,
+        force_multiplicity=False,
+        uks=True,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
     )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_mol_opt_gw.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_mol_opt_gw.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_neb.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_neb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import pathlib
 
 import ase
+import click
 from aiida import engine, orm, plugins
 
 Cp2kNebWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.neb")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 
 
-def _example_cp2k_neb(cp2k_code, uks, restart_uuid):
+def _example_cp2k_neb(cp2k_code, uks, restart_uuid, n_nodes, n_cores_per_node):
     builder = Cp2kNebWorkChain.get_builder()
 
     builder.metadata.label = "CP2K_NEB"
-    builder.metadata.description = "a NEB calculation"
+    builder.metadata.description = "NEB calculation."
     builder.code = cp2k_code
     builder.options = {
         "max_wallclock_seconds": 600,
         "resources": {
-            "num_machines": 3,
-            "num_mpiprocs_per_machine": 1,
+            "num_machines": n_nodes,
+            "num_mpiprocs_per_machine": n_cores_per_node,
             "num_cores_per_mpiproc": 1,
         },
     }
 
     # define structures
 
     # Check if test structure is already in the database.
@@ -114,31 +115,31 @@
             replicas[name] = orm.load_node(uuids[i])
         builder.replicas = replicas
 
     else:
         builder.structure = orm.load_node(restart_uuid).inputs.structure
         builder.restart_from = orm.Str(restart_uuid)
 
-    dft_params = {
-        "protocol": "debug",
-        "cutoff": 300,
-    }
+    builder.protocol = orm.Str("debug")
 
     if uks:
         magnetization_per_site = [0, 1, -1, 0]
         dft_params = {
-            "protocol": "debug",
             "uks": uks,
             "magnetization_per_site": magnetization_per_site,
             "charge": 0,
             "periodic": "NONE",
             "vdw": False,
             "multiplicity": 1,
             "cutoff": 300,
         }
+    else:
+        dft_params = {
+            "cutoff": 300,
+        }
 
     sys_params = {}
     sys_params[
         "constraints"
     ] = "fixed xyz 1 , collective 1 [ev/angstrom^2] 40 [angstrom] 1.36"
     sys_params["colvars"] = "distance atoms 2 3"
     neb_params = {
@@ -166,16 +167,42 @@
     _example_cp2k_neb(cp2k_code, False, None)
 
 
 def example_cp2k_neb_uks(cp2k_code):
     _example_cp2k_neb(cp2k_code, True, None)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.option("-n", "--n-nodes", default=3)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, n_nodes, n_cores_per_node):
     print("####  RKS")
-    uuid1 = _example_cp2k_neb(orm.load_code("cp2k@localhost"), False, None)
+    _example_cp2k_neb(
+        orm.load_code(cp2k_code),
+        uks=False,
+        restart_uuid=None,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
+    )
 
     print("####  UKS")
-    uuid2 = _example_cp2k_neb(orm.load_code("cp2k@localhost"), True, None)
+    uuid2 = _example_cp2k_neb(
+        orm.load_code(cp2k_code),
+        uks=True,
+        restart_uuid=None,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
+    )
 
     print("### restarting from ", uuid2)
-    uuid3 = _example_cp2k_neb(orm.load_code("cp2k@localhost"), True, uuid2)
+    _example_cp2k_neb(
+        orm.load_code(cp2k_code),
+        uks=True,
+        restart_uuid=uuid2,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
+    )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_orb.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_orb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import pathlib
 
 import ase.io
+import click
 from aiida import engine, orm, plugins
 
 Cp2kOrbiralsWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.orbitals")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 GEO_FILE = "c2h2.xyz"
 
 
-def _example_cp2k_orb(cp2k_code, stm_code, sc_diag, force_multiplicity, uks):
+def _example_cp2k_orb(
+    cp2k_code, stm_code, sc_diag, force_multiplicity, uks, n_nodes, n_cores_per_node
+):
     # Check test geometry is already in database.
     qb = orm.QueryBuilder()
     qb.append(orm.Node, filters={"label": {"in": [GEO_FILE]}})
     structure = None
     for node_tuple in qb.iterall():
         node = node_tuple[0]
         structure = node
@@ -27,48 +30,46 @@
 
     builder = Cp2kOrbiralsWorkChain.get_builder()
 
     builder.metadata.label = "CP2K_Orbitals"
     builder.metadata.description = "test description"
     builder.cp2k_code = cp2k_code
     builder.structure = structure
-    builder.dft_params = orm.Dict(
-        {
-            "protocol": "debug",
+    builder.protocol = orm.Str("debug")
+
+    if uks:
+        dft_params = {
+            "sc_diag": sc_diag,
+            "force_multiplicity": force_multiplicity,
+            "elpa_switch": False,
+            "periodic": "NONE",
+            "uks": uks,
+            "charge": 0,
+            "multiplicity": 1,
+            "smear_t": 150,
+            "spin_up_guess": [0],
+            "spin_dw_guess": [1],
+        }
+    else:
+        dft_params = {
             "sc_diag": sc_diag,
             "force_multiplicity": force_multiplicity,
             "elpa_switch": False,
             "periodic": "NONE",
             "uks": uks,
             "charge": 0,
             "smear_t": 150,
         }
-    )
-    if uks:
-        builder.dft_params = orm.Dict(
-            {
-                "protocol": "debug",
-                "sc_diag": sc_diag,
-                "force_multiplicity": force_multiplicity,
-                "elpa_switch": False,
-                "periodic": "NONE",
-                "uks": uks,
-                "charge": 0,
-                "multiplicity": 1,
-                "smear_t": 150,
-                "spin_up_guess": [0],
-                "spin_dw_guess": [1],
-            }
-        )
 
+    builder.dft_params = orm.Dict(dft_params)
     builder.options = {
         "max_wallclock_seconds": 600,
         "resources": {
-            "num_machines": 1,
-            "num_mpiprocs_per_machine": 1,
+            "num_machines": n_nodes,
+            "num_mpiprocs_per_machine": n_cores_per_node,
             "num_cores_per_mpiproc": 1,
         },
     }
     builder.spm_code = stm_code
     parent_dir = "./parent_calc_folder/"
     builder.spm_params = orm.Dict(
         {
@@ -100,16 +101,27 @@
     _example_cp2k_orb(cp2k_code, spm_code, False, True, False)
 
 
 def example_cp2k_orb_sc_diag(cp2k_code, spm_code):
     _example_cp2k_orb(cp2k_code, spm_code, True, True, True)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.argument("stm_code", default="stm@localhost")
+@click.option("-n", "--n-nodes", default=1)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, stm_code, n_nodes, n_cores_per_node):
     print("#### sc_diag UKS force")
     _example_cp2k_orb(
-        orm.load_code("cp2k@localhost"),
-        orm.load_code("py_stm_4576cd@localhost"),
-        True,
-        True,
-        True,
+        cp2k_code=orm.load_code(cp2k_code),
+        stm_code=orm.load_code(stm_code),
+        sc_diag=True,
+        force_multiplicity=True,
+        uks=True,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
     )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_pdos.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_pdos.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import pathlib
 
 import ase.io
+import click
 from aiida import engine, orm, plugins
 
 Cp2kPdosWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.pdos")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 GEO_FILE = "c2h2_on_au111.xyz"
 
 
-def _example_cp2k_pdos(cp2k_code, overlap_code, sc_diag, force_multiplicity, uks):
+def _example_cp2k_pdos(
+    cp2k_code, overlap_code, sc_diag, force_multiplicity, uks, n_nodes, n_cores_per_node
+):
     # Check test geometry is already in database.
     qb = orm.QueryBuilder()
     qb.append(orm.Node, filters={"label": {"in": [GEO_FILE]}})
     structure = None
     for node_tuple in qb.iterall():
         node = node_tuple[0]
         structure = node
@@ -31,55 +34,52 @@
     builder.metadata.description = "test description"
     builder.cp2k_code = cp2k_code
     ase_geom_slab = ase.io.read(DATA_DIR / GEO_FILE)
     ase_geom_mol = ase_geom_slab[0:4]
     builder.slabsys_structure = orm.StructureData(ase=ase_geom_slab)
     builder.mol_structure = orm.StructureData(ase=ase_geom_mol)
     builder.pdos_lists = orm.List([("1..4", "molecule"), ("1", "cat")])
-    builder.dft_params = orm.Dict(
-        {
-            "protocol": "debug",
+    builder.protocol = orm.Str("debug")
+    if uks:
+        dft_params = {
             "sc_diag": sc_diag,
             "force_multiplicity": force_multiplicity,
             "elpa_switch": False,
             "periodic": "XYZ",
             "uks": uks,
+            "multiplicity": 1,
             "smear_t": 150,
+            "spin_up_guess": [0],
+            "spin_dw_guess": [1],
         }
-    )
-    if uks:
-        builder.dft_params = orm.Dict(
-            {
-                "protocol": "debug",
-                "sc_diag": sc_diag,
-                "force_multiplicity": force_multiplicity,
-                "elpa_switch": False,
-                "periodic": "XYZ",
-                "uks": uks,
-                "multiplicity": 1,
-                "smear_t": 150,
-                "spin_up_guess": [0],
-                "spin_dw_guess": [1],
-            }
-        )
+    else:
+        dft_params = {
+            "sc_diag": sc_diag,
+            "force_multiplicity": force_multiplicity,
+            "elpa_switch": False,
+            "periodic": "XYZ",
+            "uks": uks,
+            "smear_t": 150,
+        }
+    builder.dft_params = orm.Dict(dft_params)
 
     builder.options = {
         "slab": {
             "max_wallclock_seconds": 600,
             "resources": {
-                "num_machines": 1,
-                "num_mpiprocs_per_machine": 1,
+                "num_machines": n_nodes,
+                "num_mpiprocs_per_machine": n_cores_per_node,
                 "num_cores_per_mpiproc": 1,
             },
         },
         "molecule": {
             "max_wallclock_seconds": 600,
             "resources": {
-                "num_machines": 1,
-                "num_mpiprocs_per_machine": 1,
+                "num_machines": n_nodes,
+                "num_mpiprocs_per_machine": n_cores_per_node,
                 "num_cores_per_mpiproc": 1,
             },
         },
     }
 
     builder.overlap_code = overlap_code
     builder.overlap_params = orm.Dict(
@@ -112,16 +112,27 @@
     _example_cp2k_pdos(cp2k_code, overlap_code, False, True)
 
 
 def example_cp2k_pdos_sc_diag(cp2k_code, overlap_code):
     _example_cp2k_pdos(cp2k_code, overlap_code, True, True)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.argument("overlap_code", default="overlap@localhost")
+@click.option("-n", "--n-nodes", default=1)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, overlap_code, n_nodes, n_cores_per_node):
     print("#### no sc_diag RKS")
     _example_cp2k_pdos(
-        orm.load_code("cp2k@localhost"),
-        orm.load_code("py_overlap_4576cd@localhost"),
-        False,
-        True,
-        False,
+        orm.load_code(cp2k_code),
+        orm.load_code(overlap_code),
+        sc_diag=False,
+        force_multiplicity=True,
+        uks=False,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
     )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_phonons.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_phonons.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pathlib
 
 import ase.io
+import click
 from aiida import engine, orm, plugins
 
 Cp2kPhononsWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.phonons")
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 GEO_FILE = "c2h2.xyz"
 
 
-def _example_cp2k_phonons(cp2k_code, uks):
+def _example_cp2k_phonons(cp2k_code, uks, n_nodes, n_cores_per_node):
     # check test geometry is already in database
     qb = orm.QueryBuilder()
     qb.append(orm.Node, filters={"label": {"in": [GEO_FILE]}})
     structure = None
     for node_tuple in qb.iterall():
         node = node_tuple[0]
         structure = node
@@ -28,39 +29,39 @@
 
     builder.metadata.label = "CP2K_Phonons"
     builder.metadata.description = "test phonons c2h2"
     builder.code = cp2k_code
     builder.options = {
         "max_wallclock_seconds": 600,
         "resources": {
-            "num_machines": 3,
-            "num_mpiprocs_per_machine": 1,
+            "num_machines": n_nodes,
+            "num_mpiprocs_per_machine": n_cores_per_node,
             "num_cores_per_mpiproc": 1,
         },
     }
 
-    dft_params = {
-        "protocol": "debug",
-        "cutoff": 300,
-    }
+    builder.protocol = orm.Str("debug")
 
     if uks:
         magnetization_per_site = [0 for i in range(len(structure.sites))]
         magnetization_per_site[1] = 1
         magnetization_per_site[2] = -1
         dft_params = {
-            "protocol": "debug",
             "uks": uks,
             "magnetization_per_site": magnetization_per_site,
             "charge": 0,
             "periodic": "XYZ",
             "vdw": False,
             "multiplicity": 1,
             "cutoff": 300,
         }
+    else:
+        dft_params = {
+            "cutoff": 300,
+        }
 
     sys_params = {}
 
     dft_params["periodic"] = "NONE"
     phonons_params = {"nproc_rep": 1}
     sys_params["colvars"] = "distance atoms 2 3 , distance atoms 1 2"
 
@@ -69,27 +70,40 @@
     builder.sys_params = orm.Dict(sys_params)
     builder.phonons_params = orm.Dict(phonons_params)
 
     _, calc_node = engine.run_get_node(builder)
 
     assert calc_node.is_finished_ok
 
-    # phonons_out_dict = dict(calc_node.outputs.output_parameters)
-    # print()
-    # for k in phonons_out_dict:
-    #    print(f"  {k}: {phonons_out_dict[k]}")
-
 
 def example_cp2k_phonons_rks(cp2k_code):
     _example_cp2k_phonons(cp2k_code, "SlabXY", False)
 
 
 def example_cp2k_phonons_uks(cp2k_code):
     _example_cp2k_phonons(cp2k_code, "SlabXY", True)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.option("-n", "--n-nodes", default=3)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, n_nodes, n_cores_per_node):
     print("#### ", " RKS")
-    _example_cp2k_phonons(orm.load_code("cp2k@localhost"), False)
+    _example_cp2k_phonons(
+        orm.load_code(cp2k_code),
+        uks=False,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
+    )
 
     print("#### ", " UKS")
-    _example_cp2k_phonons(orm.load_code("cp2k@localhost"), True)
+    _example_cp2k_phonons(
+        orm.load_code(cp2k_code),
+        uks=True,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
+    )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_replica_chain.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_replica_chain.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import pathlib
 
-import ase
+import ase.io
+import click
 from aiida import engine, orm, plugins
 
 Cp2kReplicaWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.replica")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 GEO_FILE = "c2h4.xyz"
 
 
-def _example_cp2k_replicachain(cp2k_code, targets, restart_uuid):
+def _example_cp2k_replicachain(
+    cp2k_code, targets, restart_uuid, n_nodes, n_cores_per_node
+):
     # check if test geometry is already in database
     qb = orm.QueryBuilder()
     qb.append(orm.Node, filters={"label": {"in": [GEO_FILE]}})
     structure = None
     for node_tuple in qb.iterall():
         node = node_tuple[0]
         structure = node
@@ -31,24 +34,24 @@
 
     builder.metadata.label = "CP2K_Replica"
     builder.metadata.description = "test description"
     builder.code = cp2k_code
     builder.options = {
         "max_wallclock_seconds": 600,
         "resources": {
-            "num_machines": 1,
-            "num_mpiprocs_per_machine": 1,
+            "num_machines": n_nodes,
+            "num_mpiprocs_per_machine": n_cores_per_node,
             "num_cores_per_mpiproc": 1,
         },
     }
 
     builder.structure = orm.StructureData(ase=ase.io.read(DATA_DIR / GEO_FILE))
+    builder.protocol = orm.Str("debug")
 
     dft_params = {
-        "protocol": "debug",
         "periodic": "NONE",
         "vdw": False,
         "cutoff": 300,
     }
 
     sys_params = {}
     sys_params[
@@ -69,16 +72,32 @@
 
 
 def example_cp2k_replicachain_rks(cp2k_code):
     pk1 = _example_cp2k_replicachain(cp2k_code, None)
     _example_cp2k_replicachain(cp2k_code, pk1)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.option("-n", "--n-nodes", default=1)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, n_nodes, n_cores_per_node):
     print("#### RKS")
-    pk1 = _example_cp2k_replicachain(
-        orm.load_code("cp2k@localhost"), [1.40, 1.21, 1.87], None
+    uuid = _example_cp2k_replicachain(
+        cp2k_code=orm.load_code(cp2k_code),
+        targets=[1.40, 1.21, 1.87],
+        restart_uuid=None,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
     )
-    print(f"#### RKS continuation from pk {pk1}")
-    pk2 = _example_cp2k_replicachain(
-        orm.load_code("cp2k@localhost"), [1.47, 1.27, 1.87], pk1
+    print(f"#### RKS continuation from uuid ({uuid})")
+    _example_cp2k_replicachain(
+        cp2k_code=orm.load_code(cp2k_code),
+        targets=[1.47, 1.27, 1.87],
+        restart_uuid=uuid,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
     )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_cp2k_stm.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_stm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import pathlib
 
 import ase.io
+import click
 from aiida import engine, orm, plugins
 
 Cp2kStmWorkChain = plugins.WorkflowFactory("nanotech_empa.cp2k.stm")
 
 DATA_DIR = pathlib.Path(__file__).parent.absolute()
 GEO_FILE = "c2h2_on_au111.xyz"
 
 
-def _example_cp2k_stm(cp2k_code, spm_code, sc_diag, force_multiplicity, uks):
+def _example_cp2k_stm(
+    cp2k_code, spm_code, sc_diag, force_multiplicity, uks, n_nodes, n_cores_per_node
+):
     # Check test geometry is already in database.
     qb = orm.QueryBuilder()
     qb.append(orm.Node, filters={"label": {"in": [GEO_FILE]}})
     structure = None
     for node_tuple in qb.iterall():
         node = node_tuple[0]
         structure = node
@@ -27,46 +30,45 @@
 
     builder = Cp2kStmWorkChain.get_builder()
 
     builder.metadata.label = "CP2K_STM"
     builder.metadata.description = "test description"
     builder.cp2k_code = cp2k_code
     builder.structure = structure
-    builder.dft_params = orm.Dict(
-        {
-            "protocol": "debug",
+    builder.protocol = orm.Str("debug")
+
+    if uks:
+        dft_params = {
             "sc_diag": sc_diag,
             "force_multiplicity": force_multiplicity,
             "elpa_switch": False,
             "periodic": "XYZ",
             "uks": uks,
+            "multiplicity": 1,
             "smear_t": 150,
+            "spin_up_guess": [0],
+            "spin_dw_guess": [1],
         }
-    )
-    if uks:
-        builder.dft_params = orm.Dict(
-            {
-                "protocol": "debug",
-                "sc_diag": sc_diag,
-                "force_multiplicity": force_multiplicity,
-                "elpa_switch": False,
-                "periodic": "XYZ",
-                "uks": uks,
-                "multiplicity": 1,
-                "smear_t": 150,
-                "spin_up_guess": [0],
-                "spin_dw_guess": [1],
-            }
-        )
+    else:
+        dft_params = {
+            "sc_diag": sc_diag,
+            "force_multiplicity": force_multiplicity,
+            "elpa_switch": False,
+            "periodic": "XYZ",
+            "uks": uks,
+            "smear_t": 150,
+        }
+
+    builder.dft_params = orm.Dict(dft_params)
 
     builder.options = {
         "max_wallclock_seconds": 600,
         "resources": {
-            "num_machines": 1,
-            "num_mpiprocs_per_machine": 1,
+            "num_machines": n_nodes,
+            "num_mpiprocs_per_machine": n_cores_per_node,
             "num_cores_per_mpiproc": 1,
         },
     }
     builder.spm_code = spm_code
     parent_dir = "./parent_calc_folder/"
     builder.spm_params = orm.Dict(
         {
@@ -97,16 +99,27 @@
     _example_cp2k_stm(cp2k_code, spm_code, False, True, False)
 
 
 def example_cp2k_stm_sc_diag(cp2k_code, spm_code):
     _example_cp2k_stm(cp2k_code, spm_code, True, True, True)
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("cp2k_code", default="cp2k@localhost")
+@click.argument("stm_code", default="stm@localhost")
+@click.option("-n", "--n-nodes", default=1)
+@click.option("-c", "--n-cores-per-node", default=1)
+def run_all(cp2k_code, stm_code, n_nodes, n_cores_per_node):
     print("#### no sc_diag UKS no force")
     _example_cp2k_stm(
-        orm.load_code("cp2k@localhost"),
-        orm.load_code("py_stm_4576cd@localhost"),
-        False,
-        False,
-        True,
+        cp2k_code=orm.load_code(cp2k_code),
+        spm_code=orm.load_code(stm_code),
+        sc_diag=False,
+        force_multiplicity=False,
+        uks=True,
+        n_nodes=n_nodes,
+        n_cores_per_node=n_cores_per_node,
     )
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_gaussian_casscf.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_gaussian_casscf.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_gaussian_spin.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_gaussian_spin.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/example_nanoribbon.py` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_nanoribbon.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/h2_on_au111.xyz` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/h2_on_au111.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/h2_on_hbn.xyz` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/h2_on_hbn.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/examples/workflows/si_bulk.xyz` & `aiida_nanotech_empa-1.0.0b1/examples/workflows/si_bulk.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b0/pyproject.toml` & `aiida_nanotech_empa-1.0.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 "nanotech_empa.cp2k.phonons" = "aiida_nanotech_empa.workflows.cp2k:Cp2kPhononsWorkChain"
 
 
 [project.entry-points."aiida.schedulers"]
 slurm_ethz_euler = "aiida_nanotech_empa.schedulers:ETHZEulerSlurmScheduler"
 
 [tool.bumpver]
-current_version = "v1.0.0b0"
+current_version = "v1.0.0b1"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}."
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `aiida_nanotech_empa-1.0.0b0/PKG-INFO` & `aiida_nanotech_empa-1.0.0b1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-nanotech-empa
-Version: 1.0.0b0
+Version: 1.0.0b1
 Summary: AiiDA plugins and workflows developed at nanotech@surfaces group from Empa.
 Author: nanotech@surfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: Intended Audience :: Science/Research
@@ -56,19 +56,21 @@
 
 ```shell
 pip install aiida-nanotech-empa
 ```
 
 ## For maintainers
 
-To create a new release, clone the repository, install development dependencies with `pip install '.[dev]'`, and then execute `bumpver update --major/--minor/--patch`.
+To create a new release, clone the repository, install development dependencies with `pip install '.[dev]'`, and then execute `bumpver update --dry --major (--minor/--patch)`.
+This will display the changes that will be made to the repository - check them carefully.
+
+Once you are happy with the changes, remove the `--dry` option and re-execute the command.
 This will:
 
   1. Create a tagged release with bumped version and push it to the repository.
   2. Trigger a GitHub actions workflow that creates a GitHub release.
 
 Additional notes:
 
-  - Use the `--dry` option to preview the release change.
   - The release tag (e.g. a/b/rc) is determined from the last release.
-    Use the `--tag` option to switch the release tag.
+    Use the `--tag beta (alpha/gamma)`  option to switch the release tag.
```

