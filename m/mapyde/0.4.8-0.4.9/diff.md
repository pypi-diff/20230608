# Comparing `tmp/mapyde-0.4.8.tar.gz` & `tmp/mapyde-0.4.9.tar.gz`

## Comparing `mapyde-0.4.8.tar` & `mapyde-0.4.9.tar`

### file list

```diff
@@ -1,132 +1,132 @@
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 mapyde-0.4.8/mkdocs.yml
--rw-r--r--   0        0        0    31329 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/FCChh.tcl
--rw-r--r--   0        0        0    30874 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/FCChh_PileUp.tcl
--rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/delphes_card_ATLAS.tcl
--rw-r--r--   0        0        0    21543 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/delphes_card_ATLAS_fixedbtageffic.tcl
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/delphes_card_ATLAS_lowptleptons.tcl
--rw-r--r--   0        0        0    24241 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons.tcl
--rw-r--r--   0        0        0    24350 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons_notrackineffic.tcl
--rw-r--r--   0        0        0    53993 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/dzResolutionVsP.tcl
--rw-r--r--   0        0        0    61796 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/momentumResolutionVsP.tcl
--rw-r--r--   0        0        0    77748 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/delphes/muonMomentumResolutionVsP.tcl
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/madspin/isr2L_c1c1_nodecays
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/madspin/isr2L_n2c1_nodecays
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/madspin/isr2L_n2c1_nojets_nodecays
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/madspin/isr2L_n2c1m_nodecays
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/madspin/isr2L_n2c1m_nojets_nodecays
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/madspin/isr2L_n2c1p_nodecays
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/madspin/isr2L_n2c1p_nojets_nodecays
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/madspin/isr2L_n2n1_nodecays
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/madspin/isr2L_n2n1_nojets_nodecays
--rw-r--r--   0        0        0    17921 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/GluinoBino.slha
--rw-r--r--   0        0        0    18960 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/Higgsino.slha
--rw-r--r--   0        0        0    48855 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/Higgsino_CMS_v4.slha
--rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/SleptonBino.slha
--rw-r--r--   0        0        0    20649 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/SleptonSneutrinoBino.slha
--rw-r--r--   0        0        0    22557 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/SleptonWinoBino.slha
--rw-r--r--   0        0        0    17927 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/StopBino.slha
--rw-r--r--   0        0        0    17904 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/WinoBino.slha
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/sm-full.slha
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/param/sm.slha
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/Hbb
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_EWK
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_charginos
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_charginos_v4
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_n2c1p
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_n2c1p_v4
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_v4
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_EWK_n2c1p
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_EWK_n2c1p_v4
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VBFSUSY_N2C1p
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VjjEWK
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/VjjQCD
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/Zbb
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/Zmumu
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/charginos
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/gluons
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_c1c1
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_c1c1_nodecays
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2c1
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2c1_nodecays
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2c1_nojets
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2c1_nojets_nodecays
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2c1m_nodecays
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2c1p_nodecays
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2n1
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2n1_nodecays
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2n1_nojets
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_n2n1_nojets_nodecays
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_nodecays
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_nojets
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isr2L_nojets_nodecays
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isrinc
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isrinc2j
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/isrslep
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/quarks
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/stops
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/stops_and_ttbar
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/ttbar
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/process/ttbar_and_gluino
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/pythia/pythia8_card.dat
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/pythia/pythia8_card_MLM.dat
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/pythia/pythia8_card_dipoleRecoil.dat
--rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/run/default_LO.dat
--rw-r--r--   0        0        0    17505 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/run/default_LO_oldformat.dat
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/run/default_NLO.dat
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/sherpa/tt
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 mapyde-0.4.8/cards/sherpa/ttbbjj
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/gen_ref_nav.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/index.md
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/install.md
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/intro.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/.overrides/main.html
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/.snippets/links.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/assets/css/custom.css
--rw-r--r--   0        0        0    29259 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/assets/images/logo.svg
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/cli/about.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/cli/reference.md
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/meta/authors.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mapyde-0.4.8/docs/meta/faq.md
--rw-r--r--   0        0        0  1155183 2020-02-02 00:00:00.000000 mapyde-0.4.8/likelihoods/Higgsino_2L_bkgonly.json
--rw-r--r--   0        0        0  1192502 2020-02-02 00:00:00.000000 mapyde-0.4.8/likelihoods/Slepton_bkgonly.json
--rw-r--r--   0        0        0  1155183 2020-02-02 00:00:00.000000 mapyde-0.4.8/likelihoods/WinoBino_noWeight_2L_bkgonly.json
--rwxr-xr-x   0        0        0     8087 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/Delphes2SA.py
--rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/FlatAna.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/FlatAna_uproot.py
--rw-r--r--   0        0        0    31519 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/HistCollections.py
--rwxr-xr-x   0        0        0     3750 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/SAtoJSON.py
--rwxr-xr-x   0        0        0     4109 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/SimpleAna.py
--rwxr-xr-x   0        0        0      766 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/formatSLHA.py
--rwxr-xr-x   0        0        0     1623 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/hepmcsplitter.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/likelihoodfitting.py
--rwxr-xr-x   0        0        0     2390 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/lowlevelAna.py
--rwxr-xr-x   0        0        0     4420 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/muscan.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/root2hdf5.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/root2hdf5_slepton.py
--rwxr-xr-x   0        0        0     2319 2020-02-02 00:00:00.000000 mapyde-0.4.8/scripts/tthhAna.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/_version.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/_version.pyi
--rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/container.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/prefix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/py.typed
--rw-r--r--   0        0        0    17331 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/runner.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/typing.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/backends/__init__.py
--rw-r--r--   0        0        0     9622 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/backends/madgraph.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/cli/__init__.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/cli/config.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 mapyde-0.4.8/src/mapyde/cli/run.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 mapyde-0.4.8/templates/defaults.toml
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 mapyde-0.4.8/templates/ewkinos.toml
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 mapyde-0.4.8/templates/sleptons.toml
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mapyde-0.4.8/tests/test_package.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 mapyde-0.4.8/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mapyde-0.4.8/LICENSE
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 mapyde-0.4.8/README.md
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 mapyde-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 mapyde-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 mapyde-0.4.9/mkdocs.yml
+-rw-r--r--   0        0        0    31329 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/FCChh.tcl
+-rw-r--r--   0        0        0    30874 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/FCChh_PileUp.tcl
+-rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS.tcl
+-rw-r--r--   0        0        0    21543 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_fixedbtageffic.tcl
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons.tcl
+-rw-r--r--   0        0        0    24241 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons.tcl
+-rw-r--r--   0        0        0    24350 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons_notrackineffic.tcl
+-rw-r--r--   0        0        0    53993 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/dzResolutionVsP.tcl
+-rw-r--r--   0        0        0    61796 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/momentumResolutionVsP.tcl
+-rw-r--r--   0        0        0    77748 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/delphes/muonMomentumResolutionVsP.tcl
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_c1c1_nodecays
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1_nodecays
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1_nojets_nodecays
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1m_nodecays
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1m_nojets_nodecays
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1p_nodecays
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2c1p_nojets_nodecays
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2n1_nodecays
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/madspin/isr2L_n2n1_nojets_nodecays
+-rw-r--r--   0        0        0    17921 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/GluinoBino.slha
+-rw-r--r--   0        0        0    18960 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/Higgsino.slha
+-rw-r--r--   0        0        0    48855 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/Higgsino_CMS_v4.slha
+-rw-r--r--   0        0        0    21364 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/SleptonBino.slha
+-rw-r--r--   0        0        0    20649 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/SleptonSneutrinoBino.slha
+-rw-r--r--   0        0        0    22557 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/SleptonWinoBino.slha
+-rw-r--r--   0        0        0    17927 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/StopBino.slha
+-rw-r--r--   0        0        0    17904 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/WinoBino.slha
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/sm-full.slha
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/param/sm.slha
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/Hbb
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWK
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_charginos
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_charginos_v4
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_n2c1p
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_n2c1p_v4
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_v4
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWK_n2c1p
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_EWK_n2c1p_v4
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VBFSUSY_N2C1p
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VjjEWK
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/VjjQCD
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/Zbb
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/Zmumu
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/charginos
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/gluons
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_c1c1
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_c1c1_nodecays
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1_nodecays
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1_nojets
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1_nojets_nodecays
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1m_nodecays
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2c1p_nodecays
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2n1
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2n1_nodecays
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2n1_nojets
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_n2n1_nojets_nodecays
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_nodecays
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_nojets
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isr2L_nojets_nodecays
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isrinc
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isrinc2j
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/isrslep
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/quarks
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/stops
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/stops_and_ttbar
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/ttbar
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/process/ttbar_and_gluino
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/pythia/pythia8_card.dat
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/pythia/pythia8_card_MLM.dat
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/pythia/pythia8_card_dipoleRecoil.dat
+-rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/run/default_LO.dat
+-rw-r--r--   0        0        0    17505 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/run/default_LO_oldformat.dat
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/run/default_NLO.dat
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/sherpa/tt
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 mapyde-0.4.9/cards/sherpa/ttbbjj
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/index.md
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/install.md
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/intro.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/.overrides/main.html
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    29259 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/cli/about.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/cli/reference.md
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/meta/authors.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mapyde-0.4.9/docs/meta/faq.md
+-rw-r--r--   0        0        0  1155183 2020-02-02 00:00:00.000000 mapyde-0.4.9/likelihoods/Higgsino_2L_bkgonly.json
+-rw-r--r--   0        0        0  1192502 2020-02-02 00:00:00.000000 mapyde-0.4.9/likelihoods/Slepton_bkgonly.json
+-rw-r--r--   0        0        0  1155183 2020-02-02 00:00:00.000000 mapyde-0.4.9/likelihoods/WinoBino_noWeight_2L_bkgonly.json
+-rwxr-xr-x   0        0        0     8087 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/Delphes2SA.py
+-rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/FlatAna.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/FlatAna_uproot.py
+-rw-r--r--   0        0        0    31519 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/HistCollections.py
+-rwxr-xr-x   0        0        0     3750 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/SAtoJSON.py
+-rwxr-xr-x   0        0        0     4109 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/SimpleAna.py
+-rwxr-xr-x   0        0        0      793 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/formatSLHA.py
+-rwxr-xr-x   0        0        0     1623 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/hepmcsplitter.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/likelihoodfitting.py
+-rwxr-xr-x   0        0        0     2390 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/lowlevelAna.py
+-rwxr-xr-x   0        0        0     4420 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/muscan.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/root2hdf5.py
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/root2hdf5_slepton.py
+-rwxr-xr-x   0        0        0     2319 2020-02-02 00:00:00.000000 mapyde-0.4.9/scripts/tthhAna.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/_version.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/_version.pyi
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/container.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/prefix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/py.typed
+-rw-r--r--   0        0        0    17331 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/runner.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/typing.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/backends/__init__.py
+-rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/backends/madgraph.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/cli/__init__.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/cli/config.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 mapyde-0.4.9/src/mapyde/cli/run.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 mapyde-0.4.9/templates/defaults.toml
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 mapyde-0.4.9/templates/ewkinos.toml
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 mapyde-0.4.9/templates/sleptons.toml
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mapyde-0.4.9/tests/test_package.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 mapyde-0.4.9/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mapyde-0.4.9/LICENSE
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 mapyde-0.4.9/README.md
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 mapyde-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 mapyde-0.4.9/PKG-INFO
```

