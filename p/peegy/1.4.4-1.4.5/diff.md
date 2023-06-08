# Comparing `tmp/peegy-1.4.4.tar.gz` & `tmp/peegy-1.4.5.tar.gz`

## Comparing `peegy-1.4.4.tar` & `peegy-1.4.5.tar`

### file list

```diff
@@ -1,184 +1,184 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/.gitattributes
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 peegy-1.4.4/.gitlab-ci.yml
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 peegy-1.4.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 peegy-1.4.4/CONTRIBUTING.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 peegy-1.4.4/MANIFEST.in
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 peegy-1.4.4/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/__init__.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 peegy-1.4.4/requirements.txt
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 peegy-1.4.4/setup.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/README.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/__init__.py
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_abr_peak_detection.py
--rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_eog_removal_template_.py
--rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_peak_detection.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_peak_detection_bootstrap.py
--rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_peak_detection_filters.py
--rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_video.py
--rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_weighted_average.py
--rw-r--r--   0        0        0    10304 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_acc_weighted_vs_standard_average.py
--rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_dss_frequency_domain_bias_test.py
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_dss_time_domain_bias_test.py
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_f_test.py
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_ht2_test.py
--rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_ht2_test_weighted_average.py
--rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_no_layout.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_assr_phase_locking_value_test.py
--rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_ffr_artifact_removal.py
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_using_own_data_trials.py
--rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 peegy-1.4.4/examples/example_using_own_raw_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/__init__.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/channel_definitions.py
--rw-r--r--   0        0        0    31413 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/edf_bdf_reader.py
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/eegReaderAbstractClasses.py
--rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/eeg_definitions.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/events.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/definitions/tables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/directories/__init__.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/directories/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/__init__.py
--rw-r--r--   0        0        0    20913 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/edf_bdf_reader.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/generic_csv_reader.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/synergy_reader.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/xml_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/eeg/__init__.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/eeg/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/__init__.py
--rw-r--r--   0        0        0    20273 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/file_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/__init__.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
--rw-r--r--   0        0        0    11573 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/dataReadingTools.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/extsys_tools.py
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/storage/__init__.py
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/storage/data_storage_reading_tools.py
--rw-r--r--   0        0        0    16923 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/storage/data_storage_tools.py
--rw-r--r--   0        0        0    29698 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/io/storage/plot_tools.py
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/KIT-160.lay
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/__init__.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi128.lay
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi16.lay
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi160.lay
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi256.lay
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi32.lay
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi32_2_EXT.lay
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi32_fnirs_MP.lay
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi32_fnirs_jaime.lay
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi64.lay
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi64_2_EXT.lay
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/biosemi64_3_EXT.lay
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/emotive14.lay
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/layouts.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/layouts/neuroscan64.lay
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/plot/__init__.py
--rw-r--r--   0        0        0    50141 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/plot/eeg_ave_epochs_plot_tools.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/plot/eeg_plot_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/events/__init__.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/events/event_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/__init__.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/attach.py
--rw-r--r--   0        0        0    27695 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/definitions.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/detection.py
--rw-r--r--   0        0        0    31702 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/epochs.py
--rw-r--r--   0        0        0    33830 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/general.py
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/interpolation.py
--rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/io.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/pipeline.py
--rw-r--r--   0        0        0    15881 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/plot.py
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/regression.py
--rw-r--r--   0        0        0    22127 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/simulate.py
--rw-r--r--   0        0        0    38922 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/spatial_filtering.py
--rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/statistics.py
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/storage.py
--rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/time_frequency.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/bootstrap/__init__.py
--rw-r--r--   0        0        0    22270 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/pipe/bootstrap/bootstrap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/statistics/__init__.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/statistics/definitions.py
--rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/statistics/eeg_statistic_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/system/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/system/memory.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/system/progress.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/__init__.py
--rw-r--r--   0        0        0    21075 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/eeg_epoch_operators.py
--rw-r--r--   0        0        0    70505 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/epochs_processing_tools.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/math_tools.py
--rw-r--r--   0        0        0    48694 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/weightedAverage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/detection/__init__.py
--rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/detection/definitions.py
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/detection/time_domain_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/__init__.py
--rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/eegFiltering.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/resampling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/eog_tools/__init__.py
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/eog_tools/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/__init__.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/definitions.py
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/fitting/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/fitting/fitting_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/multiprocessing/__init__.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/template_generator/__init__.py
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/template_generator/auditory_waveforms.py
--rw-r--r--   0        0        0    37074 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/template_generator/h0.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/video/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/processing/tools/video/recording.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/__init__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/dss_unit_tests.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/eeg_test_resampling.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/javerager_test.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/read_data_test.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_assr_moving_average.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_average_spectrogram_power.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_biosemi_class.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_biosemi_reader.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_bootstraping.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_edf_reader.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_eeg_notch_filter.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_eog_removal_correlation.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_eog_template_removal.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_eog_template_valderrama_20118.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_et_tools.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_filter.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_fir_filter_mt.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_fir_filter_ols.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_fiter_mt.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_freq_noise_estimation.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_freq_noise_estimation_plots.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_frequency_average_epochs.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_generic_reader.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_hotelling_t2.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_ica_average_epochs.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_multiprocessing.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_noise_generator.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_norm_corr.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_parse_processing_chain.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_peakdetection.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_phase_locking_value.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_pooled_freq_noise_estimation.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_scrolling.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_spatial_filtering_example1.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_spatial_filtering_example6.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_spatial_filtering_freq_domain.py
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_spatial_filtering_freq_domain_2.py
--rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_w_average_epochs.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_xml_to_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/artifact_removal/__init__.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/artifact_removal/ir_test.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/artifact_removal/regression_artifact_removal.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/artifact_removal/xcorr_artifact_removal.py
--rw-r--r--   0        0        0  1182949 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/aep_gui/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/signal_generator/__init__.py
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/signal_generator/noise_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/units/__init__.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 peegy-1.4.4/peegy/tools/units/unit_tools.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 peegy-1.4.4/.gitignore
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 peegy-1.4.4/LICENSE.txt
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 peegy-1.4.4/pyproject.toml
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 peegy-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/.gitattributes
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 peegy-1.4.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 peegy-1.4.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 peegy-1.4.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 peegy-1.4.5/MANIFEST.in
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 peegy-1.4.5/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 peegy-1.4.5/requirements.txt
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 peegy-1.4.5/setup.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/README.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/__init__.py
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_abr_peak_detection.py
+-rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_acc_eog_removal_template_.py
+-rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_acc_peak_detection.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_acc_peak_detection_bootstrap.py
+-rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_acc_peak_detection_filters.py
+-rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_acc_video.py
+-rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_acc_weighted_average.py
+-rw-r--r--   0        0        0    10304 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_acc_weighted_vs_standard_average.py
+-rw-r--r--   0        0        0    15706 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_assr_dss_frequency_domain_bias_test.py
+-rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_assr_dss_time_domain_bias_test.py
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_assr_f_test.py
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_assr_ht2_test.py
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_assr_ht2_test_weighted_average.py
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_assr_no_layout.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_assr_phase_locking_value_test.py
+-rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_ffr_artifact_removal.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_using_own_data_trials.py
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 peegy-1.4.5/examples/example_using_own_raw_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/definitions/__init__.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/definitions/channel_definitions.py
+-rw-r--r--   0        0        0    31413 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/definitions/edf_bdf_reader.py
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/definitions/eegReaderAbstractClasses.py
+-rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/definitions/eeg_definitions.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/definitions/events.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/definitions/tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/directories/__init__.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/directories/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/__init__.py
+-rw-r--r--   0        0        0    20913 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/edf_bdf_reader.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/generic_csv_reader.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/synergy_reader.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/xml_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/eeg/__init__.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/eeg/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/external_tools/__init__.py
+-rw-r--r--   0        0        0    20273 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/external_tools/file_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/external_tools/aep_gui/__init__.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
+-rw-r--r--   0        0        0    11573 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/external_tools/aep_gui/dataReadingTools.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/external_tools/aep_gui/extsys_tools.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/storage/__init__.py
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/storage/data_storage_reading_tools.py
+-rw-r--r--   0        0        0    16923 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/storage/data_storage_tools.py
+-rw-r--r--   0        0        0    31149 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/io/storage/plot_tools.py
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/KIT-160.lay
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/__init__.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi128.lay
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi16.lay
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi160.lay
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi256.lay
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi32.lay
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi32_2_EXT.lay
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi32_fnirs_MP.lay
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi32_fnirs_jaime.lay
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi64.lay
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi64_2_EXT.lay
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/biosemi64_3_EXT.lay
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/emotive14.lay
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/layouts.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/layouts/neuroscan64.lay
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/plot/__init__.py
+-rw-r--r--   0        0        0    50152 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/plot/eeg_ave_epochs_plot_tools.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/plot/eeg_plot_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/events/__init__.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/events/event_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/__init__.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/attach.py
+-rw-r--r--   0        0        0    27836 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/definitions.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/detection.py
+-rw-r--r--   0        0        0    31842 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/epochs.py
+-rw-r--r--   0        0        0    33830 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/general.py
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/interpolation.py
+-rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/io.py
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/pipeline.py
+-rw-r--r--   0        0        0    15881 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/plot.py
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/regression.py
+-rw-r--r--   0        0        0    22127 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/simulate.py
+-rw-r--r--   0        0        0    38921 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/spatial_filtering.py
+-rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/statistics.py
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/storage.py
+-rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/time_frequency.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/bootstrap/__init__.py
+-rw-r--r--   0        0        0    22414 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/pipe/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/statistics/__init__.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/statistics/definitions.py
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/statistics/eeg_statistic_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/system/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/system/memory.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/system/progress.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/__init__.py
+-rw-r--r--   0        0        0    21075 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/eeg_epoch_operators.py
+-rw-r--r--   0        0        0    70505 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/epochs_processing_tools.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/math_tools.py
+-rw-r--r--   0        0        0    48694 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/weightedAverage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/detection/__init__.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/detection/definitions.py
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/detection/time_domain_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/filters/__init__.py
+-rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/filters/eegFiltering.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/filters/resampling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/filters/eog_tools/__init__.py
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/filters/eog_tools/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/filters/spatial_filtering/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/filters/spatial_filtering/definitions.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/fitting/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/fitting/fitting_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/multiprocessing/__init__.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/template_generator/__init__.py
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/template_generator/auditory_waveforms.py
+-rw-r--r--   0        0        0    37074 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/template_generator/h0.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/video/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/processing/tools/video/recording.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/dss_unit_tests.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/eeg_test_resampling.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/javerager_test.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/read_data_test.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_assr_moving_average.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_average_spectrogram_power.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_biosemi_class.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_biosemi_reader.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_bootstraping.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_edf_reader.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_eeg_notch_filter.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_eog_removal_correlation.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_eog_template_removal.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_eog_template_valderrama_20118.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_et_tools.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_filter.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_fir_filter_mt.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_fir_filter_ols.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_fiter_mt.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_freq_noise_estimation.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_freq_noise_estimation_plots.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_frequency_average_epochs.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_generic_reader.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_hotelling_t2.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_ica_average_epochs.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_multiprocessing.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_noise_generator.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_norm_corr.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_parse_processing_chain.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_peakdetection.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_phase_locking_value.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_pooled_freq_noise_estimation.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_scrolling.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_spatial_filtering_example1.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_spatial_filtering_example6.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_spatial_filtering_freq_domain.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_spatial_filtering_freq_domain_2.py
+-rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_w_average_epochs.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_xml_to_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/artifact_removal/__init__.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/artifact_removal/ir_test.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/artifact_removal/regression_artifact_removal.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/artifact_removal/xcorr_artifact_removal.py
+-rw-r--r--   0        0        0  1182949 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/tools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/tools/aep_gui/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/tools/signal_generator/__init__.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/tools/signal_generator/noise_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/tools/units/__init__.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 peegy-1.4.5/peegy/tools/units/unit_tools.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 peegy-1.4.5/.gitignore
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 peegy-1.4.5/LICENSE.txt
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 peegy-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 peegy-1.4.5/PKG-INFO
```