### Comparing `mapyde-0.4.8/mkdocs.yml` & `mapyde-0.4.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/FCChh.tcl` & `mapyde-0.4.9/cards/delphes/FCChh.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/FCChh_PileUp.tcl` & `mapyde-0.4.9/cards/delphes/FCChh_PileUp.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/delphes_card_ATLAS.tcl` & `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/delphes_card_ATLAS_fixedbtageffic.tcl` & `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_fixedbtageffic.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/delphes_card_ATLAS_lowptleptons.tcl` & `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons.tcl` & `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons_notrackineffic.tcl` & `mapyde-0.4.9/cards/delphes/delphes_card_ATLAS_lowptleptons_sleptons_notrackineffic.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/dzResolutionVsP.tcl` & `mapyde-0.4.9/cards/delphes/dzResolutionVsP.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/momentumResolutionVsP.tcl` & `mapyde-0.4.9/cards/delphes/momentumResolutionVsP.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/delphes/muonMomentumResolutionVsP.tcl` & `mapyde-0.4.9/cards/delphes/muonMomentumResolutionVsP.tcl`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/madspin/isr2L_c1c1_nodecays` & `mapyde-0.4.9/cards/madspin/isr2L_c1c1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/madspin/isr2L_n2c1_nodecays` & `mapyde-0.4.9/cards/madspin/isr2L_n2c1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/madspin/isr2L_n2c1_nojets_nodecays` & `mapyde-0.4.9/cards/madspin/isr2L_n2c1_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/madspin/isr2L_n2c1m_nodecays` & `mapyde-0.4.9/cards/madspin/isr2L_n2c1m_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/madspin/isr2L_n2c1m_nojets_nodecays` & `mapyde-0.4.9/cards/madspin/isr2L_n2c1m_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/madspin/isr2L_n2c1p_nodecays` & `mapyde-0.4.9/cards/madspin/isr2L_n2c1p_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/madspin/isr2L_n2c1p_nojets_nodecays` & `mapyde-0.4.9/cards/madspin/isr2L_n2c1p_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/madspin/isr2L_n2n1_nodecays` & `mapyde-0.4.9/cards/madspin/isr2L_n2n1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/madspin/isr2L_n2n1_nojets_nodecays` & `mapyde-0.4.9/cards/madspin/isr2L_n2n1_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/GluinoBino.slha` & `mapyde-0.4.9/cards/param/GluinoBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/Higgsino.slha` & `mapyde-0.4.9/cards/param/Higgsino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/Higgsino_CMS_v4.slha` & `mapyde-0.4.9/cards/param/Higgsino_CMS_v4.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/SleptonBino.slha` & `mapyde-0.4.9/cards/param/SleptonBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/SleptonSneutrinoBino.slha` & `mapyde-0.4.9/cards/param/SleptonSneutrinoBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/SleptonWinoBino.slha` & `mapyde-0.4.9/cards/param/SleptonWinoBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/StopBino.slha` & `mapyde-0.4.9/cards/param/StopBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/WinoBino.slha` & `mapyde-0.4.9/cards/param/WinoBino.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/sm-full.slha` & `mapyde-0.4.9/cards/param/sm-full.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/param/sm.slha` & `mapyde-0.4.9/cards/param/sm.slha`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_EWK` & `mapyde-0.4.9/cards/process/VBFSUSY_EWK`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD` & `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_charginos` & `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_charginos`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_charginos_v4` & `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_charginos_v4`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_n2c1p` & `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_n2c1p`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_n2c1p_v4` & `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_n2c1p_v4`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_EWKQCD_v4` & `mapyde-0.4.9/cards/process/VBFSUSY_EWKQCD_v4`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_EWK_n2c1p` & `mapyde-0.4.9/cards/process/VBFSUSY_EWK_n2c1p`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_EWK_n2c1p_v4` & `mapyde-0.4.9/cards/process/VBFSUSY_EWK_n2c1p_v4`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/VBFSUSY_N2C1p` & `mapyde-0.4.9/cards/process/VBFSUSY_N2C1p`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/charginos` & `mapyde-0.4.9/cards/process/charginos`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L` & `mapyde-0.4.9/cards/process/isr2L`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_c1c1` & `mapyde-0.4.9/cards/process/isr2L_c1c1`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_c1c1_nodecays` & `mapyde-0.4.9/cards/process/isr2L_c1c1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2c1` & `mapyde-0.4.9/cards/process/isr2L_n2c1`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2c1_nodecays` & `mapyde-0.4.9/cards/process/isr2L_n2c1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2c1_nojets` & `mapyde-0.4.9/cards/process/isr2L_n2c1_nojets`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2c1_nojets_nodecays` & `mapyde-0.4.9/cards/process/isr2L_n2c1_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2c1m_nodecays` & `mapyde-0.4.9/cards/process/isr2L_n2c1m_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2c1p_nodecays` & `mapyde-0.4.9/cards/process/isr2L_n2c1p_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2n1` & `mapyde-0.4.9/cards/process/isr2L_n2n1`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2n1_nodecays` & `mapyde-0.4.9/cards/process/isr2L_n2n1_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2n1_nojets` & `mapyde-0.4.9/cards/process/isr2L_n2n1_nojets`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_n2n1_nojets_nodecays` & `mapyde-0.4.9/cards/process/isr2L_n2n1_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_nodecays` & `mapyde-0.4.9/cards/process/isr2L_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_nojets` & `mapyde-0.4.9/cards/process/isr2L_nojets`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isr2L_nojets_nodecays` & `mapyde-0.4.9/cards/process/isr2L_nojets_nodecays`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isrinc` & `mapyde-0.4.9/cards/process/isrinc`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isrinc2j` & `mapyde-0.4.9/cards/process/isrinc2j`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/isrslep` & `mapyde-0.4.9/cards/process/isrslep`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/stops` & `mapyde-0.4.9/cards/process/stops`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/stops_and_ttbar` & `mapyde-0.4.9/cards/process/stops_and_ttbar`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/process/ttbar_and_gluino` & `mapyde-0.4.9/cards/process/ttbar_and_gluino`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/pythia/pythia8_card.dat` & `mapyde-0.4.9/cards/pythia/pythia8_card.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/pythia/pythia8_card_MLM.dat` & `mapyde-0.4.9/cards/pythia/pythia8_card_MLM.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/pythia/pythia8_card_dipoleRecoil.dat` & `mapyde-0.4.9/cards/pythia/pythia8_card_dipoleRecoil.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/run/default_LO.dat` & `mapyde-0.4.9/cards/run/default_LO.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/run/default_LO_oldformat.dat` & `mapyde-0.4.9/cards/run/default_LO_oldformat.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/run/default_NLO.dat` & `mapyde-0.4.9/cards/run/default_NLO.dat`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/sherpa/tt` & `mapyde-0.4.9/cards/sherpa/tt`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/cards/sherpa/ttbbjj` & `mapyde-0.4.9/cards/sherpa/ttbbjj`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/docs/gen_ref_nav.py` & `mapyde-0.4.9/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/docs/index.md` & `mapyde-0.4.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/docs/install.md` & `mapyde-0.4.9/docs/install.md`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/docs/intro.md` & `mapyde-0.4.9/docs/intro.md`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/docs/assets/css/custom.css` & `mapyde-0.4.9/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/docs/assets/images/logo.svg` & `mapyde-0.4.9/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/likelihoods/Higgsino_2L_bkgonly.json` & `mapyde-0.4.9/likelihoods/Higgsino_2L_bkgonly.json`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/likelihoods/Slepton_bkgonly.json` & `mapyde-0.4.9/likelihoods/Slepton_bkgonly.json`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/likelihoods/WinoBino_noWeight_2L_bkgonly.json` & `mapyde-0.4.9/likelihoods/WinoBino_noWeight_2L_bkgonly.json`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/Delphes2SA.py` & `mapyde-0.4.9/scripts/Delphes2SA.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/FlatAna.py` & `mapyde-0.4.9/scripts/FlatAna.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/FlatAna_uproot.py` & `mapyde-0.4.9/scripts/FlatAna_uproot.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/HistCollections.py` & `mapyde-0.4.9/scripts/HistCollections.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/SAtoJSON.py` & `mapyde-0.4.9/scripts/SAtoJSON.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/SimpleAna.py` & `mapyde-0.4.9/scripts/SimpleAna.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/formatSLHA.py` & `mapyde-0.4.9/scripts/formatSLHA.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     sline = line.split()
     if len(sline) > 0:
         try:
             particle = int(sline[0])
             if (particle > 1000000 and particle <= 1000016) or (
                 particle > 2000000 and particle <= 2000016
             ):
-                line = line.replace(sline[1], "2.00000000e+03")
+                out = line.replace(sline[1], "2.00000000e+03")
         except ValueError:
             pass
-    output.write(line)
+    else:
+        out = line
+    output.write(out)
 
 
 output.close()
```

### Comparing `mapyde-0.4.8/scripts/hepmcsplitter.py` & `mapyde-0.4.9/scripts/hepmcsplitter.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/likelihoodfitting.py` & `mapyde-0.4.9/scripts/likelihoodfitting.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,13 +53,13 @@
 limit_results = cabinetry.fit.limit(model, data)
 
 print("visualizing results")
 cabinetry.visualize.limit(limit_results)
 print(limit_results.observed_limit)
 print(limit_results.expected_limit)
 
-pyhf.infer.test_statistics.q0
+# pyhf.infer.test_statistics.q0
 p_observed, p_expected = pyhf.infer.hypotest(
     1.0, data, model, test_stat="q0", return_expected=True
 )
 
 scipy.stats.norm.isf(p_expected, 0, 1)
```

### Comparing `mapyde-0.4.8/scripts/lowlevelAna.py` & `mapyde-0.4.9/scripts/lowlevelAna.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/muscan.py` & `mapyde-0.4.9/scripts/muscan.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/root2hdf5.py` & `mapyde-0.4.9/scripts/root2hdf5.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/root2hdf5_slepton.py` & `mapyde-0.4.9/scripts/root2hdf5_slepton.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/scripts/tthhAna.py` & `mapyde-0.4.9/scripts/tthhAna.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/src/mapyde/__init__.py` & `mapyde-0.4.9/src/mapyde/__init__.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/src/mapyde/container.py` & `mapyde-0.4.9/src/mapyde/container.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/src/mapyde/prefix.py` & `mapyde-0.4.9/src/mapyde/prefix.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/src/mapyde/runner.py` & `mapyde-0.4.9/src/mapyde/runner.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/src/mapyde/typing.py` & `mapyde-0.4.9/src/mapyde/typing.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/src/mapyde/utils.py` & `mapyde-0.4.9/src/mapyde/utils.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/src/mapyde/backends/madgraph.py` & `mapyde-0.4.9/src/mapyde/backends/madgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,29 +145,30 @@
     # tpl_variables = meta.find_undeclared_variables(parsed)
 
     pattern = re.compile(
         r"^\s*(?P<value>[^\s]+)\s*=\s*(?P<key>[a-z_0-9]+)\s*\!.*$", re.DOTALL
     )
     with in_place.InPlace(new_run_card_path) as fpointer:
         for line in fpointer:
+            output = line
             match = pattern.match(line)
             if match:
                 groups = match.groupdict()
                 span = match.span("value")
                 newvalue = str(run_options.pop(groups["key"], groups["value"]))
                 # update the line based on input from the user, default to what is in the file
-                line = line[: span[0]] + newvalue + line[span[1] :]
+                output = line[: span[0]] + newvalue + line[span[1] :]
                 if newvalue != groups["value"]:
                     log.info(
                         "    replacing value for %s: %s -> %s",
                         groups["key"],
                         groups["value"],
                         newvalue,
                     )
-            fpointer.write(line)
+            fpointer.write(output)
 
     unused_keys = list(run_options.keys())
     if unused_keys:
         log.error("Unused keys supplied by you: %s", unused_keys)
         raise KeyError(unused_keys[0])
 
     # Copy the proc card
@@ -251,10 +252,11 @@
 
     with mgconfig_card_path.open(mode="w", encoding="utf-8") as fpointer:
         # pylint: disable-next=consider-using-with
         for proc_line in new_proc_card_path.open(encoding="utf-8"):
             if not proc_line.strip():
                 continue
             if proc_line.startswith("output"):
-                proc_line = "output PROC_madgraph\n"
-            fpointer.write(proc_line)
+                fpointer.write("output PROC_madgraph\n")
+            else:
+                fpointer.write(proc_line)
         fpointer.write(mg5config)