### Comparing `peegy-1.4.4/.gitlab-ci.yml` & `peegy-1.4.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/CODE_OF_CONDUCT.md` & `peegy-1.4.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/CONTRIBUTING.md` & `peegy-1.4.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/Readme.md` & `peegy-1.4.5/Readme.md`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/requirements.txt` & `peegy-1.4.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/setup.py` & `peegy-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_abr_peak_detection.py` & `peegy-1.4.5/examples/example_abr_peak_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_acc_eog_removal_template_.py` & `peegy-1.4.5/examples/example_acc_eog_removal_template_.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_acc_peak_detection.py` & `peegy-1.4.5/examples/example_acc_peak_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_acc_peak_detection_bootstrap.py` & `peegy-1.4.5/examples/example_acc_peak_detection_bootstrap.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_acc_peak_detection_filters.py` & `peegy-1.4.5/examples/example_acc_peak_detection_filters.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_acc_video.py` & `peegy-1.4.5/examples/example_acc_video.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_acc_weighted_average.py` & `peegy-1.4.5/examples/example_acc_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_acc_weighted_vs_standard_average.py` & `peegy-1.4.5/examples/example_acc_weighted_vs_standard_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_assr_dss_frequency_domain_bias_test.py` & `peegy-1.4.5/examples/example_assr_dss_frequency_domain_bias_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     n_bootstraps=100,
     epoch_length=epoch_length,
     event_code=1.0,
     bootstrap_targets=[
         BootstrapTarget(
             test_name='HT2',
             group_by=['channel', 'frequency_tested'],
-            target_values=['f'])])
+            target_values=['f', 'rn', 'snr'])])
 
 pipeline.run()
 # %%
 # Compute global field power (GFP)
 # ---------------------------------------
 # We compute the GFP across channels and epochs. A new channel with the GFP is appended to the data