```

### Comparing `mapyde-0.4.8/src/mapyde/cli/__init__.py` & `mapyde-0.4.9/src/mapyde/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/src/mapyde/cli/config.py` & `mapyde-0.4.9/src/mapyde/cli/config.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/src/mapyde/cli/run.py` & `mapyde-0.4.9/src/mapyde/cli/run.py`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/templates/defaults.toml` & `mapyde-0.4.9/templates/defaults.toml`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/templates/ewkinos.toml` & `mapyde-0.4.9/templates/ewkinos.toml`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/templates/sleptons.toml` & `mapyde-0.4.9/templates/sleptons.toml`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/.gitignore` & `mapyde-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/LICENSE` & `mapyde-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/README.md` & `mapyde-0.4.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# mapyde v0.4.8
+# mapyde v0.4.9
 
 MaPyDe stands for MadGraph-Pythia-Delphes which is a utility that allows one to
 run all of the various HEP toolings or chain them together and perform a quick
 analysis with the results, such as running CERN ATLAS SimpleAnalysis or pyhf.
 
 ---
 
@@ -12,27 +12,29 @@
 <img src="https://raw.githubusercontent.com/scipp-atlas/mapyde/main/docs/assets/images/logo.svg" alt="Mapyde logo" width="500" role="img">
 
 <!-- --8<-- [start:badges] -->
 
 <!-- prettier-ignore-start -->
 | | |
 | --- | --- |
-| CI/CD | [![CI - Test][actions-badge-ci]][actions-link-ci] [![CI - Docker][actions-badge-docker]][actions-link-docker] |
-| Docs | [![Docs][actions-badge-docs]][actions-link-docs] [![Zenodo][zenodo-badge]][zenodo-link] |
+| CI/CD | [![CI - Test][actions-badge-ci]][actions-link-ci] [![CI - Docker][actions-badge-docker]][actions-link-docker] [![Docs][actions-badge-docs]][actions-link-docs] |
+| Docs |  [![doc][doc-badge]][doc-link] [![Zenodo][zenodo-badge]][zenodo-link] |
 | Package | [![PyPI - Downloads][pypi-downloads]][pypi-link] [![PyPI - Version][pypi-version]][pypi-link] [![PyPI platforms][pypi-platforms]][pypi-link] [![Conda-Forge][conda-badge]][conda-link] |
 | Meta | [![GitHub - Discussion][github-discussions-badge]][github-discussions-link] [![GitHub - Issue][github-issues-badge]][github-issues-link] [![License - Apache 2.0][license-badge]][license-link] |
 
 [actions-badge-ci]:         https://github.com/scipp-atlas/mapyde/actions/workflows/ci.yml/badge.svg?branch=main
 [actions-link-ci]:          https://github.com/scipp-atlas/mapyde/actions/workflows/ci.yml?query=branch:main
 [actions-badge-docker]:     https://github.com/scipp-atlas/mapyde/actions/workflows/docker.yml/badge.svg?branch=main
 [actions-link-docker]:      https://github.com/scipp-atlas/mapyde/actions/workflows/docker.yml?query=branch:main
 [actions-badge-docs]:       https://github.com/scipp-atlas/mapyde/actions/workflows/docs.yml/badge.svg?branch=main
 [actions-link-docs]:        https://github.com/scipp-atlas/mapyde/actions/workflows/docs.yml?query=branch:main
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/mapyde
 [conda-link]:               https://github.com/conda-forge/mapyde-feedstock