```

### Comparing `peegy-1.4.4/examples/example_assr_dss_time_domain_bias_test.py` & `peegy-1.4.5/examples/example_assr_dss_time_domain_bias_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_assr_f_test.py` & `peegy-1.4.5/examples/example_assr_f_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_assr_ht2_test.py` & `peegy-1.4.5/examples/example_assr_ht2_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_assr_ht2_test_weighted_average.py` & `peegy-1.4.5/examples/example_assr_ht2_test_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_assr_ht2_test_wrong_bias_frequnecy.py` & `peegy-1.4.5/examples/example_assr_ht2_test_wrong_bias_frequnecy.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_assr_no_layout.py` & `peegy-1.4.5/examples/example_assr_no_layout.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_assr_phase_locking_value_test.py` & `peegy-1.4.5/examples/example_assr_phase_locking_value_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_ffr_artifact_removal.py` & `peegy-1.4.5/examples/example_ffr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_using_own_data_trials.py` & `peegy-1.4.5/examples/example_using_own_data_trials.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/examples/example_using_own_raw_data.py` & `peegy-1.4.5/examples/example_using_own_raw_data.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/definitions/channel_definitions.py` & `peegy-1.4.5/peegy/definitions/channel_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/definitions/edf_bdf_reader.py` & `peegy-1.4.5/peegy/definitions/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/definitions/eegReaderAbstractClasses.py` & `peegy-1.4.5/peegy/definitions/eegReaderAbstractClasses.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/definitions/eeg_definitions.py` & `peegy-1.4.5/peegy/definitions/eeg_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/definitions/events.py` & `peegy-1.4.5/peegy/definitions/events.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/definitions/tables.py` & `peegy-1.4.5/peegy/definitions/tables.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/directories/tools.py` & `peegy-1.4.5/peegy/directories/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/edf_bdf_reader.py` & `peegy-1.4.5/peegy/io/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/generic_csv_reader.py` & `peegy-1.4.5/peegy/io/generic_csv_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/synergy_reader.py` & `peegy-1.4.5/peegy/io/synergy_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/xml_tools.py` & `peegy-1.4.5/peegy/io/xml_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/eeg/reader.py` & `peegy-1.4.5/peegy/io/eeg/reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/external_tools/file_tools.py` & `peegy-1.4.5/peegy/io/external_tools/file_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/external_tools/aep_gui/aep_matlab_tools.py` & `peegy-1.4.5/peegy/io/external_tools/aep_gui/aep_matlab_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/external_tools/aep_gui/dataReadingTools.py` & `peegy-1.4.5/peegy/io/external_tools/aep_gui/dataReadingTools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/external_tools/aep_gui/extsys_tools.py` & `peegy-1.4.5/peegy/io/external_tools/aep_gui/extsys_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py` & `peegy-1.4.5/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/storage/data_storage_reading_tools.py` & `peegy-1.4.5/peegy/io/storage/data_storage_reading_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/storage/data_storage_tools.py` & `peegy-1.4.5/peegy/io/storage/data_storage_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/io/storage/plot_tools.py` & `peegy-1.4.5/peegy/io/storage/plot_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         # col_domains = df['domain']
     idx_cols = np.arange(col_conditions.size)
 
     # common_x_axis = np.unique(col_conditions).size == 1
     groups = df.groupby(_rows_and_cols)
     fig_out, ax = plt.subplots(n_rows, n_cols)
     gs = gridspec.GridSpec(n_rows, n_cols)
+    all_ax_row_label = []
     for _id, ((_current_row_group, _current_col_group), _group) in enumerate(groups):
         _current_group = _group
         if blend_subcategories:
             _current_group = _group.iloc[[0]].copy().reset_index()
             if _current_group['y'].shape[0] > 1:
                 _current_group['y'] = _current_group['y'].apply(lambda x: np.vstack(_group.y).T)
         _idx_row = idx_rows[_current_row_group == row_conditions].squeeze()
@@ -226,14 +227,15 @@
             ax_row_label.set_yticklabels([])
             ax_row_label.tick_params(
                 axis='y',  # changes apply to the x-axis
                 which='both',  # both major and minor ticks are affected
                 right=False,  # ticks along the bottom edge are off
                 left=False,  # ticks along the top edge are off
                 labelleft=True)
+            all_ax_row_label.append(ax_row_label)
 
             if _domain == 'time':
                 if time_xlim is not None:
                     ax.set_xlim(time_xlim)
                 if time_ylim is not None:
                     ax.set_ylim(time_ylim)
                 if time_vmarkers is not None:
@@ -261,37 +263,40 @@
                           labels,
                           loc='upper center',
                           fontsize=8,
                           frameon=False,
                           ncol=len(labels))
 
     all_axes = fig_out.get_axes()
-    all_axis_with_data = np.all([ax.has_data() for ax in all_axes])
+    all_axis_with_data = np.all([ax.has_data() for ax in all_axes if ax not in all_ax_row_label])
 
     if ylabel is None:
         if y_unit_to is not None:
             fig_out.supylabel('Amplitude [{:}]'.format(y_unit_to), size=fontsize)
     else:
         fig_out.supylabel(ylabel, size=fontsize)
-    if unique_row_domains and all_axis_with_data and np.all(row_domains == 'time'):
+    if unique_row_domains and all_axis_with_data and np.all(row_domains == 'time') and n_cols > 1:
         fig_out.supxlabel('Time [{:}]'.format(_x_unit_to), size=fontsize)
-    if unique_row_domains and all_axis_with_data and np.all(row_domains == 'frequency'):
+    if unique_row_domains and all_axis_with_data and np.all(row_domains == 'frequency') and n_cols > 1:
         fig_out.supxlabel('Frequency [{:}]'.format(_x_unit_to), size=fontsize)
 
     for ax in all_axes:
-        if not ax.has_data():
+        if not ax.has_data() and ax not in all_ax_row_label:
             ax.get_xaxis().set_visible(False)
             ax.set_xticklabels([])
             ax.set_yticklabels([])
             ax.set_xlabel('')
             continue
         ax.spines['top'].set_visible(False)
-        if unique_row_domains and all_axis_with_data and not ax.get_subplotspec().is_last_row():
-            ax.set_xticklabels([])
-            ax.set_xlabel('')
+        if unique_row_domains and all_axis_with_data:
+            if not ax.get_subplotspec().is_last_row():
+                ax.set_xticklabels([])
+                ax.set_xlabel('')
+            if n_cols > 1:
+                ax.set_xlabel('')
         ax.spines['left'].set_visible(True)
         ax.spines['right'].set_visible(False)
         ax.tick_params(labelsize=6)
 
     inch = 2.54
     fig_out.set_size_inches(12.0 / inch, 2.25 * len(row_conditions) / inch)
     fig_out.subplots_adjust(top=0.98, bottom=0.08, hspace=0.0, left=0.15, right=0.95)
@@ -409,37 +414,40 @@
                                                 group_by=_rows_and_cols,
                                                 channels_column='channel',
                                                 topographic_value='topo_value',
                                                 layout=layout,
                                                 apply_function=apply_function,
                                                 fun_args=fun_args
                                                 )
-
     if color_map_label is None:
         color_map_label = topographic_value
-
     groups = sub_groups.groupby(_rows_and_cols)
     fig_out = plt.figure(constrained_layout=True)
     widths = [1.0] * n_cols
     heights = [1.0] * n_rows
     heights.append(0.1)