+[doc-badge]:                https://img.shields.io/badge/docs-online-success
+[doc-link]:                 https://scipp-atlas.github.io/mapyde/latest/
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [github-discussions-link]:  https://github.com/scipp-atlas/mapyde/discussions
 [github-issues-badge]:      https://img.shields.io/static/v1?label=Issues&message=File&color=blue&logo=github
 [github-issues-link]:       https://github.com/scipp-atlas/mapyde/issues
 [pypi-link]:                https://pypi.org/project/mapyde/
 [pypi-downloads]:           https://img.shields.io/pypi/dm/mapyde.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/mapyde
```

### Comparing `mapyde-0.4.8/pyproject.toml` & `mapyde-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mapyde-0.4.8/PKG-INFO` & `mapyde-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapyde
-Version: 0.4.8
+Version: 0.4.9
 Summary: Generation, simulation, analysis, and statistical inference in one go.
 Project-URL: Homepage, https://scipp-atlas.github.io/mapyde/latest/
 Project-URL: Documentation, https://scipp-atlas.github.io/mapyde/0.4/
 Project-URL: Tracker, https://github.com/scipp-atlas/mapyde/issues
 Project-URL: Source, https://github.com/scipp-atlas/mapyde
 Author-email: Giordon Stark <kratsg@gmail.com>
 Maintainer-email: Mike Hance <mhance@ucsc.edu>