-    gs = fig_out.add_gridspec(ncols=n_cols, nrows=n_rows + 1,
+    widths.append(0.01)
+    gs = fig_out.add_gridspec(ncols=n_cols + 1, nrows=n_rows + 1,
                               width_ratios=widths,
                               height_ratios=heights)
     if max_topographic_value is None:
-        max_sub = sub_groups.potentials.apply(lambda x: np.ma.dstack([_val for _val in x]).max()).max()
+        max_sub_groups = sub_groups[sub_groups.potentials.apply(lambda x: np.size(x) > 1)]
+        max_sub = max_sub_groups.potentials.apply(
+            lambda x: np.ma.dstack([_val for _val in x]).max()).max()
     else:
         max_sub = max_topographic_value
 
     if min_topographic_value is None:
-        min_sub = sub_groups.potentials.apply(lambda x: np.ma.dstack([_val for _val in x]).min()).min()
+        min_sub_groups = sub_groups[sub_groups.potentials.apply(lambda x: np.size(x) > 1)]
+        min_sub = min_sub_groups.potentials.apply(
+            lambda x: np.ma.dstack([_val for _val in x]).min()).min()
     else:
         min_sub = min_topographic_value
     max_distance = sub_groups.max_distance.max()
-
+    all_ax_row_label = []
     for _id, ((_current_row_group, _current_col_group), _group) in enumerate(groups):
         if _group.shape[0] == 0 or np.all(np.isnan(_group.potentials.values[0])):
             continue
         _idx_row = idx_rows[_current_row_group == row_conditions].squeeze()
         _idx_col = idx_cols[_current_col_group == col_conditions].squeeze()
         ax = plt.subplot(gs[_idx_row, _idx_col])
         panel_title = ''
@@ -448,15 +456,14 @@
         if title_by == 'col':
             panel_title = '{:}'.format(_current_col_group)
 
         if title_by == 'both':
             panel_title = '{:} / {:}'.format(_current_row_group, _current_col_group)
 
         ax.set_title(panel_title, y=1 + title_v_offset, size=fontsize)
-        # std_average = np.ma.mean(_group.potentials.values[0], axis=2)
         if _group.potentials.values.size > 1:
             std_average = _group.potentials.apply(
                 lambda x: apply_function(np.ma.dstack([_val for _val in x]), *fun_args)).values[0]
         else:
             std_average = _group.potentials.values[0]
         ax_im = ax.imshow(std_average.T, origin='lower',
                           extent=(-max_distance, max_distance, -max_distance, max_distance),
@@ -470,14 +477,38 @@
                    levels,
                    origin='lower',
                    extent=(-max_distance, max_distance, -max_distance, max_distance),
                    linewidths=contour_line_width,
                    colors='k',
                    linestyles='solid')
         ax.autoscale(enable=False)
+        ax.set_xticks([])
+        ax.set_yticks([])
+        ax.axis('off')
+        _last_col_ax = plt.subplot(gs[_idx_row, n_cols])
+        _last_col_ax.set_xticks([])
+        _last_col_ax.set_yticks([])
+        _last_col_ax.axis('off')
+        ax_row_label = _last_col_ax.twinx()
+        ax_row_label.autoscale(enable=False)
+        ax_row_label.set_ylabel(_current_row_group, size=fontsize)
+        ax_row_label.set_yticklabels([])
+        ax_row_label.tick_params(
+            axis='y',  # changes apply to the x-axis
+            which='both',  # both major and minor ticks are affected
+            right=False,  # ticks along the bottom edge are off
+            left=False,  # ticks along the top edge are off
+            labelleft=True)
+        ax_row_label.spines['left'].set_visible(False)
+        ax_row_label.spines['right'].set_visible(False)
+        ax_row_label.spines['top'].set_visible(False)
+        ax_row_label.spines['bottom'].set_visible(False)
+        ax_row_label.set_xticks([])
+        ax_row_label.set_yticks([])
+        all_ax_row_label.append(ax_row_label)
         # plot color bar
 
         if _id == 0:
             c_bar_ax = plt.subplot(gs[-1, :])
             c_bar = fig_out.colorbar(ax_im, cax=c_bar_ax, orientation='horizontal', format='%.1f')
             c_bar.set_label(color_map_label, fontsize=fontsize)
             tick_locator = ticker.MaxNLocator(nbins=3)
@@ -494,26 +525,23 @@
             for i, lay in enumerate(_layout):
                 if lay.label in channel_labels:
                     ax.plot(lay.x, lay.y, 'o', color='b', markersize=0.2)
                 else:
                     ax.plot(lay.x, lay.y, 'o', color='grey', markersize=0.2)
                 if show_sensor_label:
                     ax.text(lay.x, lay.y, s=lay.label, fontsize=6)
-        ax.set_xticks([])
-        ax.set_yticks([])
-        ax.axis('off')
 
     all_axes = fig_out.get_axes()
     for ax in all_axes:
         if ax == c_bar.ax:
             continue
         ax.spines['top'].set_visible(False)
         ax.set_xticklabels([])
         ax.set_xlabel('')
-        ax.spines['left'].set_visible(True)
+        ax.spines['left'].set_visible(False)
         ax.spines['right'].set_visible(False)
     inch = 2.54
     fig_out.suptitle(title)
     fig_out.set_size_inches(3.2 * len(col_conditions) / inch, h=3.2 * len(row_conditions) / inch)
     return fig_out
```

### Comparing `peegy-1.4.4/peegy/layouts/KIT-160.lay` & `peegy-1.4.5/peegy/layouts/KIT-160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi128.lay` & `peegy-1.4.5/peegy/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi16.lay` & `peegy-1.4.5/peegy/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi160.lay` & `peegy-1.4.5/peegy/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi256.lay` & `peegy-1.4.5/peegy/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi32.lay` & `peegy-1.4.5/peegy/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi32_2_EXT.lay` & `peegy-1.4.5/peegy/layouts/biosemi32_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi32_fnirs_MP.lay` & `peegy-1.4.5/peegy/layouts/biosemi32_fnirs_MP.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi32_fnirs_jaime.lay` & `peegy-1.4.5/peegy/layouts/biosemi32_fnirs_jaime.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi64.lay` & `peegy-1.4.5/peegy/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi64_2_EXT.lay` & `peegy-1.4.5/peegy/layouts/biosemi64_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/biosemi64_3_EXT.lay` & `peegy-1.4.5/peegy/layouts/biosemi64_3_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/emotive14.lay` & `peegy-1.4.5/peegy/layouts/emotive14.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/layouts.py` & `peegy-1.4.5/peegy/layouts/layouts.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/layouts/neuroscan64.lay` & `peegy-1.4.5/peegy/layouts/neuroscan64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/plot/eeg_ave_epochs_plot_tools.py` & `peegy-1.4.5/peegy/plot/eeg_ave_epochs_plot_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,14 @@
                 gs = gridspec.GridSpec(1, 1)
                 ax1 = plt.subplot(gs[0])
 
             if offset_step is None:
                 offset_step = np.max(np.max(np.abs(_ave_data.data[:, ch_idx]), axis=0))
         offset_vector = np.arange(n_ch_to_plot) * offset_step
         _offset_idx = np.argwhere(np.in1d(all_labels, _channels)).squeeze()
-        all_peaks = None
         all_markers = _ave_data.markers
         rn_up, rn_down = None, None
 
         all_peaks = None
         if _ave_data.peaks is not None:
             all_peaks = _ave_data.peaks
         if _ave_data.domain == Domain.time:
@@ -178,16 +177,16 @@
         # add detected peaks
         _max_peak_amp = -np.inf
         for i, _ch in enumerate(_channels):
             _current_offset = np.atleast_1d(offset_vector[_offset_idx])[i]
             if all_markers is not None:
                 _subset = all_markers.query('channel == "{:}"'.format(_ch))
                 for _idx, _m in _subset.iterrows():
-                    ax1.add_patch(Rectangle((_m.x_ini, _m.y_ini - _current_offset),
-                                            _m.x_end - _m.x_ini, _m.y_end - _m.y_ini,
+                    ax1.add_patch(Rectangle((_m.x_ini.value, _m.y_ini.value - _current_offset),
+                                            _m.x_end.value - _m.x_ini.value, _m.y_end.value - _m.y_ini.value,
                                             edgecolor='k'))
             if all_peaks is not None and all_peaks.shape[0] and \
                     not np.all(all_peaks.amp.apply(lambda x_value: np.isnan(x_value.value))):
                 _idx_amps = all_peaks.amp.apply(lambda x_value: not np.isnan(x_value.value))
                 all_peaks = all_peaks[_idx_amps]
                 _max_peak_amp = np.maximum(all_peaks.amp, _max_peak_amp)
                 _subset = all_peaks.query('channel == "{:}"'.format(_ch))
```

### Comparing `peegy-1.4.4/peegy/plot/eeg_plot_tools.py` & `peegy-1.4.5/peegy/plot/eeg_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/events/event_tools.py` & `peegy-1.4.5/peegy/processing/events/event_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/attach.py` & `peegy-1.4.5/peegy/processing/pipe/attach.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/definitions.py` & `peegy-1.4.5/peegy/processing/pipe/definitions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import copy
-
 from peegy.definitions.channel_definitions import Domain, ChannelItem, ChannelType
 from peegy.definitions import tables
 from peegy.directories.tools import DirectoryPaths
 from peegy.definitions.events import Events, SingleEvent
 from peegy.tools.units.unit_tools import set_default_unit
 import inspect
 import pandas as pd
 import io
 import gc
 import astropy.units as u
-import itertools
 import abc
 import matplotlib.pyplot as plt
 import numpy as np
 from tqdm import tqdm
 import pyqtgraph as pg
+import time
 pg.setConfigOption('leftButtonPan', False)
 
 
 class DataNode(object):
     """
     Core data object used to keep data. During the creation, it requires the sampling rate and the actual data.
     Data is passed in a numpy array of n * m or n * m * t, where n represent samples, m channels, and t trials.
@@ -300,20 +299,20 @@
         if _max_time is None:
             _max_time = self._data.shape[0] / self.fs
 
         if n_events:
             if epoch_length is None:
                 epoch_length = ((_max_time - _min_time) / n_events)
             new_event_times = np.sort(
-                _min_time + np.random.rand(n_events) * (_max_time - _min_time - epoch_length))
-            events = np.array([])
-            for _s, in zip(new_event_times):
-                events = np.append(events, SingleEvent(code=event_code,
-                                                       time_pos=_s,
-                                                       dur=dur))
+                _min_time + np.random.rand(n_events) * (_max_time - _min_time - epoch_length), kind='quicksort')
+            events = np.empty(new_event_times.size, dtype=SingleEvent)
+            for i, _s, in enumerate(new_event_times):
+                events[i] = SingleEvent(code=event_code,
+                                        time_pos=_s,
+                                        dur=dur)
             self.events = Events(events=np.array(events))
 
 
 class InputOutputQtFigure(object):
     """
     This class is a wrapper to allow sphinx showing qt figures
     """
@@ -403,15 +402,18 @@
         properties_list = [_i[0] for _i in inspect.getmembers(DataNode, lambda o: isinstance(o, property))]
         attributes = [a for a in dir(self.input_node) if not (a.startswith('__') or a.startswith('_')) and
                       a not in callable_list and a not in properties_list]
         pars = {_a: getattr(self.input_node, _a) for _a in attributes}
         self.output_node = DataNode(data=np.array([]),
                                     **pars
                                     )  # Output data must be DataNode class
+        start = time.time()
         self.transform_data(**self.function_args)
+        end = time.time()
+        print('Elapsed time - {:}: {:.3f}s'.format(self.name, end - start))
         self.ready = True
 
         if not self.keep_input_node:
             if isinstance(self.input_node, DataNode):
                 self.input_node.data = None
             self.input_node = None
             gc.collect()
@@ -463,17 +465,14 @@
     :param plot_output: bool indicating if output_node data should be plotted
     :param ch_to_plot: list of strings indicating the labels of the channels to be shown. If empty, all channels
     will be shown.
     :param de_mean: if True, lines will be centred around the mean and then offset
     """
     if not plot_input and not plot_output:
         return
-    symbols = itertools.cycle(
-        ['o', 's', 't', 'd', '+', 't1', 't2', 't3', 'p', 'h', 'star', 'x', 'arrow_up', 'arrow_right',
-         'arrow_down', 'arrow_left', 'crosshair'])
     data_in = None
     if input_output_process.input_node is not None:
         data_in = copy.copy(input_output_process.input_node.data)
         name_in = input_output_process.input_process.name
         if input_output_process.input_node.domain == Domain.frequency:
             data_in = np.abs(data_in)
     data_out = None
@@ -531,40 +530,32 @@
                 for _t in tqdm(range(data_in.shape[2]),
                                desc='Generating input plot per epochs for channel {:}'.format(_label)):
                     ax.plot(x_in, data_in[:, _i, _t], pen=_color, name=_name if _t == 0 else None)
                     pg.QtCore.QCoreApplication.processEvents()
             ax.addItem(text_item)
 
             if input_output_process.input_node.events is not None:
-                itertools.tee(symbols)
                 _codes = np.unique(input_output_process.input_node.events.get_events_code(include_bad_events=True))
                 for _code in _codes:
                     _events = input_output_process.input_node.events.get_events(code=_code, include_bad_events=True)
-                    _symbol = next(symbols)
                     _good_events = np.array([])
                     _bad_events = np.array([])
                     for _ev in _events:
                         if _ev.bad_event:
                             _bad_events = np.append(_bad_events, _ev.time_pos.value)
                         else:
                             _good_events = np.append(_good_events, _ev.time_pos.value)
                     if _good_events.size:
-                        ax.plot(x=_good_events,
-                                y=0.0 * _good_events + offset.value * _pos,
-                                pen=None,
-                                symbol=_symbol,
-                                symbolBrush=_color,
-                                symbolSize=6)
+                        _pvl = plotVerticalLines()
+                        ax.addItem(_pvl)
+                        _pvl.setVerticalLines(_good_events, pen=_color)
                     if _bad_events.size:
-                        ax.plot(x=_bad_events,
-                                y=0.0 * _bad_events + offset.value * _pos,
-                                pen=None,
-                                symbol='x',
-                                symbolBrush='red',
-                                symbolSize=9)
+                        _pvl = plotVerticalLines()
+                        ax.addItem(_pvl)
+                        _pvl.setVerticalLines(_bad_events, pen='r')
 
         if input_output_process.input_node.domain == Domain.time:
             ax.setLabel('bottom', "Time [{:}]".format(input_output_process.input_node.x.unit))
             ax.setLabel('left', "Amplitude [{:}]".format(input_output_process.input_node.data.unit))
         if input_output_process.input_node.domain == Domain.frequency:
             ax.setLabel('bottom', "Time [{:}]".format(input_output_process.input_node.x.unit))
             ax.setLabel('left', "Frequency [{:}]".format(input_output_process.input_node.data.unit))
@@ -590,42 +581,64 @@
                 for _t in tqdm(range(data_out.shape[2]),
                                desc='Generating output plot per epochs for channel {:}'.format(_label)):
                     ax.plot(x_out, data_out[:, _i, _t], pen=_color, name=_name if _t == 0 else None)
                     pg.QtCore.QCoreApplication.processEvents()
 
             ax.addItem(text_item)
             if input_output_process.output_node.events is not None:
-                itertools.tee(symbols)
                 _codes = np.unique(input_output_process.output_node.events.get_events_code())
                 for _code in _codes:
                     _events = input_output_process.output_node.events.get_events(code=_code, include_bad_events=True)
-                    _symbol = next(symbols)
                     _good_events = np.array([])
                     _bad_events = np.array([])
                     for _ev in _events:
                         if _ev.bad_event:
                             _bad_events = np.append(_bad_events, _ev.time_pos.value)
                         else:
                             _good_events = np.append(_good_events, _ev.time_pos.value)
                     if _good_events.size:
-                        ax.plot(x=_good_events,
-                                y=0.0 * _good_events + offset.value * _pos,
-                                pen=None,
-                                symbol=_symbol,
-                                symbolBrush=_color,
-                                symbolSize=6)
+                        _pvl = plotVerticalLines()
+                        ax.addItem(_pvl)
+                        _pvl.setVerticalLines(_good_events, pen=_color)
+
                     if _bad_events.size:
-                        ax.plot(x=_bad_events,
-                                y=0.0 * _bad_events + offset.value * _pos,
-                                pen=None,
-                                symbol='x',
-                                symbolBrush='red',
-                                symbolSize=9)
+                        _pvl = plotVerticalLines()
+                        ax.addItem(_pvl)
+                        _pvl.setVerticalLines(_bad_events, pen='r')
 
         if input_output_process.output_node.domain == Domain.time:
             ax.setLabel('bottom', "Time [{:}]".format(input_output_process.output_node.x.unit))
             ax.setLabel('left', "Amplitude [{:}]".format(input_output_process.output_node.data.unit))
         if input_output_process.output_node.domain == Domain.frequency:
             ax.setLabel('bottom', "Time [{:}]".format(input_output_process.output_node.x.unit))
             ax.setLabel('left', "Frequency [{:}]".format(input_output_process.output_node.data.unit))
     pg.QtCore.QCoreApplication.processEvents()
     return win
+
+
+class plotVerticalLines(pg.PlotDataItem):
+    def __init__(self, container: pg.PlotItem = None):
+        super(plotVerticalLines, self).__init__()
+        self.pen = None
+
+    def dataBounds(self, ax, frac=1.0, orthoRange=None):
+        return [None, None]
+
+    def setVerticalLines(self, x, pen=None):
+        self.pen = pen
+        x = np.vstack((x, x)).T.astype(float)
+        y = np.zeros_like(x)
+        vb = self.getViewBox()
+        xr, yr = vb.viewRange()
+        y[:, 0] = yr[0]
+        y[:, 1] = yr[1]
+        self.setData(x.ravel(), y.ravel(), connect='pairs', pen=self.pen)
+        vb.sigYRangeChanged.connect(self._y_range_changed)
+
+    def _y_range_changed(self, viewbox):
+        xr, yr = viewbox.viewRange()
+        # get the original not transformed clipped etc.
+        x = self.xData
+        y = self.yData
+        y[0::2] = yr[0]
+        y[1::2] = yr[1]
+        self.setData(x, y, connect='pairs', pen=self.pen)
```

### Comparing `peegy-1.4.4/peegy/processing/pipe/detection.py` & `peegy-1.4.5/peegy/processing/pipe/detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/epochs.py` & `peegy-1.4.5/peegy/processing/pipe/epochs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from peegy.processing.statistics.eeg_statistic_tools import hotelling_t_square_test, f_test
 from peegy.processing.tools.eeg_epoch_operators import w_mean, effective_sampling_size
 import numpy as np
 import pandas as pd
 import os
 import pyfftw
 import astropy.units as u
-from tqdm import tqdm
 from peegy.tools.units.unit_tools import set_default_unit
 from PyQt5.QtCore import QLibraryInfo
+from numba import njit
 os.environ["QT_QPA_PLATFORM_PLUGIN_PATH"] = QLibraryInfo.location(QLibraryInfo.PluginsPath)
 
 
 class EpochData(InputOutputProcess):
     def __init__(self, input_process=InputOutputProcess,
                  pre_stimulus_interval: u.quantity.Quantity = None,
                  post_stimulus_interval: u.quantity.Quantity = None,
@@ -101,19 +101,16 @@
         _idx_to_keep = np.logical_and(events_index >= 0,
                                       events_index + buffer_size <= self.input_node.data.shape[0])
         events_index = events_index[_idx_to_keep]
         possible_indexes = events_index.size
         if possible_indexes < total_indexes:
             print("{:} events ignored as data length won't fit epoch length".format(
                 total_indexes - possible_indexes))
-        epochs = np.zeros((buffer_size, self.input_node.data.shape[1], events_index.size), dtype=np.float32)
         print('There are {:} events with code {:}'.format(events_index.shape[0], self.event_code))
-        for i, _event in enumerate(tqdm(events_index, desc='Epoching data', miniters=0)):
-            # ensure that blocks match buffer size
-            epochs[:, :, i] = data[_event:_event + buffer_size, :]
+        epochs = extract_epochs(data=data, buffer_size=buffer_size, events_index=events_index)
         epochs = epochs * data.unit
         print('A total of {:} epochs were obtained using event code {:}, each with a duration of {:.3f}'.format(
             epochs.shape[2],
             self.event_code,
             (buffer_size / self.input_node.fs).to(u.s)))
         if self.demean:
             epochs = epochs - np.mean(epochs, axis=0)
@@ -124,14 +121,24 @@
                               _ini_sample)
             epochs = epochs - np.mean(epochs[_ini_sample:_end_sample, :, :], axis=0)
         self.output_node.data = epochs
         self.output_node.x_offset = pre_stimulus_interval
         self.output_node.events = None
 
 
+@njit
+def extract_epochs(data: np.array = None,
+                   events_index: np.array = None,
+                   buffer_size: int = None):
+    epochs = np.zeros((buffer_size, data.shape[1], events_index.size), dtype=np.float32)
+    for i, _event in enumerate(events_index):
+        epochs[:, :, i] = data[_event:_event + buffer_size, :]
+    return epochs
+
+
 class RejectEpochs(InputOutputProcess):
     def __init__(self, input_process=InputOutputProcess,
                  std_threshold: float = None,
                  rejection_percentage: float = None,
                  rejection_threshold: u.quantity.Quantity = None,
                  max_percentage_epochs_above_threshold: float = 1.0,
                  **kwargs):
```

### Comparing `peegy-1.4.4/peegy/processing/pipe/general.py` & `peegy-1.4.5/peegy/processing/pipe/general.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/interpolation.py` & `peegy-1.4.5/peegy/processing/pipe/interpolation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/io.py` & `peegy-1.4.5/peegy/processing/pipe/io.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/pipeline.py` & `peegy-1.4.5/peegy/processing/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/plot.py` & `peegy-1.4.5/peegy/processing/pipe/plot.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/regression.py` & `peegy-1.4.5/peegy/processing/pipe/regression.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/simulate.py` & `peegy-1.4.5/peegy/processing/pipe/simulate.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/spatial_filtering.py` & `peegy-1.4.5/peegy/processing/pipe/spatial_filtering.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 class CreateAndApplySpatialFilter(InputOutputProcess):
     def __init__(self, input_process=InputOutputProcess,
                  sf_join_frequencies: np.array = None,
                  sf_components=np.array([]),
                  sf_thr: float = 0.8,
                  keep0: int = None,
                  keep1: float = 1e-9,
-                 perc0: float = 0.99,
+                 perc0: float = 1.0,
                  perc1: float = None,
                  test_frequencies: u.Quantity = None,
                  delta_frequency: u.Quantity = 5 * u.Hz,
                  block_size: int = 10,
                  n_tracked_points: int = None,
                  demean_data: bool = True,
                  weight_data: bool = True,
```

### Comparing `peegy-1.4.4/peegy/processing/pipe/statistics.py` & `peegy-1.4.5/peegy/processing/pipe/statistics.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/storage.py` & `peegy-1.4.5/peegy/processing/pipe/storage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/time_frequency.py` & `peegy-1.4.5/peegy/processing/pipe/time_frequency.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/pipe/bootstrap/bootstrap.py` & `peegy-1.4.5/peegy/processing/pipe/bootstrap/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,21 +167,22 @@
         bootstrapped_and_ref_tables = pd.merge(boots_df,
                                                ref_table,
                                                how='left',
                                                on=common_cols,
                                                )
 
         df_boots = bootstrapped_and_ref_tables.groupby(list(set(bootstrapped_and_ref_tables.keys()).difference(
-            ['value'])), as_index=False).apply(
+            ['value', 'statistic_value'])), as_index=False).apply(
             lambda x: pd.Series({'stats': get_bootstrap_estimates(samples=x['value'],
                                                                   statistic=x['statistic_value'],
                                                                   alpha_level=self.alpha_level,
                                                                   one_sided=self.one_sided)}))
 
-        (df_boots['mean'],
+        (df_boots['statistic_value'],
+         df_boots['mean'],
          df_boots['median'],
          df_boots['std'],
          df_boots['ci_lower'],
          df_boots['ci_upper'],
          df_boots['sample_size'],
          df_boots['p_value']) = zip(*df_boots.stats)
         df_boots['one_sided'] = self.one_sided
@@ -372,33 +373,34 @@
 
 
 def get_bootstrap_estimates(samples: np.array = None,
                             statistic: np.array = None,
                             alpha_level: float = 0.05,
                             one_sided=True):
     # remove nan that may be present
-    samples = samples[~pd.isna(samples)]
-    _stat = np.unique(statistic)
+    samples = np.array(samples[~pd.isna(samples)])
+    statistic_value = np.unique(statistic)
+    assert statistic_value.size == 1
     sample_size = samples.shape[0]
     sorted_samples = np.sort(samples, axis=0)
     mean = np.mean(samples, axis=0)
     median = np.median(samples, axis=0)
     std = np.std(samples, axis=0)
     _alpha = alpha_level
     if not one_sided:
         _alpha = alpha_level / 2.0
 
     _i_upper = np.minimum(int(samples.shape[0] * (1 - _alpha)), samples.shape[0])
     _i_lower = np.maximum(int(samples.shape[0] * _alpha), 0)
     ci_lower = sorted_samples[_i_lower]
     ci_upper = sorted_samples[_i_upper]
-    diff = np.abs(_stat - sorted_samples)
+    diff = np.abs(statistic_value - sorted_samples)
     _idx_match = np.argmin(diff, axis=0) + 1
     p_value = 1 - _idx_match / sample_size
-    return [mean, median, std, ci_lower, ci_upper, sample_size, p_value]
+    return [statistic_value[0], mean, median, std, ci_lower, ci_upper, sample_size, p_value]
 
 
 def get_tables(pipeline: PipePool = None,
                targets: [BootstrapTarget] = None):
     output = pd.DataFrame()
     for _source, _value in pipeline.items():
         for _target in targets:
```

### Comparing `peegy-1.4.4/peegy/processing/statistics/definitions.py` & `peegy-1.4.5/peegy/processing/statistics/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/statistics/eeg_statistic_tools.py` & `peegy-1.4.5/peegy/processing/statistics/eeg_statistic_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/system/progress.py` & `peegy-1.4.5/peegy/processing/system/progress.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/eeg_epoch_operators.py` & `peegy-1.4.5/peegy/processing/tools/eeg_epoch_operators.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/epochs_processing_tools.py` & `peegy-1.4.5/peegy/processing/tools/epochs_processing_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/weightedAverage.py` & `peegy-1.4.5/peegy/processing/tools/weightedAverage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/detection/definitions.py` & `peegy-1.4.5/peegy/processing/tools/detection/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,13 +230,13 @@
     def __init__(self,
                  x_ini: u.Quantity = 0,
                  x_end: u.Quantity = 0,
                  y_ini: u.Quantity = 0,
                  y_end: u.Quantity = 0,
                  label: str = None,
                  channel: str = None):
-        self.x_ini = x_ini
-        self.x_end = x_end
-        self.y_ini = y_ini
-        self.y_end = y_end
+        self.x_ini = set_default_unit(x_ini, u.dimensionless_unscaled)
+        self.x_end = set_default_unit(x_end, u.dimensionless_unscaled)
+        self.y_ini = set_default_unit(y_ini, u.dimensionless_unscaled)
+        self.y_end = set_default_unit(y_end, u.dimensionless_unscaled)
         self.channel = channel
         self.label = label
```

### Comparing `peegy-1.4.4/peegy/processing/tools/detection/time_domain_tools.py` & `peegy-1.4.5/peegy/processing/tools/detection/time_domain_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/filters/eegFiltering.py` & `peegy-1.4.5/peegy/processing/tools/filters/eegFiltering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/filters/resampling.py` & `peegy-1.4.5/peegy/processing/tools/filters/resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/filters/eog_tools/tools.py` & `peegy-1.4.5/peegy/processing/tools/filters/eog_tools/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/definitions.py` & `peegy-1.4.5/peegy/processing/tools/filters/spatial_filtering/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py` & `peegy-1.4.5/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py` & `peegy-1.4.5/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/template_generator/auditory_waveforms.py` & `peegy-1.4.5/peegy/processing/tools/template_generator/auditory_waveforms.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/template_generator/h0.json` & `peegy-1.4.5/peegy/processing/tools/template_generator/h0.json`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/processing/tools/video/recording.py` & `peegy-1.4.5/peegy/processing/tools/video/recording.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/dss_unit_tests.py` & `peegy-1.4.5/peegy/test/dss_unit_tests.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/eeg_test_resampling.py` & `peegy-1.4.5/peegy/test/eeg_test_resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/javerager_test.py` & `peegy-1.4.5/peegy/test/javerager_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/read_data_test.py` & `peegy-1.4.5/peegy/test/read_data_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_assr_moving_average.py` & `peegy-1.4.5/peegy/test/test_assr_moving_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_average_spectrogram_power.py` & `peegy-1.4.5/peegy/test/test_average_spectrogram_power.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_biosemi_class.py` & `peegy-1.4.5/peegy/test/test_biosemi_class.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_biosemi_reader.py` & `peegy-1.4.5/peegy/test/test_biosemi_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_bootstraping.py` & `peegy-1.4.5/peegy/test/test_bootstraping.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_edf_reader.py` & `peegy-1.4.5/peegy/test/test_edf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_eeg_notch_filter.py` & `peegy-1.4.5/peegy/test/test_eeg_notch_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_eog_removal_correlation.py` & `peegy-1.4.5/peegy/test/test_eog_removal_correlation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_eog_template_removal.py` & `peegy-1.4.5/peegy/test/test_eog_template_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_eog_template_valderrama_20118.py` & `peegy-1.4.5/peegy/test/test_eog_template_valderrama_20118.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_et_tools.py` & `peegy-1.4.5/peegy/test/test_et_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_filter.py` & `peegy-1.4.5/peegy/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_fir_filter_mt.py` & `peegy-1.4.5/peegy/test/test_fir_filter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_fir_filter_ols.py` & `peegy-1.4.5/peegy/test/test_fir_filter_ols.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_fiter_mt.py` & `peegy-1.4.5/peegy/test/test_fiter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_freq_noise_estimation.py` & `peegy-1.4.5/peegy/test/test_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_freq_noise_estimation_plots.py` & `peegy-1.4.5/peegy/test/test_freq_noise_estimation_plots.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_frequency_average_epochs.py` & `peegy-1.4.5/peegy/test/test_frequency_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_hotelling_t2.py` & `peegy-1.4.5/peegy/test/test_hotelling_t2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_ica_average_epochs.py` & `peegy-1.4.5/peegy/test/test_ica_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_multiprocessing.py` & `peegy-1.4.5/peegy/test/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_noise_generator.py` & `peegy-1.4.5/peegy/test/test_noise_generator.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_norm_corr.py` & `peegy-1.4.5/peegy/test/test_norm_corr.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_peakdetection.py` & `peegy-1.4.5/peegy/test/test_peakdetection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_phase_locking_value.py` & `peegy-1.4.5/peegy/test/test_phase_locking_value.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_pooled_freq_noise_estimation.py` & `peegy-1.4.5/peegy/test/test_pooled_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_scrolling.py` & `peegy-1.4.5/peegy/test/test_scrolling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_spatial_filtering_example1.py` & `peegy-1.4.5/peegy/test/test_spatial_filtering_example1.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_spatial_filtering_example6.py` & `peegy-1.4.5/peegy/test/test_spatial_filtering_example6.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_spatial_filtering_freq_domain.py` & `peegy-1.4.5/peegy/test/test_spatial_filtering_freq_domain.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_spatial_filtering_freq_domain_2.py` & `peegy-1.4.5/peegy/test/test_spatial_filtering_freq_domain_2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_w_average_epochs.py` & `peegy-1.4.5/peegy/test/test_w_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/artifact_removal/ir_test.py` & `peegy-1.4.5/peegy/test/artifact_removal/ir_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/artifact_removal/regression_artifact_removal.py` & `peegy-1.4.5/peegy/test/artifact_removal/regression_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/artifact_removal/xcorr_artifact_removal.py` & `peegy-1.4.5/peegy/test/artifact_removal/xcorr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat` & `peegy-1.4.5/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/peegy/tools/signal_generator/noise_functions.py` & `peegy-1.4.5/peegy/tools/signal_generator/noise_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,25 +108,25 @@
     # ensure odd number of taps
     if n_taps is not None:
         n_taps = 2 * (n_taps // 2) + 1
     # synthesize phase
     if not frequency_domain:
         gain = np.sqrt(psd_noise)
         if freq_resolution is not None:
-            n_taps = int(np.maximum(1, n // np.floor(freq_resolution / (fs / n))))
+            n_taps = int(np.maximum(1, np.round(fs / freq_resolution)))
             n_taps = 2 * (n_taps // 2) + 1
         # force last frequency to be fs / 2
         freq[-1, :] = fs / 2
         print('noise generation: {:} taps FIR design'.format(n_taps))
         _b = firwin2(numtaps=n_taps,
                      freq=freq[:, 0],
                      fs=fs,
                      gain=gain[:, 0],
                      antisymmetric=False)
-        white_noise = np.random.rand(n, n_channels)
+        white_noise = np.random.randn(n, n_channels)
         noise = filt_data(b=_b, data=white_noise * u.dimensionless_unscaled, mode='original').value
         # plot results
         # f, h = freqz(_b, worN=np.linspace(0, fs / 2, n_taps), fs=fs)
         # import matplotlib.pyplot as plt
         # plt.plot(f, 20 * np.log10(np.abs(h)), label='Filter response')
         # plt.plot(freq.flatten(), 20 * np.log10(gain), label='Target response')
     else:
```

### Comparing `peegy-1.4.4/peegy/tools/units/unit_tools.py` & `peegy-1.4.5/peegy/tools/units/unit_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/LICENSE.txt` & `peegy-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.4.4/pyproject.toml` & `peegy-1.4.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm", "wheel", "hatchling"]
+requires = ["setuptools", "setuptools-scm", "wheel", "hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 #build-backend = "setuptools.build_meta"
 
 [project]
 name = "peegy"
-version = "1.4.4"
+version = "1.4.5"
 authors = [{name = "Jaime Undurraga", email = "jaime.undurraga@gmail.com"},]
 description = "Tools to pipeline bulk analyses of EEG and other modalities."
 requires-python = ">=3.9"
 license = {text = "MIT"}
 
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -19,16 +19,18 @@
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Bio-Informatics"]
 
 dynamic = ["dependencies", "readme"]
 
+[tool.hatch.metadata.hooks.requirements_txt]
+files = ["requirements.txt"]
+
 [tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
 readme = {file = ["README.md"]}
 
 [project.urls]
 "Homepage" = "https://gitlab.com/open-source-brain/peegy/"
 "Examples" = "https://open-source-brain.gitlab.io/peegy/"
```