@@ -27,15 +27,15 @@
 Requires-Dist: in-place
 Requires-Dist: jinja2
 Requires-Dist: toml
 Requires-Dist: typer
 Requires-Dist: typing-extensions>=3.7; python_version < '3.11'
 Description-Content-Type: text/markdown
 
-# mapyde v0.4.8
+# mapyde v0.4.9
 
 MaPyDe stands for MadGraph-Pythia-Delphes which is a utility that allows one to
 run all of the various HEP toolings or chain them together and perform a quick
 analysis with the results, such as running CERN ATLAS SimpleAnalysis or pyhf.
 
 ---
 
@@ -45,27 +45,29 @@
 <img src="https://raw.githubusercontent.com/scipp-atlas/mapyde/main/docs/assets/images/logo.svg" alt="Mapyde logo" width="500" role="img">
 
 <!-- --8<-- [start:badges] -->
 
 <!-- prettier-ignore-start -->
 | | |
 | --- | --- |
-| CI/CD | [![CI - Test][actions-badge-ci]][actions-link-ci] [![CI - Docker][actions-badge-docker]][actions-link-docker] |
-| Docs | [![Docs][actions-badge-docs]][actions-link-docs] [![Zenodo][zenodo-badge]][zenodo-link] |
+| CI/CD | [![CI - Test][actions-badge-ci]][actions-link-ci] [![CI - Docker][actions-badge-docker]][actions-link-docker] [![Docs][actions-badge-docs]][actions-link-docs] |
+| Docs |  [![doc][doc-badge]][doc-link] [![Zenodo][zenodo-badge]][zenodo-link] |
 | Package | [![PyPI - Downloads][pypi-downloads]][pypi-link] [![PyPI - Version][pypi-version]][pypi-link] [![PyPI platforms][pypi-platforms]][pypi-link] [![Conda-Forge][conda-badge]][conda-link] |
 | Meta | [![GitHub - Discussion][github-discussions-badge]][github-discussions-link] [![GitHub - Issue][github-issues-badge]][github-issues-link] [![License - Apache 2.0][license-badge]][license-link] |
 
 [actions-badge-ci]:         https://github.com/scipp-atlas/mapyde/actions/workflows/ci.yml/badge.svg?branch=main
 [actions-link-ci]:          https://github.com/scipp-atlas/mapyde/actions/workflows/ci.yml?query=branch:main
 [actions-badge-docker]:     https://github.com/scipp-atlas/mapyde/actions/workflows/docker.yml/badge.svg?branch=main
 [actions-link-docker]:      https://github.com/scipp-atlas/mapyde/actions/workflows/docker.yml?query=branch:main
 [actions-badge-docs]:       https://github.com/scipp-atlas/mapyde/actions/workflows/docs.yml/badge.svg?branch=main
 [actions-link-docs]:        https://github.com/scipp-atlas/mapyde/actions/workflows/docs.yml?query=branch:main
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/mapyde
 [conda-link]:               https://github.com/conda-forge/mapyde-feedstock
+[doc-badge]:                https://img.shields.io/badge/docs-online-success
+[doc-link]:                 https://scipp-atlas.github.io/mapyde/latest/
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [github-discussions-link]:  https://github.com/scipp-atlas/mapyde/discussions
 [github-issues-badge]:      https://img.shields.io/static/v1?label=Issues&message=File&color=blue&logo=github
 [github-issues-link]:       https://github.com/scipp-atlas/mapyde/issues
 [pypi-link]:                https://pypi.org/project/mapyde/
 [pypi-downloads]:           https://img.shields.io/pypi/dm/mapyde.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/mapyde
```

