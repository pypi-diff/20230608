# Comparing `tmp/laboneq-2.7.0-py3-none-any.whl.zip` & `tmp/laboneq-2.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,86 +1,89 @@
-Zip file size: 939609 bytes, number of entries: 248
--rw-rw-rw-  2.0 unx        5 b- defN 23-May-25 13:25 laboneq/VERSION.txt
--rw-r--r--  2.0 unx      239 b- defN 23-May-24 14:34 laboneq/__init__.py
+Zip file size: 1004041 bytes, number of entries: 311
+-rw-rw-rw-  2.0 unx        5 b- defN 23-Jun-08 11:42 laboneq/VERSION.txt
+-rw-r--r--  2.0 unx      239 b- defN 23-Jun-01 08:47 laboneq/__init__.py
 -rw-r--r--  2.0 unx     2829 b- defN 23-Feb-02 07:13 laboneq/_token.py
--rw-r--r--  2.0 unx      928 b- defN 23-May-17 00:03 laboneq/_utils.py
+-rw-r--r--  2.0 unx      928 b- defN 23-Jun-01 08:47 laboneq/_utils.py
 -rw-r--r--  2.0 unx      238 b- defN 23-Feb-02 07:13 laboneq/_version.py
--rw-r--r--  2.0 unx     1538 b- defN 23-May-25 13:25 laboneq/simple.py
+-rw-r--r--  2.0 unx     1565 b- defN 23-Jun-01 12:35 laboneq/simple.py
 -rw-r--r--  2.0 unx      184 b- defN 23-Feb-02 07:13 laboneq/_observability/__init__.py
 -rw-r--r--  2.0 unx      538 b- defN 23-Feb-02 07:13 laboneq/_observability/tracing/__init__.py
 -rw-r--r--  2.0 unx      893 b- defN 23-Feb-16 12:45 laboneq/_observability/tracing/_noop_tracer.py
 -rw-r--r--  2.0 unx     2309 b- defN 23-Feb-16 12:45 laboneq/_observability/tracing/_tracer.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/application_management/__init__.py
+-rw-r--r--  2.0 unx     2658 b- defN 23-Jun-01 08:47 laboneq/application_management/application_manager.py
 -rw-r--r--  2.0 unx      444 b- defN 23-Feb-02 07:13 laboneq/compiler/__init__.py
 -rw-r--r--  2.0 unx      204 b- defN 23-Feb-02 07:13 laboneq/compiler/fastlogging.py
 -rw-rw-rw-  2.0 unx    22524 b- defN 23-May-17 00:03 laboneq/compiler/qccs-schema_2_5_0.json
 -rw-r--r--  2.0 unx      666 b- defN 23-Feb-02 07:13 laboneq/compiler/remote.py
 -rw-r--r--  2.0 unx      654 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/__init__.py
--rw-r--r--  2.0 unx    18645 b- defN 23-May-24 13:41 laboneq/compiler/code_generator/analyze_events.py
--rw-r--r--  2.0 unx    26665 b- defN 23-May-24 13:41 laboneq/compiler/code_generator/analyze_playback.py
--rw-r--r--  2.0 unx    72652 b- defN 23-May-25 13:25 laboneq/compiler/code_generator/code_generator.py
+-rw-r--r--  2.0 unx    18669 b- defN 23-Jun-07 10:17 laboneq/compiler/code_generator/analyze_events.py
+-rw-r--r--  2.0 unx    26669 b- defN 23-Jun-07 10:17 laboneq/compiler/code_generator/analyze_playback.py
+-rw-r--r--  2.0 unx    71964 b- defN 23-Jun-08 11:34 laboneq/compiler/code_generator/code_generator.py
 -rw-r--r--  2.0 unx     4026 b- defN 23-May-17 00:03 laboneq/compiler/code_generator/command_table_tracker.py
 -rw-r--r--  2.0 unx     2880 b- defN 23-May-17 00:03 laboneq/compiler/code_generator/compressor.py
 -rw-r--r--  2.0 unx     1414 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/feedback_register_allocator.py
 -rw-r--r--  2.0 unx    10355 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/interval_calculator.py
--rw-r--r--  2.0 unx    17825 b- defN 23-May-17 00:03 laboneq/compiler/code_generator/measurement_calculator.py
--rw-r--r--  2.0 unx    30380 b- defN 23-May-25 07:57 laboneq/compiler/code_generator/sampled_event_handler.py
--rw-r--r--  2.0 unx    19239 b- defN 23-May-25 13:25 laboneq/compiler/code_generator/seq_c_generator.py
--rw-r--r--  2.0 unx     6333 b- defN 23-May-17 00:03 laboneq/compiler/code_generator/seqc_tracker.py
--rw-r--r--  2.0 unx     9915 b- defN 23-May-25 07:57 laboneq/compiler/code_generator/signatures.py
+-rw-r--r--  2.0 unx    17825 b- defN 23-Jun-01 08:47 laboneq/compiler/code_generator/measurement_calculator.py
+-rw-r--r--  2.0 unx    30380 b- defN 23-Jun-01 08:47 laboneq/compiler/code_generator/sampled_event_handler.py
+-rw-r--r--  2.0 unx    18722 b- defN 23-Jun-01 08:47 laboneq/compiler/code_generator/seq_c_generator.py
+-rw-r--r--  2.0 unx     6333 b- defN 23-Jun-01 08:47 laboneq/compiler/code_generator/seqc_tracker.py
+-rw-r--r--  2.0 unx    10031 b- defN 23-Jun-01 08:47 laboneq/compiler/code_generator/signatures.py
 -rw-r--r--  2.0 unx     3500 b- defN 23-Feb-28 13:10 laboneq/compiler/code_generator/utils.py
--rw-r--r--  2.0 unx     7697 b- defN 23-May-25 07:57 laboneq/compiler/code_generator/wave_compressor.py
+-rw-r--r--  2.0 unx     9102 b- defN 23-Jun-08 08:55 laboneq/compiler/code_generator/wave_compressor.py
 -rw-r--r--  2.0 unx     1476 b- defN 23-Feb-28 13:10 laboneq/compiler/code_generator/wave_index_tracker.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/compiler/common/__init__.py
--rw-r--r--  2.0 unx     1093 b- defN 23-Apr-06 14:15 laboneq/compiler/common/awg_info.py
--rw-r--r--  2.0 unx     1926 b- defN 23-May-17 00:03 laboneq/compiler/common/awg_sampled_event.py
+-rw-r--r--  2.0 unx     1093 b- defN 23-Jun-08 11:34 laboneq/compiler/common/awg_info.py
+-rw-r--r--  2.0 unx     1926 b- defN 23-Jun-01 08:47 laboneq/compiler/common/awg_sampled_event.py
 -rw-r--r--  2.0 unx      480 b- defN 23-Feb-02 07:13 laboneq/compiler/common/awg_signal_type.py
--rw-r--r--  2.0 unx     4015 b- defN 23-May-17 00:03 laboneq/compiler/common/compiler_settings.py
--rw-r--r--  2.0 unx     6058 b- defN 23-May-17 00:03 laboneq/compiler/common/device_type.py
--rw-r--r--  2.0 unx     1624 b- defN 23-May-23 08:56 laboneq/compiler/common/event_type.py
+-rw-r--r--  2.0 unx     4015 b- defN 23-Jun-01 08:47 laboneq/compiler/common/compiler_settings.py
+-rw-r--r--  2.0 unx     6058 b- defN 23-Jun-01 08:47 laboneq/compiler/common/device_type.py
+-rw-r--r--  2.0 unx     1624 b- defN 23-Jun-01 08:47 laboneq/compiler/common/event_type.py
 -rw-r--r--  2.0 unx      229 b- defN 23-Mar-07 13:19 laboneq/compiler/common/play_wave_type.py
 -rw-r--r--  2.0 unx      580 b- defN 23-May-17 00:03 laboneq/compiler/common/pulse_parameters.py
--rw-r--r--  2.0 unx     2594 b- defN 23-May-24 13:41 laboneq/compiler/common/signal_obj.py
+-rw-r--r--  2.0 unx     2541 b- defN 23-Jun-07 10:17 laboneq/compiler/common/signal_obj.py
 -rw-r--r--  2.0 unx      400 b- defN 23-Feb-02 07:13 laboneq/compiler/common/trigger_mode.py
 -rw-r--r--  2.0 unx      154 b- defN 23-Feb-02 07:13 laboneq/compiler/experiment_access/__init__.py
 -rw-r--r--  2.0 unx      222 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/acquire_info.py
 -rw-r--r--  2.0 unx      349 b- defN 23-May-17 00:03 laboneq/compiler/experiment_access/device_info.py
--rw-r--r--  2.0 unx    45262 b- defN 23-May-25 13:25 laboneq/compiler/experiment_access/dsl_loader.py
--rw-r--r--  2.0 unx    16767 b- defN 23-May-23 08:56 laboneq/compiler/experiment_access/experiment_dao.py
--rw-r--r--  2.0 unx    14264 b- defN 23-May-23 08:56 laboneq/compiler/experiment_access/json_dumper.py
--rw-r--r--  2.0 unx    21043 b- defN 23-May-23 08:56 laboneq/compiler/experiment_access/json_loader.py
--rw-r--r--  2.0 unx     6182 b- defN 23-May-22 15:14 laboneq/compiler/experiment_access/loader_base.py
+-rw-r--r--  2.0 unx    45124 b- defN 23-Jun-06 11:55 laboneq/compiler/experiment_access/dsl_loader.py
+-rw-r--r--  2.0 unx    16726 b- defN 23-Jun-06 11:55 laboneq/compiler/experiment_access/experiment_dao.py
+-rw-r--r--  2.0 unx    14122 b- defN 23-Jun-01 12:35 laboneq/compiler/experiment_access/json_dumper.py
+-rw-r--r--  2.0 unx    20825 b- defN 23-Jun-06 11:55 laboneq/compiler/experiment_access/json_loader.py
+-rw-r--r--  2.0 unx     6256 b- defN 23-Jun-08 11:34 laboneq/compiler/experiment_access/loader_base.py
 -rw-r--r--  2.0 unx      270 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/marker.py
 -rw-r--r--  2.0 unx      286 b- defN 23-May-17 00:03 laboneq/compiler/experiment_access/oscillator_info.py
 -rw-r--r--  2.0 unx      197 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/param_ref.py
--rw-r--r--  2.0 unx     1311 b- defN 23-May-17 00:03 laboneq/compiler/experiment_access/pulse_def.py
--rw-r--r--  2.0 unx      851 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/section_info.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/section_signal_pulse.py
+-rw-r--r--  2.0 unx     1311 b- defN 23-Jun-01 08:47 laboneq/compiler/experiment_access/pulse_def.py
+-rw-r--r--  2.0 unx      817 b- defN 23-Jun-01 12:35 laboneq/compiler/experiment_access/section_info.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-May-26 09:40 laboneq/compiler/experiment_access/section_signal_pulse.py
 -rw-r--r--  2.0 unx      387 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/signal_info.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/compiler/scheduler/__init__.py
--rw-r--r--  2.0 unx     3265 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/case_schedule.py
--rw-r--r--  2.0 unx     7439 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/interval_schedule.py
--rw-r--r--  2.0 unx     3327 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/loop_iteration_schedule.py
--rw-r--r--  2.0 unx     8576 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/loop_schedule.py
--rw-r--r--  2.0 unx    10452 b- defN 23-May-25 07:57 laboneq/compiler/scheduler/match_schedule.py
--rw-r--r--  2.0 unx     2248 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/oscillator_schedule.py
--rw-r--r--  2.0 unx     1761 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/phase_reset_schedule.py
--rw-r--r--  2.0 unx     1808 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/preorder_map.py
--rw-r--r--  2.0 unx     3821 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/pulse_phase.py
--rw-r--r--  2.0 unx     6958 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/pulse_schedule.py
--rw-r--r--  2.0 unx      621 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/reserve_schedule.py
--rw-r--r--  2.0 unx     1367 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/root_schedule.py
--rw-r--r--  2.0 unx     1949 b- defN 23-Feb-09 09:31 laboneq/compiler/scheduler/sampling_rate_tracker.py
--rw-r--r--  2.0 unx     1115 b- defN 23-May-25 07:57 laboneq/compiler/scheduler/schedule_data.py
--rw-r--r--  2.0 unx    41127 b- defN 23-May-25 07:57 laboneq/compiler/scheduler/scheduler.py
--rw-r--r--  2.0 unx    13191 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/section_schedule.py
--rw-r--r--  2.0 unx      757 b- defN 23-May-17 00:03 laboneq/compiler/scheduler/utils.py
+-rw-r--r--  2.0 unx     3265 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/case_schedule.py
+-rw-r--r--  2.0 unx     7439 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/interval_schedule.py
+-rw-r--r--  2.0 unx     3327 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/loop_iteration_schedule.py
+-rw-r--r--  2.0 unx     8576 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/loop_schedule.py
+-rw-r--r--  2.0 unx    10468 b- defN 23-Jun-07 10:17 laboneq/compiler/scheduler/match_schedule.py
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/oscillator_schedule.py
+-rw-r--r--  2.0 unx     1761 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/phase_reset_schedule.py
+-rw-r--r--  2.0 unx     1808 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/preorder_map.py
+-rw-r--r--  2.0 unx     3821 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/pulse_phase.py
+-rw-r--r--  2.0 unx     6958 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/pulse_schedule.py
+-rw-r--r--  2.0 unx      621 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/reserve_schedule.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/root_schedule.py
+-rw-r--r--  2.0 unx     1949 b- defN 23-Jun-03 00:03 laboneq/compiler/scheduler/sampling_rate_tracker.py
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-03 00:03 laboneq/compiler/scheduler/schedule_data.py
+-rw-r--r--  2.0 unx    41072 b- defN 23-Jun-08 11:34 laboneq/compiler/scheduler/scheduler.py
+-rw-r--r--  2.0 unx    13191 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/section_schedule.py
+-rw-r--r--  2.0 unx      757 b- defN 23-Jun-01 08:47 laboneq/compiler/scheduler/utils.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/compiler/workflow/__init__.py
--rw-r--r--  2.0 unx    51030 b- defN 23-May-25 13:25 laboneq/compiler/workflow/compiler.py
+-rw-r--r--  2.0 unx    47515 b- defN 23-Jun-08 11:34 laboneq/compiler/workflow/compiler.py
 -rw-r--r--  2.0 unx    12424 b- defN 23-Feb-28 13:10 laboneq/compiler/workflow/precompensation_helpers.py
--rw-r--r--  2.0 unx    12522 b- defN 23-May-25 13:25 laboneq/compiler/workflow/recipe_generator.py
+-rw-r--r--  2.0 unx     6847 b- defN 23-Jun-08 11:34 laboneq/compiler/workflow/realtime_compiler.py
+-rw-r--r--  2.0 unx    12441 b- defN 23-Jun-08 11:34 laboneq/compiler/workflow/recipe_generator.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/__init__.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/__init__.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/inspector/__init__.py
 -rw-r--r--  2.0 unx     4511 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/inspector/update_inspect.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/plotter/__init__.py
 -rw-r--r--  2.0 unx     3379 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/plotter/plot_funs.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/pulse_simulator/__init__.py
@@ -97,154 +100,214 @@
 -rw-r--r--  2.0 unx      956 b- defN 23-May-17 00:03 laboneq/contrib/example_helpers/descriptors/hdawg_uhfqa_pqsc.py
 -rw-r--r--  2.0 unx     1887 b- defN 23-May-17 00:03 laboneq/contrib/example_helpers/descriptors/shfqc.py
 -rw-r--r--  2.0 unx     1639 b- defN 23-May-17 00:03 laboneq/contrib/example_helpers/descriptors/shfsg.py
 -rw-r--r--  2.0 unx     2472 b- defN 23-May-17 00:03 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_hdawg_pqsc.py
 -rw-r--r--  2.0 unx     2160 b- defN 23-May-17 00:03 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_pqsc.py
 -rw-r--r--  2.0 unx     2708 b- defN 23-May-17 00:03 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_shfqc_hdawg_pqsc.py
 -rw-r--r--  2.0 unx       77 b- defN 23-May-17 00:03 laboneq/contrib/example_helpers/plotting/__init__.py
--rw-r--r--  2.0 unx    11127 b- defN 23-May-23 08:56 laboneq/contrib/example_helpers/plotting/plot_helpers.py
+-rw-r--r--  2.0 unx    12182 b- defN 23-Jun-01 12:35 laboneq/contrib/example_helpers/plotting/plot_helpers.py
 -rw-r--r--  2.0 unx      308 b- defN 23-Feb-13 10:57 laboneq/controller/__init__.py
--rw-r--r--  2.0 unx     3380 b- defN 23-May-23 08:56 laboneq/controller/attribute_value_tracker.py
+-rw-r--r--  2.0 unx     3380 b- defN 23-Jun-01 08:47 laboneq/controller/attribute_value_tracker.py
 -rw-r--r--  2.0 unx     1479 b- defN 23-Feb-02 07:13 laboneq/controller/cache.py
--rw-r--r--  2.0 unx    13604 b- defN 23-May-24 09:57 laboneq/controller/communication.py
--rw-r--r--  2.0 unx    34028 b- defN 23-May-25 13:25 laboneq/controller/controller.py
--rw-r--r--  2.0 unx     4892 b- defN 23-May-25 07:57 laboneq/controller/laboneq_logging.py
+-rw-r--r--  2.0 unx    13604 b- defN 23-Jun-01 08:47 laboneq/controller/communication.py
+-rw-r--r--  2.0 unx    30852 b- defN 23-Jun-08 11:34 laboneq/controller/controller.py
+-rw-r--r--  2.0 unx     4892 b- defN 23-Jun-01 08:47 laboneq/controller/laboneq_logging.py
+-rw-r--r--  2.0 unx     4671 b- defN 23-Jun-07 10:17 laboneq/controller/near_time_runner.py
 -rw-r--r--  2.0 unx      337 b- defN 23-Feb-02 07:13 laboneq/controller/protected_session.py
--rw-r--r--  2.0 unx    15188 b- defN 23-May-25 13:25 laboneq/controller/recipe_1_4_0.py
--rw-r--r--  2.0 unx      638 b- defN 23-Feb-02 07:13 laboneq/controller/recipe_enums.py
--rw-r--r--  2.0 unx    21249 b- defN 23-May-25 13:25 laboneq/controller/recipe_processor.py
--rw-r--r--  2.0 unx     1917 b- defN 23-Feb-02 07:13 laboneq/controller/results.py
+-rw-r--r--  2.0 unx    12301 b- defN 23-Jun-08 11:34 laboneq/controller/recipe_1_4_0.py
+-rw-r--r--  2.0 unx      529 b- defN 23-Jun-07 10:17 laboneq/controller/recipe_enums.py
+-rw-r--r--  2.0 unx    21441 b- defN 23-Jun-08 11:34 laboneq/controller/recipe_processor.py
+-rw-r--r--  2.0 unx     1902 b- defN 23-Jun-07 10:17 laboneq/controller/results.py
 -rw-r--r--  2.0 unx     1594 b- defN 23-Feb-13 10:57 laboneq/controller/toolkit_adapter.py
--rw-r--r--  2.0 unx     1178 b- defN 23-May-17 00:03 laboneq/controller/util.py
+-rw-r--r--  2.0 unx     1178 b- defN 23-Jun-01 08:47 laboneq/controller/util.py
 -rw-r--r--  2.0 unx      281 b- defN 23-Mar-07 07:28 laboneq/controller/versioning.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/controller/devices/__init__.py
--rw-r--r--  2.0 unx    15391 b- defN 23-May-25 13:25 laboneq/controller/devices/device_collection.py
+-rw-r--r--  2.0 unx    15692 b- defN 23-Jun-06 11:55 laboneq/controller/devices/device_collection.py
 -rw-r--r--  2.0 unx     1275 b- defN 23-May-17 00:03 laboneq/controller/devices/device_factory.py
--rw-r--r--  2.0 unx    24523 b- defN 23-May-25 07:57 laboneq/controller/devices/device_hdawg.py
+-rw-r--r--  2.0 unx    24400 b- defN 23-Jun-06 11:55 laboneq/controller/devices/device_hdawg.py
 -rw-r--r--  2.0 unx      491 b- defN 23-May-22 14:36 laboneq/controller/devices/device_nonqc.py
--rw-r--r--  2.0 unx     8115 b- defN 23-May-17 00:03 laboneq/controller/devices/device_pqsc.py
--rw-r--r--  2.0 unx     4137 b- defN 23-May-25 13:25 laboneq/controller/devices/device_setup_dao.py
--rw-r--r--  2.0 unx     4344 b- defN 23-May-23 08:56 laboneq/controller/devices/device_shfppc.py
--rw-r--r--  2.0 unx    42895 b- defN 23-May-23 08:56 laboneq/controller/devices/device_shfqa.py
--rw-r--r--  2.0 unx    21719 b- defN 23-May-23 08:56 laboneq/controller/devices/device_shfsg.py
--rw-r--r--  2.0 unx    29618 b- defN 23-May-23 08:56 laboneq/controller/devices/device_uhfqa.py
--rw-r--r--  2.0 unx    37660 b- defN 23-May-24 09:57 laboneq/controller/devices/device_zi.py
--rw-r--r--  2.0 unx    29590 b- defN 23-May-17 00:03 laboneq/controller/devices/zi_emulator.py
+-rw-r--r--  2.0 unx     7898 b- defN 23-Jun-08 11:34 laboneq/controller/devices/device_pqsc.py
+-rw-r--r--  2.0 unx     4441 b- defN 23-Jun-01 08:47 laboneq/controller/devices/device_setup_dao.py
+-rw-r--r--  2.0 unx     2064 b- defN 23-Jun-06 11:55 laboneq/controller/devices/device_shf_base.py
+-rw-r--r--  2.0 unx     4408 b- defN 23-Jun-01 12:35 laboneq/controller/devices/device_shfppc.py
+-rw-r--r--  2.0 unx    41523 b- defN 23-Jun-07 10:17 laboneq/controller/devices/device_shfqa.py
+-rw-r--r--  2.0 unx    20499 b- defN 23-Jun-07 10:17 laboneq/controller/devices/device_shfsg.py
+-rw-r--r--  2.0 unx    29497 b- defN 23-Jun-06 11:55 laboneq/controller/devices/device_uhfqa.py
+-rw-r--r--  2.0 unx    32396 b- defN 23-Jun-07 10:17 laboneq/controller/devices/device_zi.py
+-rw-r--r--  2.0 unx    29980 b- defN 23-Jun-06 11:55 laboneq/controller/devices/zi_emulator.py
 -rw-r--r--  2.0 unx    10358 b- defN 23-May-24 09:57 laboneq/controller/devices/zi_node_monitor.py
 -rw-r--r--  2.0 unx       97 b- defN 23-Feb-02 07:13 laboneq/core/__init__.py
 -rw-r--r--  2.0 unx     2015 b- defN 23-May-17 00:03 laboneq/core/path.py
 -rw-r--r--  2.0 unx     1338 b- defN 23-Feb-02 07:13 laboneq/core/validators.py
 -rw-r--r--  2.0 unx      126 b- defN 23-Feb-02 07:13 laboneq/core/exceptions/__init__.py
 -rw-r--r--  2.0 unx      123 b- defN 23-Feb-02 07:13 laboneq/core/exceptions/laboneq_exception.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/core/serialization/__init__.py
 -rw-r--r--  2.0 unx    19090 b- defN 23-May-09 12:50 laboneq/core/serialization/simple_serialization.py
 -rw-r--r--  2.0 unx      161 b- defN 23-Feb-02 07:13 laboneq/core/types/__init__.py
--rw-r--r--  2.0 unx     5169 b- defN 23-May-17 00:03 laboneq/core/types/compiled_experiment.py
+-rw-r--r--  2.0 unx     5075 b- defN 23-Jun-07 10:17 laboneq/core/types/compiled_experiment.py
 -rw-r--r--  2.0 unx     1473 b- defN 23-Feb-02 07:13 laboneq/core/types/uid.py
 -rw-r--r--  2.0 unx      660 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/__init__.py
 -rw-r--r--  2.0 unx      934 b- defN 23-Feb-07 16:25 laboneq/core/types/enums/acquisition_type.py
 -rw-r--r--  2.0 unx      213 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/averaging_mode.py
 -rw-r--r--  2.0 unx      188 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/carrier_type.py
 -rw-r--r--  2.0 unx      227 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/dsl_version.py
 -rw-r--r--  2.0 unx      185 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/execution_type.py
--rw-r--r--  2.0 unx      223 b- defN 23-May-23 07:59 laboneq/core/types/enums/high_pass_compensation_clearing.py
+-rw-r--r--  2.0 unx      333 b- defN 23-Jun-01 08:47 laboneq/core/types/enums/high_pass_compensation_clearing.py
 -rw-r--r--  2.0 unx      157 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/io_direction.py
 -rw-r--r--  2.0 unx      268 b- defN 23-May-17 00:03 laboneq/core/types/enums/io_signal_type.py
 -rw-r--r--  2.0 unx      316 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/mixer_type.py
 -rw-r--r--  2.0 unx      200 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/modulation_type.py
 -rw-r--r--  2.0 unx      152 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/port_mode.py
 -rw-r--r--  2.0 unx      188 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/reference_clock_source.py
 -rw-r--r--  2.0 unx      198 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/repetition_mode.py
 -rw-r--r--  2.0 unx      170 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/section_alignment.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/core/utilities/__init__.py
--rw-r--r--  2.0 unx     1813 b- defN 23-May-25 07:57 laboneq/core/utilities/compressed_formatter.py
+-rw-r--r--  2.0 unx     1813 b- defN 23-Jun-01 08:47 laboneq/core/utilities/compressed_formatter.py
 -rw-r--r--  2.0 unx     8039 b- defN 23-May-17 00:03 laboneq/core/utilities/pulse_sampler.py
--rw-r--r--  2.0 unx     9808 b- defN 23-May-17 00:03 laboneq/core/utilities/replace_pulse.py
--rw-r--r--  2.0 unx      178 b- defN 23-May-03 09:34 laboneq/dsl/__init__.py
--rw-r--r--  2.0 unx     2929 b- defN 23-May-25 13:25 laboneq/dsl/laboneq_facade.py
--rw-r--r--  2.0 unx     2552 b- defN 23-Feb-15 13:56 laboneq/dsl/parameter.py
--rw-r--r--  2.0 unx    25670 b- defN 23-May-24 09:57 laboneq/dsl/session.py
+-rw-r--r--  2.0 unx     9873 b- defN 23-Jun-07 10:17 laboneq/core/utilities/replace_pulse.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/data/__init__.py
+-rw-r--r--  2.0 unx     3627 b- defN 23-Jun-01 08:47 laboneq/data/data_helper.py
+-rw-r--r--  2.0 unx     1738 b- defN 23-Jun-08 11:34 laboneq/data/calibration/__init__.py
+-rw-r--r--  2.0 unx     3199 b- defN 23-Jun-01 08:47 laboneq/data/compilation_job/__init__.py
+-rw-r--r--  2.0 unx     3887 b- defN 23-Jun-07 10:17 laboneq/data/execution_payload/__init__.py
+-rw-r--r--  2.0 unx      842 b- defN 23-Jun-01 08:47 laboneq/data/execution_payload/execution_payload_helper.py
+-rw-r--r--  2.0 unx     5188 b- defN 23-Jun-08 11:34 laboneq/data/experiment_description/__init__.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jun-01 08:47 laboneq/data/experiment_description/experiment_helper.py
+-rw-r--r--  2.0 unx      950 b- defN 23-Jun-08 11:34 laboneq/data/experiment_results/__init__.py
+-rw-r--r--  2.0 unx      761 b- defN 23-Jun-01 08:47 laboneq/data/experiment_schedule/__init__.py
+-rw-r--r--  2.0 unx     1782 b- defN 23-Jun-01 08:47 laboneq/data/scheduled_experiment/__init__.py
+-rw-r--r--  2.0 unx     3367 b- defN 23-Jun-01 08:47 laboneq/data/setup_description/__init__.py
+-rw-r--r--  2.0 unx     2845 b- defN 23-Jun-01 08:47 laboneq/data/setup_description/setup_helper.py
+-rw-r--r--  2.0 unx      178 b- defN 23-Jun-06 11:55 laboneq/dsl/__init__.py
+-rw-r--r--  2.0 unx     2947 b- defN 23-Jun-01 08:47 laboneq/dsl/laboneq_facade.py
+-rw-r--r--  2.0 unx     2552 b- defN 23-Jun-08 11:34 laboneq/dsl/parameter.py
+-rw-r--r--  2.0 unx    25670 b- defN 23-Jun-01 13:02 laboneq/dsl/session.py
 -rw-r--r--  2.0 unx     2296 b- defN 23-Feb-02 07:13 laboneq/dsl/utils.py
 -rw-r--r--  2.0 unx      529 b- defN 23-May-17 00:03 laboneq/dsl/calibration/__init__.py
--rw-r--r--  2.0 unx      946 b- defN 23-May-23 08:56 laboneq/dsl/calibration/amplifier_pump.py
+-rw-r--r--  2.0 unx      946 b- defN 23-Jun-08 11:34 laboneq/dsl/calibration/amplifier_pump.py
 -rw-r--r--  2.0 unx      545 b- defN 23-Feb-02 07:13 laboneq/dsl/calibration/calibratable.py
--rw-r--r--  2.0 unx     2313 b- defN 23-May-17 00:03 laboneq/dsl/calibration/calibration.py
+-rw-r--r--  2.0 unx     2313 b- defN 23-Jun-08 11:34 laboneq/dsl/calibration/calibration.py
 -rw-r--r--  2.0 unx      111 b- defN 23-Feb-02 07:13 laboneq/dsl/calibration/calibration_item.py
--rw-r--r--  2.0 unx      992 b- defN 23-Feb-27 16:33 laboneq/dsl/calibration/mixer_calibration.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-08 11:34 laboneq/dsl/calibration/mixer_calibration.py
 -rw-r--r--  2.0 unx     3403 b- defN 23-Feb-02 07:13 laboneq/dsl/calibration/observable.py
--rw-r--r--  2.0 unx     2134 b- defN 23-May-25 07:57 laboneq/dsl/calibration/oscillator.py
--rw-r--r--  2.0 unx     2650 b- defN 23-May-23 07:59 laboneq/dsl/calibration/precompensation.py
--rw-r--r--  2.0 unx     5614 b- defN 23-May-23 08:56 laboneq/dsl/calibration/signal_calibration.py
--rw-r--r--  2.0 unx      553 b- defN 23-Feb-02 07:13 laboneq/dsl/calibration/units.py
+-rw-r--r--  2.0 unx     2134 b- defN 23-Jun-08 11:34 laboneq/dsl/calibration/oscillator.py
+-rw-r--r--  2.0 unx     3140 b- defN 23-Jun-08 11:34 laboneq/dsl/calibration/precompensation.py
+-rw-r--r--  2.0 unx     5614 b- defN 23-Jun-08 11:34 laboneq/dsl/calibration/signal_calibration.py
+-rw-r--r--  2.0 unx      553 b- defN 23-Jun-08 11:34 laboneq/dsl/calibration/units.py
 -rw-r--r--  2.0 unx      363 b- defN 23-Feb-02 07:13 laboneq/dsl/device/__init__.py
 -rw-r--r--  2.0 unx    45826 b- defN 23-May-17 00:03 laboneq/dsl/device/_device_setup_generator.py
--rw-r--r--  2.0 unx      601 b- defN 23-Feb-02 07:13 laboneq/dsl/device/connection.py
--rw-r--r--  2.0 unx    13663 b- defN 23-May-17 00:03 laboneq/dsl/device/device_setup.py
+-rw-r--r--  2.0 unx      601 b- defN 23-Jun-08 11:34 laboneq/dsl/device/connection.py
+-rw-r--r--  2.0 unx    13663 b- defN 23-Jun-08 11:34 laboneq/dsl/device/device_setup.py
 -rw-r--r--  2.0 unx     2551 b- defN 23-Apr-06 14:15 laboneq/dsl/device/device_setup_helper.py
--rw-r--r--  2.0 unx     1362 b- defN 23-May-17 00:03 laboneq/dsl/device/instrument.py
--rw-r--r--  2.0 unx     1893 b- defN 23-Feb-02 07:13 laboneq/dsl/device/logical_signal_group.py
--rw-r--r--  2.0 unx     1729 b- defN 23-Feb-02 07:13 laboneq/dsl/device/physical_channel_group.py
--rw-r--r--  2.0 unx      538 b- defN 23-Feb-02 07:13 laboneq/dsl/device/ports.py
--rw-r--r--  2.0 unx     3422 b- defN 23-May-25 12:48 laboneq/dsl/device/quantum_operations.py
--rw-r--r--  2.0 unx     4557 b- defN 23-May-25 13:25 laboneq/dsl/device/qubits.py
--rw-r--r--  2.0 unx      215 b- defN 23-Feb-02 07:13 laboneq/dsl/device/server.py
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-08 11:34 laboneq/dsl/device/instrument.py
+-rw-r--r--  2.0 unx     1893 b- defN 23-Jun-08 11:34 laboneq/dsl/device/logical_signal_group.py
+-rw-r--r--  2.0 unx     1729 b- defN 23-Jun-08 11:34 laboneq/dsl/device/physical_channel_group.py
+-rw-r--r--  2.0 unx      538 b- defN 23-Jun-08 11:34 laboneq/dsl/device/ports.py
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-08 11:34 laboneq/dsl/device/server.py
 -rw-r--r--  2.0 unx      328 b- defN 23-May-17 00:03 laboneq/dsl/device/instruments/__init__.py
--rw-r--r--  2.0 unx     1778 b- defN 23-Feb-02 07:13 laboneq/dsl/device/instruments/hdawg.py
--rw-r--r--  2.0 unx      466 b- defN 23-Feb-13 10:57 laboneq/dsl/device/instruments/nonqc.py
--rw-r--r--  2.0 unx      948 b- defN 23-Feb-02 07:13 laboneq/dsl/device/instruments/pqsc.py
--rw-r--r--  2.0 unx      927 b- defN 23-May-17 00:03 laboneq/dsl/device/instruments/shfppc.py
--rw-r--r--  2.0 unx     2248 b- defN 23-Feb-06 17:42 laboneq/dsl/device/instruments/shfqa.py
--rw-r--r--  2.0 unx     1659 b- defN 23-Feb-06 17:42 laboneq/dsl/device/instruments/shfsg.py
--rw-r--r--  2.0 unx     2312 b- defN 23-Feb-16 12:45 laboneq/dsl/device/instruments/uhfqa.py
--rw-r--r--  2.0 unx      888 b- defN 23-Feb-13 10:57 laboneq/dsl/device/instruments/zi_standard_instrument.py
+-rw-r--r--  2.0 unx     1778 b- defN 23-Jun-08 11:34 laboneq/dsl/device/instruments/hdawg.py
+-rw-r--r--  2.0 unx      466 b- defN 23-Jun-08 11:34 laboneq/dsl/device/instruments/nonqc.py
+-rw-r--r--  2.0 unx      948 b- defN 23-Jun-08 11:34 laboneq/dsl/device/instruments/pqsc.py
+-rw-r--r--  2.0 unx      927 b- defN 23-Jun-08 11:34 laboneq/dsl/device/instruments/shfppc.py
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-08 11:34 laboneq/dsl/device/instruments/shfqa.py
+-rw-r--r--  2.0 unx     1659 b- defN 23-Jun-08 11:34 laboneq/dsl/device/instruments/shfsg.py
+-rw-r--r--  2.0 unx     2312 b- defN 23-Jun-08 11:34 laboneq/dsl/device/instruments/uhfqa.py
+-rw-r--r--  2.0 unx      888 b- defN 23-Jun-08 11:34 laboneq/dsl/device/instruments/zi_standard_instrument.py
 -rw-r--r--  2.0 unx      187 b- defN 23-Feb-02 07:13 laboneq/dsl/device/io_units/__init__.py
--rw-r--r--  2.0 unx    12750 b- defN 23-May-22 15:14 laboneq/dsl/device/io_units/logical_signal.py
--rw-r--r--  2.0 unx     3828 b- defN 23-May-23 08:56 laboneq/dsl/device/io_units/physical_channel.py
+-rw-r--r--  2.0 unx    12750 b- defN 23-Jun-08 11:34 laboneq/dsl/device/io_units/logical_signal.py
+-rw-r--r--  2.0 unx     3828 b- defN 23-Jun-08 11:34 laboneq/dsl/device/io_units/physical_channel.py
 -rw-r--r--  2.0 unx      114 b- defN 23-Feb-02 07:13 laboneq/dsl/device/servers/__init__.py
--rw-r--r--  2.0 unx      704 b- defN 23-Feb-02 07:13 laboneq/dsl/device/servers/data_server.py
+-rw-r--r--  2.0 unx      704 b- defN 23-Jun-08 11:34 laboneq/dsl/device/servers/data_server.py
 -rw-r--r--  2.0 unx      718 b- defN 23-Feb-02 07:13 laboneq/dsl/enums/__init__.py
 -rw-r--r--  2.0 unx      508 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/__init__.py
--rw-r--r--  2.0 unx      972 b- defN 23-May-22 15:14 laboneq/dsl/experiment/acquire.py
--rw-r--r--  2.0 unx      814 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/call.py
--rw-r--r--  2.0 unx      780 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/delay.py
--rw-r--r--  2.0 unx    39761 b- defN 23-May-23 08:56 laboneq/dsl/experiment/experiment.py
--rw-r--r--  2.0 unx     8216 b- defN 23-May-22 15:14 laboneq/dsl/experiment/experiment_signal.py
--rw-r--r--  2.0 unx      401 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/operation.py
--rw-r--r--  2.0 unx     1647 b- defN 23-Feb-28 13:10 laboneq/dsl/experiment/play_pulse.py
--rw-r--r--  2.0 unx     3953 b- defN 23-May-17 00:03 laboneq/dsl/experiment/pulse.py
--rw-r--r--  2.0 unx     8194 b- defN 23-May-17 00:03 laboneq/dsl/experiment/pulse_library.py
--rw-r--r--  2.0 unx      890 b- defN 23-Feb-16 12:45 laboneq/dsl/experiment/reserve.py
--rw-r--r--  2.0 unx    11431 b- defN 23-May-22 15:14 laboneq/dsl/experiment/section.py
--rw-r--r--  2.0 unx      640 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/set.py
--rw-r--r--  2.0 unx      323 b- defN 23-May-22 15:14 laboneq/dsl/experiment/utils.py
+-rw-r--r--  2.0 unx      972 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/acquire.py
+-rw-r--r--  2.0 unx      814 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/call.py
+-rw-r--r--  2.0 unx      780 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/delay.py
+-rw-r--r--  2.0 unx    40011 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/experiment.py
+-rw-r--r--  2.0 unx     8216 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/experiment_signal.py
+-rw-r--r--  2.0 unx      401 b- defN 23-Jun-08 08:19 laboneq/dsl/experiment/operation.py
+-rw-r--r--  2.0 unx     1647 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/play_pulse.py
+-rw-r--r--  2.0 unx     3953 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/pulse.py
+-rw-r--r--  2.0 unx     8194 b- defN 23-Jun-01 08:47 laboneq/dsl/experiment/pulse_library.py
+-rw-r--r--  2.0 unx      890 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/reserve.py
+-rw-r--r--  2.0 unx    11431 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/section.py
+-rw-r--r--  2.0 unx      640 b- defN 23-Jun-08 11:34 laboneq/dsl/experiment/set.py
+-rw-r--r--  2.0 unx      323 b- defN 23-May-26 09:40 laboneq/dsl/experiment/utils.py
+-rw-r--r--  2.0 unx      224 b- defN 23-Jun-01 08:47 laboneq/dsl/quantum/__init__.py
+-rw-r--r--  2.0 unx     3423 b- defN 23-Jun-08 08:19 laboneq/dsl/quantum/quantum_operations.py
+-rw-r--r--  2.0 unx    10892 b- defN 23-Jun-08 11:34 laboneq/dsl/quantum/qubits.py
 -rw-r--r--  2.0 unx      151 b- defN 23-Feb-14 15:16 laboneq/dsl/result/__init__.py
--rw-r--r--  2.0 unx     1766 b- defN 23-Feb-02 07:13 laboneq/dsl/result/acquired_result.py
--rw-r--r--  2.0 unx     7240 b- defN 23-Feb-02 07:13 laboneq/dsl/result/results.py
+-rw-r--r--  2.0 unx     1766 b- defN 23-Jun-08 11:34 laboneq/dsl/result/acquired_result.py
+-rw-r--r--  2.0 unx     7189 b- defN 23-Jun-08 11:34 laboneq/dsl/result/results.py
 -rw-r--r--  2.0 unx      113 b- defN 23-Feb-02 07:13 laboneq/dsl/serialization/__init__.py
--rw-r--r--  2.0 unx     5392 b- defN 23-May-25 12:48 laboneq/dsl/serialization/serializer.py
+-rw-r--r--  2.0 unx     5394 b- defN 23-Jun-01 08:47 laboneq/dsl/serialization/serializer.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/executor/__init__.py
 -rw-r--r--  2.0 unx     3819 b- defN 23-Feb-16 12:45 laboneq/executor/execution_from_experiment.py
--rw-r--r--  2.0 unx     8152 b- defN 23-Apr-06 14:15 laboneq/executor/executor.py
+-rw-r--r--  2.0 unx     8152 b- defN 23-Jun-08 11:34 laboneq/executor/executor.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/implementation/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/implementation/compilation_service/__init__.py
+-rw-r--r--  2.0 unx     1156 b- defN 23-Jun-01 08:47 laboneq/implementation/compilation_service/compilation_service.py
+-rw-r--r--  2.0 unx     7894 b- defN 23-Jun-01 08:47 laboneq/implementation/compilation_service/compilation_service_legacy.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/implementation/data_storage/__init__.py
+-rw-r--r--  2.0 unx      916 b- defN 23-Jun-01 13:41 laboneq/implementation/data_storage/l1q_database_wrapper.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/implementation/data_storage_service/__init__.py
+-rw-r--r--  2.0 unx     6103 b- defN 23-Jun-01 08:47 laboneq/implementation/data_storage_service/data_storage_service_sqlite_dict.py
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-01 08:47 laboneq/implementation/experiment_workflow/__init__.py
+-rw-r--r--  2.0 unx    16908 b- defN 23-Jun-01 08:47 laboneq/implementation/experiment_workflow/device_setup_generator.py
+-rw-r--r--  2.0 unx     6106 b- defN 23-Jun-01 08:47 laboneq/implementation/experiment_workflow/experiment_workflow.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/implementation/legacy_adapters/__init__.py
+-rw-r--r--  2.0 unx     3084 b- defN 23-Jun-01 08:47 laboneq/implementation/legacy_adapters/dynamic_converter.py
+-rw-r--r--  2.0 unx      950 b- defN 23-Jun-01 08:47 laboneq/implementation/legacy_adapters/simple2.py
+-rw-r--r--  2.0 unx     7740 b- defN 23-Jun-08 11:34 laboneq/implementation/legacy_adapters/converters_calibration/__init__.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-01 08:47 laboneq/implementation/legacy_adapters/converters_calibration/post_process_calibration.py
+-rw-r--r--  2.0 unx    22847 b- defN 23-Jun-08 11:34 laboneq/implementation/legacy_adapters/converters_experiment_description/__init__.py
+-rw-r--r--  2.0 unx     1659 b- defN 23-Jun-01 08:47 laboneq/implementation/legacy_adapters/converters_experiment_description/post_process_experiment_description.py
+-rw-r--r--  2.0 unx     1741 b- defN 23-Jun-08 11:34 laboneq/implementation/legacy_adapters/converters_experiment_results/__init__.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-01 08:47 laboneq/implementation/legacy_adapters/converters_experiment_results/post_process_experiment_results.py
+-rw-r--r--  2.0 unx     4376 b- defN 23-Jun-08 11:34 laboneq/implementation/legacy_adapters/converters_scheduled_experiment/__init__.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-01 08:47 laboneq/implementation/legacy_adapters/converters_scheduled_experiment/post_process_scheduled_experiment.py
+-rw-r--r--  2.0 unx    13804 b- defN 23-Jun-08 11:34 laboneq/implementation/legacy_adapters/converters_setup_description/__init__.py
+-rw-r--r--  2.0 unx     5165 b- defN 23-Jun-01 08:47 laboneq/implementation/legacy_adapters/converters_setup_description/post_process_setup_description.py
+-rw-r--r--  2.0 unx     9204 b- defN 23-Jun-01 08:47 laboneq/implementation/legacy_adapters/legacy_dsl_adapters/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/implementation/payload_builder/__init__.py
+-rw-r--r--  2.0 unx    25577 b- defN 23-Jun-07 10:17 laboneq/implementation/payload_builder/payload_builder.py
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-01 08:47 laboneq/implementation/runner/__init__.py
+-rw-r--r--  2.0 unx     2293 b- defN 23-Jun-01 08:47 laboneq/implementation/runner/runner.py
+-rw-r--r--  2.0 unx    14574 b- defN 23-Jun-07 10:17 laboneq/implementation/runner/runner_legacy.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/interfaces/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/interfaces/application_management/__init__.py
+-rw-r--r--  2.0 unx      384 b- defN 23-Jun-01 08:47 laboneq/interfaces/application_management/laboneq_settings.py
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-01 08:47 laboneq/interfaces/compilation_service/__init__.py
+-rw-r--r--  2.0 unx      779 b- defN 23-Jun-01 08:47 laboneq/interfaces/compilation_service/compilation_service_api.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/interfaces/data_storage/__init__.py
+-rw-r--r--  2.0 unx     2272 b- defN 23-Jun-01 08:47 laboneq/interfaces/data_storage/data_storage_api.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-01 08:47 laboneq/interfaces/experiment/__init__.py
+-rw-r--r--  2.0 unx     2004 b- defN 23-Jun-01 08:47 laboneq/interfaces/experiment/experiment_api.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/interfaces/payload_builder/__init__.py
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-01 08:47 laboneq/interfaces/payload_builder/payload_builder_api.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-07 10:17 laboneq/interfaces/runner/__init__.py
+-rw-r--r--  2.0 unx      766 b- defN 23-Jun-01 08:47 laboneq/interfaces/runner/runner_api.py
+-rw-r--r--  2.0 unx      793 b- defN 23-Jun-01 08:47 laboneq/interfaces/runner/runner_control_api.py
 -rw-r--r--  2.0 unx      145 b- defN 23-Feb-14 15:16 laboneq/openqasm3/__init__.py
--rw-r--r--  2.0 unx     8903 b- defN 23-May-23 08:56 laboneq/openqasm3/expression.py
--rw-r--r--  2.0 unx     1671 b- defN 23-May-22 15:14 laboneq/openqasm3/gate_store.py
--rw-r--r--  2.0 unx     2593 b- defN 23-May-23 08:56 laboneq/openqasm3/namespace.py
--rw-r--r--  2.0 unx    15459 b- defN 23-May-23 14:08 laboneq/openqasm3/openqasm3_importer.py
+-rw-r--r--  2.0 unx     8903 b- defN 23-Jun-01 08:47 laboneq/openqasm3/expression.py
+-rw-r--r--  2.0 unx     1671 b- defN 23-Jun-05 13:15 laboneq/openqasm3/gate_store.py
+-rw-r--r--  2.0 unx     2593 b- defN 23-Jun-01 08:47 laboneq/openqasm3/namespace.py
+-rw-r--r--  2.0 unx    15459 b- defN 23-Jun-05 13:15 laboneq/openqasm3/openqasm3_importer.py
 -rw-r--r--  2.0 unx     1732 b- defN 23-May-17 00:03 laboneq/openqasm3/openqasm_error.py
--rw-r--r--  2.0 unx     4850 b- defN 23-May-22 15:14 laboneq/openqasm3/reset_gate_factory.py
--rw-r--r--  2.0 unx     1517 b- defN 23-May-23 08:56 laboneq/openqasm3/signal_store.py
+-rw-r--r--  2.0 unx     4850 b- defN 23-Jun-01 08:47 laboneq/openqasm3/reset_gate_factory.py
+-rw-r--r--  2.0 unx     1517 b- defN 23-Jun-01 08:47 laboneq/openqasm3/signal_store.py
 -rw-r--r--  2.0 unx      127 b- defN 23-Feb-02 07:13 laboneq/pulse_sheet_viewer/__init__.py
 -rw-r--r--  2.0 unx     2059 b- defN 23-Feb-16 12:45 laboneq/pulse_sheet_viewer/event_graph_viewer.py
 -rw-r--r--  2.0 unx     2692 b- defN 23-Feb-02 14:48 laboneq/pulse_sheet_viewer/interactive_psv.py
 -rw-r--r--  2.0 unx     3288 b- defN 23-Feb-02 14:48 laboneq/pulse_sheet_viewer/pulse_sheet_viewer.py
 -rw-rw-rw-  2.0 unx  1443040 b- defN 23-May-17 00:03 laboneq/pulse_sheet_viewer/pulse_sheet_viewer_template.html
 -rw-r--r--  2.0 unx      152 b- defN 23-Feb-14 15:16 laboneq/simulator/__init__.py
--rw-r--r--  2.0 unx     5904 b- defN 23-Feb-02 14:48 laboneq/simulator/output_simulator.py
--rw-r--r--  2.0 unx    40863 b- defN 23-May-25 13:25 laboneq/simulator/seqc_parser.py
--rw-r--r--  2.0 unx    12500 b- defN 23-May-24 14:34 laboneq/simulator/wave_scroller.py
--rw-rw-rw-  2.0 unx       22 b- defN 23-May-25 13:27 laboneq-2.7.0.dist-info/AUTHORS
--rw-rw-rw-  2.0 unx    11358 b- defN 23-May-25 13:27 laboneq-2.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3188 b- defN 23-May-25 13:27 laboneq-2.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 13:27 laboneq-2.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-25 13:27 laboneq-2.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    24183 b- defN 23-May-25 13:27 laboneq-2.7.0.dist-info/RECORD
-248 files, 2880660 bytes uncompressed, 900375 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx     6090 b- defN 23-Jun-08 11:34 laboneq/simulator/output_simulator.py
+-rw-r--r--  2.0 unx    41644 b- defN 23-Jun-08 11:34 laboneq/simulator/seqc_parser.py
+-rw-r--r--  2.0 unx    17091 b- defN 23-Jun-06 11:55 laboneq/simulator/wave_scroller.py
+-rw-rw-rw-  2.0 unx       22 b- defN 23-Jun-08 11:43 laboneq-2.8.0.dist-info/AUTHORS
+-rw-rw-rw-  2.0 unx    11358 b- defN 23-Jun-08 11:43 laboneq-2.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3255 b- defN 23-Jun-08 11:43 laboneq-2.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 11:43 laboneq-2.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-08 11:43 laboneq-2.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    31232 b- defN 23-Jun-08 11:43 laboneq-2.8.0.dist-info/RECORD
+311 files, 3091552 bytes uncompressed, 953027 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -24,14 +24,20 @@
 
 Filename: laboneq/_observability/tracing/_noop_tracer.py
 Comment: 
 
 Filename: laboneq/_observability/tracing/_tracer.py
 Comment: 
 
+Filename: laboneq/application_management/__init__.py
+Comment: 
+
+Filename: laboneq/application_management/application_manager.py
+Comment: 
+
 Filename: laboneq/compiler/__init__.py
 Comment: 
 
 Filename: laboneq/compiler/fastlogging.py
 Comment: 
 
 Filename: laboneq/compiler/qccs-schema_2_5_0.json
@@ -225,14 +231,17 @@
 
 Filename: laboneq/compiler/workflow/compiler.py
 Comment: 
 
 Filename: laboneq/compiler/workflow/precompensation_helpers.py
 Comment: 
 
+Filename: laboneq/compiler/workflow/realtime_compiler.py
+Comment: 
+
 Filename: laboneq/compiler/workflow/recipe_generator.py
 Comment: 
 
 Filename: laboneq/contrib/__init__.py
 Comment: 
 
 Filename: laboneq/contrib/bloch_simulator_pulse_plotter/__init__.py
@@ -321,14 +330,17 @@
 
 Filename: laboneq/controller/controller.py
 Comment: 
 
 Filename: laboneq/controller/laboneq_logging.py
 Comment: 
 
+Filename: laboneq/controller/near_time_runner.py
+Comment: 
+
 Filename: laboneq/controller/protected_session.py
 Comment: 
 
 Filename: laboneq/controller/recipe_1_4_0.py
 Comment: 
 
 Filename: laboneq/controller/recipe_enums.py
@@ -366,14 +378,17 @@
 
 Filename: laboneq/controller/devices/device_pqsc.py
 Comment: 
 
 Filename: laboneq/controller/devices/device_setup_dao.py
 Comment: 
 
+Filename: laboneq/controller/devices/device_shf_base.py
+Comment: 
+
 Filename: laboneq/controller/devices/device_shfppc.py
 Comment: 
 
 Filename: laboneq/controller/devices/device_shfqa.py
 Comment: 
 
 Filename: laboneq/controller/devices/device_shfsg.py
@@ -474,14 +489,53 @@
 
 Filename: laboneq/core/utilities/pulse_sampler.py
 Comment: 
 
 Filename: laboneq/core/utilities/replace_pulse.py
 Comment: 
 
+Filename: laboneq/data/__init__.py
+Comment: 
+
+Filename: laboneq/data/data_helper.py
+Comment: 
+
+Filename: laboneq/data/calibration/__init__.py
+Comment: 
+
+Filename: laboneq/data/compilation_job/__init__.py
+Comment: 
+
+Filename: laboneq/data/execution_payload/__init__.py
+Comment: 
+
+Filename: laboneq/data/execution_payload/execution_payload_helper.py
+Comment: 
+
+Filename: laboneq/data/experiment_description/__init__.py
+Comment: 
+
+Filename: laboneq/data/experiment_description/experiment_helper.py
+Comment: 
+
+Filename: laboneq/data/experiment_results/__init__.py
+Comment: 
+
+Filename: laboneq/data/experiment_schedule/__init__.py
+Comment: 
+
+Filename: laboneq/data/scheduled_experiment/__init__.py
+Comment: 
+
+Filename: laboneq/data/setup_description/__init__.py
+Comment: 
+
+Filename: laboneq/data/setup_description/setup_helper.py
+Comment: 
+
 Filename: laboneq/dsl/__init__.py
 Comment: 
 
 Filename: laboneq/dsl/laboneq_facade.py
 Comment: 
 
 Filename: laboneq/dsl/parameter.py
@@ -549,20 +603,14 @@
 
 Filename: laboneq/dsl/device/physical_channel_group.py
 Comment: 
 
 Filename: laboneq/dsl/device/ports.py
 Comment: 
 
-Filename: laboneq/dsl/device/quantum_operations.py
-Comment: 
-
-Filename: laboneq/dsl/device/qubits.py
-Comment: 
-
 Filename: laboneq/dsl/device/server.py
 Comment: 
 
 Filename: laboneq/dsl/device/instruments/__init__.py
 Comment: 
 
 Filename: laboneq/dsl/device/instruments/hdawg.py
@@ -645,14 +693,23 @@
 
 Filename: laboneq/dsl/experiment/set.py
 Comment: 
 
 Filename: laboneq/dsl/experiment/utils.py
 Comment: 
 
+Filename: laboneq/dsl/quantum/__init__.py
+Comment: 
+
+Filename: laboneq/dsl/quantum/quantum_operations.py
+Comment: 
+
+Filename: laboneq/dsl/quantum/qubits.py
+Comment: 
+
 Filename: laboneq/dsl/result/__init__.py
 Comment: 
 
 Filename: laboneq/dsl/result/acquired_result.py
 Comment: 
 
 Filename: laboneq/dsl/result/results.py
@@ -669,14 +726,146 @@
 
 Filename: laboneq/executor/execution_from_experiment.py
 Comment: 
 
 Filename: laboneq/executor/executor.py
 Comment: 
 
+Filename: laboneq/implementation/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/compilation_service/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/compilation_service/compilation_service.py
+Comment: 
+
+Filename: laboneq/implementation/compilation_service/compilation_service_legacy.py
+Comment: 
+
+Filename: laboneq/implementation/data_storage/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/data_storage/l1q_database_wrapper.py
+Comment: 
+
+Filename: laboneq/implementation/data_storage_service/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/data_storage_service/data_storage_service_sqlite_dict.py
+Comment: 
+
+Filename: laboneq/implementation/experiment_workflow/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/experiment_workflow/device_setup_generator.py
+Comment: 
+
+Filename: laboneq/implementation/experiment_workflow/experiment_workflow.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/dynamic_converter.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/simple2.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_calibration/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_calibration/post_process_calibration.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_experiment_description/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_experiment_description/post_process_experiment_description.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_experiment_results/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_experiment_results/post_process_experiment_results.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_scheduled_experiment/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_scheduled_experiment/post_process_scheduled_experiment.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_setup_description/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/converters_setup_description/post_process_setup_description.py
+Comment: 
+
+Filename: laboneq/implementation/legacy_adapters/legacy_dsl_adapters/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/payload_builder/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/payload_builder/payload_builder.py
+Comment: 
+
+Filename: laboneq/implementation/runner/__init__.py
+Comment: 
+
+Filename: laboneq/implementation/runner/runner.py
+Comment: 
+
+Filename: laboneq/implementation/runner/runner_legacy.py
+Comment: 
+
+Filename: laboneq/interfaces/__init__.py
+Comment: 
+
+Filename: laboneq/interfaces/application_management/__init__.py
+Comment: 
+
+Filename: laboneq/interfaces/application_management/laboneq_settings.py
+Comment: 
+
+Filename: laboneq/interfaces/compilation_service/__init__.py
+Comment: 
+
+Filename: laboneq/interfaces/compilation_service/compilation_service_api.py
+Comment: 
+
+Filename: laboneq/interfaces/data_storage/__init__.py
+Comment: 
+
+Filename: laboneq/interfaces/data_storage/data_storage_api.py
+Comment: 
+
+Filename: laboneq/interfaces/experiment/__init__.py
+Comment: 
+
+Filename: laboneq/interfaces/experiment/experiment_api.py
+Comment: 
+
+Filename: laboneq/interfaces/payload_builder/__init__.py
+Comment: 
+
+Filename: laboneq/interfaces/payload_builder/payload_builder_api.py
+Comment: 
+
+Filename: laboneq/interfaces/runner/__init__.py
+Comment: 
+
+Filename: laboneq/interfaces/runner/runner_api.py
+Comment: 
+
+Filename: laboneq/interfaces/runner/runner_control_api.py
+Comment: 
+
 Filename: laboneq/openqasm3/__init__.py
 Comment: 
 
 Filename: laboneq/openqasm3/expression.py
 Comment: 
 
 Filename: laboneq/openqasm3/gate_store.py
@@ -720,26 +909,26 @@
 
 Filename: laboneq/simulator/seqc_parser.py
 Comment: 
 
 Filename: laboneq/simulator/wave_scroller.py
 Comment: 
 
-Filename: laboneq-2.7.0.dist-info/AUTHORS
+Filename: laboneq-2.8.0.dist-info/AUTHORS
 Comment: 
 
-Filename: laboneq-2.7.0.dist-info/LICENSE
+Filename: laboneq-2.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: laboneq-2.7.0.dist-info/METADATA
+Filename: laboneq-2.8.0.dist-info/METADATA
 Comment: 
 
-Filename: laboneq-2.7.0.dist-info/WHEEL
+Filename: laboneq-2.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: laboneq-2.7.0.dist-info/top_level.txt
+Filename: laboneq-2.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: laboneq-2.7.0.dist-info/RECORD
+Filename: laboneq-2.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## laboneq/VERSION.txt

```diff
@@ -1 +1 @@
-2.7.0
+2.8.0
```

## laboneq/simple.py

```diff
@@ -21,16 +21,14 @@
     Oscillator,
     Precompensation,
     SignalCalibration,
     units,
 )
 from laboneq.dsl.device import DeviceSetup
 from laboneq.dsl.device.device_setup_helper import DeviceSetupHelper
-from laboneq.dsl.device.quantum_operations import QuantumOperation
-from laboneq.dsl.device.qubits import QuantumElement, Qubit
 from laboneq.dsl.enums import (
     AcquisitionType,
     AveragingMode,
     CarrierType,
     ExecutionType,
     HighPassCompensationClearing,
     ModulationType,
@@ -45,12 +43,14 @@
     Experiment,
     ExperimentSignal,
     Match,
     Section,
     Sweep,
     pulse_library,
 )
+from laboneq.dsl.quantum import QuantumOperation, Qubit, QubitParameters
 from laboneq.dsl.result import Results
 from laboneq.dsl.session import Session
 from laboneq.dsl.utils import has_onboard_lo
+from laboneq.implementation.data_storage.l1q_database_wrapper import L1QDatabase
 from laboneq.pulse_sheet_viewer.pulse_sheet_viewer import show_pulse_sheet
 from laboneq.simulator.output_simulator import OutputSimulator
```

## laboneq/compiler/code_generator/analyze_events.py

```diff
@@ -289,17 +289,17 @@
 
 
 def analyze_set_oscillator_times(
     events: List,
     signal_obj: SignalObj,
 ) -> AWGSampledEventSequence:
     signal_id = signal_obj.id
-    device_id = signal_obj.device_id
-    device_type = signal_obj.device_type
-    sampling_rate = signal_obj.sampling_rate
+    device_id = signal_obj.awg.device_id
+    device_type = signal_obj.awg.device_type
+    sampling_rate = signal_obj.awg.sampling_rate
     delay = signal_obj.total_delay
     set_oscillator_events = [
         event
         for event in events
         if event["event_type"] == "SET_OSCILLATOR_FREQUENCY_START"
         and event.get("device_id") == device_id
         and event.get("signal") == signal_id
@@ -352,17 +352,17 @@
 def analyze_acquire_times(
     events: List[Any],
     signal_obj: SignalObj,
     feedback_register_allocator: FeedbackRegisterAllocator,
 ) -> AWGSampledEventSequence:
 
     signal_id = signal_obj.id
-    sampling_rate = signal_obj.sampling_rate
+    sampling_rate = signal_obj.awg.sampling_rate
     delay = signal_obj.total_delay
-    sample_multiple = signal_obj.device_type.sample_multiple
+    sample_multiple = signal_obj.awg.device_type.sample_multiple
     channels = signal_obj.channels
 
     _logger.debug(
         "Calculating acquire times for signal %s with delay %s ( %s samples)",
         signal_id,
         str(delay),
         str(round(delay * sampling_rate)),
@@ -461,15 +461,15 @@
     digital_signal_change_events = [
         event
         for event in events
         if event["event_type"] == EventType.DIGITAL_SIGNAL_STATE_CHANGE
         and signal.id == event["signal"]
     ]
     delay = signal.total_delay
-    sampling_rate = signal.sampling_rate
+    sampling_rate = signal.awg.sampling_rate
     device_type = signal.awg.device_type
 
     sampled_digital_signal_change_events = AWGSampledEventSequence()
 
     for event in digital_signal_change_events:
         time_in_samples = length_to_samples(event["time"] + delay, sampling_rate)
         sampled_digital_signal_change_events.add(
```

## laboneq/compiler/code_generator/analyze_playback.py

```diff
@@ -454,15 +454,15 @@
     )
     return signature, pulse_parameters
 
 
 def _interval_start_after_oscillator_reset(
     events, signals, compacted_intervals: IntervalTree, delay, sampling_rate
 ):
-    device_id = next(iter(signals.values())).device_id
+    device_id = next(iter(signals.values())).awg.device_id
 
     osc_reset_event_time = [
         length_to_samples(event["time"] + delay, sampling_rate)
         for event in events
         if event["event_type"] == "RESET_HW_OSCILLATOR_PHASE"
         and event["device_id"] == device_id
     ]
```

## laboneq/compiler/code_generator/code_generator.py

```diff
@@ -3,19 +3,18 @@
 
 from __future__ import annotations
 
 import bisect
 import copy
 import logging
 import math
-import os
-import re
+from collections import namedtuple
 from contextlib import suppress
 from itertools import groupby
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, NamedTuple, Tuple
 
 import numpy as np
 from engineering_notation import EngNumber
 
 from laboneq.compiler.code_generator.analyze_events import (
     analyze_acquire_times,
     analyze_init_times,
@@ -68,17 +67,15 @@
     round_min_playwave_hint,
 )
 from laboneq.compiler.common.device_type import DeviceType
 from laboneq.compiler.common.event_type import EventList, EventType
 from laboneq.compiler.common.pulse_parameters import decode_pulse_parameters
 from laboneq.compiler.common.signal_obj import SignalObj
 from laboneq.compiler.common.trigger_mode import TriggerMode
-from laboneq.compiler.experiment_access import ExperimentDAO
 from laboneq.compiler.experiment_access.pulse_def import PulseDef
-from laboneq.compiler.experiment_access.section_info import SectionInfo
 from laboneq.core.exceptions import LabOneQException
 from laboneq.core.types.compiled_experiment import (
     PulseInstance,
     PulseMapEntry,
     PulseWaveformMap,
 )
 from laboneq.core.utilities.pulse_sampler import (
@@ -194,15 +191,15 @@
                         continue
 
                     samples = pulse_def.samples
                     amplitude = pulse_def.effective_amplitude
 
                     length = pulse_def.length
                     if length is None:
-                        length = len(samples) / signal_obj.sampling_rate
+                        length = len(samples) / signal_obj.awg.sampling_rate
 
                     _logger.debug(
                         "Sampling integration weights for %s with modulation_frequency %s",
                         signal_obj.id,
                         str(signal_obj.oscillator_frequency),
                     )
 
@@ -210,15 +207,15 @@
                         event.params.get("pulse_pulse_parameters"),
                         None,
                         event.params.get("play_pulse_parameters"),
                     )
                     pulse_parameters = decode_pulse_parameters(pulse_parameters)
                     integration_weight = sample_pulse(
                         signal_type="iq",
-                        sampling_rate=signal_obj.sampling_rate,
+                        sampling_rate=signal_obj.awg.sampling_rate,
                         length=length,
                         amplitude=amplitude,
                         pulse_function=pulse_def.function,
                         modulation_frequency=signal_obj.oscillator_frequency,
                         samples=samples,
                         mixer_type=signal_obj.mixer_type,
                         pulse_parameters=pulse_parameters,
@@ -228,15 +225,15 @@
                         integration_weight,
                         pulse_def.id,
                         signal_obj.mixer_type,
                         signal_obj.id,
                     )
 
                     integration_weight["basename"] = (
-                        signal_obj.device_id
+                        signal_obj.awg.device_id
                         + "_"
                         + str(signal_obj.awg.awg_number)
                         + "_"
                         + str(min(signal_obj.channels))
                         + "_"
                         + play_wave_id
                     )
@@ -298,15 +295,14 @@
     def total_execution_time(self):
         return self._total_execution_time
 
     def _add_signal_to_awg(self, signal_obj: SignalObj):
         awg_key = signal_obj.awg.key
         if awg_key not in self._awgs:
             self._awgs[awg_key] = copy.deepcopy(signal_obj.awg)
-            self._awgs[awg_key].device_type = signal_obj.device_type
         self._awgs[awg_key].signals.append(signal_obj)
 
     def add_signal(self, signal: SignalObj):
         signal_obj = copy.deepcopy(signal)
         signal_obj.pulses = []
         _logger.debug(signal_obj)
         self._signals[signal.id] = signal_obj
@@ -339,15 +335,15 @@
         for awg in self._awgs.values():
             # Handle integration weights separately
             for signal_obj in awg.signals:
                 if signal_obj.id in self._integration_weights:
                     signal_weights = self._integration_weights[signal_obj.id]
                     for weight in signal_weights.values():
                         basename = weight["basename"]
-                        if signal_obj.device_type.supports_complex_waves:
+                        if signal_obj.awg.device_type.supports_complex_waves:
                             self._save_wave_bin(
                                 CodeGenerator.SHFQA_COMPLEX_SAMPLE_SCALING
                                 * (weight["samples_i"] - 1j * weight["samples_q"]),
                                 None,
                                 basename,
                                 "",
                             )
@@ -384,15 +380,15 @@
                         for (
                             signature_key,
                             sampled_signature,
                         ) in self._sampled_signatures[signal_obj.id].items():
                             if not sampled_signature:
                                 continue
                             sig_string = signature_key.signature_string()
-                            if signal_obj.device_type.supports_binary_waves:
+                            if signal_obj.awg.device_type.supports_binary_waves:
                                 if awg.signal_type == AWGSignalType.SINGLE:
                                     self._save_wave_bin(
                                         sampled_signature["samples_i"],
                                         sampled_signature["signature_pulse_map"],
                                         sig_string,
                                         "",
                                     )
@@ -421,36 +417,36 @@
                                         self._save_wave_bin(
                                             sampled_signature["samples_marker2"],
                                             sampled_signature["signature_pulse_map"],
                                             sig_string,
                                             "_marker2",
                                         )
 
-                            elif signal_obj.device_type.supports_complex_waves:
+                            elif signal_obj.awg.device_type.supports_complex_waves:
                                 self._save_wave_bin(
                                     CodeGenerator.SHFQA_COMPLEX_SAMPLE_SCALING
                                     * (
                                         sampled_signature["samples_i"]
                                         - 1j * sampled_signature["samples_q"]
                                     ),
                                     sampled_signature["signature_pulse_map"],
                                     sig_string,
                                     "",
                                 )
                             else:
                                 raise RuntimeError(
-                                    f"Device type {signal_obj.device_type} has invalid supported waves config."
+                                    f"Device type {signal_obj.awg.device_type} has invalid supported waves config."
                                 )
             else:
                 signal_obj = awg.signals[0]
                 for signature_key, sampled_signature in self._sampled_signatures[
                     virtual_signal_id
                 ].items():
                     sig_string = signature_key.signature_string()
-                    if signal_obj.device_type.supports_binary_waves:
+                    if signal_obj.awg.device_type.supports_binary_waves:
                         self._save_wave_bin(
                             sampled_signature["samples_i"],
                             sampled_signature["signature_pulse_map"],
                             sig_string,
                             "_i",
                         )
                         if "samples_q" in sampled_signature:
@@ -473,15 +469,15 @@
                                 sampled_signature["signature_pulse_map"],
                                 sig_string,
                                 "_marker2",
                             )
 
                     else:
                         raise RuntimeError(
-                            f"Device type {signal_obj.device_type} has invalid supported waves config."
+                            f"Device type {signal_obj.awg.device_type} has invalid supported waves config."
                         )
 
         # check that there are no duplicate filenames in the wave pool (QCSW-1079)
         waves = sorted(
             [(wave["filename"], wave["samples"]) for wave in self._waves],
             key=lambda w: w[0],
         )
@@ -490,82 +486,33 @@
             assert all(np.all(group[0][1] == g[1]) for g in group[1:])
 
         if _logger.getEffectiveLevel() == logging.DEBUG:
             _logger.debug("Sampled signatures: %s", self._sampled_signatures)
 
             _logger.debug(self._waves)
 
-    def gen_acquire_map(self, events: EventList, sections: ExperimentDAO):
-        # todo (PW): this can EASILY be factored out into a separate file
-        loop_events = [
-            e
-            for e in events
-            if e["event_type"] == "LOOP_ITERATION_END" and not e.get("shadow")
-        ]
-        averaging_loop_info: SectionInfo = None
-        innermost_loop: Dict[str, Any] = None
-        outermost_loop: Dict[str, Any] = None
-        for e in loop_events:
-            section_info = sections.section_info(e["section_name"])
-            if section_info.averaging_type == "hardware":
-                averaging_loop_info = section_info
-            if (
-                innermost_loop is None
-                or e["nesting_level"] > innermost_loop["nesting_level"]
-            ):
-                innermost_loop = e
-            if (
-                outermost_loop is None
-                or e["nesting_level"] < outermost_loop["nesting_level"]
-            ):
-                outermost_loop = e
-        averaging_loop = (
-            None
-            if averaging_loop_info is None
-            else innermost_loop
-            if averaging_loop_info.averaging_mode == "sequential"
-            else outermost_loop
-        )
-        if (
-            averaging_loop is not None
-            and averaging_loop["section_name"] != averaging_loop_info.section_id
-        ):
-            raise RuntimeError(
-                f"Internal error: couldn't unambiguously determine the hardware averaging loop - "
-                f"innermost '{innermost_loop['section_name']}', outermost '{outermost_loop['section_name']}', "
-                f"hw avg '{averaging_loop_info.section_id}' with mode '{averaging_loop_info.averaging_mode}' "
-                f"expected to match '{averaging_loop['section_name']}'"
-            )
-        unrolled_avg_matcher = re.compile(
-            "(?!)"  # Never match anything
-            if averaging_loop is None
-            else f"{averaging_loop['section_name']}_[0-9]+"
-        )
+    def gen_acquire_map(self, events: EventList):
         # timestamp -> map[signal -> handle]
         self._simultaneous_acquires: Dict[float, Dict[str, str]] = {}
         for e in (e for e in events if e["event_type"] == "ACQUIRE_START"):
-            if e.get("shadow") and unrolled_avg_matcher.match(e.get("loop_iteration")):
-                continue  # Skip events for unrolled averaging loop
             time_events = self._simultaneous_acquires.setdefault(e["time"], {})
             time_events[e["signal"]] = e["acquire_handle"]
 
     def gen_seq_c(self, events: List[Any], pulse_defs: Dict[str, PulseDef]):
-        signal_keys = [
-            "sampling_rate",
-            "id",
-            "device_id",
-            "device_type",
-            "delay_signal",
-        ]
         signal_info_map = {
-            id: {k: getattr(s, k) for k in signal_keys}
-            for id, s in self._signals.items()
+            signal_id: {"id": s.id, "delay_signal": s.delay_signal}
+            for signal_id, s in self._signals.items()
         }
+
         for k, s in signal_info_map.items():
-            s["awg_number"] = self._signals[k].awg.awg_number
+            signal_obj = self._signals[k]
+            s["sampling_rate"] = signal_obj.awg.sampling_rate
+            s["awg_number"] = signal_obj.awg.awg_number
+            s["device_id"] = signal_obj.awg.device_id
+            s["device_type"] = signal_obj.awg.device_type
 
         (
             self._integration_times,
             self._signal_delays,
         ) = self._measurement_calculator.calculate_integration_times(
             signal_info_map, events
         )
@@ -642,20 +589,20 @@
                 # for this to work, we need to ignore the play delay when generating code for loop events
                 # and we use the start delay (lead time) to calculate the global delay
                 relevant_delay = signal_obj.start_delay
             else:
                 relevant_delay = signal_obj.total_delay
 
             if (
-                round(relevant_delay * signal_obj.sampling_rate)
-                % signal_obj.device_type.sample_multiple
+                round(relevant_delay * signal_obj.awg.sampling_rate)
+                % signal_obj.awg.device_type.sample_multiple
                 != 0
             ):
                 raise RuntimeError(
-                    f"Delay {relevant_delay} s = {round(relevant_delay*signal_obj.sampling_rate)} samples on signal {signal_obj.id} is not compatible with the sample multiple of {signal_obj.device_type.sample_multiple} on {signal_obj.device_type}"
+                    f"Delay {relevant_delay} s = {round(relevant_delay*signal_obj.awg.sampling_rate)} samples on signal {signal_obj.id} is not compatible with the sample multiple of {signal_obj.awg.device_type.sample_multiple} on {signal_obj.awg.device_type}"
                 )
             all_relevant_delays[signal_obj.id] = relevant_delay
 
             if signal_obj.signal_type != "integration":
 
                 if awg.signal_type != AWGSignalType.IQ and global_delay is not None:
                     if global_delay != relevant_delay:
@@ -669,15 +616,15 @@
                     if relevant_delay < global_delay:
                         # use minimum delay as global delay
                         # this makes sure that loop start events happen first and are not shifted beyond loop body events
                         global_delay = relevant_delay
                 else:
                     global_delay = relevant_delay
 
-            global_sampling_rate = signal_obj.sampling_rate
+            global_sampling_rate = signal_obj.awg.sampling_rate
             signals_so_far.add(signal_obj.id)
 
         if global_delay is None:
             global_delay = 0
 
         if (
             global_delay > 0
@@ -733,14 +680,27 @@
                         params=new_params,
                     )
                 )
 
                 time += new_length
         return new_awg_events, pulse_name_mapping
 
+    def _pulses_compatible_for_compression(self, pulses: List[NamedTuple]):
+        sorted_pulses = sorted(pulses, key=lambda x: x.start)
+        n = len(sorted_pulses)
+
+        for i in range(n - 1):
+            pi = sorted_pulses[i]
+            pj = sorted_pulses[i + 1]
+
+            if pi.end > pj.start and pi.can_compress != pj.can_compress:
+                return False
+
+        return True
+
     def _compress_waves(
         self, sampled_events, sampled_signatures, signal_id, min_play_wave, pulse_defs
     ):
         compressed_waveform_signatures = set()
         for event_group in sampled_events.sequence.values():
             event_replacement = {}
             for i, event in enumerate(event_group):
@@ -754,15 +714,15 @@
                     assert all(
                         pulse is None or pulse == "dummy_precomp_reset"
                         for pulse in pulses_not_in_pulsedef
                     )
                     if len(pulses_not_in_pulsedef) > 0:
                         continue
 
-                    if any(
+                    if all(
                         not pulse_defs[pulse.pulse].can_compress
                         for pulse in wave_form.pulses
                     ):
                         continue
                     sampled_signature = sampled_signatures[wave_form]
                     sample_dict = {
                         k: sampled_signature[k]
@@ -770,16 +730,38 @@
                             "samples_i",
                             "samples_q",
                             "samples_marker1",
                             "samples_marker2",
                         )
                         if k in sampled_signature
                     }
+                    pulse_compr_info = namedtuple(
+                        "PulseComprInfo", ["start", "end", "can_compress"]
+                    )
+                    pulse_compr_infos = [
+                        pulse_compr_info(
+                            start=pulse.start,
+                            end=pulse.start + pulse.length,
+                            can_compress=pulse_defs[pulse.pulse].can_compress,
+                        )
+                        for pulse in wave_form.pulses
+                    ]
+                    if not self._pulses_compatible_for_compression(pulse_compr_infos):
+                        raise LabOneQException(
+                            "overlapping pulses need to either all have can_compress=True or can_compress=False"
+                        )
+                    compressible_segments = [
+                        (pulse.start, pulse.start + pulse.length)
+                        for pulse in wave_form.pulses
+                        if pulse_defs[pulse.pulse].can_compress
+                    ]
+                    # remove duplicates, keep order
+                    compressible_segments = [*dict.fromkeys(compressible_segments)]
                     new_events = self._wave_compressor.compress_wave(
-                        sample_dict, min_play_wave
+                        sample_dict, min_play_wave, compressible_segments
                     )
                     pulse_names = [pulse.pulse for pulse in wave_form.pulses]
                     if new_events is None:
                         _logger.info(
                             "Requested to compress pulse(s) %s which has(have) either no, or too short, constant sections. Skipping compression",
                             ",".join(pulse_names),
                         )
@@ -994,16 +976,16 @@
 
             sampled_events.merge(acquire_events)
 
         if awg.signal_type == AWGSignalType.MULTI:
             _logger.debug("Multi signal %s", awg)
             assert len(awg.signals) > 0
             delay = 0.0
-            device_type = awg.signals[0].device_type
-            sampling_rate = awg.signals[0].sampling_rate
+            device_type = awg.signals[0].awg.device_type
+            sampling_rate = awg.signals[0].awg.sampling_rate
             mixer_type = awg.signals[0].mixer_type
             for signal_obj in awg.signals:
                 if signal_obj.signal_type != "integration":
                     _logger.debug(
                         "Non-integration signal in multi signal: %s", signal_obj
                     )
                     delay = max(delay, signal_obj.total_delay)
@@ -1034,15 +1016,15 @@
                 mixer_type=mixer_type,
             )
 
             self._sampled_signatures[virtual_signal_id] = sampled_signatures
             sampled_events.merge(interval_events)
 
             min_play_waves = [
-                signal.device_type.min_play_wave for signal in awg.signals
+                signal.awg.device_type.min_play_wave for signal in awg.signals
             ]
             assert all(
                 min_play_wave == min_play_waves[0] for min_play_wave in min_play_waves
             )
             self._compress_waves(
                 sampled_events=sampled_events,
                 sampled_signatures=sampled_signatures,
@@ -1066,51 +1048,51 @@
                         False,
                         False,
                     )
 
         elif awg.signal_type != AWGSignalType.DOUBLE:
             for signal_obj in awg.signals:
 
-                if signal_obj.device_type == DeviceType.SHFQA:
+                if signal_obj.awg.device_type == DeviceType.SHFQA:
                     sub_channel = signal_obj.channels[0]
                 else:
                     sub_channel = None
                 interval_events = analyze_play_wave_times(
                     events=events,
                     signals={signal_obj.id: signal_obj},
-                    device_type=signal_obj.device_type,
-                    sampling_rate=signal_obj.sampling_rate,
+                    device_type=signal_obj.awg.device_type,
+                    sampling_rate=signal_obj.awg.sampling_rate,
                     delay=signal_obj.total_delay,
                     other_events=sampled_events,
                     phase_resolution_range=self.phase_resolution_range(),
                     waveform_size_hints=self.waveform_size_hints(
-                        signal_obj.device_type
+                        signal_obj.awg.device_type
                     ),
                     sub_channel=sub_channel,
                     use_command_table=use_command_table,
                 )
 
                 sampled_signatures = self._sample_pulses(
                     signal_obj.id,
                     interval_events,
                     pulse_defs=pulse_defs,
-                    sampling_rate=signal_obj.sampling_rate,
+                    sampling_rate=signal_obj.awg.sampling_rate,
                     signal_type=signal_obj.signal_type,
-                    device_type=signal_obj.device_type,
+                    device_type=signal_obj.awg.device_type,
                     mixer_type=signal_obj.mixer_type,
                 )
 
                 self._sampled_signatures[signal_obj.id] = sampled_signatures
                 sampled_events.merge(interval_events)
 
                 self._compress_waves(
                     sampled_events=sampled_events,
                     sampled_signatures=sampled_signatures,
                     signal_id=signal_obj.id,
-                    min_play_wave=signal_obj.device_type.min_play_wave,
+                    min_play_wave=signal_obj.awg.device_type.min_play_wave,
                     pulse_defs=pulse_defs,
                 )
 
                 if signal_obj.id in self._sampled_signatures:
                     signature_infos = []
                     for sig, sampled in self._sampled_signatures[signal_obj.id].items():
                         has_marker1 = False
@@ -1125,70 +1107,71 @@
                             length = sig.length
                             signature_infos.append(
                                 (sig_string, length, (has_marker1, has_marker2))
                             )
 
                     for siginfo in sorted(signature_infos):
                         declarations_generator.add_wave_declaration(
-                            signal_obj.device_type,
+                            signal_obj.awg.device_type,
                             signal_obj.signal_type,
                             siginfo[0],
                             siginfo[1],
                             siginfo[2][0],
                             siginfo[2][1],
                         )
         else:  # awg.signal_type == AWGSignalType.DOUBLE
             assert len(awg.signals) == 2
             signal_a, signal_b = awg.signals
             virtual_signal_id = signal_a.id + "_" + signal_b.id
             interval_events = analyze_play_wave_times(
                 events=events,
                 signals={s.id: s for s in awg.signals},
-                device_type=signal_a.device_type,
-                sampling_rate=signal_a.sampling_rate,
+                device_type=signal_a.awg.device_type,
+                sampling_rate=signal_a.awg.sampling_rate,
                 delay=signal_a.total_delay,
                 other_events=sampled_events,
                 phase_resolution_range=self.phase_resolution_range(),
-                waveform_size_hints=self.waveform_size_hints(signal_a.device_type),
+                waveform_size_hints=self.waveform_size_hints(signal_a.awg.device_type),
                 use_command_table=False,  # do not set amplitude/oscillator phase via CT
             )
 
             sampled_signatures = self._sample_pulses(
                 virtual_signal_id,
                 interval_events,
                 pulse_defs=pulse_defs,
-                sampling_rate=signal_a.sampling_rate,
+                sampling_rate=signal_a.awg.sampling_rate,
                 signal_type=signal_a.signal_type,
-                device_type=signal_a.device_type,
+                device_type=signal_a.awg.device_type,
                 mixer_type=signal_a.mixer_type,
             )
 
             self._sampled_signatures[virtual_signal_id] = sampled_signatures
             sampled_events.merge(interval_events)
 
             assert (
-                signal_a.device_type.min_play_wave == signal_b.device_type.min_play_wave
+                signal_a.awg.device_type.min_play_wave
+                == signal_b.awg.device_type.min_play_wave
             )
 
             self._compress_waves(
                 sampled_events=sampled_events,
                 sampled_signatures=sampled_signatures,
                 signal_id=virtual_signal_id,
-                min_play_wave=signal_a.device_type.min_play_wave,
+                min_play_wave=signal_a.awg.device_type.min_play_wave,
                 pulse_defs=pulse_defs,
             )
 
             if virtual_signal_id in self._sampled_signatures:
                 for sig, sampled in self._sampled_signatures[virtual_signal_id].items():
                     if not sampled:
                         continue
                     sig_string = sig.signature_string()
                     length = sig.length
                     declarations_generator.add_wave_declaration(
-                        signal_a.device_type,
+                        awg.device_type,
                         awg.signal_type.value,
                         sig_string,
                         length,
                         False,
                         False,
                     )
         self.post_process_sampled_events(awg, sampled_events)
@@ -1264,15 +1247,15 @@
 
         for line in seq_c_text.splitlines():
             _logger.debug(line)
 
         self._src.append({"filename": filename, "text": seq_c_text})
         self._wave_indices_all.append(
             {
-                "filename": os.path.splitext(filename)[0] + "_waveindices.csv",
+                "filename": filename,
                 "value": handler.wave_indices.wave_indices(),
             }
         )
         if use_command_table:
             self._command_tables.append(
                 {"seqc": filename, "ct": handler.command_table_tracker.command_table()}
             )
@@ -1331,15 +1314,14 @@
                     _logger.debug("Signature found %s in %s", signature, interval_event)
                     if any(p.pulse for p in signature.waveform.pulses):
                         signatures.add(signature)
                     else:
                         sampled_signatures[signature.waveform] = None
         _logger.debug("Signatures: %s", signatures)
 
-        max_amplitude = 0.0
         needs_conjugate = device_type == DeviceType.SHFSG
         for signature in signatures:
             length = signature.waveform.length
             _logger.debug(
                 "Sampling pulses for signature %s for signal %s, length %d device type %s",
                 signature.waveform.signature_string(),
                 signal_id,
@@ -1391,17 +1373,14 @@
                     sampling_signal_type = "iq"
 
                 amplitude = pulse_def.effective_amplitude
 
                 if pulse_part.amplitude is not None:
                     amplitude *= pulse_part.amplitude
 
-                if abs(amplitude) > max_amplitude:
-                    max_amplitude = abs(amplitude)
-
                 oscillator_phase = pulse_part.oscillator_phase
 
                 baseband_phase = pulse_part.baseband_phase
                 used_oscillator_frequency = pulse_part.oscillator_frequency
 
                 _logger.debug(
                     " Sampling pulse %s using oscillator frequency %s",
@@ -1586,16 +1565,15 @@
                 sampled_pulse_obj["samples_q"] = samples_q
 
             if has_marker1:
                 sampled_pulse_obj["samples_marker1"] = samples_marker1
             if has_marker2:
                 sampled_pulse_obj["samples_marker2"] = samples_marker2
 
-            if max_amplitude > 1e-9:
-                sampled_signatures[signature.waveform] = sampled_pulse_obj
+            sampled_signatures[signature.waveform] = sampled_pulse_obj
 
             verify_amplitude_no_clipping(
                 sampled_pulse_obj,
                 None,
                 mixer_type,
                 signal_id,
             )
```

## laboneq/compiler/code_generator/seq_c_generator.py

```diff
@@ -49,15 +49,14 @@
 
 
 SeqCStatement = Dict[str, Any]
 
 
 class SeqCGenerator:
     def __init__(self):
-        self._seq_c_text = ""
         self._statements: List[SeqCStatement] = []
 
     def num_statements(self):
         return len(self._statements)
 
     def num_noncomment_statements(self):
         retval = 0
@@ -315,90 +314,90 @@
         context of the added playHold(s). The passed list will be drained.
         """
         self._add_play_zero_or_hold(
             num_samples, device_type, "playHold", deferred_calls
         )
 
     def generate_seq_c(self):
-        self._seq_c_text = ""
+        seq_c_statements = []
         for statement in self._statements:
             _logger.debug("processing statement %s", statement)
-            self.emit_statement(statement)
-        return self._seq_c_text
+            seq_c_statements.append(self.emit_statement(statement))
+        return "".join(seq_c_statements)
 
     def emit_statement(self, statement: SeqCStatement):
         if statement["type"] == "generic_statement":
             if "assign_to" in statement:
-                self._seq_c_text += f"{statement['assign_to']} = "
-            self._seq_c_text += statement["function"] + "("
+                assign_to = f"{statement['assign_to']} = "
+            else:
+                assign_to = ""
             if "args" in statement:
-                is_first = True
-                for arg in statement["args"]:
-                    if not is_first:
-                        self._seq_c_text += ","
-                    else:
-                        is_first = False
-                    self._seq_c_text += str(arg)
-            self._seq_c_text += ");\n"
+                args = ",".join(str(s) for s in statement["args"])
+            else:
+                args = ""
+            return f"{assign_to}{statement['function']}({args});\n"
 
         elif statement["type"] == "wave_declaration":
             if statement["device_type"].supports_binary_waves:
-                self._seq_c_text += self._gen_wave_declaration_placeholder(statement)
+                return self._gen_wave_declaration_placeholder(statement)
+            else:
+                return ""
+
         elif statement["type"] == "function_def":
-            self._seq_c_text += statement["text"]
+            return statement["text"]
+
         elif statement["type"] == "variable_declaration":
-            self._seq_c_text += "var " + statement["variable_name"]
             if "initial_value" in statement:
-                self._seq_c_text += " = " + str(statement["initial_value"]) + ";\n"
+                initial_value = f" = {statement['initial_value']}"
             else:
-                self._seq_c_text += ";\n"
+                initial_value = ""
+            return f"var {statement['variable_name']}{initial_value};\n"
+
         elif statement["type"] == "variable_assignment":
-            self._seq_c_text += statement["variable_name"]
-            self._seq_c_text += " = " + str(statement["value"]) + ";\n"
+            return f"{statement['variable_name']} = {statement['value']};\n"
+
         elif statement["type"] == "variable_increment":
-            self._seq_c_text += statement["variable_name"]
-            self._seq_c_text += " += " + str(statement["value"]) + ";\n"
+            return f"{statement['variable_name']} += {statement['value']};\n"
 
         elif statement["type"] == "do_while":
-            self._seq_c_text += "do {\n"
-            self._seq_c_text += textwrap.indent(
-                statement["body"].generate_seq_c(), "  "
-            )
-            self._seq_c_text += "}\nwhile(" + statement["condition"] + ");\n"
+            body = textwrap.indent(statement["body"].generate_seq_c(), "  ")
+            return f"do {{\n{body}}}\nwhile({statement['condition']});\n"
 
         elif statement["type"] == "repeat":
-            self._seq_c_text += f"repeat ({statement['num_repeats']}) {{\n"
-            self._seq_c_text += textwrap.indent(
-                statement["body"].generate_seq_c(), "  "
-            )
-            self._seq_c_text += "}\n"
+            body = textwrap.indent(statement["body"].generate_seq_c(), "  ")
+            return f"repeat ({statement['num_repeats']}) {{\n{body}}}\n"
 
         elif statement["type"] == "assignWaveIndex":
             wave_channels = self._build_wave_channel_assignment(statement)
-            self._seq_c_text += (
-                f'assignWaveIndex({wave_channels},{statement["wave_index"]});\n'
-            )
+            return f'assignWaveIndex({wave_channels},{statement["wave_index"]});\n'
+
         elif statement["type"] == "playWave":
             wave_channels = self._build_wave_channel_assignment(statement)
-            self._seq_c_text += f"playWave({wave_channels});\n"
+            return f"playWave({wave_channels});\n"
+
         elif statement["type"] == "executeTableEntry":
-            self._seq_c_text += f"executeTableEntry({statement['table_index']}"
             latency = statement.get("latency", None)
             if latency is not None:
-                self._seq_c_text += f", {latency}"
-            self._seq_c_text += ");"
+                latency = f", {latency}"
+            else:
+                latency = ""
             if statement["comment"] != "":
-                self._seq_c_text += f"  // {statement['comment']}"
-            self._seq_c_text += "\n"
+                comment = f"  // {statement['comment']}"
+            else:
+                comment = ""
+            return f"executeTableEntry({statement['table_index']}{latency});{comment}\n"
+
         elif statement["type"] == "comment":
-            self._seq_c_text += "/* " + statement["text"] + " */\n"
+            return "/* " + statement["text"] + " */\n"
+
         elif statement["type"] == "playZero":
-            self._seq_c_text += f"playZero({statement['num_samples']});\n"
+            return f"playZero({statement['num_samples']});\n"
+
         elif statement["type"] == "playHold":
-            self._seq_c_text += f"playHold({statement['num_samples']});\n"
+            return f"playHold({statement['num_samples']});\n"
 
     def _gen_wave_declaration_placeholder(self, statement: SeqCStatement) -> str:
         dual_channel = statement["signal_type"] in ["iq", "double", "multi"]
         sig_string = statement["wave_id"]
         length = statement["length"]
         device_type = statement["device_type"]
         assert length >= device_type.min_play_wave
@@ -406,18 +405,17 @@
         makers_declaration2 = ""
         if statement["has_marker1"]:
             makers_declaration1 = ",true"
         if statement["has_marker2"]:
             makers_declaration2 = ",true"
 
         if dual_channel:
-
             return (
                 f"wave w{sig_string}_i = placeholder({length}{makers_declaration1});\n"
-                + f"wave w{sig_string}_q = placeholder({length}{makers_declaration2});\n"
+                f"wave w{sig_string}_q = placeholder({length}{makers_declaration2});\n"
             )
         else:
             return f"wave w{sig_string} = placeholder({length}{makers_declaration1});\n"
 
     def _build_wave_channel_assignment(self, statement) -> str:
         dual_channel = statement["signal_type"] in ["iq", "double", "multi"]
         sig_string = statement["wave_id"]
```

## laboneq/compiler/code_generator/signatures.py

```diff
@@ -1,15 +1,14 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import hashlib
 import math
-from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import Any, Dict, FrozenSet, Optional, Tuple
 
 import numpy as np
 from orjson import orjson
 
 from laboneq.compiler.code_generator.seq_c_generator import string_sanitize
@@ -203,16 +202,18 @@
 
 
 def reduce_signature_phase(
     signature: PlaybackSignature,
     use_ct_phase: bool,
     prev_hw_oscillator_phase: Optional[float],
 ) -> PlaybackSignature:
-    signature = deepcopy(signature)
+    """Reduces the phase of the signature.
 
+    Modifies the passed in `signature` object in-place.
+    """
     if use_ct_phase:
         this_hw_oscillator_phase = signature.waveform.pulses[-1].baseband_phase or 0.0
         if prev_hw_oscillator_phase is not None:
             increment = (this_hw_oscillator_phase - prev_hw_oscillator_phase) % (
                 2 * math.pi
             )
             if increment != 0:
@@ -235,19 +236,21 @@
             pulse.phase = (pulse.phase or 0.0) + pulse.oscillator_phase
             pulse.oscillator_phase = None
 
     return signature
 
 
 def reduce_signature_amplitude(signature: PlaybackSignature) -> PlaybackSignature:
-    # Absorb the pulse amplitude into the command table. Whenever possible, the
-    # waveforms will be sampled at unit amplitude, making waveform reuse more likely.
+    """Reduces the amplitude of the signature.
 
-    signature = deepcopy(signature)
+    Modifies the passed in `signature` object in-place.
 
+    Absorb the pulse amplitude into the command table. Whenever possible, the
+    waveforms will be sampled at unit amplitude, making waveform reuse more likely.
+    """
     if len(signature.waveform.pulses) == 0:
         return signature
     signature.set_amplitude = 1.0
     if any(pulse.amplitude is None for pulse in signature.waveform.pulses):
         return signature
 
     ct_amplitude = max(abs(pulse.amplitude) for pulse in signature.waveform.pulses)
```

## laboneq/compiler/code_generator/wave_compressor.py

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from dataclasses import dataclass
 from itertools import groupby
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
 
 @dataclass
 class PlayHold:
     num_samples: int
@@ -144,29 +144,40 @@
             self.wave_number += 1
             return events
 
     def _compress_wave_general(
         self,
         samples: Dict[str, np.array],
         stacked_samples: np.ndarray,
+        compressable_segments: List[Tuple[int, int]],
         num_sample_channles: int,
         num_frames: int,
+        num_samples: int,
         sample_multiple: int,
     ) -> Union[List[Union[PlayHold, PlaySamples]], None]:
         last_vals = np.zeros((num_sample_channles, num_frames))
         for i in range(0, num_frames):
             _, hi = self._get_frame_idx(samples, sample_multiple, i, num_frames)
             last_vals[:, i] = stacked_samples[:, hi - 1]
 
+        compressable_frames = []
+        for seg_lo, seg_hi in compressable_segments:
+            frame_lo = seg_lo // sample_multiple + 1
+            frame_hi = (
+                num_frames if seg_hi == num_samples else seg_hi // sample_multiple - 1
+            )
+            compressable_frames.append((frame_lo, frame_hi))
+
         can_compress = [False] * num_frames
-        for i in range(1, num_frames):
-            lo, hi = self._get_frame_idx(samples, sample_multiple, i, num_frames)
-            can_compress[i] = self._stacked_samples_constant(
-                stacked_samples, lo, hi
-            ) and np.all(last_vals[:, i - 1] == stacked_samples[:, lo])
+        for frame_lo, frame_hi in compressable_frames:
+            for i in range(frame_lo, frame_hi):
+                lo, hi = self._get_frame_idx(samples, sample_multiple, i, num_frames)
+                can_compress[i] = self._stacked_samples_constant(
+                    stacked_samples, lo, hi
+                ) and np.all(last_vals[:, i - 1] == stacked_samples[:, lo])
 
         if not any(can_compress):
             return None
 
         events = []
         sequences = [
             (key, list(group))
@@ -197,27 +208,58 @@
                     )
                 )
                 self.wave_number += 1
 
         return events
 
     def compress_wave(
-        self, samples: Dict[str, np.array], sample_multiple: int
+        self,
+        samples: Dict[str, np.array],
+        sample_multiple: int,
+        compressible_segments: Optional[List[Tuple[int, int]]] = None,
     ) -> Union[List[Union[PlayHold, PlaySamples]], None]:
         ref_length = len(list(samples.values())[0])
         num_sample_channles = len(list(samples.values()))
         if not all(len(v) == ref_length for v in samples.values()):
             raise ValueError("All sample arrays must have the same length")
         num_frames = int(ref_length / sample_multiple)
+        num_samples = ref_length
+
+        compressible_segments = (
+            [(0, num_samples)]
+            if compressible_segments is None
+            else compressible_segments
+        )
 
         stacked_samples = np.array(list(samples.values()))
 
-        runs = self._runs_longer_than_threshold(stacked_samples, 32)
+        if len(compressible_segments) > 1:
+            return self._compress_wave_general(
+                samples,
+                stacked_samples,
+                compressible_segments,
+                num_sample_channles,
+                num_frames,
+                num_samples,
+                sample_multiple,
+            )
+
+        compr_start, compr_end = compressible_segments[0]
+        runs = self._runs_longer_than_threshold(
+            stacked_samples[:, compr_start:compr_end], 32
+        )
         if len(runs) == 0:
             return None
         if len(runs) == 1:
+            runs = [(run[0] + compr_start, run[1] + compr_start) for run in runs]
             return self._compress_wave_simple(
                 samples, sample_multiple, ref_length, runs[0]
             )
         return self._compress_wave_general(
-            samples, stacked_samples, num_sample_channles, num_frames, sample_multiple
+            samples,
+            stacked_samples,
+            compressible_segments,
+            num_sample_channles,
+            num_frames,
+            num_samples,
+            sample_multiple,
         )
```

## laboneq/compiler/common/signal_obj.py

```diff
@@ -2,19 +2,19 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, List, Optional
 
+from laboneq.compiler.common.awg_signal_type import AWGSignalType
 from laboneq.core.types.enums.mixer_type import MixerType
 
 if TYPE_CHECKING:
     from laboneq.compiler.common.awg_info import AWGInfo
-    from laboneq.compiler.common.device_type import DeviceType
 
 
 @dataclass(init=True, repr=True, order=True)
 class SignalObj:
     """A collection of a signal's properties relevant for code generation. The delay
     fields are in seconds and their meaning is as follows:
     - start_delay: the delay from the trigger to the start of the sequence (lead time),
@@ -34,20 +34,17 @@
     - port_delay: port delay specified via the calibration; realized via the device node
       in addition to potential on-device delays.
     - base_port_delay: in case of an acquisition pulse, the port_delay of the
       corresponding measure pulse on the same AWG
     """
 
     id: str
-    sampling_rate: float
     start_delay: float
     delay_signal: float
-    signal_type: str
-    device_id: str
-    device_type: DeviceType
+    signal_type: AWGSignalType | str
     base_delay_signal: Optional[float] = None
     oscillator_frequency: float = None  # for software modulation only
     pulses: List = field(default_factory=list)
     channels: List = field(default_factory=list)
     awg: AWGInfo = None
     total_delay: float = None
     on_device_delay: float = 0
```

## laboneq/compiler/experiment_access/dsl_loader.py

```diff
@@ -3,14 +3,15 @@
 
 from __future__ import annotations
 
 import copy
 import logging
 import typing
 import uuid
+from dataclasses import dataclass
 from numbers import Number
 from types import SimpleNamespace
 from typing import Any, Callable, Dict, Tuple
 
 from laboneq.compiler.experiment_access.acquire_info import AcquireInfo
 from laboneq.compiler.experiment_access.loader_base import LoaderBase
 from laboneq.compiler.experiment_access.marker import Marker
@@ -25,14 +26,15 @@
     IODirection,
     IOSignalType,
 )
 
 if typing.TYPE_CHECKING:
     from laboneq.dsl.device import DeviceSetup
     from laboneq.dsl.device.io_units import LogicalSignal
+    from laboneq.dsl.device.ports import Port
     from laboneq.dsl.experiment import Experiment, ExperimentSignal
     from laboneq.dsl.parameter import Parameter
 
 _logger = logging.getLogger(__name__)
 
 
 def find_value_or_parameter_attr(entity: Any, attr: str, value_types: Tuple[type, ...]):
@@ -50,15 +52,17 @@
 
         for server in device_setup.servers.values():
             if hasattr(server, "leader_uid"):
                 global_leader_device_id = server.leader_uid
             self.add_server(server.uid, server.host, server.port, server.api_level)
 
         dest_path_devices = {}
-        ppc_connections = {}
+
+        # signal -> (device_uid, channel)
+        ppc_connections: dict[str, tuple[str, int]] = {}
 
         reference_clock = None
         for device in device_setup.instruments:
             if hasattr(device, "reference_clock"):
                 reference_clock = device.reference_clock
 
         for device in sorted(device_setup.instruments, key=lambda x: x.uid):
@@ -152,67 +156,72 @@
             for lsg in device_setup.logical_signal_groups.values()
             for ls in lsg.logical_signals.values()
         ]
         for ls in all_logical_signals:
             ls_map[ls.path] = ls
 
         mapped_logical_signals: Dict["LogicalSignal", "ExperimentSignal"] = {}
+        experiment_signals_by_physical_channel = {}
         for signal in experiment.signals.values():
             # Need to create copy here as we'll possibly patch those ExperimentSignals
             # that touch the same PhysicalChannel
             try:
-                mapped_logical_signals[
-                    ls_map[signal.mapped_logical_signal_path]
-                ] = copy.deepcopy(signal)
+                mapped_ls = ls_map[signal.mapped_logical_signal_path]
             except KeyError:
                 raise LabOneQException(
                     f"Experiment signal '{signal.uid}' has no mapping to a logical signal."
                 )
-
-        experiment_signals_by_physical_channel = {}
-        for ls, exp_signal in mapped_logical_signals.items():
+            sig_copy = copy.deepcopy(signal)
+            mapped_logical_signals[mapped_ls] = sig_copy
             experiment_signals_by_physical_channel.setdefault(
-                ls.physical_channel, []
-            ).append(exp_signal)
+                mapped_ls.physical_channel, []
+            )
+            experiment_signals_by_physical_channel[mapped_ls.physical_channel].append(
+                sig_copy
+            )
 
         from laboneq.dsl.device.io_units.physical_channel import (
             PHYSICAL_CHANNEL_CALIBRATION_FIELDS,
         )
 
         # Merge the calibration of those ExperimentSignals that touch the same
         # PhysicalChannel.
         for pc, exp_signals in experiment_signals_by_physical_channel.items():
             for field_ in PHYSICAL_CHANNEL_CALIBRATION_FIELDS:
                 if field_ in ["mixer_calibration", "precompensation"]:
                     continue
-                values = set()
+                unique_value = None
+                conflicting = False
                 for exp_signal in exp_signals:
                     if not exp_signal.is_calibrated():
                         continue
                     value = getattr(exp_signal, field_)
                     if value is not None:
-                        values.add(value)
-                if len(values) > 1:
+                        if unique_value is None:
+                            unique_value = value
+                        elif unique_value != value:
+                            conflicting = True
+                            break
+                if conflicting:
                     conflicting_signals = [
                         exp_signal.uid
                         for exp_signal in exp_signals
                         if exp_signal.is_calibrated()
                         and getattr(exp_signal.calibration, field_) is not None
                     ]
                     raise LabOneQException(
                         f"The experiment signals {', '.join(conflicting_signals)} all "
                         f"touch physical channel '{pc.uid}', but provide conflicting "
                         f"settings for calibration field '{field_}'."
                     )
-                if len(values) > 0:
+                if unique_value is not None:
                     # Make sure all the experiment signals agree.
-                    value = values.pop()
                     for exp_signal in exp_signals:
                         if exp_signal.is_calibrated():
-                            setattr(exp_signal.calibration, field_, value)
+                            setattr(exp_signal.calibration, field_, unique_value)
 
         for ls in all_logical_signals:
             calibration = ls.calibration
             experiment_signal_for_ls = mapped_logical_signals.get(ls)
             if experiment_signal_for_ls is not None:
                 experiment_signal_calibration = experiment_signal_for_ls.calibration
                 if experiment_signal_calibration is not None:
@@ -364,16 +373,17 @@
                         _logger.warning(
                             "'amplifier_pump' calibration for logical signal %s will be ignored - "
                             "no PPC is connected to it",
                             ls.path,
                         )
                     else:
                         ls_amplifier_pumps[ls.path] = (
-                            *ppc_connections[ls.path],
+                            ppc_connections[ls.path][0],
                             {
+                                "channel": ppc_connections[ls.path][1],
                                 "pump_freq": opt_param(amp_pump.pump_freq),
                                 "pump_power": opt_param(amp_pump.pump_power),
                                 "cancellation": amp_pump.cancellation,
                                 "alc_engaged": amp_pump.alc_engaged,
                                 "use_probe": amp_pump.use_probe,
                                 "probe_frequency": opt_param(amp_pump.probe_frequency),
                                 "probe_power": opt_param(amp_pump.probe_power),
@@ -475,54 +485,48 @@
                     "port_mode": ls_port_modes.get(lsuid),
                     "threshold": ls_thresholds.get(lsuid),
                     "amplitude": ls_amplitudes.get(lsuid),
                     "amplifier_pump": ls_amplifier_pumps.get(lsuid),
                 },
             )
 
-        open_inputs = {}
-        for instrument in device_setup.instruments:
-            for input_obj in instrument.ports:
-                if input_obj.direction == IODirection.IN:
-                    open_inputs[
-                        (instrument.uid, input_obj.signal_type)
-                    ] = input_obj.connector_labels
-
-        syncing_connections = []
-        for instrument in device_setup.instruments:
-            for connection in instrument.connections:
-                open_input_found = open_inputs.get(
-                    (connection.remote_path, connection.signal_type)
-                )
-                output = instrument.output_by_uid(connection.local_port)
-
-                if open_input_found is not None:
-                    syncing_connections.append(
-                        (
-                            instrument.uid,
-                            connection.remote_path,
-                            connection.signal_type,
-                            open_input_found,
-                            output,
-                        )
-                    )
+        available_inputs = {
+            (instrument.uid, input_obj.signal_type)
+            for instrument in device_setup.instruments
+            for input_obj in instrument.ports
+            if input_obj.direction == IODirection.IN
+        }
+
+        @dataclass
+        class _SyncingConnection:
+            leader_device_uid: str
+            follower_device_uid: str
+            signal_type: IOSignalType
+            output: Port | None
+
+        syncing_connections: list[_SyncingConnection] = [
+            _SyncingConnection(
+                leader_device_uid=instrument.uid,
+                follower_device_uid=connection.remote_path,
+                signal_type=connection.signal_type,
+                output=instrument.output_by_uid(connection.local_port),
+            )
+            for instrument in device_setup.instruments
+            for connection in instrument.connections
+            if (connection.remote_path, connection.signal_type) in available_inputs
+        ]
 
-        for syncing_connection in syncing_connections:
-            signal_type = syncing_connection[2]
-            assert isinstance(syncing_connection[2], type(IOSignalType.DIO))
-            if signal_type == IOSignalType.DIO:
-                dio_leader = syncing_connection[0]
-                dio_follower = syncing_connection[1]
-                self._dios.append((dio_leader, dio_follower))
-
-            elif signal_type == IOSignalType.ZSYNC:
-                zsync_leader = syncing_connection[0]
-                zsync_follower = syncing_connection[1]
-                port = syncing_connection[4].physical_port_ids[0]
-                self._pqsc_ports.append((zsync_leader, zsync_follower, int(port)))
+        for sc in syncing_connections:
+            if sc.signal_type == IOSignalType.DIO:
+                self.dios.append((sc.leader_device_uid, sc.follower_device_uid))
+            elif sc.signal_type == IOSignalType.ZSYNC:
+                port = int(sc.output.physical_port_ids[0])
+                self.pqsc_ports.append(
+                    (sc.leader_device_uid, sc.follower_device_uid, port)
+                )
 
         seq_avg_section, sweep_sections = find_sequential_averaging(experiment)
         if seq_avg_section is not None and len(sweep_sections) > 0:
             if len(sweep_sections) > 1:
                 raise LabOneQException(
                     f"Sequential averaging section {seq_avg_section.uid} has multiple "
                     f"sweeping subsections: {[s.uid for s in sweep_sections]}. There "
@@ -624,21 +628,17 @@
         acquisition_type,
         exchanger_map: Callable[[Any], Any],
         instance_id: str,
     ):
         has_repeat = False
         count = 1
 
-        averaging_type = None
         if hasattr(section, "count"):
             has_repeat = True
             count = section.count
-            if hasattr(section, "averaging_mode"):
-                if section.averaging_mode.value in ["cyclic", "sequential"]:
-                    averaging_type = "hardware"
 
         if hasattr(section, "parameters"):
             for parameter in section.parameters:
                 values_list = None
                 if parameter.values is not None:
                     values_list = list(parameter.values)
                 axis_name = getattr(parameter, "axis_name", None)
@@ -726,15 +726,14 @@
             SectionInfo(
                 section_id=instance_id,
                 section_display_name=section.uid,
                 has_repeat=has_repeat,
                 execution_type=execution_type,
                 count=count,
                 acquisition_types=acquisition_types,
-                averaging_type=averaging_type,
                 align=align,
                 on_system_grid=on_system_grid,
                 length=length,
                 averaging_mode=averaging_mode,
                 repetition_mode=repetition_mode,
                 repetition_time=repetition_time,
                 play_after=getattr(section, "play_after", None),
```

## laboneq/compiler/experiment_access/experiment_dao.py

```diff
@@ -23,20 +23,24 @@
 from laboneq.core.validators import dicts_equal
 
 _logger = logging.getLogger(__name__)
 
 
 class ExperimentDAO:
     def __init__(self, experiment, core_device_setup=None, core_experiment=None):
-        self._data = {}
+        self._data: dict[str, Any] = {}
         self._acquisition_type: AcquisitionType = None  # type: ignore
+
         if core_device_setup is not None and core_experiment is not None:
-            self._load_from_core(core_device_setup, core_experiment)
+            self._loader = self._load_from_core(core_device_setup, core_experiment)
         else:
-            self._load_experiment(experiment)
+            self._loader = self._load_experiment(experiment)
+        self._data = self._loader.data()
+        self._acquisition_type = self._loader.acquisition_type
+
         self.validate_experiment()
 
     def __eq__(self, other):
         if not isinstance(other, ExperimentDAO):
             return False
 
         return self._acquisition_type == other._acquisition_type and dicts_equal(
@@ -68,32 +72,30 @@
             "delay_signal": None,
             "port_mode": None,
             "threshold": None,
             "amplitude": None,
             "amplifier_pump": None,
         }
 
-    def _load_experiment(self, experiment):
+    def _load_experiment(self, experiment) -> JsonLoader:
         loader = JsonLoader()
         try:
             validator = loader.schema_validator()
             validator.validate(experiment)
         except ValidationError as exception:
             _logger.warning("Failed to validate input:")
             for line in str(exception).splitlines():
                 _logger.warning("validation error: %s", line)
         loader.load(experiment)
-        self._data = loader.data()
-        self._acquisition_type = loader.acquisition_type
+        return loader
 
-    def _load_from_core(self, device_setup, experiment):
+    def _load_from_core(self, device_setup, experiment) -> DSLLoader:
         loader = DSLLoader()
         loader.load(experiment, device_setup)
-        self._data = loader.data()
-        self._acquisition_type = loader.acquisition_type
+        return loader
 
     @staticmethod
     def dump(experiment_dao: "ExperimentDAO"):
         return json_dumper.dump(experiment_dao)
 
     @property
     def acquisition_type(self) -> AcquisitionType:
@@ -274,38 +276,35 @@
             )
         except StopIteration:
             return None
 
     def is_branch(self, section_id):
         return self._data["sections"][section_id].state is not None
 
-    def pqscs(self):
-        return [p[0] for p in self._data["pqsc_ports"]]
+    def pqscs(self) -> list[str]:
+        return list({p[0] for p in self._loader.pqsc_ports})
 
-    def pqsc_ports(self, pqsc_device_id):
+    def pqsc_ports(self, pqsc_device_uid: str):
         return [
             {"device": p[1], "port": p[2]}
-            for p in self._data["pqsc_ports"]
-            if p[0] == pqsc_device_id
+            for p in self._loader.pqsc_ports
+            if p[0] == pqsc_device_uid
         ]
 
-    def dio_followers(self):
-        return [d[1] for d in self._data["dios"]]
+    def dio_followers(self) -> list[str]:
+        return [d[1] for d in self._loader.dios]
 
-    def dio_leader(self, device_id):
+    def dio_leader(self, device_id) -> str | None:
         try:
-            return next(d[0] for d in self._data["dios"] if d[1] == device_id)
+            return next(d[0] for d in self._loader.dios if d[1] == device_id)
         except StopIteration:
             return None
 
-    def dio_connections(self):
-        return [(dio[0], dio[1]) for dio in self._data["dios"]]
-
-    def is_dio_leader(self, device_id):
-        return bool({d[1] for d in self._data["dios"] if d[0] == device_id})
+    def dio_connections(self) -> list[tuple[str, str]]:
+        return self._loader.dios
 
     def section_signals(self, section_id):
         return self._data["section_signals"].get(section_id, set())
 
     @cached_method()
     def section_signals_with_children(self, section_id):
         retval = set()
@@ -385,15 +384,15 @@
 
     def threshold(self, signal_id):
         return self._data["signal_connections"][signal_id]["threshold"]
 
     def amplitude(self, signal_id) -> float | str | None:
         return self._data["signal_connections"][signal_id]["amplitude"]
 
-    def amplifier_pump(self, signal_id) -> tuple[str, int, dict[str, Any]] | None:
+    def amplifier_pump(self, signal_id) -> tuple[str, dict[str, Any]] | None:
         return self._data["signal_connections"][signal_id]["amplifier_pump"]
 
     def section_pulses(self, section_id, signal_id):
         retval = self._section_pulses_raw(section_id, signal_id)
         for sp in retval:
             pulse_id = sp.pulse_id
             if pulse_id is not None:
```

## laboneq/compiler/experiment_access/json_dumper.py

```diff
@@ -233,16 +233,14 @@
         ]
 
         if section_info.has_repeat:
             out_section["repeat"] = {
                 "execution_type": section_info.execution_type,
                 "count": section_info.count,
             }
-            if section_info.averaging_type is not None:
-                out_section["repeat"]["averaging_type"] = section_info.averaging_type
 
             section_parameters = experiment_dao.section_parameters(section_id)
             if len(section_parameters) > 0:
                 out_section["repeat"]["parameters"] = []
                 for parameter in section_parameters:
                     param_object = {"id": parameter["id"]}
                     keys = ["start", "step", "values"]
```

## laboneq/compiler/experiment_access/json_loader.py

```diff
@@ -123,15 +123,15 @@
                     bool(oscillator["hardware"]),
                 )
 
     def _load_connectivity(self, experiment):
         if "connectivity" in experiment:
             if "dios" in experiment["connectivity"]:
                 for dio in experiment["connectivity"]["dios"]:
-                    self._dios.append((dio["leader"]["$ref"], dio["follower"]["$ref"]))
+                    self.dios.append((dio["leader"]["$ref"], dio["follower"]["$ref"]))
             if "leader" in experiment["connectivity"]:
 
                 leader_device_id = experiment["connectivity"]["leader"]["$ref"]
                 self._devices[leader_device_id]["is_global_leader"] = True
 
             if "reference_clock" in experiment["connectivity"]:
                 reference_clock = experiment["connectivity"]["reference_clock"]
@@ -141,15 +141,15 @@
 
             if "pqscs" in experiment["connectivity"]:
                 pqscs = experiment["connectivity"]["pqscs"]
                 for pqsc in pqscs:
                     pqsc_device_id = pqsc["device"]["$ref"]
                     if "ports" in pqsc:
                         for port in pqsc["ports"]:
-                            self._pqsc_ports.append(
+                            self.pqsc_ports.append(
                                 (pqsc_device_id, port["device"]["$ref"], port["port"])
                             )
 
     def _load_signals(self, experiment):
         for signal in sorted(experiment["signals"], key=lambda s: s["id"]):
             self.add_signal(
                 signal["id"],
@@ -270,21 +270,18 @@
                     sections_to_process.appendleft(
                         (child_section_ref["$ref"], instance_id)
                     )
             has_repeat = False
             execution_type = None
             length = None
             count: int = 1
-            averaging_type = None
 
             if "repeat" in section:
                 has_repeat = True
                 execution_type = section["repeat"]["execution_type"]
-                if "averaging_type" in section["repeat"]:
-                    averaging_type = section["repeat"]["averaging_type"]
 
                 count = int(section["repeat"]["count"])
                 if "parameters" in section["repeat"]:
                     for parameter in section["repeat"]["parameters"]:
                         values = None
                         if parameter.get("values") is not None:
                             values = copy.deepcopy(list(parameter["values"]))
@@ -357,15 +354,14 @@
                 SectionInfo(
                     section_id=instance_id,
                     section_display_name=section["id"],
                     has_repeat=has_repeat,
                     execution_type=execution_type,
                     count=count,
                     acquisition_types=acquisition_types,
-                    averaging_type=averaging_type,
                     align=align,
                     on_system_grid=on_system_grid,
                     length=length,
                     averaging_mode=averaging_mode,
                     repetition_mode=repetition_mode,
                     repetition_time=repetition_time,
                     play_after=section.get("play_after"),
```

## laboneq/compiler/experiment_access/loader_base.py

```diff
@@ -1,31 +1,35 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 import logging
-from typing import Optional
+from typing import Any, Optional
 
 from laboneq.compiler.experiment_access.pulse_def import PulseDef
 from laboneq.compiler.experiment_access.section_info import SectionInfo
 from laboneq.compiler.experiment_access.section_signal_pulse import SectionSignalPulse
 from laboneq.core.exceptions import LabOneQException
 from laboneq.core.types.enums import AcquisitionType
 
 logger = logging.getLogger(__name__)
 
 
 class LoaderBase:
     def __init__(self):
         self.acquisition_type: Optional[AcquisitionType] = None
 
+        # leader_uid, follower_uid, port
+        self.pqsc_ports: list[tuple[str, str, int]] = []
+
+        # leader_uid, follower_uid
+        self.dios: list[tuple[str, str]] = []
+
         self._devices = {}
         self._device_oscillators = {}
-        self._dios = []
         self._oscillators = {}
-        self._pqsc_ports = []
         self._pulses = {}
         self._sections = {}
         self._section_parameters = {}
         self._section_signals = {}
         self._section_signal_pulses = {}
         self._section_tree = {}
         self._servers = {}
@@ -33,21 +37,19 @@
         self._signal_connections = {}
         self._signal_markers = {}
         self._signal_oscillator = {}
         self._signal_trigger = {}
         self._root_sections = set()
         self._handle_acquires = {}
 
-    def data(self):
+    def data(self) -> dict[str, Any]:
         return {
             "devices": self._devices,
             "device_oscillators": self._device_oscillators,
-            "dios": self._dios,
             "oscillators": self._oscillators,
-            "pqsc_ports": self._pqsc_ports,
             "pulses": self._pulses,
             "root_sections": self._root_sections,
             "sections": self._sections,
             "section_parameters": self._section_parameters,
             "section_signals": self._section_signals,
             "section_signal_pulses": self._section_signal_pulses,
             "section_tree": self._section_tree,
```

## laboneq/compiler/experiment_access/section_info.py

```diff
@@ -9,15 +9,14 @@
 
 @dataclass
 class SectionInfo:
     section_id: str
     has_repeat: bool
     execution_type: Optional[str]
     acquisition_types: Optional[List[str]]
-    averaging_type: Optional[str]
     count: int
     align: Optional[str]
     on_system_grid: bool
     length: Optional[float]
     averaging_mode: Optional[str]
     repetition_mode: Optional[str]
     repetition_time: Optional[float]
```

## laboneq/compiler/scheduler/match_schedule.py

```diff
@@ -100,16 +100,16 @@
     # - The sum of the settings of the delay_signal parameter for the acquisition AWG
     #   for measure and acquire pulse
     # - The sum of the settings of the port_delay parameter for the acquisition device
     #   for measure and acquire pulse
 
     qa_signal_obj = schedule_data.signal_objects[acquire_pulse.pulse.signal_id]
 
-    qa_device_type = qa_signal_obj.device_type
-    qa_sampling_rate = qa_signal_obj.sampling_rate
+    qa_device_type = qa_signal_obj.awg.device_type
+    qa_sampling_rate = qa_signal_obj.awg.sampling_rate
 
     if qa_signal_obj.is_qc:
         toolkit_qatype = QAType.SHFQC
     else:
         toolkit_qatype = {"shfqa": QAType.SHFQA, "shfqc": QAType.SHFQC}.get(
             qa_device_type.str_value
         )
@@ -147,15 +147,15 @@
             * qa_sampling_rate
         )
         + qa_total_port_delay
     )
 
     for signal in signals:
         sg_signal_obj = schedule_data.signal_objects[signal]
-        sg_device_type = sg_signal_obj.device_type
+        sg_device_type = sg_signal_obj.awg.device_type
         if sg_signal_obj.is_qc:
             toolkit_sgtype = SGType.SHFQC
         else:
             toolkit_sgtype = {
                 "hdawg": SGType.HDAWG,
                 "shfsg": SGType.SHFSG,
                 "shfqc": SGType.SHFQC,
@@ -179,15 +179,15 @@
         # (arrival time of data in register + 3), which also simplifies phase
         # calculation for software modulated signals, and take care of subtracting it
         # later
 
         time_of_pulse_played = time_of_arrival_at_register + EXECUTETABLEENTRY_LATENCY
 
         sg_seq_rate = schedule_data.sampling_rate_tracker.sequencer_rate_for_device(
-            sg_signal_obj.device_id
+            sg_signal_obj.awg.device_id
         )
         sg_seq_dt_for_latency_in_ts = round(
             1 / (2 * sg_seq_rate * schedule_data.TINYSAMPLE)
         )
         latency_in_ts = time_of_pulse_played * sg_seq_dt_for_latency_in_ts
 
         # Calculate the shift of compiler zero time for the SG; we may subtract this
```

## laboneq/compiler/scheduler/scheduler.py

```diff
@@ -84,16 +84,14 @@
 
 class Scheduler:
     def __init__(
         self,
         experiment_dao: ExperimentDAO,
         sampling_rate_tracker: SamplingRateTracker,
         signal_objects: Dict[str, SignalObj],
-        # For compatibility with old scheduler, remove once we remove that
-        _clock_settings: Optional[Dict] = None,
         settings: Optional[CompilerSettings] = None,
     ):
         self._schedule_data = ScheduleData(
             experiment_dao=experiment_dao,
             settings=settings or CompilerSettings(),
             sampling_rate_tracker=sampling_rate_tracker,
             signal_objects=signal_objects,
@@ -415,18 +413,18 @@
     def _schedule_phase_reset(
         self,
         section_id: str,
         grid: int,
         signals: FrozenSet[str],
         hw_signals: FrozenSet[str],
     ) -> List[PhaseResetSchedule]:
-        reset_sw_oscillators = (
-            len(hw_signals) > 0
-            or self._experiment_dao.section_info(section_id).averaging_type
-            == "hardware"
+        section_info = self._experiment_dao.section_info(section_id)
+        reset_sw_oscillators = len(hw_signals) > 0 or (
+            section_info.execution_type == "hardware"
+            and section_info.averaging_mode is not None
         )
 
         if not reset_sw_oscillators and len(hw_signals) == 0:
             return []
 
         length = 0
         hw_osc_devices = {}
```

## laboneq/compiler/workflow/compiler.py

```diff
@@ -9,15 +9,14 @@
 from collections import Counter
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 from sortedcollections import SortedDict
 
 from laboneq._observability.tracing import trace
-from laboneq.compiler.code_generator import CodeGenerator
 from laboneq.compiler.code_generator.measurement_calculator import (
     IntegrationTimes,
     SignalDelays,
 )
 from laboneq.compiler.common import compiler_settings
 from laboneq.compiler.common.awg_info import AWGInfo, AwgKey
 from laboneq.compiler.common.awg_signal_type import AWGSignalType
@@ -33,26 +32,30 @@
 from laboneq.compiler.scheduler.scheduler import Scheduler
 from laboneq.compiler.workflow.precompensation_helpers import (
     compute_precompensation_delays_on_grid,
     compute_precompensations_and_delays,
     precompensation_is_nonzero,
     verify_precompensation_parameters,
 )
+from laboneq.compiler.workflow.realtime_compiler import (
+    RealtimeCompiler,
+    RealtimeCompilerOutput,
+)
 from laboneq.compiler.workflow.recipe_generator import RecipeGenerator
 from laboneq.core.exceptions import LabOneQException
 from laboneq.core.types.compiled_experiment import CompiledExperiment
 from laboneq.core.types.enums.acquisition_type import AcquisitionType
 from laboneq.core.types.enums.mixer_type import MixerType
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass
 class LeaderProperties:
-    global_leader: str = None
+    global_leader: str | None = None
     is_desktop_setup: bool = False
     internal_followers: List[str] = field(default_factory=list)
 
 
 _AWGMapping = Dict[str, Dict[int, AWGInfo]]
 
 
@@ -60,14 +63,15 @@
     def __init__(self, settings: Optional[Dict] = None):
         self._osc_numbering = None
         self._section_grids = {}
         self._experiment_dao: ExperimentDAO = None
         self._settings = compiler_settings.from_dict(settings)
         self._sampling_rate_tracker: SamplingRateTracker = None
         self._scheduler: Scheduler = None
+        self._rt_compiler_output: RealtimeCompilerOutput = None
 
         self._leader_properties = LeaderProperties()
         self._clock_settings: Dict[str, Any] = {}
         self._integration_unit_allocation = None
         self._awgs: _AWGMapping = {}
         self._precompensations: Dict[
             str, Dict[str, Union[Dict[str, Any], float]]
@@ -209,41 +213,34 @@
                     first_shfqa = get_first_instr_of(device_infos, "shfqa")
                     if first_shfqa.reference_clock_source is None:
                         self._clock_settings[first_shfqa.id] = "internal"
 
         self._clock_settings["use_2GHz_for_HDAWG"] = has_shf
         self._leader_properties.global_leader = leader
 
-    def _process_experiment(self, experiment):
+    def _process_experiment(self):
         self._calc_osc_numbering()
         self._calc_awgs()
         self._calc_shfqa_generator_allocation()
 
         self._sampling_rate_tracker = SamplingRateTracker(
             self._experiment_dao, self._clock_settings
         )
         self._calc_integration_unit_allocation()
         self._precompensations = self._calc_precompensations()
         self._signal_objects = self._generate_signal_objects()
-        _logger.debug("Processing Sections:::::::")
-
-        if not self._settings.USE_EXPERIMENTAL_SCHEDULER:
-            _logger.warning(
-                "The legacy scheduler has been removed; "
-                "the 'USE_EXPERIMENTAL_SCHEDULER' compiler flag is ignored."
-            )
 
-        self._scheduler = Scheduler(
+        rt_compiler = RealtimeCompiler(
             self._experiment_dao,
             self._sampling_rate_tracker,
             self._signal_objects,
-            self._clock_settings,
             self._settings,
         )
-        self._scheduler.run()
+
+        self._rt_compiler_output = rt_compiler.run()
 
     @staticmethod
     def _get_total_rounded_delay(delay, signal_id, device_type, sampling_rate):
         if delay < 0:
             raise RuntimeError(
                 f"Negative signal delay for signal {signal_id} specified."
             )
@@ -261,37 +258,14 @@
                 signal_id,
                 device_type.name,
                 delay_rounded * 1e9,
                 device_type.sample_multiple,
             )
         return delay_rounded
 
-    @trace("compiler.generate-code()")
-    def _generate_code(self):
-        code_generator = CodeGenerator(self._settings)
-        self._code_generator = code_generator
-
-        for signal_obj in self._signal_objects.values():
-            code_generator.add_signal(signal_obj)
-
-        _logger.debug("Preparing events for code generator")
-        events = self._scheduler.event_timing(expand_loops=False)
-
-        code_generator.gen_acquire_map(events, self._experiment_dao)
-        code_generator.gen_seq_c(
-            events,
-            {k: self._experiment_dao.pulse(k) for k in self._experiment_dao.pulses()},
-        )
-        self._command_table_match_offsets = code_generator.command_table_match_offsets()
-        self._feedback_connections = code_generator.feedback_connections()
-        self._feedback_registers = code_generator.feedback_registers()
-        code_generator.gen_waves()
-
-        _logger.debug("Code generation completed")
-
     def _calc_osc_numbering(self):
         self._osc_numbering = {}
 
         for signal_id in self._experiment_dao.signals():
             signal_info = self._experiment_dao.signal_info(signal_id)
             device_type = DeviceType(signal_info.device_type)
 
@@ -592,21 +566,18 @@
             if signal_type != "integration":
                 delay_info = delay_measure_acquire.setdefault(awg.key, DelayInfo())
                 delay_info.port_delay_gen = port_delay
                 delay_info.delay_signal_gen = delay_signal
 
             signal_obj = SignalObj(
                 id=signal_id,
-                sampling_rate=sampling_rate,
                 start_delay=start_delay,
                 delay_signal=delay_signal,
                 signal_type=signal_type,
-                device_id=device_id,
                 awg=awg,
-                device_type=device_type,
                 oscillator_frequency=oscillator_frequency,
                 channels=channels,
                 port_delay=port_delay,
                 mixer_type=mixer_type,
                 hw_oscillator=hw_oscillator,
                 is_qc=device_info.is_qc,
             )
@@ -946,15 +917,15 @@
 
     def _generate_recipe(self):
         recipe_generator = RecipeGenerator()
         recipe_generator.from_experiment(
             self._experiment_dao, self._leader_properties, self._clock_settings
         )
 
-        for output in self.calc_outputs(self._code_generator.signal_delays()):
+        for output in self.calc_outputs(self._rt_compiler_output.signal_delays):
             _logger.debug("Adding output %s", output)
             recipe_generator.add_output(
                 output["device_id"],
                 output["channel"],
                 output["offset"],
                 output["diagonal"],
                 output["off_diagonal"],
@@ -968,15 +939,15 @@
                 output_range_unit=output["range_unit"],
                 port_delay=output["port_delay"],
                 scheduler_port_delay=output["scheduler_port_delay"],
                 marker_mode=output.get("marker_mode"),
                 amplitude=output["amplitude"],
             )
 
-        for input in self.calc_inputs(self._code_generator.signal_delays()):
+        for input in self.calc_inputs(self._rt_compiler_output.signal_delays):
             _logger.debug("Adding input %s", input)
             recipe_generator.add_input(
                 input["device_id"],
                 input["channel"],
                 lo_frequency=input["lo_frequency"],
                 input_range=input["range"],
                 input_range_unit=input["range_unit"],
@@ -996,148 +967,83 @@
                     awg_signals = {c for c, _ in awg.signal_channels}
                 if signal_type == AWGSignalType.MULTI:
                     signal_type = AWGSignalType.IQ
                 # Find the acquire signal from which we read the feedback from and which
                 # is used via a match/state construct for the drive signals of this awg
                 qa_signal_ids = {
                     h.acquire
-                    for h in self._feedback_connections.values()
+                    for h in self._rt_compiler_output.feedback_connections.values()
                     if h.drive.intersection(awg_signals)
                 }
                 if len(qa_signal_ids) > 1:
                     raise Exception(
                         f"The drive signal(s) ({set(awg_signals)}) can only react to "
                         f"one acquire signal for feedback, got {qa_signal_ids}."
                     )
                 recipe_generator.add_awg(
                     device_id=device_id,
                     awg_number=awg.awg_number,
                     signal_type=signal_type.value,
-                    seqc=awg.seqc,
                     qa_signal_id=next(iter(qa_signal_ids), None),
-                    command_table_match_offset=self._command_table_match_offsets.get(
+                    command_table_match_offset=self._rt_compiler_output.command_table_match_offsets.get(
                         awg.key
                     ),
-                    feedback_register=self._feedback_registers.get(awg.key),
+                    feedback_register=self._rt_compiler_output.feedback_registers.get(
+                        awg.key
+                    ),
+                )
+                recipe_generator.add_realtime_step(
+                    device_id=device_id,
+                    awg_id=awg.awg_number,
+                    seqc_filename=awg.seqc,
+                    wave_indices_name="",  # todo
+                    nt_loop_indices=[],  # todo
                 )
 
-        if self._code_generator is None:
-            raise Exception("Code generator not initialized")
+        assert self._rt_compiler_output is not None
         recipe_generator.add_oscillator_params(self._experiment_dao)
         recipe_generator.add_integrator_allocations(
             self._integration_unit_allocation,
             self._experiment_dao,
-            self._code_generator.integration_weights(),
+            self._rt_compiler_output.integration_weights,
         )
 
         recipe_generator.add_acquire_lengths(
-            integration_times=self._code_generator.integration_times()
+            integration_times=self._rt_compiler_output.integration_times
         )
 
         recipe_generator.add_measurements(
             self.calc_measurement_map(
-                integration_times=self._code_generator.integration_times()
+                integration_times=self._rt_compiler_output.integration_times
             )
         )
 
         recipe_generator.add_simultaneous_acquires(
-            self._code_generator.simultaneous_acquires()
+            self._rt_compiler_output.simultaneous_acquires
         )
 
         recipe_generator.add_total_execution_time(
-            self._code_generator.total_execution_time()
+            self._rt_compiler_output.total_execution_time
         )
 
         self._recipe = recipe_generator.recipe()
         _logger.debug("Recipe generation completed")
 
     def compiler_output(self) -> CompiledExperiment:
         return CompiledExperiment(
             recipe=self._recipe,
-            src=self._code_generator.src(),
-            waves=self._code_generator.waves(),
-            wave_indices=self._code_generator.wave_indices(),
-            command_tables=self._code_generator.command_tables(),
-            schedule=self._prepare_schedule(),
+            src=self._rt_compiler_output.src,
+            waves=self._rt_compiler_output.waves,
+            wave_indices=self._rt_compiler_output.wave_indices,
+            command_tables=self._rt_compiler_output.command_tables,
+            schedule=self._rt_compiler_output.schedule,
             experiment_dict=ExperimentDAO.dump(self._experiment_dao),
-            pulse_map=self._code_generator.pulse_map(),
+            pulse_map=self._rt_compiler_output.pulse_map,
         )
 
-    def _prepare_schedule(self):
-        event_list = self._scheduler.event_timing(
-            expand_loops=self._settings.EXPAND_LOOPS_FOR_SCHEDULE,
-            max_events=self._settings.MAX_EVENTS_TO_PUBLISH,
-        )
-
-        event_list = [
-            {k: v for k, v in event.items() if v is not None} for event in event_list
-        ]
-
-        try:
-            root_section = self._experiment_dao.root_rt_sections()[0]
-        except IndexError:
-            return {
-                "event_list": [],
-                "section_graph": {},
-                "section_info": {},
-                "subsection_map": {},
-                "section_signals_with_children": {},
-                "sampling_rates": [],
-            }
-
-        preorder_map = self._scheduler.preorder_map()
-
-        section_info_out = {}
-
-        section_signals_with_children = {}
-
-        for section in [
-            root_section,
-            *self._experiment_dao.all_section_children(root_section),
-        ]:
-            section_info = self._experiment_dao.section_info(section)
-            section_display_name = section_info.section_display_name
-            section_signals_with_children[section] = list(
-                self._experiment_dao.section_signals_with_children(section)
-            )
-            section_info_out[section] = {
-                "section_display_name": section_display_name,
-                "preorder": preorder_map[section],
-            }
-
-        sampling_rate_tuples = []
-        for signal_id in self._experiment_dao.signals():
-            signal_info = self._experiment_dao.signal_info(signal_id)
-            device_id = signal_info.device_id
-            device_type = signal_info.device_type
-            sampling_rate_tuples.append(
-                (
-                    device_type,
-                    int(
-                        self._sampling_rate_tracker.sampling_rate_for_device(device_id)
-                    ),
-                )
-            )
-
-        sampling_rates = [
-            [list(set([d[0] for d in sampling_rate_tuples if d[1] == r])), r]
-            for r in set([t[1] for t in sampling_rate_tuples])
-        ]
-
-        _logger.debug("Pulse sheet generation completed")
-
-        return {
-            "event_list": event_list,
-            "section_graph": [],  # deprecated: not needed by PSV
-            "section_info": section_info_out,
-            "subsection_map": {},  # deprecated: not needed by PSV
-            "section_signals_with_children": section_signals_with_children,
-            "sampling_rates": sampling_rates,
-        }
-
     def dump_src(self, info=False):
         for src in self.compiler_output().src:
             if info:
                 _logger.info("*** %s", src["filename"])
             else:
                 _logger.debug("*** %s", src["filename"])
             for line in src["text"].splitlines():
@@ -1152,17 +1058,15 @@
 
     @trace("compiler.run()")
     def run(self, data) -> CompiledExperiment:
         _logger.debug("ES Compiler run")
 
         self.use_experiment(data)
         self._analyze_setup()
-        self._process_experiment(data)
-
-        self._generate_code()
+        self._process_experiment()
         self._generate_recipe()
 
         retval = self.compiler_output()
 
         total_seqc_lines = 0
         for f in retval.src:
             total_seqc_lines += f["text"].count("\n")
```

## laboneq/compiler/workflow/recipe_generator.py

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from laboneq.compiler.code_generator.measurement_calculator import IntegrationTimes
 from laboneq.compiler.common.device_type import DeviceType
 from laboneq.compiler.experiment_access.experiment_dao import ExperimentDAO
 
 if TYPE_CHECKING:
     from laboneq.compiler.workflow.compiler import LeaderProperties
@@ -24,15 +24,15 @@
         ] = "../../interface/qccs/interface/schemas/recipe-schema-1_4_0.json"
         self._recipe["line_endings"] = "unix"
         self._recipe["header"] = {
             "version": "1.4.0",
             "unit": {"time": "s", "frequency": "Hz", "phase": "rad"},
             "epsilon": {"time": 1e-12},
         }
-        self._recipe["experiment"] = {}
+        self._recipe["experiment"] = {"realtime_execution_init": []}
 
     def add_oscillator_params(self, experiment_dao: ExperimentDAO):
         hw_oscillators = {}
         for oscillator in experiment_dao.hardware_oscillators():
             hw_oscillators[oscillator.id] = oscillator
 
         oscillator_params = []
@@ -118,73 +118,55 @@
         clock_settings: Dict[str, Any],
     ):
         if leader_properties.global_leader is not None:
             initialization = self._find_initialization(leader_properties.global_leader)
             initialization["config"]["repetitions"] = 1
             initialization["config"]["holdoff"] = 0
             if leader_properties.is_desktop_setup:
-                initialization["config"]["dio_mode"] = "hdawg_leader"
+                initialization["config"]["triggering_mode"] = "desktop_leader"
         if leader_properties.is_desktop_setup:
             # Internal followers are followers on the same device as the leader. This
             # is necessary for the standalone SHFQC, where the SHFSG part does neither
             # appear in the PQSC device connections nor the DIO connections.
             for f in leader_properties.internal_followers:
                 initialization = self._find_initialization(f)
-                initialization["config"]["dio_mode"] = "hdawg"
+                initialization["config"]["triggering_mode"] = "internal_follower"
 
         for device in experiment_dao.device_infos():
             device_uid = device.id
             initialization = self._find_initialization(device_uid)
             reference_clock = experiment_dao.device_reference_clock(device_uid)
             if reference_clock is not None:
                 initialization["config"]["reference_clock"] = reference_clock
 
-            try:
-                initialization["config"]["reference_clock_source"] = clock_settings[
-                    device_uid
-                ]
-            except KeyError:
-                initialization["config"][
-                    "reference_clock_source"
-                ] = device.reference_clock_source
-
             if device.device_type == "hdawg" and clock_settings["use_2GHz_for_HDAWG"]:
                 initialization["config"][
                     "sampling_rate"
                 ] = DeviceType.HDAWG.sampling_rate_2GHz
 
             if device.device_type == "shfppc":
-                ppchannels = {}
+                ppchannels = []
                 for signal in experiment_dao.signals():
                     amplifier_pump = experiment_dao.amplifier_pump(signal)
                     if amplifier_pump is not None and amplifier_pump[0] == device_uid:
-                        ppchannels[amplifier_pump[1]] = amplifier_pump[2]
+                        ppchannels.append(amplifier_pump[1])
                 initialization["ppchannels"] = ppchannels
 
             for follower in experiment_dao.dio_followers():
                 initialization = self._find_initialization(follower)
-                if not leader_properties.is_desktop_setup:
-                    initialization["config"]["dio_mode"] = "hdawg"
+                if leader_properties.is_desktop_setup:
+                    initialization["config"]["triggering_mode"] = "desktop_dio_follower"
                 else:
-                    initialization["config"][
-                        "dio_mode"
-                    ] = "dio_follower_of_hdawg_leader"
+                    initialization["config"]["triggering_mode"] = "dio_follower"
 
         for pqsc_device_id in experiment_dao.pqscs():
-            pqsc_device = self._find_initialization(pqsc_device_id)
-            out_ports = []
             for port in experiment_dao.pqsc_ports(pqsc_device_id):
                 follower_device_id = port["device"]
-                out_ports.append(
-                    {"port": port["port"], "device_uid": follower_device_id}
-                )
                 follower_device_init = self._find_initialization(follower_device_id)
-                follower_device_init["config"]["dio_mode"] = "zsync_dio"
-
-            pqsc_device["ports"] = out_ports
+                follower_device_init["config"]["triggering_mode"] = "zsync_follower"
 
     def add_output(
         self,
         device_id,
         channel,
         offset=0.0,
         diagonal=1.0,
@@ -262,33 +244,49 @@
         inputs.append(input)
 
     def add_awg(
         self,
         device_id: str,
         awg_number: int,
         signal_type: str,
-        seqc: str,
         qa_signal_id: Optional[str],
         command_table_match_offset: Optional[int],
         feedback_register: Optional[int],
     ):
         initialization = self._find_initialization(device_id)
 
         if "awgs" not in initialization:
             initialization["awgs"] = []
         awg = {
             "awg": awg_number,
-            "seqc": seqc,
             "signal_type": signal_type,
             "qa_signal_id": qa_signal_id,
             "command_table_match_offset": command_table_match_offset,
             "feedback_register": feedback_register,
         }
         initialization["awgs"].append(awg)
 
+    def add_realtime_step(
+        self,
+        device_id: str,
+        awg_id: int,
+        seqc_filename: str,
+        wave_indices_name: str,
+        nt_loop_indices: List[int],
+    ):
+        self._recipe["experiment"]["realtime_execution_init"].append(
+            {
+                "device_id": device_id,
+                "awg_id": awg_id,
+                "seqc_ref": seqc_filename,
+                "wave_indices_ref": wave_indices_name,
+                "nt_step": {"indices": nt_loop_indices},
+            }
+        )
+
     def from_experiment(
         self,
         experiment_dao: ExperimentDAO,
         leader_properties: LeaderProperties,
         clock_settings: Dict[str, Any],
     ):
         self.add_devices_from_experiment(experiment_dao)
```

## laboneq/contrib/example_helpers/plotting/plot_helpers.py

```diff
@@ -34,14 +34,17 @@
     compiled_experiment,
     start_time=0.0,
     length=10e-6,
     xaxis_label="Time (s)",
     yaxis_label="Amplitude",
     plot_width=6,
     plot_height=2,
+    save=False,
+    filename="filename",
+    filetype="svg",
 ):
     simulation = OutputSimulator(compiled_experiment)
 
     mapped_signals = compiled_experiment.experiment.signal_mapping_status[
         "mapped_signals"
     ]
 
@@ -69,14 +72,15 @@
         my_snippet = simulation.get_snippet(
             compiled_experiment.device_setup.logical_signal_groups[signal_group_name]
             .logical_signals[signal_line_name]
             .physical_channel,
             start=start_time,
             output_length=length,
             get_trigger=True,
+            get_marker=True,
             get_frequency=True,
         )
 
         physcial_channel = (
             compiled_experiment.device_setup.logical_signal_groups[signal_group_name]
             .logical_signals[signal_line_name]
             .physical_channel.uid.replace("_", " ")
@@ -131,26 +135,50 @@
             try:
                 if my_snippet.time is not None:
                     time_length = len(my_snippet.time)
 
                     xs.append(my_snippet.time)
 
                     y1s.append(my_snippet.trigger)
-                    labels1.append(f"{signal} Trigger")
+                    labels1.append(f"{signal} - Trigger")
 
                     titles.append(f"{physcial_channel} - Trigger".upper())
 
                     empty_array = np.empty((1, time_length))
                     empty_array.fill(np.nan)
                     y2s.append(empty_array[0])
                     labels2.append(None)
 
             except Exception:
                 pass
 
+        if np.any(my_snippet.marker):
+            try:
+                if my_snippet.time is not None:
+                    time_length = len(my_snippet.time)
+
+                    xs.append(my_snippet.time)
+
+                    y1s.append(my_snippet.marker.real)
+                    labels1.append(f"{signal} - Marker 1")
+
+                    if np.any(my_snippet.marker.imag):
+                        y2s.append(my_snippet.marker.imag)
+                        labels2.append(f"{signal} - Marker 2")
+                    else:
+                        empty_array = np.empty((1, time_length))
+                        empty_array.fill(np.nan)
+                        y2s.append(empty_array[0])
+                        labels2.append(None)
+
+                    titles.append(f"{physcial_channel} - {signal} - Marker".upper())
+
+            except Exception:
+                pass
+
     fig, axes = plt.subplots(
         nrows=len(y1s),
         sharex=False,
         figsize=(plot_width, len(y1s) * plot_height),
     )
 
     colors = plt.rcParams["axes.prop_cycle"]()
@@ -184,14 +212,16 @@
             axes.set_xlabel(xaxis_label)
             axes.set_title(title)
             axes.legend(loc="upper right")
             axes.ticklabel_format(axis="both", style="sci", scilimits=(0, 0))
             axes.grid(True)
 
     fig.tight_layout()
+    if save is True:
+        fig.savefig(f"{filename}.{filetype}", format=f"{filetype}")
     # fig.legend(loc="upper left")
     plt.show()
 
 
 # general result plotting
 def plot_results(
     results,
```

## laboneq/controller/controller.py

```diff
@@ -4,54 +4,51 @@
 from __future__ import annotations
 
 import concurrent.futures
 import itertools
 import logging
 import os
 import time
-import traceback
 from collections import defaultdict
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable
 
 import numpy as np
 import zhinst.utils
 from numpy import typing as npt
 
 from laboneq import __version__
 from laboneq._observability import tracing
 from laboneq.controller.communication import (
-    CachingStrategy,
     DaqNodeAction,
     DaqNodeSetAction,
     DaqWrapper,
     batch_set,
 )
 from laboneq.controller.devices.device_collection import DeviceCollection
 from laboneq.controller.devices.device_uhfqa import DeviceUHFQA
 from laboneq.controller.devices.device_zi import DeviceZI
 from laboneq.controller.devices.zi_node_monitor import ResponseWaiter
-from laboneq.controller.protected_session import ProtectedSession
+from laboneq.controller.near_time_runner import NearTimeRunner
 from laboneq.controller.recipe_1_4_0 import *  # noqa: F401, F403
 from laboneq.controller.recipe_processor import (
     RecipeData,
     RtExecutionInfo,
     pre_process_compiled,
 )
 from laboneq.controller.results import (
     build_partial_result,
     make_acquired_result,
     make_empty_results,
 )
-from laboneq.controller.util import LabOneQControllerException, SweepParamsTracker
+from laboneq.controller.util import LabOneQControllerException
 from laboneq.core.types.enums.acquisition_type import AcquisitionType
 from laboneq.core.types.enums.averaging_mode import AveragingMode
 from laboneq.core.utilities.replace_pulse import ReplacementType, calc_wave_replacements
-from laboneq.executor.executor import ExecutorBase, LoopingMode, LoopType
 
 if TYPE_CHECKING:
     from laboneq.core.types import CompiledExperiment
     from laboneq.dsl import Session
     from laboneq.dsl.device.device_setup import DeviceSetup
     from laboneq.dsl.experiment.pulse import Pulse
     from laboneq.dsl.result.results import Results
@@ -77,34 +74,49 @@
 
 
 # atexit hook
 def _stop_controller(controller: "Controller"):
     controller.shut_down()
 
 
+@dataclass
+class _SeqCCompileItem:
+    awg_index: int
+    seqc_code: str | None = None
+    seqc_filename: str | None = None
+    elf: bytes | None = None
+
+
+@dataclass
+class _UploadItem:
+    seqc_item: _SeqCCompileItem | None
+    waves: list[Any] | None
+    command_table: dict[Any] | None
+
+
 class Controller:
     def __init__(
         self,
         run_parameters: ControllerRunParameters = None,
         device_setup: DeviceSetup = None,
-        user_functions: Dict[str, Callable] = None,
+        user_functions: dict[str, Callable] = None,
     ):
         self._run_parameters = run_parameters or ControllerRunParameters()
         self._devices = DeviceCollection(
             device_setup,
             self._run_parameters.dry_run,
             self._run_parameters.ignore_version_mismatch,
         )
 
         self._last_connect_check_ts: float = None
 
         # Waves which are uploaded to the devices via pulse replacements
         self._current_waves = []
-        self._user_functions: Dict[str, Callable] = user_functions
-        self._nodes_from_user_functions: List[DaqNodeAction] = []
+        self._user_functions: dict[str, Callable] = user_functions
+        self._nodes_from_user_functions: list[DaqNodeAction] = []
         self._recipe_data: RecipeData = None
         self._session = None
         self._results: Results = None
 
         _logger.debug("Controller created")
         _logger.debug("Controller debug logging is on")
 
@@ -118,21 +130,16 @@
 
     def _reset_to_idle_state(self):
         reset_nodes = []
         for _, device in self._devices.all:
             reset_nodes.extend(device.collect_reset_nodes())
         batch_set(reset_nodes)
 
-    def _wait_for_conditions_to_start(self):
-        for initialization in self._recipe_data.initializations:
-            device = self._devices.find_by_uid(initialization.device_uid)
-            device.wait_for_conditions_to_start()
-
     def _apply_recipe_initializations(self):
-        nodes_to_initialize: List[DaqNodeAction] = []
+        nodes_to_initialize: list[DaqNodeAction] = []
         for initialization in self._recipe_data.initializations:
             device = self._devices.find_by_uid(initialization.device_uid)
             nodes_to_initialize.extend(
                 device.collect_initialization_nodes(
                     self._recipe_data.device_settings[initialization.device_uid],
                     initialization,
                 )
@@ -149,107 +156,117 @@
                 device.collect_awg_before_upload_nodes(
                     initialization, self._recipe_data
                 )
             )
         batch_set(nodes_to_initialize)
 
     @tracing.trace("awg-program-handler")
-    def _upload_awg_programs(self):
-        @dataclass
-        class UploadItem:
-            awg_index: int
-            seqc_code: str
-            seqc_filename: str
-            waves: List[Any]
-            command_table: Dict[Any]
-            elf: Optional[bytes]
-
+    def _upload_awg_programs(self, nt_step: NtStepKey):
+        if any(i != 0 for i in nt_step.indices):
+            # Only execute for the 1st NT step
+            # TODO(2K): remove, once NT steps are properly passed in the recipe.
+            # See also commented out condition on selection of realtime_execution_init
+            # element below
+            return
         # Mise en place:
-        awg_data: Dict[DeviceZI, List[UploadItem]] = defaultdict(list)
+        awg_data: dict[DeviceZI, list[_UploadItem]] = defaultdict(list)
+        compile_data: dict[DeviceZI, list[_SeqCCompileItem]] = defaultdict(list)
         recipe_data = self._recipe_data
         acquisition_type = RtExecutionInfo.get_acquisition_type(
             recipe_data.rt_execution_infos
         )
         for initialization in recipe_data.initializations:
             device = self._devices.find_by_uid(initialization.device_uid)
 
             if initialization.awgs is None:
                 continue
 
             for awg_obj in initialization.awgs:
                 awg_index = awg_obj.awg
-                seqc_code, waves, command_table = device.prepare_seqc(
-                    awg_obj.seqc, recipe_data.compiled
-                )
+                rt_exec_step = next(
+                    (
+                        r
+                        for r in recipe_data.recipe.experiment.realtime_execution_init
+                        if r.device_id == initialization.device_uid
+                        and r.awg_id == awg_obj.awg
+                        # and r.nt_step == nt_step # TODO(2K): Enable once ready in recipe
+                    ),
+                    None,
+                )
+                if rt_exec_step is None:
+                    continue
+
+                seqc_code = device.prepare_seqc(
+                    recipe_data.compiled, rt_exec_step.seqc_ref
+                )
+                # TODO(2K): rt_exec_step.wave_indices_ref instead of seqc_ref
+                waves = device.prepare_waves(
+                    recipe_data.compiled, rt_exec_step.seqc_ref
+                )
+                # TODO(2K): rt_exec_step.ct_ref instead of seqc_ref
+                command_table = device.prepare_command_table(
+                    recipe_data.compiled, rt_exec_step.seqc_ref
+                )
+
+                seqc_item = _SeqCCompileItem(
+                    awg_index=awg_index,
+                )
+
+                if seqc_code is not None:
+                    seqc_item.seqc_code = seqc_code
+                    seqc_item.seqc_filename = rt_exec_step.seqc_ref
+                    compile_data[device].append(seqc_item)
+
                 awg_data[device].append(
-                    UploadItem(
-                        awg_index, seqc_code, awg_obj.seqc, waves, command_table, None
+                    _UploadItem(
+                        seqc_item=seqc_item,
+                        waves=waves,
+                        command_table=command_table,
                     )
                 )
 
-        # Compile in parallel:
-        def worker(device: DeviceZI, item: UploadItem, span: tracing.Span):
-            with tracing.get_tracer().start_span("compile-awg-thread", span) as _:
-                item.elf = device.compile_seqc(
-                    item.seqc_code, item.awg_index, item.seqc_filename
-                )
-
-        _logger.debug("Started compilation of AWG programs...")
-        with tracing.get_tracer().start_span("compile-awg-programs") as awg_span:
-            max_workers = os.environ.get("LABONEQ_AWG_COMPILER_MAX_WORKERS")
-            max_workers = int(max_workers) if max_workers is not None else None
-            with concurrent.futures.ThreadPoolExecutor(
-                max_workers=max_workers
-            ) as executor:
-                futures = [
-                    executor.submit(worker, device, item, awg_span)
-                    for device, items in awg_data.items()
-                    for item in items
-                ]
-                concurrent.futures.wait(futures)
-                exceptions = [
-                    future.exception()
-                    for future in futures
-                    if future.exception() is not None
-                ]
-                if len(exceptions) > 0:
-                    raise LabOneQControllerException(
-                        "Compilation failed. See log output for details."
-                    )
-        _logger.debug("Finished compilation.")
+        self._awg_compile(compile_data)
 
         # Upload AWG programs, waveforms, and command tables:
-        elf_node_settings: Dict[DaqWrapper, List[DaqNodeSetAction]] = defaultdict(list)
-        elf_upload_conditions: Dict[DaqWrapper, Dict[str, Any]] = defaultdict(dict)
-        wf_node_settings: Dict[DaqWrapper, List[DaqNodeSetAction]] = defaultdict(list)
+        elf_node_settings: dict[DaqWrapper, list[DaqNodeSetAction]] = defaultdict(list)
+        elf_upload_conditions: dict[DaqWrapper, dict[str, Any]] = defaultdict(dict)
+        wf_node_settings: dict[DaqWrapper, list[DaqNodeSetAction]] = defaultdict(list)
         for device, items in awg_data.items():
             for item in items:
-                elf_filename = item.seqc_filename.rsplit(".seqc", 1)[0] + ".elf"
-                set_action = device.prepare_upload_elf(
-                    item.elf, item.awg_index, elf_filename
-                )
-                node_settings = elf_node_settings[device.daq]
-                node_settings.append(set_action)
+                seqc_item = item.seqc_item
+                if seqc_item.elf is not None:
+                    set_action = device.prepare_upload_elf(
+                        seqc_item.elf, seqc_item.awg_index, seqc_item.seqc_filename
+                    )
+                    node_settings = elf_node_settings[device.daq]
+                    node_settings.append(set_action)
+
+                    if isinstance(device, DeviceUHFQA):
+                        # UHFQA does not yet support upload of ELF and waveforms in
+                        # a single transaction.
+                        ready_node = device.get_sequencer_paths(
+                            seqc_item.awg_index
+                        ).ready
+                        elf_upload_conditions[device.daq][ready_node] = 1
 
                 if isinstance(device, DeviceUHFQA):
-                    # UHFQA does not yet support upload of ELF and waveforms in
-                    # a single transaction.
-                    ready_node = device.get_sequencer_paths(item.awg_index)["ready"]
-                    elf_upload_conditions[device.daq][ready_node] = 1
-                    node_settings = wf_node_settings[device.daq]
+                    wf_dev_nodes = wf_node_settings[device.daq]
+                else:
+                    wf_dev_nodes = elf_node_settings[device.daq]
 
-                node_settings += device.prepare_upload_all_binary_waves(
-                    item.awg_index, item.waves, acquisition_type
-                )
+                if item.waves is not None:
+                    wf_dev_nodes += device.prepare_upload_all_binary_waves(
+                        seqc_item.awg_index, item.waves, acquisition_type
+                    )
 
                 if item.command_table is not None:
                     set_action = device.prepare_upload_command_table(
-                        item.awg_index, item.command_table
+                        seqc_item.awg_index, item.command_table
                     )
-                    node_settings.append(set_action)
+                    wf_dev_nodes.append(set_action)
 
         if len(elf_upload_conditions) > 0:
             for daq in elf_upload_conditions.keys():
                 daq.node_monitor.flush()
 
         _logger.debug("Started upload of AWG programs...")
         with tracing.get_tracer().start_span("upload-awg-programs") as _:
@@ -265,64 +282,69 @@
                         conditions=conditions,
                     )
                 timeout_s = 10
                 if not response_waiter.wait_all(timeout=timeout_s):
                     raise LabOneQControllerException(
                         f"AWGs not in ready state within timeout ({timeout_s} s)."
                     )
-
+            if len(wf_node_settings) > 0:
                 _logger.debug("Started upload of waveforms...")
                 with tracing.get_tracer().start_span("upload-waveforms") as _:
                     for daq, nodes in wf_node_settings.items():
                         daq.batch_set(nodes)
         _logger.debug("Finished upload.")
 
+    @classmethod
+    def _awg_compile(cls, awg_data: dict[DeviceZI, list[_SeqCCompileItem]]):
+        # Compile in parallel:
+        def worker(device: DeviceZI, item: _SeqCCompileItem, span: tracing.Span):
+            with tracing.get_tracer().start_span("compile-awg-thread", span) as _:
+                item.elf = device.compile_seqc(
+                    item.seqc_code, item.awg_index, item.seqc_filename
+                )
+
+        _logger.debug("Started compilation of AWG programs...")
+        with tracing.get_tracer().start_span("compile-awg-programs") as awg_span:
+            max_workers = os.environ.get("LABONEQ_AWG_COMPILER_MAX_WORKERS")
+            max_workers = int(max_workers) if max_workers is not None else None
+            with concurrent.futures.ThreadPoolExecutor(
+                max_workers=max_workers
+            ) as executor:
+                futures = [
+                    executor.submit(worker, device, item, awg_span)
+                    for device, items in awg_data.items()
+                    for item in items
+                ]
+                concurrent.futures.wait(futures)
+                exceptions = [
+                    future.exception()
+                    for future in futures
+                    if future.exception() is not None
+                ]
+                if len(exceptions) > 0:
+                    raise LabOneQControllerException(
+                        "Compilation failed. See log output for details."
+                    )
+        _logger.debug("Finished compilation.")
+
     def _set_nodes_after_awg_program_upload(self):
         nodes_to_initialize = []
         for initialization in self._recipe_data.initializations:
             device = self._devices.find_by_uid(initialization.device_uid)
             nodes_to_initialize.extend(
                 device.collect_awg_after_upload_nodes(initialization)
             )
 
         batch_set(nodes_to_initialize)
 
-    def _initialize_awgs(self):
+    def _initialize_awgs(self, nt_step: NtStepKey):
         self._set_nodes_before_awg_program_upload()
-        self._upload_awg_programs()
+        self._upload_awg_programs(nt_step=nt_step)
         self._set_nodes_after_awg_program_upload()
 
-    def _configure_leaders(self):
-        _logger.debug(
-            "Using %s as leaders.",
-            [d.dev_repr for _, d in self._devices.leaders],
-        )
-        for uid, device in self._devices.leaders:
-            init = self._recipe_data.get_initialization_by_device_uid(uid)
-            if init is None:
-                continue
-            device.configure_as_leader(init)
-
-    def _configure_followers(self):
-        _logger.debug(
-            "Using %s as followers.",
-            [d.dev_repr for _, d in self._devices.followers],
-        )
-        nodes_to_configure_followers = []
-
-        for uid, device in self._devices.followers:
-            init = self._recipe_data.get_initialization_by_device_uid(uid)
-            if init is None:
-                continue
-            nodes_to_configure_followers.extend(
-                device.collect_follower_configuration_nodes(init)
-            )
-
-        batch_set(nodes_to_configure_followers)
-
     def _configure_triggers(self):
         nodes_to_configure_triggers = []
 
         for uid, device in itertools.chain(
             self._devices.leaders, self._devices.followers
         ):
             init = self._recipe_data.get_initialization_by_device_uid(uid)
@@ -334,19 +356,14 @@
 
         batch_set(nodes_to_configure_triggers)
 
     def _initialize_devices(self):
         self._reset_to_idle_state()
         self._allocate_resources()
         self._apply_recipe_initializations()
-        self._initialize_awgs()
-        self._configure_leaders()
-        self._configure_followers()
-        self._configure_triggers()
-        self._wait_for_conditions_to_start()
 
     def _execute_one_step_followers(self):
         _logger.debug("Settings nodes to start on followers")
 
         nodes_to_execute = []
         for _, device in self._devices.followers:
             nodes_to_execute.extend(device.collect_execution_nodes())
@@ -357,16 +374,16 @@
         for _, device in self._devices.followers:
             response_waiter.add(
                 target=device.daq.node_monitor,
                 conditions=device.conditions_for_execution_ready(),
             )
         if not response_waiter.wait_all(timeout=2):
             _logger.warning(
-                "Conditions to start RT on followers still not fulfilled after 2 seconds, "
-                "nonetheless trying to continue..."
+                "Conditions to start RT on followers still not fulfilled after 2"
+                " seconds, nonetheless trying to continue..."
             )
 
         # Standalone workaround: The device is triggering itself,
         # thus split the execution into AWG trigger arming and triggering
         nodes_to_execute = []
         for _, device in self._devices.followers:
             nodes_to_execute.extend(device.collect_start_execution_nodes())
@@ -398,16 +415,18 @@
         for _, device in self._devices.followers:
             response_waiter.add(
                 target=device.daq.node_monitor,
                 conditions=device.conditions_for_execution_done(acquisition_type),
             )
         if not response_waiter.wait_all(timeout=guarded_wait_time):
             _logger.warning(
-                "Stop conditions still not fulfilled after %f s, estimated execution time "
-                "was %.2f s. Continuing to the next step.",
+                (
+                    "Stop conditions still not fulfilled after %f s, estimated"
+                    " execution time was %.2f s. Continuing to the next step."
+                ),
                 guarded_wait_time,
                 min_wait_time,
             )
 
     def _execute_one_step(self, acquisition_type: AcquisitionType):
         _logger.debug("Step executing")
 
@@ -431,16 +450,16 @@
             or now - self._last_connect_check_ts > CONNECT_CHECK_HOLDOFF
         ):
             self._devices.connect()
         self._last_connect_check_ts = now
 
     def disable_outputs(
         self,
-        device_uids: List[str] = None,
-        logical_signals: List[str] = None,
+        device_uids: list[str] = None,
+        logical_signals: list[str] = None,
         unused_only: bool = False,
     ):
         self._devices.disable_outputs(device_uids, logical_signals, unused_only)
 
     def shut_down(self):
         _logger.info("Shutting down all devices...")
         self._devices.shut_down()
@@ -470,42 +489,37 @@
             self._initialize_devices()
 
             # Ensure no side effects from the previous execution in the same session
             self._current_waves = []
             self._nodes_from_user_functions = []
             _logger.info("Starting near-time execution...")
             with tracing.get_tracer().start_span("near-time-execution"):
-                Controller.NearTimeExecutor(controller=self).run(
-                    self._recipe_data.execution
-                )
+                NearTimeRunner(controller=self).run(self._recipe_data.execution)
             _logger.info("Finished near-time execution.")
             for _, device in self._devices.all:
                 device.check_errors()
         finally:
             self._devices.stop_monitor()
 
         if self._run_parameters.shut_down is True:
             self.shut_down()
 
         if self._run_parameters.disconnect is True:
             self.disconnect()
 
-    def _find_awg(self, seqc_name: str) -> Tuple[str, int]:
+    def _find_awg(self, seqc_name: str) -> tuple[str, int]:
         # TODO(2K): Do this in the recipe preprocessor, or even modify the compiled experiment
-        # data model
-        for init in self._recipe_data.initializations:
-            if init.awgs is None:
-                continue
-            for awg in init.awgs:
-                if awg.seqc == seqc_name:
-                    return init.device_uid, awg.awg
+        #  data model
+        for rt_exec_step in self._recipe_data.recipe.experiment.realtime_execution_init:
+            if rt_exec_step.seqc_ref == seqc_name:
+                return rt_exec_step.device_id, rt_exec_step.awg_id
         return None, None
 
     def replace_pulse(
-        self, pulse_uid: Union[str, Pulse], pulse_or_array: Union[npt.ArrayLike, Pulse]
+        self, pulse_uid: str | Pulse, pulse_or_array: npt.ArrayLike | Pulse
     ):
         """Replaces specific pulse with the new sample data on the device.
 
         This is useful when called from the user function, allows fast waveform replacement within
         near-time loop without experiment recompilation.
 
         Args:
@@ -515,22 +529,28 @@
         """
         if isinstance(pulse_uid, str):
             for waveform in self._recipe_data.compiled.pulse_map[
                 pulse_uid
             ].waveforms.values():
                 if any([instance.can_compress for instance in waveform.instances]):
                     _logger.error(
-                        "Pulse replacement on pulses that allow compression not allowed. Pulse %s",
+                        (
+                            "Pulse replacement on pulses that allow compression not"
+                            " allowed. Pulse %s"
+                        ),
                         pulse_uid,
                     )
                     return
 
         if hasattr(pulse_uid, "can_compress") and pulse_uid.can_compress:
             _logger.error(
-                "Pulse replacement on pulses that allow compression not allowed. Pulse %s",
+                (
+                    "Pulse replacement on pulses that allow compression not allowed."
+                    " Pulse %s"
+                ),
                 pulse_uid.uid,
             )
             return
 
         acquisition_type = RtExecutionInfo.get_acquisition_type(
             self._recipe_data.rt_execution_infos
         )
@@ -539,17 +559,17 @@
         )
         for repl in wave_replacements:
             awg_indices = next(
                 a
                 for a in self._recipe_data.compiled.wave_indices
                 if a["filename"] == repl.awg_id
             )
-            awg_wave_map: Dict[str, List[Union[int, str]]] = awg_indices["value"]
+            awg_wave_map: dict[str, list[int | str]] = awg_indices["value"]
             target_wave = awg_wave_map.get(repl.sig_string)
-            seqc_name = repl.awg_id[: -len("_waveindices.csv")] + ".seqc"
+            seqc_name = repl.awg_id
             awg = self._find_awg(seqc_name)
             device = self._devices.find_by_uid(awg[0])
 
             if repl.replacement_type == ReplacementType.I_Q:
                 clipped = np.clip(repl.samples, -1.0, 1.0)
                 bin_wave = zhinst.utils.convert_awg_waveform(*clipped)
                 self._nodes_from_user_functions.append(
@@ -600,128 +620,31 @@
                     effective_averages,
                     effective_averaging_mode,
                     rt_execution_info.acquisition_type,
                 )
             )
         return nodes_to_prepare_rt
 
-    class NearTimeExecutor(ExecutorBase):
-        def __init__(self, controller: Controller):
-            super().__init__(looping_mode=LoopingMode.EXECUTE)
-            self.controller = controller
-            self.user_set_nodes = []
-            self.nt_loop_indices: list[int] = []
-            self.sweep_params_tracker = SweepParamsTracker()
-
-        def set_handler(self, path: str, value):
-            dev = self.controller._devices.find_by_node_path(path)
-            self.user_set_nodes.append(
-                DaqNodeSetAction(
-                    dev._daq, path, value, caching_strategy=CachingStrategy.NO_CACHE
-                )
-            )
-
-        def user_func_handler(self, func_name: str, args: Dict[str, Any]):
-            func = self.controller._user_functions.get(func_name)
-            if func is None:
-                raise LabOneQControllerException(
-                    f"User function '{func_name}' is not registered."
-                )
-            res = func(ProtectedSession(self.controller._session), **args)
-            user_func_results = self.controller._results.user_func_results.setdefault(
-                func_name, []
-            )
-            user_func_results.append(res)
-
-        def set_sw_param_handler(
-            self,
-            name: str,
-            index: int,
-            value: float,
-            axis_name: str,
-            values: npt.ArrayLike,
-        ):
-            self.sweep_params_tracker.set_param(name, value)
-
-        def for_loop_handler(
-            self, count: int, index: int, loop_type: LoopType, enter: bool
-        ):
-            if enter:
-                self.nt_loop_indices.append(index)
-            else:
-                self.nt_loop_indices.pop()
-
-        def rt_handler(
-            self,
-            count: int,
-            uid: str,
-            averaging_mode: AveragingMode,
-            acquisition_type: AcquisitionType,
-            enter: bool,
-        ):
-            if enter:
-                attribute_value_tracker = (
-                    self.controller._recipe_data.attribute_value_tracker
-                )
-                for param in self.sweep_params_tracker.updated_params():
-                    attribute_value_tracker.update(
-                        param, self.sweep_params_tracker.get_param(param)
-                    )
-                self.sweep_params_tracker.clear_for_next_step()
-
-                nt_sweep_nodes: list[DaqNodeAction] = []
-                for device_uid, device in self.controller._devices.all:
-                    nt_sweep_nodes.extend(
-                        device.collect_prepare_nt_step_nodes(
-                            attribute_value_tracker.device_view(device_uid),
-                            self.controller._recipe_data,
-                        )
-                    )
-
-                step_prepare_nodes = self.controller._prepare_rt_execution(
-                    rt_section_uid=uid
-                )
-
-                batch_set([*self.user_set_nodes, *nt_sweep_nodes, *step_prepare_nodes])
-                self.user_set_nodes.clear()
-
-                for retry in range(3):  # Up to 3 retries
-                    if retry > 0:
-                        _logger.info("Step retry %s of 3...", retry + 1)
-                        batch_set(step_prepare_nodes)
-                    try:
-                        self.controller._execute_one_step(acquisition_type)
-                        self.controller._read_one_step_results(
-                            nt_loop_indices=self.nt_loop_indices, rt_section_uid=uid
-                        )
-                        break
-                    except LabOneQControllerException:  # TODO(2K): introduce "hard" controller exceptions
-                        self.controller._report_step_error(
-                            nt_loop_indices=self.nt_loop_indices,
-                            rt_section_uid=uid,
-                            message=traceback.format_exc(),
-                        )
-
     def _prepare_result_shapes(self):
         if self._results is None:
             self._results = make_empty_results()
         if len(self._recipe_data.rt_execution_infos) == 0:
             return
         if len(self._recipe_data.rt_execution_infos) > 1:
             raise LabOneQControllerException(
                 "Multiple 'acquire_loop_rt' sections per experiment is not supported."
             )
         rt_info = next(iter(self._recipe_data.rt_execution_infos.values()))
         for handle, shape_info in self._recipe_data.result_shapes.items():
             if rt_info.acquisition_type == AcquisitionType.RAW:
                 if len(self._recipe_data.result_shapes) > 1:
                     raise LabOneQControllerException(
-                        f"Multiple raw acquire events with handles "
+                        "Multiple raw acquire events with handles "
                         f"{list(self._recipe_data.result_shapes.keys())}. "
-                        f"Only single raw acquire per experiment allowed."
+                        "Only single raw acquire per experiment allowed."
                     )
                 signal_id = rt_info.signal_by_handle(handle)
                 awg_config = self._recipe_data.awg_config_by_acquire_signal(signal_id)
                 # Use default length 4096, in case AWG config is not available
                 raw_acquire_length = (
                     4096 if awg_config is None else awg_config.raw_acquire_length
                 )
@@ -751,15 +674,15 @@
             )
             if len(shape) == 0:
                 empty_res.data = np.nan
             else:
                 empty_res.data[:] = np.nan
             self._results.acquired_results[handle] = empty_res
 
-    def _read_one_step_results(self, nt_loop_indices: List[int], rt_section_uid: str):
+    def _read_one_step_results(self, nt_step: NtStepKey, rt_section_uid: str):
         if rt_section_uid is None:
             return  # Old recipe-based execution - skip partial result processing
         rt_execution_info = self._recipe_data.rt_execution_infos[rt_section_uid]
         for awg_key, awg_config in self._recipe_data.awgs_producing_results():
             device = self._devices.find_by_uid(awg_key.device_uid)
             if rt_execution_info.acquisition_type == AcquisitionType.RAW:
                 raw_results = device.get_input_monitor_data(
@@ -803,16 +726,14 @@
                     mapping = rt_execution_info.signal_result_map.get(signal, [])
                     unique_handles = set(mapping)
                     for handle in unique_handles:
                         if handle is None:
                             continue  # unused entries in sparse result vector map to None handle
                         result = self._results.acquired_results[handle]
                         build_partial_result(
-                            result, nt_loop_indices, raw_results, mapping, handle
+                            result, nt_step, raw_results, mapping, handle
                         )
 
-    def _report_step_error(
-        self, nt_loop_indices: List[int], rt_section_uid: str, message: str
-    ):
+    def _report_step_error(self, nt_step: NtStepKey, rt_section_uid: str, message: str):
         self._results.execution_errors.append(
-            (deepcopy(nt_loop_indices), rt_section_uid, message)
+            (list(nt_step.indices), rt_section_uid, message)
         )
```

## laboneq/controller/recipe_1_4_0.py

```diff
@@ -1,23 +1,18 @@
 # Copyright 2019 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
+from __future__ import annotations
+
 from dataclasses import dataclass, field
-from typing import Any, AnyStr, Dict, List, Optional
+from typing import Any
 
 from marshmallow import EXCLUDE, Schema, fields, post_load
 
-from .recipe_enums import (
-    DIOConfigType,
-    ExecutionType,
-    OperationType,
-    RefClkType,
-    ReferenceClockSource,
-    SignalType,
-)
+from .recipe_enums import NtStepKey, RefClkType, SignalType, TriggeringMode
 from .util import LabOneQControllerException
 
 
 class QCCSSchema(Schema):
     @post_load
     def from_json(self, data, **kwargs):
         return self.Data(**data)
@@ -26,16 +21,16 @@
 class Server(QCCSSchema):
     class Meta:
         fields = ("server_uid", "host", "port", "api_level")
         ordered = True
 
     @dataclass
     class Data:
-        server_uid: AnyStr
-        host: AnyStr
+        server_uid: str
+        host: str
         port: int
         api_level: int
 
     server_uid = fields.Str()
     host = fields.Str()
     port = fields.Integer()
     api_level = fields.Integer()
@@ -44,32 +39,32 @@
 class DriverOption(fields.Field):
     class Meta:
         fields = ("parameter_name", "value")
         ordered = False
 
     @dataclass
     class Data:
-        key: AnyStr
-        value: AnyStr
+        key: str
+        value: str
 
     key = fields.Str(required=True)
     value = fields.Str(required=True)
 
 
 class Device(QCCSSchema):
     class Meta:
         fields = ("device_uid", "driver", "options")
         ordered = True
         unknown = EXCLUDE
 
     @dataclass
     class Data:
-        device_uid: AnyStr
-        driver: AnyStr
-        options: Optional[List[DriverOption]] = None
+        device_uid: str
+        driver: str
+        options: list[DriverOption] | None = None
 
         def _get_option(self, key):
             for option in self.options:
                 if key == option["parameter_name"]:
                     return option["value"]
             return None
 
@@ -129,30 +124,30 @@
             "amplitude",
         )
         ordered = True
 
     @dataclass
     class Data:
         channel: int
-        enable: Optional[bool] = None
-        modulation: Optional[bool] = None
-        oscillator: Optional[int] = None
-        oscillator_frequency: Optional[int] = None
-        offset: Optional[float] = None
-        gains: Optional[Gains] = None
-        range: Optional[float] = None
-        range_unit: Optional[str] = None
-        precompensation: Optional[Dict[str, Dict]] = None
-        lo_frequency: Optional[Any] = None
-        port_mode: Optional[str] = None
-        port_delay: Optional[Any] = None
+        enable: bool | None = None
+        modulation: bool | None = None
+        oscillator: int | None = None
+        oscillator_frequency: int | None = None
+        offset: float | None = None
+        gains: Gains | None = None
+        range: float | None = None
+        range_unit: str | None = None
+        precompensation: dict[str, dict] | None = None
+        lo_frequency: Any | None = None
+        port_mode: str | None = None
+        port_delay: Any | None = None
         scheduler_port_delay: float = 0.0
-        delay_signal: Optional[float] = None
-        marker_mode: Optional[str] = None
-        amplitude: Optional[Any] = None
+        delay_signal: float | None = None
+        marker_mode: str | None = None
+        amplitude: Any | None = None
 
     channel = fields.Integer()
     enable = fields.Boolean(required=False)
     modulation = fields.Boolean(required=False)
     oscillator = fields.Integer(required=False)
     oscillator_frequency = fields.Integer(required=False)
     offset = fields.Float(required=False)
@@ -177,33 +172,30 @@
         return SignalType[value.upper()]
 
 
 class AWG(QCCSSchema):
     class Meta:
         fields = (
             "awg",
-            "seqc",
             "signal_type",
             "qa_signal_id",
             "command_table_match_offset",
             "feedback_register",
         )
         ordered = False
 
     @dataclass
     class Data:
         awg: int
-        seqc: str
         signal_type: SignalType = SignalType.SINGLE
-        qa_signal_id: Optional[str] = None
-        command_table_match_offset: Optional[int] = None
-        feedback_register: Optional[int] = None
+        qa_signal_id: str | None = None
+        command_table_match_offset: int | None = None
+        feedback_register: int | None = None
 
     awg = fields.Integer()
-    seqc = fields.Str()
     signal_type = SignalTypeField()
     qa_signal_id = fields.Str(required=False, allow_none=True)
     command_table_match_offset = fields.Integer(required=False, allow_none=True)
     feedback_register = fields.Integer(required=False, allow_none=True)
 
 
 class Port(QCCSSchema):
@@ -216,123 +208,14 @@
         port: int
         device_uid: str
 
     port = fields.Integer()
     device_uid = fields.Str()
 
 
-class ExecutionTypeField(fields.Field):
-    def _serialize(self, value, attr, obj, **kwargs):
-        return value.name
-
-    def _deserialize(self, value, attr, data, **kwargs):
-        return ExecutionType[value.upper()]
-
-
-class listElement(QCCSSchema):
-    class Meta:
-        # TODO(MG) data_type is deprecated and should be removed
-        fields = ("source", "data_type")
-        ordered = True
-
-    @dataclass
-    class Data:
-        source: AnyStr
-        # TODO(MG) data_type is deprecated and should be removed
-        data_type: AnyStr
-
-    source = fields.Str()
-    # TODO(MG) data_type is deprecated and should be removed
-    data_type = fields.Str()
-
-
-class Location(QCCSSchema):
-    @dataclass
-    class Data:
-        type: AnyStr
-        index: int
-
-    type = fields.Str()
-    index = fields.Integer()
-
-
-class Parameter(QCCSSchema):
-    class Meta:
-        fields = (
-            "device_uid",
-            "location",
-            "parameter_uid",
-            "index",
-            "list",
-            "start",
-            "step",
-        )
-        ordered = True
-
-    @dataclass
-    class Data:
-        device_uid: AnyStr = None
-        location: Optional[Location] = None
-        parameter_uid: Optional[AnyStr] = None
-        index: Optional[int] = None
-        list: Optional[listElement] = None
-        start: Optional[float] = None
-        step: Optional[float] = None
-
-    device_uid = fields.Str()
-    location = fields.Nested(Location)
-    parameter_uid = fields.Str(required=False)
-    index = fields.Integer(required=False)
-    list = fields.Nested(listElement, required=False)
-    start = fields.Float(required=False)
-    step: fields.Float(required=False)
-
-
-class OperationTypeField(fields.Field):
-    def _serialize(self, value, attr, obj, **kwargs):
-        return value.name
-
-    def _deserialize(self, value, attr, data, **kwargs):
-        return OperationType[value.upper()]
-
-
-class SectionOperation(QCCSSchema):
-    class Meta:
-        fields = ("op_type", "operation", "args")
-        ordered = True
-
-    @dataclass
-    class Data:
-        op_type: OperationType = None
-        operation: str = None
-        args: Dict[str, Any] = None
-
-    op_type = OperationTypeField(required=True)
-    operation = fields.Str(required=True)
-    args = fields.Dict(required=False, allow_none=True)
-
-
-class Execution(QCCSSchema):
-    class Meta:
-        fields = ("type", "count", "parameters", "children")
-        ordered = True
-
-    @dataclass
-    class Data:
-        type: ExecutionType
-        count: int = None
-        parameters: List[Parameter.Data] = None
-        children: List[Any] = None
-
-    type = ExecutionTypeField(required=False)
-    count = fields.Integer(required=False)
-    parameters = fields.List(fields.Nested(Parameter), required=False)
-    children = fields.List(fields.Nested(lambda: Execution()), required=False)
-
-
 class Measurement(QCCSSchema):
     class Meta:
         fields = ("length", "channel")
 
     @dataclass
     class Data:
         length: int
@@ -353,100 +236,78 @@
             return RefClkType._100MHZ.value
         else:
             raise LabOneQControllerException(
                 f"UNsupported reference clock value {value}"
             )
 
 
-class DIOConfigTypeField(fields.Field):
-    def _serialize(self, value, attr, obj, **kwargs):
-        return value.name
-
-    def _deserialize(self, value, attr, data, **kwargs):
-        return DIOConfigType[value.upper()]
-
-
-class ReferenceClockSourceField(fields.Field):
-    def __init__(self, *args, **kwargs) -> None:
-        kwargs["allow_none"] = True
-        super().__init__(*args, **kwargs)
-
+class TriggeringModeField(fields.Field):
     def _serialize(self, value, attr, obj, **kwargs):
-        if value is None:
-            return None
         return value.name
 
     def _deserialize(self, value, attr, data, **kwargs):
-        if value is None:
-            return None
-        return ReferenceClockSource[value.upper()]
+        return TriggeringMode[value.upper()]
 
 
 class Config(QCCSSchema):
     class Meta:
         fields = (
             "repetitions",
             "reference_clock",
             "holdoff",
-            "dio_mode",
+            "triggering_mode",
             "sampling_rate",
-            "reference_clock_source",
         )
         ordered = True
 
     @dataclass
     class Data:
         repetitions: int = 1
         reference_clock: RefClkType = None
         holdoff: float = 0
-        dio_mode: DIOConfigType = DIOConfigType.HDAWG
-        sampling_rate: Optional[float] = None
-        reference_clock_source: Optional[ReferenceClockSource] = None
+        triggering_mode: TriggeringMode = TriggeringMode.DIO_FOLLOWER
+        sampling_rate: float | None = None
 
     repetitions = fields.Int()
     reference_clock = RefClkTypeField()
     holdoff = fields.Float()
-    dio_mode = DIOConfigTypeField()
+    triggering_mode = TriggeringModeField()
     sampling_rate = fields.Float()
-    reference_clock_source = ReferenceClockSourceField()
 
 
 class Initialization(QCCSSchema):
     class Meta:
         fields = (
             "device_uid",
             "config",
             "awgs",
-            "ports",
             "outputs",
             "inputs",
             "measurements",
             "ppchannels",
         )
         ordered = True
 
     @dataclass
     class Data:
-        device_uid: AnyStr
+        device_uid: str
         config: Config.Data
-        awgs: List[AWG.Data] = None
-        ports: List[Port.Data] = None
-        outputs: List[IO.Data] = None
-        inputs: List[IO.Data] = None
-        measurements: List[Measurement.Data] = field(default_factory=list)
-        ppchannels: Dict[int, Any] = None
+        awgs: list[AWG.Data] = None
+        outputs: list[IO.Data] = None
+        inputs: list[IO.Data] = None
+        measurements: list[Measurement.Data] = field(default_factory=list)
+        ppchannels: list[dict[str, Any]] | None = None
 
     device_uid = fields.Str()
     config = fields.Nested(Config)
     awgs = fields.List(fields.Nested(AWG), required=False)
-    ports = fields.List(fields.Nested(Port), required=False)
     outputs = fields.List(fields.Nested(IO), required=False)
     inputs = fields.List(fields.Nested(IO), required=False)
     measurements = fields.List(fields.Nested(Measurement), required=False)
-    ppchannels = fields.Dict(required=False, allow_none=True)
+    ppchannels = fields.List(fields.Raw, required=False, allow_none=True)
 
 
 class OscillatorParam(QCCSSchema):
     class Meta:
         fields = ("id", "device_id", "channel", "frequency", "param")
         ordered = True
 
@@ -471,15 +332,15 @@
         ordered = True
 
     @dataclass
     class Data:
         signal_id: str
         device_id: str
         awg: int
-        channels: List[int]
+        channels: list[int]
         weights: str = None
         threshold: float = 0.0
 
     signal_id = fields.Str()
     device_id = fields.Str()
     awg = fields.Int()
     channels = fields.List(fields.Int())
@@ -499,38 +360,72 @@
         acquire_length: int
 
     section_id = fields.Str()
     signal_id = fields.Str()
     acquire_length = fields.Int()
 
 
+class NtStepKeyField(fields.Field):
+    def _deserialize(self, value, attr, data, **kwargs):
+        return NtStepKey(indices=tuple(value["indices"]))
+
+
+class RealtimeExecutionInit(QCCSSchema):
+    class Meta:
+        fields = (
+            "device_id",
+            "awg_id",
+            "seqc_ref",
+            "wave_indices_ref",
+            "nt_step",
+        )
+        ordered = True
+
+    @dataclass
+    class Data:
+        device_id: str
+        awg_id: int
+        seqc_ref: str
+        wave_indices_ref: str
+        nt_step: NtStepKey
+
+    device_id = fields.Str()
+    awg_id = fields.Int()
+    seqc_ref = fields.Str()
+    wave_indices_ref = fields.Str()
+    nt_step = NtStepKeyField()
+
+
 class Experiment(QCCSSchema):
     class Meta:
         fields = (
             "initializations",
+            "realtime_execution_init",
             "oscillator_params",
             "integrator_allocations",
             "acquire_lengths",
             "simultaneous_acquires",
             "total_execution_time",
         )
         ordered = True
 
     @dataclass
     class Data:
-        initializations: List[Initialization.Data]
-        oscillator_params: List[OscillatorParam.Data] = field(default_factory=list)
-        integrator_allocations: List[IntegratorAllocation.Data] = field(
+        initializations: list[Initialization.Data]
+        realtime_execution_init: list[RealtimeExecutionInit.Data]
+        oscillator_params: list[OscillatorParam.Data] = field(default_factory=list)
+        integrator_allocations: list[IntegratorAllocation.Data] = field(
             default_factory=list
         )
-        acquire_lengths: List[AcquireLength.Data] = field(default_factory=list)
-        simultaneous_acquires: List[Dict[str, str]] = field(default_factory=list)
+        acquire_lengths: list[AcquireLength.Data] = field(default_factory=list)
+        simultaneous_acquires: list[dict[str, str]] = field(default_factory=list)
         total_execution_time: float = None
 
     initializations = fields.List(fields.Nested(Initialization))
+    realtime_execution_init = fields.List(fields.Nested(RealtimeExecutionInit))
     oscillator_params = fields.List(fields.Nested(OscillatorParam), required=False)
     integrator_allocations = fields.List(
         fields.Nested(IntegratorAllocation), required=False
     )
     acquire_lengths = fields.List(fields.Nested(AcquireLength), required=False)
     simultaneous_acquires = fields.List(
         fields.Dict(fields.Str(), fields.Str()), required=False, allow_none=True
@@ -542,16 +437,16 @@
     class Meta:
         unknown = EXCLUDE
         fields = ("line_endings", "experiment", "servers", "devices")
         ordered = False
 
     @dataclass
     class Data:
-        line_endings: AnyStr
+        line_endings: str
         experiment: Experiment.Data
-        servers: Optional[List[Server.Data]] = None
-        devices: Optional[List[Device.Data]] = None
+        servers: list[Server.Data] | None = None
+        devices: list[Device.Data] | None = None
 
     line_endings = fields.Str()
     experiment = fields.Nested(Experiment)
     servers = fields.List(fields.Nested(Server), required=False)
     devices = fields.List(fields.Nested(Device), required=False)
```

## laboneq/controller/recipe_enums.py

```diff
@@ -1,39 +1,30 @@
 # Copyright 2019 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
+from dataclasses import dataclass
 from enum import Enum
 
 
 class SignalType(Enum):
     IQ = "iq"
     SINGLE = "single"
     INTEGRATION = "integration"
     MARKER = "marker"
 
 
-class ExecutionType(Enum):
-    SINGLE = 1
-    SWEEP = 2
-
-
 class RefClkType(Enum):
     _10MHZ = 10
     _100MHZ = 100
 
 
-class DIOConfigType(Enum):
-    ZSYNC_DIO = 1
-    HDAWG = 2
-    HDAWG_LEADER = 3
-    DIO_FOLLOWER_OF_HDAWG_LEADER = 4
-
-
-class OperationType(Enum):
-    ACQUIRE = "acquire"
-    USER_FUNC = "user_func"
-    SET = "set"
-
-
-class ReferenceClockSource(Enum):
-    INTERNAL = "internal"
-    EXTERNAL = "external"
+class TriggeringMode(Enum):
+    ZSYNC_FOLLOWER = 1
+    DIO_FOLLOWER = 2
+    DESKTOP_LEADER = 3
+    DESKTOP_DIO_FOLLOWER = 4
+    INTERNAL_FOLLOWER = 5
+
+
+@dataclass(frozen=True)
+class NtStepKey:
+    indices: tuple[int]
```

## laboneq/controller/recipe_processor.py

```diff
@@ -54,24 +54,24 @@
     device_uid: str
     awg_index: int
 
 
 @dataclass
 class AwgConfig:
     # QA
-    raw_acquire_length: int = None
-    result_length: int = None
+    raw_acquire_length: int | None = None
+    result_length: int | None = None
     acquire_signals: Set[str] = field(default_factory=set)
-    target_feedback_register: int = None
+    target_feedback_register: int | None = None
     # SG
-    qa_signal_id: str = None
-    command_table_match_offset: int = None
-    source_feedback_register: int = None
-    zsync_bit: int = None
-    feedback_register_bit: int = None
+    qa_signal_id: str | None = None
+    command_table_match_offset: int | None = None
+    source_feedback_register: int | None = None
+    zsync_bit: int | None = None
+    feedback_register_bit: int | None = None
 
 
 AwgConfigs = Dict[AwgKey, AwgConfig]
 
 
 @dataclass
 class DeviceRecipeData:
@@ -519,15 +519,20 @@
 
     device_settings: DeviceSettings = defaultdict(DeviceRecipeData)
     for initialization in recipe.experiment.initializations:
         device_settings[initialization.device_uid] = DeviceRecipeData(
             iq_settings=_pre_process_iq_settings_hdawg(initialization)
         )
 
-    execution = ExecutionFactoryFromExperiment().make(compiled_experiment.experiment)
+    if hasattr(compiled_experiment, "execution"):
+        execution = compiled_experiment.execution
+    else:
+        execution = ExecutionFactoryFromExperiment().make(
+            compiled_experiment.experiment
+        )
     result_shapes, rt_execution_infos = _calculate_result_shapes(execution)
     awg_configs = _calculate_awg_configs(rt_execution_infos, recipe.experiment)
     attribute_value_tracker, oscillator_ids = _pre_process_attributes(
         recipe.experiment, devices
     )
 
     recipe_data = RecipeData(
```

## laboneq/controller/results.py

```diff
@@ -1,59 +1,60 @@
 # Copyright 2019 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
-from copy import deepcopy
-from typing import TYPE_CHECKING, Any, List, Union
+from typing import TYPE_CHECKING, Any
 
 import numpy as np
 from numpy.typing import ArrayLike
 
+from laboneq.controller.recipe_enums import NtStepKey
+
 if TYPE_CHECKING:
     from laboneq.dsl.result.acquired_result import AcquiredResult
     from laboneq.dsl.result.results import Results
 
 
 def make_empty_results() -> Results:
     from laboneq.dsl.result.results import Results
 
     return Results(acquired_results={}, user_func_results={}, execution_errors=[])
 
 
 def make_acquired_result(
     data: ArrayLike,
-    axis_name: List[Union[str, List[str]]],
-    axis: List[Union[ArrayLike, List[ArrayLike]]],
+    axis_name: list[str | list[str]],
+    axis: list[ArrayLike | list[ArrayLike]],
 ) -> AcquiredResult:
     from laboneq.dsl.result.acquired_result import AcquiredResult
 
     return AcquiredResult(data, axis_name, axis)
 
 
 def build_partial_result(
     result: AcquiredResult,
-    nt_loop_indices: List[int],
+    nt_step: NtStepKey,
     raw_result: Any,
-    mapping: List[str],
+    mapping: list[str],
     handle: str,
 ):
-    result.last_nt_step = deepcopy(nt_loop_indices)
-    if len(np.shape(result.data)) == len(nt_loop_indices):
+    result.last_nt_step = list(nt_step.indices)
+    if len(np.shape(result.data)) == len(nt_step.indices):
         # No loops in RT, just a single value produced
         for raw_result_idx in range(len(raw_result)):
             if mapping[raw_result_idx % len(mapping)] == handle:
-                if len(nt_loop_indices) == 0:
+                if len(nt_step.indices) == 0:
                     result.data = raw_result[raw_result_idx]
                 else:
-                    result.data[tuple(nt_loop_indices)] = raw_result[raw_result_idx]
+                    result.data[nt_step.indices] = raw_result[raw_result_idx]
                 break
     else:
         inner_res = result.data
-        for index in nt_loop_indices:
+        for index in nt_step.indices:
             inner_res = inner_res[index]
         res_flat = np.ravel(inner_res)
         res_flat_idx = 0
         for raw_result_idx in range(len(raw_result)):
             if mapping[raw_result_idx % len(mapping)] == handle:
                 res_flat[res_flat_idx] = raw_result[raw_result_idx]
                 res_flat_idx += 1
```

## laboneq/controller/devices/device_collection.py

```diff
@@ -82,15 +82,15 @@
         if device is None:
             raise LabOneQControllerException(
                 f"Could not find device object for the device uid '{device_uid}'"
             )
         return device
 
     def find_by_node_path(self, path: str) -> DeviceZI:
-        m = re.match(r"^/?(DEV\d+)/.+", path.upper())
+        m = re.match(r"^/?(DEV[^/]+)/.+", path.upper())
         if m is None:
             raise LabOneQControllerException(
                 f"Path '{path}' is not referring to any device"
             )
         serial = m.group(1).lower()
         for dev in self._devices.values():
             if dev.serial == serial:
@@ -345,22 +345,26 @@
                     if to_dev is None:
                         raise LabOneQControllerException(
                             f"Could not find destination device '{connection.remote_path}' for "
                             f"the port '{connection.local_port}' connection of the "
                             f"device '{instrument.uid}'"
                         )
                     to_port = f"{connection.signal_type.name}/{connection.remote_port}"
-                    from_dev.add_downlink(from_port, to_dev_uid, to_dev)
+                    if not to_dev.is_secondary:
+                        from_dev.add_downlink(from_port, to_dev_uid, to_dev)
                     to_dev.add_uplink(to_port, from_dev)
 
         # Move various device settings from device setup
         for instrument in self._ds.instruments:
             dev = self._devices[instrument.uid]
 
-            # Set clock source (external by default)
+            # Set the clock source (external by default)
+            # TODO(2K): Simplify the logic in this code snippet and the one in 'update_clock_source'.
+            # Currently, it adheres to the previously existing logic in the compiler, but it appears
+            # unnecessarily convoluted.
             force_internal: bool | None = None
             if instrument.reference_clock_source is not None:
                 force_internal = (
                     instrument.reference_clock_source == ReferenceClockSource.INTERNAL
                 )
             dev.update_clock_source(force_internal)
```

## laboneq/controller/devices/device_hdawg.py

```diff
@@ -24,15 +24,15 @@
     Condition,
     FloatWithTolerance,
     NodeControlBase,
     Prepare,
     Response,
 )
 from laboneq.controller.recipe_1_4_0 import Initialization
-from laboneq.controller.recipe_enums import DIOConfigType, SignalType
+from laboneq.controller.recipe_enums import SignalType, TriggeringMode
 from laboneq.controller.recipe_processor import DeviceRecipeData, RecipeData
 from laboneq.controller.util import LabOneQControllerException
 from laboneq.core.types.enums.acquisition_type import AcquisitionType
 
 _logger = logging.getLogger(__name__)
 
 DIG_TRIGGER_1_LEVEL = 0.225
@@ -441,19 +441,14 @@
                     path=f"/{self.serial}/sigouts/{ch}/delay",
                     value=output_delay_rounded,
                 )
             )
 
         return nodes_to_set
 
-    def wait_for_conditions_to_start(self):
-        self._wait_for_node(
-            f"/{self.serial}/system/clocks/sampleclock/status", 0, timeout=5
-        )
-
     def collect_awg_before_upload_nodes(
         self, initialization: Initialization.Data, recipe_data: RecipeData
     ):
         device_specific_initialization_nodes = [
             DaqNodeSetAction(
                 self._daq, f"/{self.serial}/system/awg/oscillatorcontrol", 1
             ),
@@ -473,16 +468,16 @@
 
     def collect_trigger_configuration_nodes(
         self, initialization: Initialization.Data, recipe_data: RecipeData
     ) -> list[DaqNodeAction]:
         _logger.debug("%s: Configuring trigger configuration nodes.", self.dev_repr)
         nodes_to_configure_triggers = []
 
-        dio_mode = initialization.config.dio_mode
-        if dio_mode == DIOConfigType.ZSYNC_DIO:
+        triggering_mode = initialization.config.triggering_mode
+        if triggering_mode == TriggeringMode.ZSYNC_FOLLOWER:
             _logger.debug(
                 "%s: Configuring DIO mode: ZSync pass-through.", self.dev_repr
             )
             _logger.debug("%s: Configuring external clock to ZSync.", self.dev_repr)
             nodes_to_configure_triggers.append(
                 DaqNodeSetAction(self._daq, f"/{self.serial}/dios/0/mode", 3)
             )
@@ -534,15 +529,15 @@
                             DaqNodeSetAction(
                                 self._daq,
                                 f"{awg_path}/zsync/register/offset",
                                 awg_config.command_table_match_offset,
                             ),
                         ]
                     )
-        elif dio_mode == DIOConfigType.HDAWG_LEADER:
+        elif triggering_mode == TriggeringMode.DESKTOP_LEADER:
 
             nodes_to_configure_triggers.append(
                 DaqNodeSetAction(
                     self._daq,
                     f"/{self.serial}/triggers/in/0/level",
                     DIG_TRIGGER_1_LEVEL,
                 )
```

## laboneq/controller/devices/device_pqsc.py

```diff
@@ -1,13 +1,14 @@
 # Copyright 2019 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import logging
+from enum import IntEnum
 from typing import Any
 
 from laboneq.controller.communication import (
     CachingStrategy,
     DaqNodeAction,
     DaqNodeSetAction,
 )
@@ -16,21 +17,22 @@
     Command,
     Condition,
     NodeControlBase,
     Response,
 )
 from laboneq.controller.recipe_1_4_0 import Initialization
 from laboneq.controller.recipe_processor import DeviceRecipeData, RecipeData
-from laboneq.controller.util import LabOneQControllerException
 from laboneq.core.types.enums.acquisition_type import AcquisitionType
 
 _logger = logging.getLogger(__name__)
 
-REFERENCE_CLOCK_SOURCE_INTERNAL = 0
-REFERENCE_CLOCK_SOURCE_EXTERNAL = 1
+
+class ReferenceClockSourcePQSC(IntEnum):
+    INTERNAL = 0
+    EXTERNAL = 1
 
 
 class DevicePQSC(DeviceZI):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.dev_type = "PQSC"
         self.dev_opts = []
@@ -42,17 +44,17 @@
         return nodes
 
     def update_clock_source(self, force_internal: bool | None):
         self._use_internal_clock = force_internal is True
 
     def clock_source_control_nodes(self) -> list[NodeControlBase]:
         source = (
-            REFERENCE_CLOCK_SOURCE_INTERNAL
+            ReferenceClockSourcePQSC.INTERNAL
             if self._use_internal_clock
-            else REFERENCE_CLOCK_SOURCE_EXTERNAL
+            else ReferenceClockSourcePQSC.EXTERNAL
         )
         expected_freq = None if self._use_internal_clock else 10e6
         return [
             Condition(
                 f"/{self.serial}/system/clocks/referenceclock/in/freq", expected_freq
             ),
             Command(f"/{self.serial}/system/clocks/referenceclock/in/source", source),
@@ -134,14 +136,43 @@
         self, acquisition_type: AcquisitionType
     ) -> dict[str, Any]:
         return {f"/{self.serial}/execution/enable": 0}
 
     def collect_trigger_configuration_nodes(
         self, initialization: Initialization.Data, recipe_data: RecipeData
     ) -> list[DaqNodeAction]:
+        # TODO(2K): This was moved as is from no more existing "configure_as_leader".
+        # Verify, if separate `batch_set` per node is truly necessary here, or the corresponding
+        # nodes can be set in one batch with others.
+        _logger.debug(
+            "%s: Setting reference clock frequency to %d MHz...",
+            self.dev_repr,
+            initialization.config.reference_clock,
+        )
+
+        self._daq.batch_set(
+            [
+                DaqNodeSetAction(
+                    self._daq,
+                    f"/{self.serial}/system/clocks/referenceclock/out/enable",
+                    1,
+                )
+            ]
+        )
+
+        self._daq.batch_set(
+            [
+                DaqNodeSetAction(
+                    self._daq,
+                    f"/{self.serial}/system/clocks/referenceclock/out/freq",
+                    initialization.config.reference_clock,
+                )
+            ]
+        )
+
         # Ensure ZSync links are established
         # TODO(2K): This is rather a hotfix, waiting to be done in parallel for all devices with
         # subscription / poll
         # TODO(2K): Verify also the downlink device serial (.../connection/serial) matches
         for port in self._downlinks:
             self._wait_for_node(
                 f"/{self.serial}/{port.lower()}/connection/status", 2, timeout=10
@@ -178,42 +209,7 @@
                 self._daq,
                 f"/{self.serial}/execution/repetitions",
                 initialization.config.repetitions,
             )
         )
 
         return nodes_to_configure_triggers
-
-    def collect_follower_configuration_nodes(
-        self, initialization: Initialization.Data
-    ) -> list[DaqNodeAction]:
-        raise LabOneQControllerException("PQSC cannot be configured as follower")
-
-    def configure_as_leader(self, initialization: Initialization.Data):
-        _logger.debug("%s: Configuring as leader...", self.dev_repr)
-        _logger.debug("%s: Enabling reference clock...", self.dev_repr)
-
-        _logger.debug(
-            "%s: Setting reference clock frequency to %d MHz...",
-            self.dev_repr,
-            initialization.config.reference_clock,
-        )
-
-        self._daq.batch_set(
-            [
-                DaqNodeSetAction(
-                    self._daq,
-                    f"/{self.serial}/system/clocks/referenceclock/out/enable",
-                    1,
-                )
-            ]
-        )
-
-        self._daq.batch_set(
-            [
-                DaqNodeSetAction(
-                    self._daq,
-                    f"/{self.serial}/system/clocks/referenceclock/out/freq",
-                    initialization.config.reference_clock,
-                )
-            ]
-        )
```

## laboneq/controller/devices/device_setup_dao.py

```diff
@@ -33,14 +33,23 @@
         self._device_setup = device_setup
 
     @property
     def instruments(self) -> Iterator[ZIStandardInstrument]:
         for instrument in self._device_setup.instruments:
             if isinstance(instrument, ZIStandardInstrument):
                 yield instrument
+            if hasattr(instrument, "device_type"):
+                if instrument.device_type.name in {
+                    "HDAWG",
+                    "UHFQA",
+                    "SHFQA",
+                    "SHFQC",
+                    "SHFSG",
+                }:
+                    yield instrument
 
     @property
     def servers(self) -> Iterator[tuple[str, DataServer]]:
         return self._device_setup.servers.items()
 
     @cached_property
     def has_shf(self):
```

## laboneq/controller/devices/device_shfppc.py

```diff
@@ -48,16 +48,17 @@
         self._use_internal_clock = force_internal is True
 
     def pre_process_attributes(
         self,
         initialization: Initialization.Data,
     ) -> Iterator[DeviceAttribute]:
         yield from super().pre_process_attributes(initialization)
-        ppchannels = initialization.ppchannels or {}
-        for channel, settings in ppchannels.items():
+        ppchannels = initialization.ppchannels or []
+        for settings in ppchannels:
+            channel = settings["channel"]
             for key, attribute_name in DeviceSHFPPC.attribute_keys.items():
                 if key in settings:
                     yield DeviceAttribute(
                         name=attribute_name, index=channel, value_or_param=settings[key]
                     )
 
     def check_errors(self):
@@ -66,27 +67,28 @@
     def collect_reset_nodes(self) -> list[DaqNodeAction]:
         return []
 
     def collect_initialization_nodes(
         self, device_recipe_data: DeviceRecipeData, initialization: Initialization.Data
     ) -> list[DaqNodeAction]:
         nodes_to_set: list[DaqNodeAction] = []
-        ppchannels = initialization.ppchannels or {}
+        ppchannels = initialization.ppchannels or []
 
         def _convert(value):
             if isinstance(value, bool):
                 return 1 if value else 0
             return value
 
-        for ch, settings in ppchannels.items():
+        for settings in ppchannels:
+            ch = settings["channel"]
             nodes_to_set.append(
                 DaqNodeSetAction(self._daq, self._key_to_path("_on", ch), 1)
             )
             for key, value in settings.items():
-                if value is None or key in DeviceSHFPPC.attribute_keys:
+                if value is None or key in [*DeviceSHFPPC.attribute_keys, "channel"]:
                     # Skip not set values, or values that are bound to sweep params and will
                     # be set during the NT execution.
                     continue
                 nodes_to_set.append(
                     DaqNodeSetAction(
                         self._daq, self._key_to_path(key, ch), _convert(value)
                     )
```

## laboneq/controller/devices/device_shfqa.py

```diff
@@ -17,55 +17,54 @@
 )
 from laboneq.controller.communication import (
     CachingStrategy,
     DaqNodeAction,
     DaqNodeGetAction,
     DaqNodeSetAction,
 )
-from laboneq.controller.devices.device_zi import DeviceZI, delay_to_rounded_samples
+from laboneq.controller.devices.device_shf_base import DeviceSHFBase
+from laboneq.controller.devices.device_zi import (
+    SequencerPaths,
+    delay_to_rounded_samples,
+)
 from laboneq.controller.recipe_1_4_0 import (
     IO,
     Initialization,
     IntegratorAllocation,
     Measurement,
 )
-from laboneq.controller.recipe_enums import DIOConfigType
+from laboneq.controller.recipe_enums import TriggeringMode
 from laboneq.controller.recipe_processor import (
     AwgConfig,
     AwgKey,
     DeviceRecipeData,
     RecipeData,
     RtExecutionInfo,
     get_wave,
 )
 from laboneq.controller.util import LabOneQControllerException
 from laboneq.core.types.enums.acquisition_type import AcquisitionType
 from laboneq.core.types.enums.averaging_mode import AveragingMode
-from laboneq.core.types.enums.reference_clock_source import ReferenceClockSource
 
 _logger = logging.getLogger(__name__)
 
-REFERENCE_CLOCK_SOURCE_INTERNAL = 0
-REFERENCE_CLOCK_SOURCE_EXTERNAL = 1
-REFERENCE_CLOCK_SOURCE_ZSYNC = 2
-
 INTERNAL_TRIGGER_CHANNEL = 1024  # PQSC style triggering on the SHFSG/QC
 SOFTWARE_TRIGGER_CHANNEL = 8  # Software triggering on the SHFQA
 
 SAMPLE_FREQUENCY_HZ = 2.0e9
 DELAY_NODE_GRANULARITY_SAMPLES = 4
 DELAY_NODE_MAX_SAMPLES = 1e-6 * SAMPLE_FREQUENCY_HZ
 # About DELAY_NODE_MAX_SAMPLES: The max time is actually 131e-6 s (at least I can set that
 # value in GUI and API). However, there were concerns that these long times are not tested
 # often enough - also, if you read the value back from the API, some lesser significant bits
 # have strange values which looked a bit suspicious. Therefore, it was decided to limit the
 # maximum delay to 1 us for now
 
 
-class DeviceSHFQA(DeviceZI):
+class DeviceSHFQA(DeviceSHFBase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.dev_type = "SHFQA4"
         self.dev_opts = []
         self._channels = 4
         self._wait_for_awgs = True
         self._emit_trigger = False
@@ -90,21 +89,21 @@
                 self.dev_type,
             )
             self._channels = 4
 
     def _get_sequencer_type(self) -> str:
         return "qa"
 
-    def _get_sequencer_path_patterns(self) -> dict:
-        return {
-            "elf": "/{serial}/qachannels/{index}/generator/elf/data",
-            "progress": "/{serial}/qachannels/{index}/generator/elf/progress",
-            "enable": "/{serial}/qachannels/{index}/generator/enable",
-            "ready": "/{serial}/qachannels/{index}/generator/ready",
-        }
+    def get_sequencer_paths(self, index: int) -> SequencerPaths:
+        return SequencerPaths(
+            elf=f"/{self.serial}/qachannels/{index}/generator/elf/data",
+            progress=f"/{self.serial}/qachannels/{index}/generator/elf/progress",
+            enable=f"/{self.serial}/qachannels/{index}/generator/enable",
+            ready=f"/{self.serial}/qachannels/{index}/generator/ready",
+        )
 
     def _get_num_awgs(self):
         return self._channels
 
     def _validate_range(self, io: IO.Data, is_out: bool):
         if io.range is None:
             return
@@ -882,15 +881,15 @@
                         f"/{self.serial}/qachannels/{dev_input.channel}/input/range",
                         dev_input.range,
                     )
                 )
 
         for measurement in initialization.measurements:
             channel = 0
-            if initialization.config.dio_mode == DIOConfigType.HDAWG_LEADER:
+            if initialization.config.triggering_mode == TriggeringMode.DESKTOP_LEADER:
                 # standalone QA oder QC
                 channel = (
                     SOFTWARE_TRIGGER_CHANNEL
                     if self.options.is_qc
                     else INTERNAL_TRIGGER_CHANNEL
                 )
             nodes_to_initialize_measurement.append(
@@ -909,86 +908,47 @@
     ) -> list[DaqNodeAction]:
         _logger.debug("Configuring triggers...")
         self._wait_for_awgs = True
         self._emit_trigger = False
 
         nodes_to_configure_triggers = []
 
-        dio_mode = initialization.config.dio_mode
+        triggering_mode = initialization.config.triggering_mode
 
-        if dio_mode == DIOConfigType.ZSYNC_DIO:
+        if triggering_mode == TriggeringMode.ZSYNC_FOLLOWER:
             pass
-        elif dio_mode == DIOConfigType.HDAWG_LEADER:
+        elif triggering_mode == TriggeringMode.DESKTOP_LEADER:
             self._wait_for_awgs = False
             self._emit_trigger = True
-            clock_source = initialization.config.reference_clock_source
-            ntc = [
-                (
-                    "system/clocks/referenceclock/in/source",
-                    REFERENCE_CLOCK_SOURCE_INTERNAL
-                    if clock_source
-                    and clock_source.value == ReferenceClockSource.INTERNAL.value
-                    else REFERENCE_CLOCK_SOURCE_EXTERNAL,
-                )
-            ]
             if self.options.is_qc:
-                ntc += [
-                    ("system/internaltrigger/enable", 0),
-                    ("system/internaltrigger/repetitions", 1),
-                ]
-            return [
-                DaqNodeSetAction(self._daq, f"/{self.serial}/{node}", v)
-                for node, v in ntc
-            ]
-
+                int_trig_base = f"/{self.serial}/system/internaltrigger"
+                nodes_to_configure_triggers.append(
+                    DaqNodeSetAction(self._daq, f"{int_trig_base}/enable", 0)
+                )
+                nodes_to_configure_triggers.append(
+                    DaqNodeSetAction(self._daq, f"{int_trig_base}/repetitions", 1)
+                )
         else:
             raise LabOneQControllerException(
-                f"Unsupported DIO mode: {dio_mode} for device type SHFQA."
+                f"Unsupported triggering mode: {triggering_mode} for device type SHFQA."
             )
 
         for awg_index in (
             self._allocated_awgs if len(self._allocated_awgs) > 0 else range(1)
         ):
-            marker_path = f"/{self.serial}/qachannels/{awg_index}/markers"
+            markers_base = f"/{self.serial}/qachannels/{awg_index}/markers"
             src = 32 + awg_index
             nodes_to_configure_triggers.append(
-                DaqNodeSetAction(self._daq, f"{marker_path}/0/source", src),
+                DaqNodeSetAction(self._daq, f"{markers_base}/0/source", src),
             )
             nodes_to_configure_triggers.append(
-                DaqNodeSetAction(self._daq, f"{marker_path}/1/source", src),
+                DaqNodeSetAction(self._daq, f"{markers_base}/1/source", src),
             )
         return nodes_to_configure_triggers
 
-    def configure_as_leader(self, initialization: Initialization.Data):
-        raise LabOneQControllerException("SHFQA cannot be configured as leader")
-
-    def collect_follower_configuration_nodes(
-        self, initialization: Initialization.Data
-    ) -> list[DaqNodeAction]:
-        dio_mode = initialization.config.dio_mode
-        _logger.debug("%s: Configuring as a follower...", self.dev_repr)
-
-        nodes_to_configure_as_follower = []
-
-        if dio_mode == DIOConfigType.ZSYNC_DIO:
-            _logger.debug(
-                "%s: Configuring reference clock to use ZSYNC as a reference...",
-                self.dev_repr,
-            )
-            self._switch_reference_clock(source=2, expected_freqs=100e6)
-        elif dio_mode == DIOConfigType.HDAWG_LEADER:
-            # standalone
-            pass
-        else:
-            raise LabOneQControllerException(
-                f"Unsupported DIO mode: {dio_mode} for device type SHFQA."
-            )
-
-        return nodes_to_configure_as_follower
-
     def get_measurement_data(
         self,
         channel: int,
         acquisition_type: AcquisitionType,
         result_indices: list[int],
         num_results: int,
         hw_averages: int,
```

## laboneq/controller/devices/device_shfsg.py

```diff
@@ -15,29 +15,27 @@
     DeviceAttributesView,
 )
 from laboneq.controller.communication import (
     CachingStrategy,
     DaqNodeAction,
     DaqNodeSetAction,
 )
-from laboneq.controller.devices.device_zi import DeviceZI
+from laboneq.controller.devices.device_shf_base import DeviceSHFBase
+from laboneq.controller.devices.device_zi import SequencerPaths
+from laboneq.controller.devices.zi_node_monitor import NodeControlBase
 from laboneq.controller.recipe_1_4_0 import IO, Initialization
-from laboneq.controller.recipe_enums import DIOConfigType, ReferenceClockSource
+from laboneq.controller.recipe_enums import TriggeringMode
 from laboneq.controller.recipe_processor import DeviceRecipeData, RecipeData
 from laboneq.controller.util import LabOneQControllerException
 from laboneq.core.types.enums.acquisition_type import AcquisitionType
 
 _logger = logging.getLogger(__name__)
 
-REFERENCE_CLOCK_SOURCE_INTERNAL = 0
-REFERENCE_CLOCK_SOURCE_EXTERNAL = 1
-REFERENCE_CLOCK_SOURCE_ZSYNC = 2
 
-
-class DeviceSHFSG(DeviceZI):
+class DeviceSHFSG(DeviceSHFBase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.dev_type = "SHFSG8"
         self.dev_opts = []
         self._channels = 8
         self._output_to_synth_map = [0, 0, 1, 1, 2, 2, 3, 3]
         self._wait_for_awgs = True
@@ -45,14 +43,18 @@
 
     @property
     def dev_repr(self) -> str:
         if self.options.is_qc:
             return f"SHFQC/SG:{self.serial}"
         return f"SHFSG:{self.serial}"
 
+    @property
+    def is_secondary(self) -> bool:
+        return self.options.qc_with_qa
+
     def _process_dev_opts(self):
         if self.dev_type == "SHFSG8":
             self._channels = 8
             self._output_to_synth_map = [0, 0, 1, 1, 2, 2, 3, 3]
         elif self.dev_type == "SHFSG4":
             self._channels = 4
             self._output_to_synth_map = [0, 1, 2, 3]
@@ -84,21 +86,21 @@
             )
             self._channels = 4
             self._output_to_synth_map = [0, 1, 2, 3]
 
     def _get_sequencer_type(self) -> str:
         return "sg"
 
-    def _get_sequencer_path_patterns(self) -> dict:
-        return {
-            "elf": "/{serial}/sgchannels/{index}/awg/elf/data",
-            "progress": "/{serial}/sgchannels/{index}/awg/elf/progress",
-            "enable": "/{serial}/sgchannels/{index}/awg/enable",
-            "ready": "/{serial}/sgchannels/{index}/awg/ready",
-        }
+    def get_sequencer_paths(self, index: int) -> SequencerPaths:
+        return SequencerPaths(
+            elf=f"/{self.serial}/sgchannels/{index}/awg/elf/data",
+            progress=f"/{self.serial}/sgchannels/{index}/awg/elf/progress",
+            enable=f"/{self.serial}/sgchannels/{index}/awg/enable",
+            ready=f"/{self.serial}/sgchannels/{index}/awg/ready",
+        )
 
     def _get_num_awgs(self):
         return self._channels
 
     def _validate_range(self, io: IO.Data):
         if io.range is None:
             return
@@ -155,14 +157,20 @@
     def _nodes_to_monitor_impl(self) -> list[str]:
         nodes = super()._nodes_to_monitor_impl()
         for awg in range(self._get_num_awgs()):
             nodes.append(f"/{self.serial}/sgchannels/{awg}/awg/enable")
             nodes.append(f"/{self.serial}/sgchannels/{awg}/awg/ready")
         return nodes
 
+    def clock_source_control_nodes(self) -> list[NodeControlBase]:
+        if self.is_secondary:
+            return []  # QA will initialize the nodes
+        else:
+            return super().clock_source_control_nodes()
+
     def collect_execution_nodes(self):
         _logger.debug("Starting execution...")
         return [
             DaqNodeSetAction(
                 self._daq,
                 f"/{self.serial}/sgchannels/{awg_index}/awg/enable",
                 1,
@@ -436,15 +444,15 @@
 
         for awg_key, awg_config in recipe_data.awg_configs.items():
             if (
                 awg_key.device_uid != initialization.device_uid
                 or awg_config.qa_signal_id is None
             ):
                 continue
-            if awg_config.source_feedback_register is None and self.options.qc_with_qa:
+            if awg_config.source_feedback_register is None and self.is_secondary:
                 # local feedback
                 ntc.extend(
                     [
                         (
                             f"sgchannels/{awg_key.awg_index}/awg/intfeedback/direct/shift",
                             awg_config.feedback_register_bit,
                         ),
@@ -476,48 +484,43 @@
                         ),
                         (
                             f"sgchannels/{awg_key.awg_index}/awg/zsync/register/offset",
                             awg_config.command_table_match_offset,
                         ),
                     ]
                 )
-        dio_mode = initialization.config.dio_mode
+        triggering_mode = initialization.config.triggering_mode
 
-        if dio_mode == DIOConfigType.ZSYNC_DIO:
+        if triggering_mode == TriggeringMode.ZSYNC_FOLLOWER:
             pass
-        elif dio_mode in (DIOConfigType.HDAWG_LEADER, DIOConfigType.HDAWG):
+        elif triggering_mode in (
+            TriggeringMode.DESKTOP_LEADER,
+            TriggeringMode.INTERNAL_FOLLOWER,
+        ):
             # standalone SHFSG or SHFQC
             self._wait_for_awgs = False
-            if not self.options.qc_with_qa:
+            if not self.is_secondary:
                 # otherwise, the QA will initialize the nodes
                 self._emit_trigger = True
-                clock_source = initialization.config.reference_clock_source
                 ntc += [
-                    (
-                        "system/clocks/referenceclock/in/source",
-                        REFERENCE_CLOCK_SOURCE_INTERNAL
-                        if clock_source
-                        and clock_source.value == ReferenceClockSource.INTERNAL.value
-                        else REFERENCE_CLOCK_SOURCE_EXTERNAL,
-                    ),
                     ("system/internaltrigger/enable", 0),
                     ("system/internaltrigger/repetitions", 1),
                 ]
             for awg_index in (
                 self._allocated_awgs if len(self._allocated_awgs) > 0 else range(1)
             ):
                 ntc += [
                     # Rise
                     (f"sgchannels/{awg_index}/awg/auxtriggers/0/slope", 1),
                     # Internal trigger
                     (f"sgchannels/{awg_index}/awg/auxtriggers/0/channel", 8),
                 ]
         else:
             raise LabOneQControllerException(
-                f"Unsupported DIO mode: {dio_mode} for device type SHFSG."
+                f"Unsupported triggering mode: {triggering_mode} for device type SHFSG."
             )
 
         nodes_to_configure_triggers = [
             DaqNodeSetAction(self._daq, f"/{self.serial}/{node}", v) for node, v in ntc
         ]
         return nodes_to_configure_triggers
 
@@ -527,47 +530,14 @@
             "header": {"version": "1.1.0"},
             "table": body,
         }
 
     def command_table_path(self, awg_index: int) -> str:
         return f"/{self.serial}/sgchannels/{awg_index}/awg/commandtable/"
 
-    def configure_as_leader(self, initialization: Initialization.Data):
-        raise LabOneQControllerException("SHFSG cannot be configured as leader")
-
-    def collect_follower_configuration_nodes(
-        self, initialization: Initialization.Data
-    ) -> list[DaqNodeAction]:
-        if self.options.qc_with_qa:
-            return []  # QC follower config is done over it's QA part
-
-        dio_mode = initialization.config.dio_mode
-        _logger.debug("%s: Configuring as a follower...", self.dev_repr)
-
-        nodes_to_configure_as_follower = []
-
-        if dio_mode == DIOConfigType.ZSYNC_DIO:
-            _logger.debug(
-                "%s: Configuring reference clock to use ZSYNC as a reference...",
-                self.dev_repr,
-            )
-            self._switch_reference_clock(source=2, expected_freqs=100e6)
-        elif dio_mode == DIOConfigType.HDAWG_LEADER:
-            # standalone
-            pass
-        elif dio_mode == DIOConfigType.HDAWG:
-            # standalone as part of an SHFQC with active QA part
-            pass
-        else:
-            raise LabOneQControllerException(
-                f"Unsupported DIO mode: {dio_mode} for device type SHFSG."
-            )
-
-        return nodes_to_configure_as_follower
-
     def collect_reset_nodes(self) -> list[DaqNodeAction]:
         reset_nodes = super().collect_reset_nodes()
         reset_nodes.append(
             DaqNodeSetAction(
                 self._daq,
                 f"/{self.serial}/sgchannels/*/awg/enable",
                 0,
```

## laboneq/controller/devices/device_uhfqa.py

```diff
@@ -17,15 +17,15 @@
     DaqNodeAction,
     DaqNodeGetAction,
     DaqNodeSetAction,
 )
 from laboneq.controller.devices.device_zi import DeviceZI, delay_to_rounded_samples
 from laboneq.controller.devices.zi_node_monitor import Command, NodeControlBase
 from laboneq.controller.recipe_1_4_0 import IO, Initialization, IntegratorAllocation
-from laboneq.controller.recipe_enums import DIOConfigType
+from laboneq.controller.recipe_enums import TriggeringMode
 from laboneq.controller.recipe_processor import (
     AwgConfig,
     AwgKey,
     DeviceRecipeData,
     RecipeData,
     RtExecutionInfo,
     get_wave,
@@ -84,29 +84,26 @@
     def _nodes_to_monitor_impl(self) -> list[str]:
         nodes = super()._nodes_to_monitor_impl()
         for awg in range(self._get_num_awgs()):
             nodes.append(f"/{self.serial}/awgs/{awg}/enable")
             nodes.append(f"/{self.serial}/awgs/{awg}/ready")
         return nodes
 
-    def _error_as_leader(self):
-        raise LabOneQControllerException(
-            f"{self.dev_repr}: UHFQA cannot be configured as leader, ensure correct DIO "
-            f"connection in the device setup"
-        )
-
     def _error_ambiguous_upstream(self):
         raise LabOneQControllerException(
             f"{self.dev_repr}: Can't determine unambiguously upstream device for UHFQA, ensure "
             f"correct DIO connection in the device setup"
         )
 
     def update_clock_source(self, force_internal: bool | None):
         if len(self._uplinks) == 0:
-            self._error_as_leader()
+            raise LabOneQControllerException(
+                f"{self.dev_repr}: UHFQA cannot be configured as leader, ensure correct DIO "
+                f"connection in the device setup"
+            )
         if len(self._uplinks) > 1:
             self._error_ambiguous_upstream()
         upstream = next(iter(self._uplinks.values()))()
         if upstream is None:
             self._error_ambiguous_upstream()
         is_desktop = upstream.is_leader() and (
             upstream.device_qualifier.driver.upper() == "HDAWG"
@@ -625,25 +622,25 @@
                     DaqNodeSetAction(self._daq, f"{awg_path}/dio/strobe/index", 16),
                     DaqNodeSetAction(self._daq, f"{awg_path}/dio/strobe/slope", 0),
                     DaqNodeSetAction(self._daq, f"{awg_path}/dio/valid/polarity", 2),
                     DaqNodeSetAction(self._daq, f"{awg_path}/dio/valid/index", 16),
                 ]
             )
 
-        dio_mode = initialization.config.dio_mode
+        triggering_mode = initialization.config.triggering_mode
 
-        if dio_mode == DIOConfigType.HDAWG or dio_mode is None:
+        if triggering_mode == TriggeringMode.DIO_FOLLOWER or triggering_mode is None:
             nodes_to_configure_triggers.extend(
                 [
                     DaqNodeSetAction(self._daq, f"/{self.serial}/dios/0/mode", 2),
                     DaqNodeSetAction(self._daq, f"/{self.serial}/dios/0/drive", 0x3),
                     DaqNodeSetAction(self._daq, f"/{self.serial}/dios/0/extclk", 0x2),
                 ]
             )
-        elif dio_mode == DIOConfigType.DIO_FOLLOWER_OF_HDAWG_LEADER:
+        elif triggering_mode == TriggeringMode.DESKTOP_DIO_FOLLOWER:
             nodes_to_configure_triggers.extend(
                 [
                     DaqNodeSetAction(self._daq, f"/{self.serial}/dios/0/mode", 0),
                     DaqNodeSetAction(self._daq, f"/{self.serial}/dios/0/drive", 0),
                     DaqNodeSetAction(self._daq, f"/{self.serial}/dios/0/extclk", 0x2),
                     DaqNodeSetAction(
                         self._daq, f"/{self.serial}/awgs/0/auxtriggers/0/channel", 0
@@ -665,17 +662,14 @@
                         self._daq, f"{trigger_path}/source", 32 + trigger_index
                     ),
                 ]
             )
 
         return nodes_to_configure_triggers
 
-    def configure_as_leader(self, initialization: Initialization.Data):
-        self._error_as_leader()
-
     def _get_integrator_measurement_data(
         self, result_index, num_results, averages_divider: int
     ):
         result_path = f"/{self.serial}/qas/0/result/data/{result_index}/wave"
         # @TODO(andreyk): replace the raw daq reply parsing on site here and hide it inside
         # Communication class
         data_node_query = self._daq.get_raw(result_path)
```

## laboneq/controller/devices/device_zi.py

```diff
@@ -2,16 +2,14 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import json
 import logging
 import math
-import os
-import os.path
 import re
 import time
 from abc import ABC
 from copy import deepcopy
 from dataclasses import dataclass
 from enum import Enum
 from math import floor
@@ -93,14 +91,22 @@
 class DeviceQualifier:
     dry_run: bool = True
     driver: str = None
     server: DaqWrapper = None
     options: DeviceOptions = None
 
 
+@dataclass
+class SequencerPaths:
+    elf: str
+    progress: str
+    enable: str
+    ready: str
+
+
 def delay_to_rounded_samples(
     channel: int,
     dev_repr: str,
     delay: float,
     sample_frequency_hz,
     granularity_samples,
     max_node_delay_samples,
@@ -193,14 +199,18 @@
     def interface(self):
         return self.options.interface.lower()
 
     @property
     def daq(self):
         return self._daq
 
+    @property
+    def is_secondary(self) -> bool:
+        return False
+
     def add_command_table_header(self, body: dict) -> dict:
         # Stub, implement in sub-class
         _logger.debug("Command table unavailable on device %s", self.dev_repr)
         return {}
 
     def command_table_path(self, awg_index: int) -> str:
         # Stub, implement in sub-class
@@ -221,29 +231,21 @@
 
     def _process_dev_opts(self):
         pass
 
     def _get_sequencer_type(self) -> str:
         return "auto-detect"
 
-    def _get_sequencer_path_patterns(self) -> dict[str, str]:
-        return {
-            "elf": "/{serial}/awgs/{index}/elf/data",
-            "progress": "/{serial}/awgs/{index}/elf/progress",
-            "enable": "/{serial}/awgs/{index}/enable",
-            "ready": "/{serial}/awgs/{index}/ready",
-        }
-
-    def get_sequencer_paths(self, index: int) -> dict[str, str]:
-        props = {
-            "serial": self.serial,
-            "index": index,
-        }
-        patterns = self._get_sequencer_path_patterns()
-        return {k: v.format(**props) for k, v in patterns.items()}
+    def get_sequencer_paths(self, index: int) -> SequencerPaths:
+        return SequencerPaths(
+            elf=f"/{self.serial}/awgs/{index}/elf/data",
+            progress=f"/{self.serial}/awgs/{index}/elf/progress",
+            enable=f"/{self.serial}/awgs/{index}/enable",
+            ready=f"/{self.serial}/awgs/{index}/ready",
+        )
 
     def add_downlink(self, port: str, linked_device_uid: str, linked_device: DeviceZI):
         self._downlinks[port] = (linked_device_uid, ref(linked_device))
 
     def add_uplink(self, port: str, linked_device: DeviceZI):
         self._uplinks[port] = ref(linked_device)
 
@@ -302,22 +304,14 @@
         return []
 
     def collect_trigger_configuration_nodes(
         self, initialization: Initialization.Data, recipe_data: RecipeData
     ) -> list[DaqNodeAction]:
         return []
 
-    def configure_as_leader(self, initialization: Initialization.Data):
-        pass
-
-    def collect_follower_configuration_nodes(
-        self, initialization: Initialization.Data
-    ) -> list[DaqNodeAction]:
-        return []
-
     def _connect_to_data_server(self):
         if self._connected:
             return
 
         _logger.debug("%s: Connecting to %s interface.", self.dev_repr, self.interface)
         try:
             self._daq.connectDevice(self.serial, self.interface)
@@ -473,17 +467,14 @@
         hw_averages: int,
     ):
         return None  # default -> no results available from the device
 
     def get_input_monitor_data(self, channel: int, num_results: int):
         return None  # default -> no results available from the device
 
-    def wait_for_conditions_to_start(self):
-        pass
-
     def conditions_for_execution_ready(self) -> dict[str, Any]:
         return {}
 
     def conditions_for_execution_done(
         self, acquisition_type: AcquisitionType
     ) -> dict[str, Any]:
         return {}
@@ -541,117 +532,14 @@
                 continue
 
             if guard_start is None:
                 guard_start = time.time()
             if time.time() - guard_start >= guard_time:
                 break
 
-    def _switch_reference_clock(self, source, expected_freqs):
-        if expected_freqs is not None and not isinstance(expected_freqs, list):
-            expected_freqs = [expected_freqs]
-
-        source_path = f"/{self.serial}/system/clocks/referenceclock/in/source"
-        status_path = f"/{self.serial}/system/clocks/referenceclock/in/status"
-        sourceactual_path = (
-            f"/{self.serial}/system/clocks/referenceclock/in/sourceactual"
-        )
-        freq_path = f"/{self.serial}/system/clocks/referenceclock/in/freq"
-
-        self._daq.batch_set(
-            [
-                DaqNodeSetAction(
-                    self._daq,
-                    source_path,
-                    source,
-                    caching_strategy=CachingStrategy.NO_CACHE,
-                )
-            ]
-        )
-
-        retries = 0
-        timeout = 60  # s
-        start_time = time.time()
-        last_report = start_time
-        sourceactual = None
-        status = None
-        freq = None
-
-        while True:
-            if retries > 0:
-                now = time.time()
-                elapsed = floor(now - start_time)
-                if now - start_time > timeout:
-                    raise LabOneQControllerException(
-                        f"Unable to switch reference clock within {timeout}s. "
-                        f"Requested source: {source}, actual: {sourceactual}, status: {status}, "
-                        f"expected frequencies: {expected_freqs}, actual: {freq}"
-                    )
-                if now - last_report > 5:
-                    _logger.debug(
-                        "Waiting for reference clock switching, %f s remaining "
-                        "until %f s timeout...",
-                        timeout - elapsed,
-                        timeout,
-                    )
-                    last_report = now
-                time.sleep(0.1)
-            retries += 1
-
-            daq_reply = self._daq.batch_get(
-                [
-                    DaqNodeGetAction(
-                        self._daq,
-                        sourceactual_path,
-                        caching_strategy=CachingStrategy.NO_CACHE,
-                    )
-                ]
-            )
-            sourceactual = daq_reply[sourceactual_path]
-            if sourceactual != source and not self.dry_run:
-                continue
-
-            daq_reply = self._daq.batch_get(
-                [
-                    DaqNodeGetAction(
-                        self._daq,
-                        status_path,
-                        caching_strategy=CachingStrategy.NO_CACHE,
-                    )
-                ]
-            )
-            status = daq_reply[status_path]
-            if not self.dry_run:
-                if status == 2:  # still locking
-                    continue
-                if status == 1:  # error while locking
-                    raise LabOneQControllerException(
-                        f"Unable to switch reference clock, device returned error "
-                        f"after {elapsed}s. Requested source: {source}, actual: {sourceactual}, "
-                        f"status: {status}, expected frequency: {expected_freqs}, actual: {freq}"
-                    )
-
-            if expected_freqs is None:
-                break
-            daq_reply = self._daq.batch_get(
-                [
-                    DaqNodeGetAction(
-                        self._daq, freq_path, caching_strategy=CachingStrategy.NO_CACHE
-                    )
-                ]
-            )
-            freq = daq_reply[freq_path]
-            if freq in expected_freqs or self.dry_run:
-                break
-            else:
-                raise LabOneQControllerException(
-                    f"Unexpected frequency after switching the reference clock. "
-                    f"Requested source: {source}, actual: {sourceactual}, status: {status}, "
-                    f"expected frequency: {expected_freqs}, actual: {freq}"
-                )
-
     def _adjust_frequency(self, freq):
         return freq
 
     def collect_prepare_nt_step_nodes(
         self, attributes: DeviceAttributesView, recipe_data: RecipeData
     ) -> list[DaqNodeAction]:
         nodes_to_set: list[DaqNodeAction] = []
@@ -770,54 +658,53 @@
         if not wave:
             raise LabOneQControllerException(
                 f"Wave not found, signature '{sig}' filename '{filename_to_find}'"
             )
 
         return sig, np.array(wave["samples"], dtype=np.complex128)
 
-    def _prepare_waves(
-        self, compiled: CompiledExperiment, seqc_filename: str
+    def prepare_waves(
+        self, compiled: CompiledExperiment, wave_indices_ref: str
     ) -> list[tuple[str, npt.ArrayLike]]:
-        wave_indices_filename = os.path.splitext(seqc_filename)[0] + "_waveindices.csv"
+        if wave_indices_ref is None:
+            return None
         wave_indices: dict[str, list[int | str]] = next(
-            (
-                i
-                for i in compiled.wave_indices
-                if i["filename"] == wave_indices_filename
-            ),
+            (i for i in compiled.wave_indices if i["filename"] == wave_indices_ref),
             {"value": {}},
         )["value"]
 
         waves_by_index = {}
         waves = compiled.waves or []
         for sig, [idx, sig_type] in wave_indices.items():
             if sig_type in ("iq", "double", "multi"):
                 waves_by_index[idx] = self._prepare_wave_iq(waves, sig)
             elif sig_type == "single":
                 waves_by_index[idx] = self._prepare_wave_single(waves, sig)
             elif sig_type == "complex":
                 waves_by_index[idx] = self._prepare_wave_complex(waves, sig)
             else:
                 raise LabOneQControllerException(
-                    f"Unexpected signal type for binary wave for '{sig}' in '{seqc_filename}' - "
+                    f"Unexpected signal type for binary wave for '{sig}' in '{wave_indices_ref}' - "
                     f"'{sig_type}', should be one of [iq, double, multi, single, complex]"
                 )
 
         bin_waves: list[tuple[str, npt.ArrayLike]] = []
         idx = 0
         while idx in waves_by_index:
             bin_waves.append(waves_by_index[idx])
             idx += 1
         return bin_waves
 
-    def _prepare_command_table(
-        self, compiled: CompiledExperiment, seqc_filename: str
+    def prepare_command_table(
+        self, compiled: CompiledExperiment, ct_ref: str
     ) -> dict | None:
+        if ct_ref is None:
+            return None
         command_table_body = next(
-            (ct["ct"] for ct in compiled.command_tables if ct["seqc"] == seqc_filename),
+            (ct["ct"] for ct in compiled.command_tables if ct["seqc"] == ct_ref),
             None,
         )
 
         if command_table_body is None:
             return None
 
         oscillator_map = {osc.id: osc.index for osc in self._allocated_oscs}
@@ -826,60 +713,42 @@
             if "oscillatorSelect" not in entry:
                 continue
             oscillator_uid = entry["oscillatorSelect"]["value"]["$ref"]
             entry["oscillatorSelect"]["value"] = oscillator_map[oscillator_uid]
 
         return self.add_command_table_header(command_table_body)
 
-    def prepare_seqc(
-        self, seqc_filename: str, compiled: CompiledExperiment
-    ) -> tuple[str, list[tuple[str, npt.ArrayLike]], dict[Any]]:
-        """
-        `compiled` expected to have the following members:
-         - `src`   -> list[dict[str, str]]
-                        `filename` -> `<seqc_filename>`
-                        `text`     -> `<seqc_content>`
-         - `waves` -> list[dict[str, str]]
-                        `filename` -> `<wave_filename_csv>`
-                        `text`     -> `<wave_content_csv>`
-
-        Returns a tuple of
-         1. str: seqc text to pass to the awg compiler
-         2. list[(str, array)]: waves(id, samples) to upload to the instrument (ordered by index)
-         3. dict: command table
-        """
-        seqc = next((s for s in compiled.src if s["filename"] == seqc_filename), None)
+    def prepare_seqc(self, compiled: CompiledExperiment, seqc_ref: str) -> str:
+        if seqc_ref is None:
+            return None
+
+        seqc = next((s for s in compiled.src if s["filename"] == seqc_ref), None)
         if seqc is None:
-            raise LabOneQControllerException(
-                f"SeqC program '{seqc_filename}' not found"
-            )
+            raise LabOneQControllerException(f"SeqC program '{seqc_ref}' not found")
 
         # Substitute oscillator nodes by actual assignment
         seqc_lines = seqc["text"].split("\n")
         for i, seqc_line in enumerate(seqc_lines):
             m = seqc_osc_match.match(seqc_line)
             if m is not None:
                 param = m.group(2)
                 for osc in self._allocated_oscs:
                     if osc.param == param:
                         seqc_lines[
                             i
                         ] = f"{m.group(1)}{m.group(2)}{m.group(3)}{osc.index}{m.group(4)}"
         seqc_text = "\n".join(seqc_lines)
 
-        bin_waves = self._prepare_waves(compiled, seqc_filename)
-        command_table = self._prepare_command_table(compiled, seqc_filename)
-
-        return seqc_text, bin_waves, command_table
+        return seqc_text
 
     def prepare_upload_elf(self, elf: bytes, awg_index: int, filename: str):
         sequencer_paths = self.get_sequencer_paths(awg_index)
         return DaqNodeSetAction(
             self._daq,
-            sequencer_paths["elf"],
+            sequencer_paths.elf,
             elf,
             filename=filename,
             caching_strategy=CachingStrategy.NO_CACHE,
         )
 
     def prepare_upload_binary_wave(
         self,
```

## laboneq/controller/devices/zi_emulator.py

```diff
@@ -405,40 +405,35 @@
         for result_index in range(10):
             nd[f"qas/0/result/data/{result_index}/wave"] = NodeInfo(
                 type=NodeType.VECTOR_COMPLEX
             )
         return nd
 
 
-class DevEmuPQSC(DevEmuHW):
-    def _trig_stop(self):
-        self._set_val("execution/enable", 0)
-
-    def _trig_execute(self, node: NodeBase):
-        self._scheduler.enter(delay=0.001, priority=0, action=self._trig_stop)
-
+class Gen2Base(DevEmuHW):
     def _ref_clock_switched(self, requested_source: int):
+        # 0 - INTERNAL
+        # 1 - EXTERNAL
+        # 2 - ZSYNC
+        freq = 10e6 if requested_source == 1 else 100e6
         self._set_val("system/clocks/referenceclock/in/sourceactual", requested_source)
         self._set_val("system/clocks/referenceclock/in/status", 0)
-        self._set_val("system/clocks/referenceclock/in/freq", 10e6)
+        self._set_val("system/clocks/referenceclock/in/freq", freq)
 
     def _ref_clock(self, node: NodeBase):
         node_int: NodeInt = node
         self._scheduler.enter(
             delay=0.001,
             priority=0,
             action=self._ref_clock_switched,
             argument=(node_int.value,),
         )
 
-    def _node_def(self) -> dict[str, NodeInfo]:
+    def _node_def_gen2(self) -> dict[str, NodeInfo]:
         return {
-            "execution/enable": NodeInfo(
-                type=NodeType.INT, default=0, handler=DevEmuPQSC._trig_execute
-            ),
             "system/clocks/referenceclock/in/source": NodeInfo(
                 type=NodeType.INT, default=0, handler=DevEmuPQSC._ref_clock
             ),
             "system/clocks/referenceclock/in/sourceactual": NodeInfo(
                 type=NodeType.INT, default=0
             ),
             "system/clocks/referenceclock/in/status": NodeInfo(
@@ -446,15 +441,31 @@
             ),
             "system/clocks/referenceclock/in/freq": NodeInfo(
                 type=NodeType.FLOAT, default=100e6
             ),
         }
 
 
-class DevEmuSHFQABase(DevEmuHW):
+class DevEmuPQSC(Gen2Base):
+    def _trig_stop(self):
+        self._set_val("execution/enable", 0)
+
+    def _trig_execute(self, node: NodeBase):
+        self._scheduler.enter(delay=0.001, priority=0, action=self._trig_stop)
+
+    def _node_def(self) -> dict[str, NodeInfo]:
+        return {
+            **self._node_def_gen2(),
+            "execution/enable": NodeInfo(
+                type=NodeType.INT, default=0, handler=DevEmuPQSC._trig_execute
+            ),
+        }
+
+
+class DevEmuSHFQABase(Gen2Base):
     def _awg_stop_qa(self, channel: int):
         readout_enable = self._get_node(
             f"qachannels/{channel}/readout/result/enable"
         ).value
         spectroscopy_enable = self._get_node(
             f"qachannels/{channel}/spectroscopy/result/enable"
         ).value
@@ -543,19 +554,20 @@
                 default=self._dev_opts.get("features/devtype", "SHFQA4"),
             ),
             "features/options": NodeInfo(
                 type=NodeType.STR,
                 default=self._dev_opts.get("features/options", ""),
             ),
         }
+        nd.update(self._node_def_gen2())
         nd.update(self._node_def_qa())
         return nd
 
 
-class DevEmuSHFSGBase(DevEmuHW):
+class DevEmuSHFSGBase(Gen2Base):
     def _awg_stop_sg(self, channel: int):
         self._set_val(f"sgchannels/{channel}/awg/enable", 0)
 
     def _awg_execute_sg(self, node: NodeBase, channel: int):
         self._scheduler.enter(
             delay=0.001, priority=0, action=self._awg_stop_sg, argument=(channel,)
         )
@@ -579,14 +591,15 @@
                 default=self._dev_opts.get("features/devtype", "SHFSG8"),
             ),
             "features/options": NodeInfo(
                 type=NodeType.STR,
                 default=self._dev_opts.get("features/options", ""),
             ),
         }
+        nd.update(self._node_def_gen2())
         nd.update(self._node_def_sg())
         return nd
 
 
 class DevEmuSHFQC(DevEmuSHFQABase, DevEmuSHFSGBase):
     def _node_def(self) -> dict[str, NodeInfo]:
         nd = {
@@ -595,14 +608,15 @@
                 default=self._dev_opts.get("features/devtype", "SHFQC"),
             ),
             "features/options": NodeInfo(
                 type=NodeType.STR,
                 default=self._dev_opts.get("features/options", "QC6CH"),
             ),
         }
+        nd.update(self._node_def_gen2())
         nd.update(self._node_def_qa())
         nd.update(self._node_def_sg())
         return nd
 
 
 class DevEmuNONQC(DevEmuHW):
     def _node_def(self) -> dict[str, NodeInfo]:
```

## laboneq/core/types/compiled_experiment.py

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any
 
 from laboneq.core.types.enums.mixer_type import MixerType
 from laboneq.core.validators import dicts_equal
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike
 
@@ -23,81 +23,81 @@
     amplitude: float = None  # instance (final) amplitude
     length: float = None  # instance (final) length
     iq_phase: float = None
     modulation_frequency: float = None
     modulation_phase: float = None
     channel: int = None  # The AWG channel for rf_signals
     needs_conjugate: bool = False  # SHF devices need that for now
-    play_pulse_parameters: Optional[Dict[str, Any]] = field(default_factory=dict)
-    pulse_pulse_parameters: Optional[Dict[str, Any]] = field(default_factory=dict)
+    play_pulse_parameters: dict[str, Any] = field(default_factory=dict)
+    pulse_pulse_parameters: dict[str, Any] = field(default_factory=dict)
 
     # uid of pulses that this instance overlaps with
-    overlaps: List[str] = None
+    overlaps: list[str] = None
     has_marker1: bool = False
     has_marker2: bool = False
     can_compress: bool = False
 
 
 @dataclass
 class PulseWaveformMap:
     """Data structure to store mappings between the given pulse and an AWG waveform."""
 
     sampling_rate: float
     length_samples: int
     signal_type: str
     # UHFQA's HW modulation is not an IQ mixer. None for flux pulses etc.
-    mixer_type: Optional[MixerType] = field(default=None)
-    instances: List[PulseInstance] = field(default_factory=list)
+    mixer_type: MixerType | None = None
+    instances: list[PulseInstance] = field(default_factory=list)
 
 
 @dataclass
 class PulseMapEntry:
     """Data structure to store the :py:class:`PulseWaveformMap` of each AWG waveform."""
 
     # key: waveform signature string
     #: A mapping of signals to :py:class:`PulseWaveformMap`
-    waveforms: Dict[str, PulseWaveformMap] = field(default_factory=dict)
+    waveforms: dict[str, PulseWaveformMap] = field(default_factory=dict)
 
 
 @dataclass(init=True, repr=True, order=True)
 class CompiledExperiment:
     """Data structure to store the output of the compiler."""
 
     #: The source device setup.
     device_setup: DeviceSetup = field(default=None)
 
     #: The source experiment.
     experiment: Experiment = field(default=None)
 
     #: Instructions to the controller for running the experiment.
-    recipe: Dict[str, Any] = field(default=None)
+    recipe: dict[str, Any] = field(default=None)
 
     #: The seqC source code, per device.
-    src: List[Dict[str, str]] = field(default=None)
+    src: list[dict[str, str]] = field(default=None)
 
     #: The waveforms that will be uploaded to the devices.
-    waves: List[Dict[str, Any]] = field(default=None)
+    waves: list[dict[str, Any]] = field(default=None)
 
     #: Data structure for storing the indices or filenames by which the waveforms are
     #: referred to during and after upload.
-    wave_indices: List[Dict[str, Any]] = field(default=None)
+    wave_indices: list[dict[str, Any]] = field(default=None)
 
-    #: Datastructure for storing the command table data
-    command_tables: List[Dict[str, Any]] = field(default_factory=list)
+    #: Data structure for storing the command table data
+    command_tables: list[dict[str, Any]] = field(default_factory=list)
 
-    #: List of events as scheduled by the compiler.
-    schedule: Dict[str, Any] = field(default=None)
+    #: list of events as scheduled by the compiler.
+    schedule: dict[str, Any] = field(default=None)
 
     #: A representation of the source experiment, using primitive Python datatypes only
     #: (dicts, lists, etc.)
-    experiment_dict: Dict[str, Any] = field(default=None)
+    experiment_dict: dict[str, Any] = field(default=None)
 
     #: Data structure for mapping pulses (in the experiment) to waveforms (on the
     #: device).
-    pulse_map: Dict[str, PulseMapEntry] = field(default=None)
+    pulse_map: dict[str, PulseMapEntry] = field(default=None)
 
     def __eq__(self, other: CompiledExperiment):
         if self is other:
             return True
 
         if len(self.waves) != len(other.waves):
             return False
@@ -109,17 +109,15 @@
             and self.wave_indices == other.wave_indices
             and self.schedule == other.schedule
             and dicts_equal(other.experiment_dict, self.experiment_dict)
             and dicts_equal(other.waves, self.waves)
             and self.pulse_map == other.pulse_map
         )
 
-    def replace_pulse(
-        self, pulse_uid: Union[str, Pulse], pulse_or_array: "Union[ArrayLike, Pulse]"
-    ):
+    def replace_pulse(self, pulse_uid: str | Pulse, pulse_or_array: ArrayLike | Pulse):
         """Permanently replaces specific pulse with the new sample data in the compiled
         experiment. Previous pulse data is lost.
 
         Args:
             pulse_uid: pulse to replace, can be :py:class:`~.dsl.experiment.pulse.Pulse`
                 object or uid of the pulse
             pulse_or_array: replacement pulse, can be
```

## laboneq/core/types/enums/high_pass_compensation_clearing.py

```diff
@@ -1,11 +1,18 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from enum import Enum, auto
 
 
 class HighPassCompensationClearing(Enum):
+    """High-pass compensation clearing.
+
+    .. deprecated:: 2.8
+
+        This has no functionality.
+    """
+
     LEVEL = auto()
     RISE = auto()
     FALL = auto()
     BOTH = auto()
```

## laboneq/core/utilities/replace_pulse.py

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import TYPE_CHECKING, Dict, List, Optional, Union
+from typing import TYPE_CHECKING
 
 import numpy as np
 from numpy.typing import ArrayLike
 
 from laboneq.compiler.common.pulse_parameters import decode_pulse_parameters
 from laboneq.core.exceptions.laboneq_exception import LabOneQException
 from laboneq.core.utilities.pulse_sampler import (
@@ -36,19 +36,19 @@
     IMAG = auto()
     COMPLEX = auto()
 
 
 def _replace_pulse_in_wave(
     compiled_experiment: CompiledExperiment,
     wave_name: str,
-    pulse_or_array: Union[ArrayLike, Pulse],
+    pulse_or_array: ArrayLike | Pulse,
     pwm: PulseWaveformMap,
     component: Component = Component.COMPLEX,
     is_complex: bool = True,
-    current_waves: Optional[List] = None,
+    current_waves: list | None = None,
 ):
     current_wave = None
     if current_waves is not None:
         current_wave = next(
             (w for w in current_waves if w["filename"] == wave_name), None
         )
     if current_wave is None:
@@ -148,34 +148,34 @@
 
 
 @dataclass
 class WaveReplacement:
     awg_id: str
     sig_string: str
     replacement_type: ReplacementType
-    samples: List[ArrayLike]
+    samples: list[ArrayLike]
 
 
 def calc_wave_replacements(
     compiled_experiment: CompiledExperiment,
-    pulse_uid: Union[str, Pulse],
-    pulse_or_array: Union[ArrayLike, Pulse],
-    current_waves: Optional[List] = None,
-) -> List[WaveReplacement]:
+    pulse_uid: str | Pulse,
+    pulse_or_array: ArrayLike | Pulse,
+    current_waves: list | None = None,
+) -> list[WaveReplacement]:
     if not isinstance(pulse_uid, str):
         pulse_uid = pulse_uid.uid
     pm = compiled_experiment.pulse_map.get(pulse_uid)
     if pm is None:
         _logger.warning("No mapping found for pulse '%s' - ignoring", pulse_uid)
         return []
 
-    replacements: List[WaveReplacement] = []
+    replacements: list[WaveReplacement] = []
     for sig_string, pwm in pm.waveforms.items():
         for awgs in compiled_experiment.wave_indices:
-            awg_wave_map: Dict[str, List[Union[int, str]]] = awgs["value"]
+            awg_wave_map: dict[str, list[int | str]] = awgs["value"]
             target_wave = awg_wave_map.get(sig_string)
             if target_wave is None:
                 continue
             wave_type: str = target_wave[1]
             is_complex = wave_type in ("iq", "complex")
             if wave_type == "single":
                 replacement_type = ReplacementType.I_Q
@@ -218,24 +218,29 @@
                     pulse_or_array,
                     pwm,
                     component=Component.COMPLEX,
                     is_complex=is_complex,
                     current_waves=current_waves,
                 )
             replacements.append(
-                WaveReplacement(awgs["filename"], sig_string, replacement_type, samples)
+                WaveReplacement(
+                    awg_id=awgs["filename"],
+                    sig_string=sig_string,
+                    replacement_type=replacement_type,
+                    samples=samples,
+                )
             )
 
     return replacements
 
 
 def replace_pulse(
-    target: Union[CompiledExperiment, Session],
-    pulse_uid: Union[str, Pulse],
-    pulse_or_array: Union[ArrayLike, Pulse],
+    target: CompiledExperiment | Session,
+    pulse_uid: str | Pulse,
+    pulse_or_array: ArrayLike | Pulse,
 ):
     """Replaces specific pulse with the new sample data.
 
     Args:
         target: CompiledExperiment or Session.
                 See CompiledExperiment.replace_pulse and Session.replace_pulse for details.
         pulse_uid: pulse to replace, can be Pulse object or uid of the pulse
```

## laboneq/dsl/laboneq_facade.py

```diff
@@ -5,15 +5,15 @@
 
 import atexit
 from typing import TYPE_CHECKING, Dict
 
 from numpy import typing as npt
 
 from laboneq import controller as ctrl
-from laboneq.compiler import Compiler
+from laboneq.compiler.workflow.compiler import Compiler
 from laboneq.core.types import CompiledExperiment
 
 if TYPE_CHECKING:
     from laboneq.dsl.experiment.pulse import Pulse
     from laboneq.dsl.session import Session
```

## laboneq/dsl/calibration/precompensation.py

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
+import warnings
 from dataclasses import dataclass, field
 from typing import List, Optional
 
 import numpy as np
 from numpy.typing import ArrayLike
 
 from laboneq.core.types.enums import HighPassCompensationClearing
@@ -30,20 +31,35 @@
     timeconstant: float = 1e-6
     #: Exponential filter amplitude
     amplitude: float = 0.0
 
 
 @dataclass
 class HighPassCompensation(Observable):
-    """Data object containing highpass filter parameters for the signal precompensation"""
+    """Data object containing highpass filter parameters for the signal precompensation.
+
+    .. versionchanged:: 2.8
+
+        Deprecated `clearing` argument: It has no functionality.
+    """
 
     #: high-pass filter time constant
     timeconstant: float = 1e-6
-    #: choose the clearing mode of the high-pass filter
-    clearing: HighPassCompensationClearing = HighPassCompensationClearing.RISE
+    #: Deprecated. Choose the clearing mode of the high-pass filter
+    clearing: HighPassCompensationClearing = field(default=None)
+
+    def __post_init__(self):
+        if self.clearing is not None:
+            warnings.warn(
+                "`HighPassCompensation` argument `clearing` will be removed in the future versions. It has no functionality.",
+                FutureWarning,
+            )
+        else:
+            self.clearing = HighPassCompensationClearing.RISE
+        super().__post_init__()
 
 
 @dataclass
 class FIRCompensation(Observable):
     """Data object containing FIR filter parameters for the signal precompensation"""
 
     #: FIR filter coefficients
```

## laboneq/dsl/experiment/experiment.py

```diff
@@ -33,23 +33,33 @@
     retval = f"exp_{experiment_id}"
     experiment_id += 1
     return retval
 
 
 @dataclass(init=True, repr=True, order=True)
 class Experiment:
+    """LabOne Q Experiment.
+
+    Args:
+        uid: UID of the experiment.
+        signals: Experiment signals.
+        version: Used DSL version.
+        epsilon: Epsilon. Not used.
+        sections: Sections in the experiment.
+    """
+
     uid: str = field(default_factory=experiment_id_generator)
     signals: Union[Dict[str, ExperimentSignal], List[ExperimentSignal]] = field(
         default_factory=dict
     )
     version: DSLVersion = field(default=DSLVersion.V3_0_0)
     epsilon: float = field(default=0.0)
     sections: List[Section] = field(default_factory=list)
     _section_stack: Deque[Section] = field(
-        default_factory=deque, repr=False, compare=False
+        default_factory=deque, repr=False, compare=False, init=False
     )
 
     def __post_init__(self):
         if self.signals is not None and isinstance(self.signals, List):
             signals_dict = {}
             for s in self.signals:
                 if isinstance(s, str):
```

## laboneq/dsl/result/results.py

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any
 
 from laboneq.core.exceptions import LabOneQException
 
 from ..calibration import Calibration
 from ..serialization import Serializer
 from .acquired_result import AcquiredResult
 
@@ -28,26 +28,26 @@
     #: The device setup on which the experiment was run.
     device_setup: DeviceSetup = field(default=None)
 
     #: The compiled experiment.
     compiled_experiment: CompiledExperiment = field(default=None)
 
     #: The acquired results, organized by handle.
-    acquired_results: Dict[str, AcquiredResult] = field(default=None)
+    acquired_results: dict[str, AcquiredResult] = field(default=None)
 
     #: List of the results of each user user function, by name of the function.
-    user_func_results: Dict[str, List[Any]] = field(default=None)
+    user_func_results: dict[str, list[Any]] = field(default=None)
 
     #: Any exceptions that occurred during the execution of the experiment. Entries are
     #: tuples of
     #:
     #: * the indices of the loops where the error occurred,
     #: * the section uid,
     #: * the error message.
-    execution_errors: List[Tuple[List[int], str, str]] = field(default=None)
+    execution_errors: list[tuple[list[int], str, str]] = field(default=None)
 
     def __eq__(self, other):
         if self is other:
             return True
         return (
             self.experiment == other.experiment
             and self.device_setup == other.device_setup
@@ -95,15 +95,15 @@
         Raises:
             LabOneQException: No result is available for the provided handle.
         """
 
         self._check_handle(handle)
         return self.acquired_results[handle].data
 
-    def get_axis_name(self, handle: str) -> List[Union[str, List[str]]]:
+    def get_axis_name(self, handle: str) -> list[str | list[str]]:
         """Returns the names of axes.
 
         Returns the list of axis names, that correspond to the dimensions of the result returned by
         'get'. Elements in the list are in the same order as the dimensions of the array returned by
         'get'. Each element is either a string for a simple sweep, or a list of strings for a parallel
         sweep. Values are given by the 'axis_name' argument of the corresponding sweep parameter, or
         the 'uid' of the same parameter, if 'axis_name' is not specified.
@@ -117,15 +117,15 @@
         Raises:
             LabOneQException: No result is available for the provided handle.
         """
 
         self._check_handle(handle)
         return self.acquired_results[handle].axis_name
 
-    def get_axis(self, handle: str) -> List[Union[ArrayLike, List[ArrayLike]]]:
+    def get_axis(self, handle: str) -> list[ArrayLike | list[ArrayLike]]:
         """Returns the axes grids.
 
         Returns the list, where each element represents an axis of the corresponding dimension of
         the result array returned by 'get'. Each element is either a 1D numpy array for a simple
         sweep, or a list of 1D numpy arrays for a parallel sweep. The length of each array matches
         the number of steps of the corresponding sweep, and the values are the sweep parameter
         values at each step.
@@ -140,15 +140,15 @@
         Raises:
             LabOneQException: No result is available for the provided handle.
         """
 
         self._check_handle(handle)
         return self.acquired_results[handle].axis
 
-    def get_last_nt_step(self, handle: str) -> List[int]:
+    def get_last_nt_step(self, handle: str) -> list[int]:
         """Returns the list of axis indices of the last measured near-time point.
 
         Returns the list of axis indices that represent the last measured near-time point. Use this
         to retrieve the last recorded partial result from the 'data' array. 'None' means that no
         measurements were taken so far. The list only covers axes that correspond to the near-time
         sweeps / dimensions. All the elements of inner real-time sweeps that correspond to a single
         real-time execution step are read at once and filled entirely.
@@ -163,15 +163,15 @@
             LabOneQException: No result is available for the provided handle.
         """
 
         self._check_handle(handle)
         return self.acquired_results[handle].last_nt_step
 
     @property
-    def device_calibration(self) -> Optional[Calibration]:
+    def device_calibration(self) -> Calibration | None:
         """Get the device setup's calibration.
 
         See Also:
             :py:meth:`DeviceSetup.get_calibration() <laboneq.dsl.device.device_setup.DeviceSetup.get_calibration>`
         """
         if self.device_setup is None:
             return None
```

## laboneq/dsl/serialization/serializer.py

```diff
@@ -98,16 +98,16 @@
             "laboneq.dsl.experiment",
             "laboneq.dsl.calibration.oscillator",
             "laboneq.dsl.calibration.signal_calibration",
             "laboneq.dsl.result.results",
             "laboneq.dsl.parameter",
             "laboneq.dsl.calibration",
             "laboneq.dsl.device",
-            "laboneq.dsl.device.qubits",
-            "laboneq.dsl.device.quantum_operations",
+            "laboneq.dsl.quantum.qubits",
+            "laboneq.dsl.quantum.quantum_operations",
             "laboneq.dsl.device.server",
             "laboneq.dsl.device.servers.data_server",
             "laboneq.core.types.enums",
             "laboneq.core.types.compiled_experiment",
             "laboneq.dsl.device.io_units.logical_signal",
             "laboneq.dsl.device.io_units.physical_channel",
             "laboneq.dsl.device.instruments",
```

## laboneq/openqasm3/openqasm3_importer.py

 * *Ordering differences only*

```diff
@@ -145,22 +145,22 @@
                     self._handle_include(child)
                 elif isinstance(child, ast.QuantumGate):
                     subsect = self._handle_quantum_gate(child)
                 elif isinstance(child, ast.Box):
                     subsect = self._handle_box(child)
                 elif isinstance(child, ast.QuantumBarrier):
                     subsect = self._handle_barrier(child)
-                elif isinstance(child, ast.QuantumReset):
-                    subsect = self._handle_quantum_reset(child)
                 elif isinstance(child, ast.DelayInstruction):
                     subsect = self._handle_delay_instruction(child)
                 elif isinstance(child, ast.ClassicalAssignment):
                     self._handle_assignment(child)
                 elif isinstance(child, ast.QuantumMeasurementStatement):
                     subsect = self._handle_measurement(child)
+                elif isinstance(child, ast.QuantumReset):
+                    subsect = self._handle_quantum_reset(child)
                 else:
                     msg = f"Statement type {type(child)} not supported"
                     raise OpenQasmException(msg, mark=child.span)
             except OpenQasmException:
                 raise
             except Exception as e:
                 msg = "Failed to process statement"
@@ -297,25 +297,14 @@
         return sect
 
     def _handle_include(self, statement: ast.Include) -> None:
         if statement.filename != "stdgates.inc":
             msg = f"Only 'stdgates.inc' is supported for include, found '{statement.filename}'."
             raise OpenQasmException(msg, mark=statement.span)
 
-    def _handle_quantum_reset(self, statement: ast.QuantumReset):
-        # Although ``qubits`` is plural, only a single qubit is allowed.
-        qubit_name = eval_expression(
-            statement.qubits, namespace=self.scope
-        ).canonical_name
-        try:
-            return self.gate_store.lookup_gate("reset", (qubit_name,))
-        except KeyError as e:
-            msg = f"Reset gate for qubit '{qubit_name}' not found."
-            raise OpenQasmException(msg, mark=statement.span) from e
-
     def _handle_delay_instruction(self, statement: ast.DelayInstruction):
         qubits = statement.qubits
         duration = eval_expression(statement.duration, namespace=self.scope, type=float)
         qubit_names = [
             eval_expression(qubit, namespace=self.scope).canonical_name
             for qubit in qubits
         ]
@@ -390,7 +379,18 @@
                     mark=statement.span,
                 ) from e
             s.add(gate_section)
 
             # Set the bit to a special value to disallow compile time arithmetic
             b.value = MeasurementResult()
         return s
+
+    def _handle_quantum_reset(self, statement: ast.QuantumReset):
+        # Although ``qubits`` is plural, only a single qubit is allowed.
+        qubit_name = eval_expression(
+            statement.qubits, namespace=self.scope
+        ).canonical_name
+        try:
+            return self.gate_store.lookup_gate("reset", (qubit_name,))
+        except KeyError as e:
+            msg = f"Reset gate for qubit '{qubit_name}' not found."
+            raise OpenQasmException(msg, mark=statement.span) from e
```

## laboneq/simulator/output_simulator.py

```diff
@@ -16,14 +16,15 @@
 
 
 @dataclass
 class OutputData:
     time: ArrayLike
     wave: ArrayLike = None
     trigger: ArrayLike = None
+    marker: ArrayLike = None
     frequency: ArrayLike = None
 
 
 @dataclass
 class _AWG_ID:
     is_out: bool
     prog: str
@@ -141,14 +142,15 @@
     def get_snippet(
         self,
         physical_channel: Union[str, PhysicalChannel],
         start: float,
         output_length: float,
         get_wave: bool = True,
         get_trigger: bool = False,
+        get_marker: bool = False,
         get_frequency: bool = False,
     ) -> OutputData:
         channel = (
             physical_channel
             if isinstance(physical_channel, PhysicalChannel)
             else self._uid_to_channel(physical_channel)
         )
@@ -158,21 +160,24 @@
         sim_targets = SimTarget.NONE
         if get_wave and awg_id.is_out:
             sim_targets |= SimTarget.PLAY
         if get_wave and not awg_id.is_out:
             sim_targets |= SimTarget.ACQUIRE
         if get_trigger and awg_id.is_out:
             sim_targets |= SimTarget.TRIGGER
+        if get_marker and awg_id.is_out:
+            sim_targets |= SimTarget.MARKER
         if get_frequency and awg_id.is_out:
             sim_targets |= SimTarget.FREQUENCY
         ws = WaveScroller(
             ch=awg_id.channels,
             sim_targets=sim_targets,
             sim=sim,
         )
         ws.calc_snippet(start, output_length)
         return OutputData(
             time=ws.time_axis,
             wave=ws.wave_snippet if awg_id.is_out else ws.acquire_snippet,
+            marker=ws.marker_snippet,
             trigger=ws.trigger_snippet,
             frequency=ws.frequency_snippet,
         )
```

## laboneq/simulator/seqc_parser.py

```diff
@@ -7,15 +7,15 @@
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from functools import lru_cache
 from types import SimpleNamespace
 
 # Note: The simulator may be used as a testing tool, so it must be independent of the production code
 # Do not add dependencies to the code being tested here (such as compiler, DSL asf.)
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any
 
 import numpy as np
 from numpy import typing as npt
 from pycparser.c_ast import (
     ID,
     Assignment,
     BinaryOp,
@@ -290,17 +290,17 @@
     awg_index: int
     measurement_delay_samples: int
     startup_delay: float
     sample_multiple: int
     sampling_rate: float
     output_port_delay: float
     source: str = None
-    channels: List[int] = None
-    wave_index: Dict[Any, Any] = None
-    command_table: List[Any] = None
+    channels: list[int] = None
+    wave_index: dict[Any, Any] = None
+    command_table: list[Any] = None
 
 
 class Operation(Enum):
     PLAY_ZERO = auto()
     PLAY_WAVE = auto()
     START_QA = auto()
     SET_OSC_FREQ = auto()
@@ -311,32 +311,32 @@
 
 
 @dataclass
 class SeqCEvent:
     start_samples: int
     length_samples: int
     operation: Operation
-    args: List[Any]
+    args: list[Any]
 
 
 @dataclass
 class WaveRefInfo:
     assigned_index: int = -1
-    wave_data_idx: List[int] = field(default_factory=list)
+    wave_data_idx: list[int] = field(default_factory=list)
     length_samples: int = None
 
 
 @dataclass
 class CommandTableEntryInfo:
-    abs_phase: Optional[float] = None
-    rel_phase: Optional[float] = None
-    abs_amplitude: Optional[float] = None
+    abs_phase: float | None = None
+    rel_phase: float | None = None
+    abs_amplitude: float | None = None
 
     @classmethod
-    def from_ct_entry(cls, ct_entry: Dict):
+    def from_ct_entry(cls, ct_entry: dict):
         d = {}
         if "phase" in ct_entry:
             # SHFSG
             incr = ct_entry["phase"].get("increment", False)
             if incr:
                 d["rel_phase"] = ct_entry["phase"]["value"]
             else:
@@ -383,28 +383,28 @@
             d["abs_amplitude"] = amplitude
 
         return cls(**d)
 
 
 @dataclass
 class SeqCSimulation:
-    events: List[SeqCEvent] = field(default_factory=list)
+    events: list[SeqCEvent] = field(default_factory=list)
     device_type: str = ""
-    waves: List[Any] = field(default_factory=list)
+    waves: list[Any] = field(default_factory=list)
     sampling_rate: float = field(default=2.0e9)
     startup_delay: float = field(default=0.0)
     output_port_delay: float = field(default=0.0)
 
 
 class SimpleRuntime:
     def __init__(
         self,
         descriptor: SeqCDescriptor,
         waves,
-        max_time: Optional[float],
+        max_time: float | None,
     ):
         self.predefined_consts = {
             "QA_INT_0": 0b1,
             "QA_INT_1": 0b10,
             "QA_INT_2": 0b100,
             "QA_INT_3": 0b1000,
             "QA_INT_4": 0b10000,
@@ -466,26 +466,29 @@
         self.variables = {}
         self.seqc_simulation = SeqCSimulation()
         self.times = {}
         self.times_at_port = {}
         self.descriptor = descriptor
         self.waves = waves
         self.source = preprocess_source(descriptor.source)
-        self.wave_lookup_by_args: Dict[Any, WaveRefInfo] = {}
-        self.wave_names_by_index: Dict[int, List[str]] = {}
-        self.wave_data: List[Any] = []
-        self.max_time: Optional[float] = max_time
+        self.wave_lookup_by_args: dict[Any, WaveRefInfo] = {}
+        self.wave_names_by_index: dict[int, list[str]] = {}
+        self.wave_data: list[Any] = []
+        self.max_time: float | None = max_time
         self._oscillator_sweep_config = {}
-        self._oscillator_sweep_params: Dict[str, Dict[int, float]] = {}
+        self._oscillator_sweep_params: dict[str, dict[int, float]] = {}
+        self._command_table_by_index = {
+            ct["index"]: ct for ct in self.descriptor.command_table
+        }
 
     def _last_played_sample(self) -> int:
         ev = self.seqc_simulation.events
         return ev[-1].start_samples + ev[-1].length_samples if len(ev) > 0 else 0
 
-    def _last_play_start_samples(self) -> Tuple[int, int]:
+    def _last_play_start_samples(self) -> tuple[int, int]:
         # Returns a time in samples and an index where the next point-in-time event
         # has to be positioned relative to the last time-span event. This is to support
         # the SeqC rule of point-in-time events (like startQA) be aligned with the start
         # of the preceding time-span event (like playWave).
         ev = self.seqc_simulation.events
         if len(ev) == 0:
             return 0, 0
@@ -515,15 +518,15 @@
         if name in self.predefined_consts:
             return self.predefined_consts[name]
         return self.variables[name]["value"]
 
     def _args2key(self, args):
         return tuple(tuple(a.items()) if isinstance(a, dict) else a for a in args)
 
-    def _update_wave_refs(self, wave_names: List[str], known_wave: WaveRefInfo):
+    def _update_wave_refs(self, wave_names: list[str], known_wave: WaveRefInfo):
         known_length = known_wave.length_samples  # make VSCode's code parser happy
         if known_length is not None:
             return
         for wave_name in wave_names:
             if wave_name is None:
                 known_wave.wave_data_idx.append(None)
                 continue
@@ -574,27 +577,38 @@
             elif known_wave.length_samples != wave_len:
                 raise Exception(
                     f"Inconsistent wave lengths {known_wave.length_samples} != {wave_len} in single 'playWave': {wave_names}"
                 )
 
     def _append_wave_event(
         self,
-        wave_names: List[str],
+        wave_names: list[str],
         known_wave: WaveRefInfo,
-        ct_info: Optional[CommandTableEntryInfo],
+        ct_info: CommandTableEntryInfo | None,
     ):
         self._update_wave_refs(wave_names, known_wave)
 
+        uses_marker_1 = any(
+            ["marker1" in wave for wave in wave_names if wave is not None]
+        )
+        uses_marker_2 = any(
+            ["marker2" in wave for wave in wave_names if wave is not None]
+        )
+
         time_samples = self._last_played_sample()
         self.seqc_simulation.events.append(
             SeqCEvent(
                 start_samples=time_samples,
                 length_samples=known_wave.length_samples,
                 operation=Operation.PLAY_WAVE,
-                args=[known_wave.wave_data_idx, ct_info],
+                args=[
+                    known_wave.wave_data_idx,
+                    ct_info,
+                    {"marker1": uses_marker_1, "marker2": uses_marker_2},
+                ],
             )
         )
 
     def assignWaveIndex(self, *args):
         idx = args[-1]
         wave_key = self._args2key(args[:-1])
         known_wave = self.wave_lookup_by_args.get(wave_key)
@@ -667,17 +681,15 @@
             # todo(JL): Find a better index via the command table offset; take last for now
             ct_index = self.descriptor.command_table[-1]["index"]
         elif ct_index == ZSYNC_DATA_PQSC_REGISTER_HD:
             assert self.descriptor.device_type == "HDAWG"
             # todo(JL): Find a better index via the command table offset; take last for now
             ct_index = self.descriptor.command_table[-1]["index"]
 
-        ct_entry = next(
-            iter(i for i in self.descriptor.command_table if i["index"] == ct_index)
-        )
+        ct_entry = self._command_table_by_index[ct_index]
         if "waveform" not in ct_entry:
             return  # todo: simulator does not yet support playZero via command table
 
         wave_index = ct_entry["waveform"]["index"]
         known_wave = WaveRefInfo(assigned_index=wave_index)
 
         wave = self.descriptor.wave_index[wave_index]
@@ -690,14 +702,18 @@
             wave_names = [
                 name + ".wave" if name is not None else None
                 for name in self.wave_names_by_index[wave_index]
             ]
         else:
             assert False, f"Unknown signal type: {wave['type']}"
 
+        for candidate_wave in self.waves.keys():
+            if wave["wave_name"] in candidate_wave and "marker" in candidate_wave:
+                wave_names.append(candidate_wave)
+
         ct_info = CommandTableEntryInfo.from_ct_entry(ct_entry)
 
         if latency is not None:
             time_samples = self._last_played_sample()
             corrected_latency = latency + EXECUTETABLEENTRY_LATENCY
             if corrected_latency * 8 < time_samples:
                 raise RuntimeError(
@@ -911,59 +927,65 @@
         if device["device_uid"] == device_uid:
             return device
     return None
 
 
 def analyze_recipe(
     recipe, sources, wave_indices, command_tables
-) -> List[SeqCDescriptor]:
-    outputs: Dict[str, List[int]] = {}
-    seqc_descriptors_from_recipe: Dict[str, SeqCDescriptor] = {}
+) -> list[SeqCDescriptor]:
+    outputs: dict[str, list[int]] = {}
+    seqc_descriptors_from_recipe: dict[str, SeqCDescriptor] = {}
     for init in recipe["experiment"]["initializations"]:
         device_uid = init["device_uid"]
         device = find_device(recipe, device_uid)
         device_type = device["driver"]
         sample_multiple = get_sample_multiple(device_type)
         try:
             sampling_rate = init["config"]["sampling_rate"]
         except KeyError:
             sampling_rate = None
         if sampling_rate is None or sampling_rate == 0:
             sampling_rate = get_frequency(device_type)
         startup_delay = -80e-9
         if device_type == "HDAWG" and "config" in init:
-            if "dio_mode" in init["config"]:
-                dio_mode = init["config"]["dio_mode"]
-                if dio_mode == "hdawg_leader":
-                    if sampling_rate == 2e9:
-                        startup_delay = -24e-9
-                    else:
-                        startup_delay = -20e-9
+            triggering_mode = init["config"].get("triggering_mode")
+            if triggering_mode == "desktop_leader":
+                if sampling_rate == 2e9:
+                    startup_delay = -24e-9
+                else:
+                    startup_delay = -20e-9
 
         # TODO(2K): input port_delay previously was not taken into account by the simulator
         # - keeping it as is for not breaking the tests. To be cleaned up.
-        input_channel_delays: Dict[int, float] = {
+        input_channel_delays: dict[int, float] = {
             i["channel"]: i["scheduler_port_delay"]  # + i.get("port_delay", 0.0)
             for i in init.get("inputs", [])
         }
 
-        output_channel_delays: Dict[int, float] = {
+        output_channel_delays: dict[int, float] = {
             o["channel"]: o["scheduler_port_delay"] + o.get("port_delay", 0.0)
             for o in init.get("outputs", [])
         }
 
         output_channel_precompensation = {
             o["channel"]: o.get("precompensation", {}) for o in init.get("outputs", [])
         }
 
         awg_index = 0
         if "awgs" in init:
             for awg in init["awgs"]:
-                seqc = awg["seqc"]
                 awg_nr = awg["awg"]
+                rt_exec_step = next(
+                    iter(
+                        r
+                        for r in recipe["experiment"]["realtime_execution_init"]
+                        if r["device_id"] == device_uid and r["awg_id"] == awg_nr
+                    )
+                )
+                seqc = rt_exec_step["seqc_ref"]
                 if device_type == "SHFSG" or device_type == "SHFQA":
                     input_channel = awg_nr
                     output_channels = [awg_nr]
                 else:
                     input_channel = 2 * awg_nr
                     output_channels = [2 * awg_nr, 2 * awg_nr + 1]
 
@@ -991,30 +1013,28 @@
                         precompensation_delay_samples(precompensation_info)
                         / sampling_rate
                     )
                     seqc_descriptors_from_recipe[
                         seqc
                     ].output_port_delay += precompensation_delay
 
-                channels: List[int] = [
+                channels: list[int] = [
                     output["channel"]
                     for output in init["outputs"]
                     if output["channel"] in output_channels
                 ]
                 if len(channels) == 0:
                     channels.append(0)
                 outputs[seqc] = channels
 
                 awg_index += 1
 
     seq_c_wave_indices = {}
     for wave_index in wave_indices:
-        wave_seq_c_filename = (
-            wave_index["filename"][: -len("_waveindices.csv")] + ".seqc"
-        )
+        wave_seq_c_filename = wave_index["filename"]
         if len(wave_index["value"]) > 0:
             seq_c_wave_indices[wave_seq_c_filename] = {}
             for wave_name, index_value in wave_index["value"].items():
                 seq_c_wave_indices[wave_seq_c_filename][index_value[0]] = {
                     "type": index_value[1],
                     "wave_name": wave_name,
                 }
@@ -1090,30 +1110,33 @@
         )
 
     return source
 
 
 def _analyze_compiled(
     compiled: CompiledExperiment,
-) -> Tuple[List[SeqCDescriptor], Dict[str, npt.ArrayLike]]:
+) -> tuple[list[SeqCDescriptor], dict[str, npt.ArrayLike]]:
     if isinstance(compiled, dict):
         compiled = SimpleNamespace(
             recipe=compiled["recipe"],
             src=compiled["src"],
             waves=compiled["waves"],
             wave_indices=compiled["wave_indices"],
         )
     seqc_descriptors = analyze_recipe(
-        compiled.recipe, compiled.src, compiled.wave_indices, compiled.command_tables
+        compiled.recipe,
+        compiled.src,
+        compiled.wave_indices,
+        compiled.command_tables,
     )
 
     read_wave_bin = lambda w: w if w.ndim == 1 else np.array([[s] for s in w])
     waves = {w["filename"]: read_wave_bin(w["samples"]) for w in compiled.waves}
     return seqc_descriptors, waves
 
 
-def simulate(compiled: CompiledExperiment, max_time=None) -> Dict[str, SeqCSimulation]:
+def simulate(compiled: CompiledExperiment, max_time=None) -> dict[str, SeqCSimulation]:
     seqc_descriptors, waves = _analyze_compiled(compiled)
-    results: Dict[str, SeqCSimulation] = {}
+    results: dict[str, SeqCSimulation] = {}
     for descriptor in seqc_descriptors:
         results[descriptor.name] = run_single_source(descriptor, waves, max_time)
     return results
```

## laboneq/simulator/wave_scroller.py

```diff
@@ -1,173 +1,352 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import math
 from enum import Flag
-from typing import List, Optional, Set, Tuple
+from typing import List, Optional, Set
 
 import numpy as np
 from numpy.typing import ArrayLike
 
 from laboneq.simulator.seqc_parser import (
     CommandTableEntryInfo,
     Operation,
     SeqCEvent,
     SeqCSimulation,
 )
 
 
+def _overlaps(a_start: int, a_length: int, b_start: int, b_length: int):
+    """Return True if the first and second sample intervals overlap.
+
+    Intervals that touch are considered to overlap.
+
+    Args:
+        a_start: The starting sample of the first interval.
+        a_length: The number of samples in the first interval.
+        b_start: The starting sample of the second interval.
+        b_length: The number of samples in the second interval.
+
+    Returns:
+        True if the intervals overlap. False otherwise.
+    """
+    a_end = a_start + a_length
+    b_end = b_start + b_length
+    return a_start <= b_end and b_start <= a_end
+
+
+def _slice_copy(
+    a: ArrayLike,
+    a_start: int,
+    b: ArrayLike,
+    b_start: int,
+    b_len: int,
+):
+    """Copy up to ``b_len`` samples from array ``b`` to array ``a`` without exceeding
+    the end of ``a`` and aligning the two arrays according to their starting samples.
+
+    Args:
+        a: An array-like to copy values to.
+        a_start: The starting sample of the destination array.
+        b: An array-like to copy values from.
+        b_start: The starting sample of the source array.
+        b_len: The maximum number of samples to copy from the source array.
+
+    Returns:
+        Nothing is returned. The destination array is modified inplace.
+    """
+    a_end = a_start + len(a)
+    b_end = b_start + b_len
+    if not (a_start < b_end and b_start < a_end):
+        # handle the case of intervals that don't overlap or only touch
+        return
+
+    left = max(a_start, b_start)
+    right = min(a_end, b_end)
+
+    a[left - a_start : right - a_start] = b[left - b_start : right - b_start]
+
+
+def _slice_add(
+    a: ArrayLike,
+    a_start: int,
+    b: ArrayLike,
+    b_start: int,
+    b_len: int,
+):
+    """Add up to ``b_len`` samples from array ``b`` to the corresponding entries from
+    array ``a`` without exceeding the end of ``a`` and aligning the two arrays according
+    to their starting samples.
+
+    Args:
+        a: An array-like to add values to.
+        a_start: The starting sample of the destination array.
+        b: An array-like to add values from.
+        b_start: The starting sample of the source array.
+        b_len: The maximum number of samples to copy from the source array.
+
+    Returns:
+        Nothing is returned. The destination array is modified inplace.
+    """
+    a_end = a_start + len(a)
+    b_end = b_start + b_len
+    if not (a_start < b_end and b_start < a_end):
+        # handle the case of intervals that don't overlap or only touch
+        return
+
+    left = max(a_start, b_start)
+    right = min(a_end, b_end)
+
+    a[left - a_start : right - a_start] += b[left - b_start : right - b_start]
+
+
+def _slice_set(a: ArrayLike, a_start: int, b, b_start: int, b_len: int):
+    """Set up to ``b_len`` samples in array ``a`` to value ``b`` without exceeding
+    the end of ``a`` and aligning the intervals according to their starting samples.
+
+    Args:
+        a: An array like to copy values to.
+        a_start: The starting sample of the destination array.
+        b: The value to set.
+        b_start: The starting sample of the source event.
+        b_len: The length of the source event.
+
+    Returns:
+        Nothing is returned. The destination array is modified inplace.
+    """
+    a_end = a_start + len(a)
+    b_end = b_start + b_len
+    if not (a_start < b_end and b_start < a_end):
+        # handle the case of intervals that don't overlap or only touch
+        return
+
+    left = max(a_start, b_start)
+    right = min(a_end, b_end)
+
+    a[left - a_start : right - a_start] = b
+
+
 class SimTarget(Flag):
     NONE = 0
     PLAY = 1
     ACQUIRE = 2
     TRIGGER = 4
     FREQUENCY = 8
+    MARKER = 16
 
 
 class WaveScroller:
     def __init__(
         self,
         *,
         ch: List[int],
         sim_targets: SimTarget,
         sim: SeqCSimulation,
     ):
         self.ch = ch
-        self.sim_targets = sim_targets
         self.sim = sim
 
         self.is_shfqa = sim.device_type == "SHFQA"
 
+        self.sim_targets = sim_targets
+
         self.wave_snippet = None
+        self.marker_snippet = None
         self.acquire_snippet = None
         self.trigger_snippet = None
         self.frequency_snippet = None
         self.time_axis = None
 
         self.last_trig_set_samples = 0
         self.last_trig = 0
         self.last_freq_set_samples = 0
         self.last_freq = np.nan
+        self.last_played_value = 0
         self.oscillator_phase: Optional[float] = None
 
         self.processors = {
             Operation.PLAY_WAVE: self._process_play_wave,
             Operation.PLAY_HOLD: self._process_play_hold,
+            Operation.PLAY_ZERO: self._process_play_zero,
             Operation.START_QA: self._process_start_qa,
             Operation.SET_TRIGGER: self._process_set_trigger,
             Operation.SET_OSC_FREQ: self._process_set_osc_freq,
         }
 
     def is_output(self) -> bool:
         return any(
             t in self.sim_targets
-            for t in [SimTarget.PLAY, SimTarget.TRIGGER, SimTarget.FREQUENCY]
+            for t in [
+                SimTarget.PLAY,
+                SimTarget.TRIGGER,
+                SimTarget.FREQUENCY,
+                SimTarget.MARKER,
+            ]
         )
 
-    def prepare(self, snippet_length: int):
+    def prepare(self, snippet_start_samples: int, snippet_length: int):
         if SimTarget.PLAY in self.sim_targets:
             if len(self.ch) > 1 or self.is_shfqa:
                 self.wave_snippet = np.zeros(snippet_length, dtype=np.complex128)
             else:
                 self.wave_snippet = np.zeros(snippet_length, dtype=np.float64)
         if SimTarget.ACQUIRE in self.sim_targets:
             self.acquire_snippet = np.zeros(snippet_length, dtype=np.uint8)
         if SimTarget.TRIGGER in self.sim_targets:
             self.trigger_snippet = np.zeros(snippet_length, dtype=np.uint8)
+        if SimTarget.MARKER in self.sim_targets:
+            self.marker_snippet = np.zeros(snippet_length, dtype=np.complex128)
         if SimTarget.FREQUENCY in self.sim_targets:
             self.frequency_snippet = np.full(snippet_length, np.nan, dtype=np.float64)
 
-    def target_events(self) -> Set[Operation]:
-        target_events: Set[Operation] = set()
+    def target_ops(self) -> Set[Operation]:
+        target_ops: Set[Operation] = set()
         if (
             SimTarget.ACQUIRE in self.sim_targets
             or SimTarget.TRIGGER in self.sim_targets
             or SimTarget.PLAY in self.sim_targets
             and self.is_shfqa
         ):
-            target_events.add(Operation.START_QA)
+            target_ops.add(Operation.START_QA)
         if SimTarget.PLAY in self.sim_targets and not self.is_shfqa:
-            target_events.add(Operation.PLAY_WAVE)
-            target_events.add(Operation.PLAY_HOLD)
+            target_ops.add(Operation.PLAY_WAVE)
+            target_ops.add(Operation.PLAY_HOLD)
+            target_ops.add(Operation.PLAY_ZERO)
         if SimTarget.TRIGGER in self.sim_targets:
-            target_events.add(Operation.SET_TRIGGER)
+            target_ops.add(Operation.SET_TRIGGER)
         if SimTarget.FREQUENCY in self.sim_targets:
-            target_events.add(Operation.SET_OSC_FREQ)
-        return target_events
+            target_ops.add(Operation.SET_OSC_FREQ)
+        return target_ops
 
     def _process_play_wave(self, event: SeqCEvent, snippet_start_samples: int):
+        channels = event.args[0]
         ct_info: CommandTableEntryInfo = event.args[1]
-        if len(self.ch) > 1:
+        if channels[self.ch[0] % 2] is None:
+            # A None for the first channel represents a FUNCTIONAL pulse
+            # which is not yet supported by the simulator
+            return
 
+        if len(self.ch) > 1:
             ct_abs_phase = ct_info.abs_phase if ct_info is not None else None
             ct_rel_phase = ct_info.rel_phase if ct_info is not None else None
             if ct_abs_phase is not None:
                 self.oscillator_phase = ct_abs_phase / (180 / math.pi)
             if ct_rel_phase is not None:
                 self.oscillator_phase = (
                     self.oscillator_phase or 0.0
                 ) + ct_rel_phase / (180 / math.pi)
-            wave = 1j * self.sim.waves[event.args[0][self.ch[1] % 2]]
-            wave += self.sim.waves[event.args[0][self.ch[0] % 2]]
 
-            # If the command table phase is set, assume that the signal is complex (rather than 2x real)
+            wave = 1j * self.sim.waves[channels[self.ch[1] % 2]]
+            wave += self.sim.waves[channels[self.ch[0] % 2]]
+
+            # If the command table phase is set, assume that the signal is complex
+            # (rather than 2x real)
             if self.oscillator_phase is not None:
                 wave *= np.exp(-1j * self.oscillator_phase)
+
         else:
-            wave = self.sim.waves[event.args[0][self.ch[0] % 2]]
+            wave = self.sim.waves[channels[self.ch[0] % 2]]
             # Note: CT phase not implemented on RF signals
+
         ct_abs_amplitude = ct_info.abs_amplitude if ct_info is not None else None
         if ct_abs_amplitude is not None:
             wave = wave * ct_abs_amplitude
-        wave_start_samples = event.start_samples - snippet_start_samples
-        self.wave_snippet[wave_start_samples : wave_start_samples + len(wave)] = wave
+
+        _slice_copy(
+            self.wave_snippet,
+            snippet_start_samples,
+            wave,
+            event.start_samples,
+            event.length_samples,
+        )
+        self.last_played_value = wave[event.length_samples - 1]
+
+        markers = event.args[2] if len(event.args) > 2 else {}
+
+        if markers.get("marker1"):
+            _slice_copy(
+                self.marker_snippet,
+                snippet_start_samples,
+                self.sim.waves[event.args[0][2]],
+                event.start_samples,
+                event.length_samples,
+            )
+
+        if markers.get("marker2"):
+            wave_arg_pos = 3 if event.args[2]["marker1"] else 2
+            _slice_add(
+                self.marker_snippet,
+                snippet_start_samples,
+                1j * self.sim.waves[event.args[0][wave_arg_pos]],
+                event.start_samples,
+                event.length_samples,
+            )
 
     def _process_play_hold(self, event: SeqCEvent, snippet_start_samples: int):
-        wave_start_samples = event.start_samples - snippet_start_samples
-        self.wave_snippet[
-            wave_start_samples : wave_start_samples + event.length_samples
-        ] = self.wave_snippet[wave_start_samples - 1]
+        _slice_set(
+            self.wave_snippet,
+            snippet_start_samples,
+            self.last_played_value,
+            event.start_samples,
+            event.length_samples,
+        )
+
+    def _process_play_zero(self, event: SeqCEvent, snippet_start_samples: int):
+        _slice_set(
+            self.wave_snippet,
+            snippet_start_samples,
+            0.0,
+            event.start_samples,
+            event.length_samples,
+        )
+        self.last_played_value = 0.0
 
     def _process_start_qa(self, event: SeqCEvent, snippet_start_samples: int):
         if SimTarget.PLAY in self.sim_targets and self.is_shfqa:
             self._process_shfqa_gen(event, snippet_start_samples)
         if (
             SimTarget.ACQUIRE in self.sim_targets
             or SimTarget.TRIGGER in self.sim_targets
         ):
             self._process_acquire(event, snippet_start_samples)
 
     def _process_shfqa_gen(self, event: SeqCEvent, snippet_start_samples: int):
         generator_mask: int = event.args[0]
+        if self.ch[0] < 0:
+            # The old_output_simulator sets ChannelInfo("QAResult", -1, SimTarget.ACQUIRE) to
+            # skip producing the SHFQA acquire play pulse, so we support that here too.
+            return
         if (generator_mask & (1 << self.ch[0])) != 0:
-            wave_start_samples = event.start_samples - snippet_start_samples
             wave = 1j * self.sim.waves[event.args[4][1]]
             wave += self.sim.waves[event.args[4][0]]
-            # TODO(2K): ensure wave doesn't exceed snippet boundary,
-            # as the wave length is not included in the event length
-            self.wave_snippet[
-                wave_start_samples : wave_start_samples + len(wave)
-            ] = wave
+            _slice_copy(
+                self.wave_snippet,
+                snippet_start_samples,
+                wave,
+                event.start_samples,
+                event.length_samples,
+            )
+            self.last_played_value = wave[event.length_samples - 1]
 
     def _process_acquire(self, event: SeqCEvent, snippet_start_samples: int):
         if SimTarget.ACQUIRE in self.sim_targets:
             integrator_mask: int = event.args[1]
             test_mask = 0xFFFF if self.ch[0] < 0 else (1 << self.ch[0])
             if (integrator_mask & test_mask) != 0:
                 measurement_delay_samples: int = event.args[2]
                 wave_start_samples = (
                     event.start_samples
                     - snippet_start_samples
                     + measurement_delay_samples
                 )
-                if wave_start_samples < len(self.acquire_snippet):
-                    self.acquire_snippet[wave_start_samples] = 1.0
+                if 0 <= wave_start_samples < len(self.acquire_snippet):
+                    self.acquire_snippet[wave_start_samples] = 1
         if SimTarget.TRIGGER in self.sim_targets:
             trigger_index = 5 if self.is_shfqa else 4
             if event.args[trigger_index] is None:
                 self._process_set_trigger(
                     SeqCEvent(event.start_samples, 0, Operation.SET_TRIGGER, [0]),
                     snippet_start_samples,
                 )
@@ -181,127 +360,106 @@
                     ),
                     snippet_start_samples,
                 )
 
     def _process_set_trigger(self, event: SeqCEvent, snippet_start_samples: int):
         value: int = int(event.args[0])
         wave_start_samples = event.start_samples - snippet_start_samples
-        if (
-            wave_start_samples <= len(self.trigger_snippet)
-            and self.last_trig is not None
-        ):
+        if 0 <= wave_start_samples <= len(self.trigger_snippet):
             self.trigger_snippet[
                 self.last_trig_set_samples : wave_start_samples
             ] = self.last_trig
-        self.last_trig_set_samples = wave_start_samples
+        self.last_trig_set_samples = max(0, wave_start_samples)
         self.last_trig = value
 
     def _process_set_osc_freq(self, event: SeqCEvent, snippet_start_samples: int):
         oscillator: int = event.args[0]
-        # TODO(2K): Track oscillator switching, currently osc 0 is hard-coded for Hw sweeps
+        # TODO(2K): Track oscillator switching, currently osc 0 is hard-coded for
+        #           Hw sweeps
         if oscillator == 0:
             frequency: float = event.args[1]
             wave_start_samples = event.start_samples - snippet_start_samples
-            if wave_start_samples <= len(self.frequency_snippet):
+            if 0 <= wave_start_samples <= len(self.frequency_snippet):
                 self.frequency_snippet[
                     self.last_freq_set_samples : wave_start_samples
                 ] = self.last_freq
-            self.last_freq_set_samples = wave_start_samples
+            self.last_freq_set_samples = max(0, wave_start_samples)
             self.last_freq = frequency
 
     def process(self, event: SeqCEvent, snippet_start_samples: int):
         processor = self.processors.get(event.operation)
         if processor is not None:
             processor(event, snippet_start_samples)
 
-    def trim(self, offset: int, length: int):
-        if self.wave_snippet is not None:
-            self.wave_snippet = self.wave_snippet[offset : offset + length]
-        if self.acquire_snippet is not None:
-            self.acquire_snippet = self.acquire_snippet[offset : offset + length]
+    def finalize(self):
         if self.trigger_snippet is not None:
             if self.last_trig_set_samples < len(self.trigger_snippet):
                 self.trigger_snippet[self.last_trig_set_samples :] = self.last_trig
-            self.trigger_snippet = self.trigger_snippet[offset : offset + length]
+
         if self.frequency_snippet is not None:
             if self.last_freq_set_samples < len(self.frequency_snippet):
                 self.frequency_snippet[self.last_freq_set_samples :] = self.last_freq
-            self.frequency_snippet = self.frequency_snippet[offset : offset + length]
 
     def calc_snippet(
         self,
         start_secs: float,
         length_secs: float,
-    ) -> Tuple[ArrayLike, ArrayLike]:
+    ):
         time_delay_secs = self.sim.output_port_delay if self.is_output() else 0.0
         time_delay_secs += self.sim.startup_delay
-        target_events = self.target_events()
         start_samples = int(
             np.round((start_secs - time_delay_secs) * self.sim.sampling_rate)
         )
         length_samples = int(np.round(length_secs * self.sim.sampling_rate))
+        if start_samples < 0:
+            # truncate any part of the interval that extends into negative
+            # sample counts (there are no events with negative samples)
+            length_samples = max(0, length_samples + start_samples)
+            start_samples = 0
         end_samples = start_samples + length_samples
 
-        def overlaps(a_start, a_length, b_start, b_length):
-            return (
-                min(a_start + a_length, b_start + b_length) - max(a_length, b_length)
-                != 0
-            )
-
-        max_event_idx = next(
-            (
-                i
-                for i, e in enumerate(self.sim.events)
-                if e.start_samples > start_samples + length_samples
-            ),
-            None,
-        )
+        # filter relevant events into events pre-interval and events that
+        # overlap the interval, keeping only the last of each kind of
+        # operation
+        pre_events = {}
+        interval_events = []
+        target_ops = self.target_ops()
+        for ev in self.sim.events:
+            if ev.start_samples > end_samples:
+                break
+            if ev.operation not in target_ops:
+                continue
+            if _overlaps(
+                start_samples,
+                length_samples,
+                ev.start_samples,
+                ev.length_samples,
+            ):
+                interval_events.append(ev)
+            else:
+                pre_events[ev.operation] = ev
+        pre_events = sorted(pre_events.values(), key=lambda ev: ev.start_samples)
 
-        events_in_window = [
-            ev
-            for ev in self.sim.events[:max_event_idx]
-            if overlaps(
-                start_samples, length_samples, ev.start_samples, ev.length_samples
-            )
-        ]
-        if len(events_in_window):
-            snippet_start_samples = min(ev.start_samples for ev in events_in_window)
-            snippet_length = (
-                max(
-                    # in case the last event had zero length, add one sample so that
-                    # for example a final setTrigger(0) can take effect and set the
-                    # last sample to 0
-                    ev.start_samples + (ev.length_samples or 1)
-                    for ev in events_in_window
-                )
-                - snippet_start_samples
+        # truncate sample length to the end of the last contained event
+        if interval_events:
+            ev_end = max(
+                ev.start_samples + (ev.length_samples or 1) for ev in interval_events
             )
+            end_samples = min(ev_end, end_samples)
+            length_samples = end_samples - start_samples
         else:
-            snippet_start_samples = start_samples
-            snippet_length = length_samples
+            end_samples = start_samples
+            length_samples = 0
 
-        op_events = [ev for ev in events_in_window if ev.operation in target_events]
-        self.prepare(snippet_length)
-
-        for ev in op_events:
-            self.process(ev, snippet_start_samples)
-
-        # clip to actually available samples, even if wider range requested
-        end_samples = min(end_samples, snippet_start_samples + snippet_length)
-        start_samples = max(0, start_samples)
-        length_samples = end_samples - start_samples
-        if length_samples <= 0:
-            return np.array([]), np.array([])
+        # prepare and populate the snippets
+        self.prepare(start_samples, length_samples)
+        for ev in pre_events:
+            self.process(ev, start_samples)
+        for ev in interval_events:
+            self.process(ev, start_samples)
+        self.finalize()
 
         exact_start_secs = start_samples / self.sim.sampling_rate + time_delay_secs
-        ofs = start_samples - snippet_start_samples
-
-        if ofs > 0:
-            self.trim(ofs, length_samples)
-        else:
-            self.trim(0, length_samples)
-            exact_start_secs -= ofs / self.sim.sampling_rate
-
         exact_length_secs = (length_samples - 1) / self.sim.sampling_rate
         self.time_axis = np.linspace(
             exact_start_secs, exact_start_secs + exact_length_secs, length_samples
         )
```

## Comparing `laboneq/dsl/device/quantum_operations.py` & `laboneq/dsl/quantum/quantum_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # SPDX-License-Identifier: Apache-2.0
 
 
 import uuid
 from os import PathLike
 from typing import Dict, Optional, Tuple, Union
 
-from laboneq.dsl.device.qubits import QuantumElement
 from laboneq.dsl.experiment.section import Section
+from laboneq.dsl.quantum.qubits import QuantumElement
 from laboneq.dsl.serialization import Serializer
 
 QuantumElementTuple = Tuple[QuantumElement, ...]
 
 
 class QuantumOperation:
     """A class for quantum operations."""
```

## Comparing `laboneq-2.7.0.dist-info/LICENSE` & `laboneq-2.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `laboneq-2.7.0.dist-info/METADATA` & `laboneq-2.8.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laboneq
-Version: 2.7.0
+Version: 2.8.0
 Summary: Zurich Instruments LabOne Q software framework for quantum computing control
 Author-email: Zurich Instruments Development Team <info@zhinst.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/zhinst/laboneq
 Keywords: quantum,sdk,zhinst
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -35,17 +35,20 @@
 Requires-Dist: openqasm3
 Requires-Dist: orjson
 Requires-Dist: pybase64
 Requires-Dist: pycparser
 Requires-Dist: python-box
 Requires-Dist: pyyaml
 Requires-Dist: requests
+Requires-Dist: rich
 Requires-Dist: rustworkx
 Requires-Dist: scipy
+Requires-Dist: sqlitedict
 Requires-Dist: sortedcollections
+Requires-Dist: lagom
 Requires-Dist: zhinst-core (==23.2.42414)
 Requires-Dist: zhinst-toolkit (~=0.5.0)
 Requires-Dist: zhinst-utils (~=0.3.0)
 
 ![LabOne Q logo](https://github.com/zhinst/laboneq/raw/main/docs/images/Logo_LabOneQ.png)
```

## Comparing `laboneq-2.7.0.dist-info/RECORD` & `laboneq-2.8.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,88 @@
-laboneq/VERSION.txt,sha256=-XIIQTG4wuupM59byVz22FGD6xsa-HxyPxLEhUL4REU,5
+laboneq/VERSION.txt,sha256=op_rvxnmr4MCu4de1UkQY6h1VcwBx-VceZAvgEHqxC8,5
 laboneq/__init__.py,sha256=OrHAykevakOnwEAHajG2qdB1PxEirEowKhDX2V5cHKA,239
 laboneq/_token.py,sha256=D2wS1TbZ6-CzF73l5kd6Wilcm18IPyymygB6VakHyRc,2829
 laboneq/_utils.py,sha256=4TRw9Hv192vqcPwcPDBsqXcdAGhIOvH_D24mZdyfZok,928
 laboneq/_version.py,sha256=zaxeCShR641vx5bH27_dVdirv71bA2i9ciFcH4A2krE,238
-laboneq/simple.py,sha256=aaLhD2w9pE3e89JUJVdiezHUuwsh4q2U5qx6bFTfJc0,1538
+laboneq/simple.py,sha256=PA8D5jqJYnNvSWb0LBZGWah4nNEA85Li0tWmZHbmwSY,1565
 laboneq/_observability/__init__.py,sha256=rcsPn8d52W6G9ZGkI8TPrEtwSJ2WbQN_Urc2DiIaUDg,184
 laboneq/_observability/tracing/__init__.py,sha256=rEFK2BFplAYa8ZHwQpiaVKv9EaSDrUWKHBplg-AmzGE,538
 laboneq/_observability/tracing/_noop_tracer.py,sha256=z7yhOOaTwCbWTQVQJ3i0SPCYsvd2wdbngf7ygoPJVCE,893
 laboneq/_observability/tracing/_tracer.py,sha256=vqgWJiy17tpzSMIOFXgkXHg9oQotbM8Jd-cWjNyVvk0,2309
+laboneq/application_management/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/application_management/application_manager.py,sha256=H8j88An67TfPUcyDwfj3IrLaxbYqwho5bL_yYuGXuaU,2658
 laboneq/compiler/__init__.py,sha256=PQOZ0TyWFSH0U7NJZnaYtO62iQW7DGgEV5KQD0lyKVw,444
 laboneq/compiler/fastlogging.py,sha256=SCJykQ5V_qvRPvWkkDZOqFexmazzhW-fbP2jkglOUkA,204
 laboneq/compiler/qccs-schema_2_5_0.json,sha256=YauxP1Z39AGXi5lUB7eKRLsRxsllayxNlzeyHQBGOSY,22524
 laboneq/compiler/remote.py,sha256=Fyb1RaWU-JBudPSv3LN56yQhYndduOchiai2brTE1WA,666
 laboneq/compiler/code_generator/__init__.py,sha256=s8ihwbuWxGpCAMjnsBXQ0kdoXGqT-B8doSsk850gQA0,654
-laboneq/compiler/code_generator/analyze_events.py,sha256=xA7nDePKXzxQHeR4m95cOmN0CBTR6KY5T3mccT7bBM8,18645
-laboneq/compiler/code_generator/analyze_playback.py,sha256=dcRfLFAltlXyGbQIGtb_YAl-8sdkx4GLAYf37a837pE,26665
-laboneq/compiler/code_generator/code_generator.py,sha256=kEqAX0xdjbmMffH6JkoCnIFeyKnhJxhyAYIJO_uOTvI,72652
+laboneq/compiler/code_generator/analyze_events.py,sha256=Ohg_gOZul-azPbaK1XVXDffSDEaLzj5i-EZ2SAYiVWg,18669
+laboneq/compiler/code_generator/analyze_playback.py,sha256=F7H8nLlO2LsNFsedP5-j-afsem6II5cUrF8qtH-RUoI,26669
+laboneq/compiler/code_generator/code_generator.py,sha256=yVE7FT4BDItQZsY_P3j4ziNo1saqRuEMxIgNeN0_X_4,71964
 laboneq/compiler/code_generator/command_table_tracker.py,sha256=jXD4Ep8SMIgS_DNqgdfnGujma-oRhRZcvFcIa-AkAXc,4026
 laboneq/compiler/code_generator/compressor.py,sha256=sIbtla_ju0NM1FL1oWGV7SMyxpZoNKwMzHKvbyb3Ut8,2880
 laboneq/compiler/code_generator/feedback_register_allocator.py,sha256=iXuwHFa9g5YQriNqLHXoHIzkBanyR8XnD9C0mw6sPQU,1414
 laboneq/compiler/code_generator/interval_calculator.py,sha256=7dyk02iUdPHyzS4DU6JvkTKn36yWpUE2lhvUynY0aYQ,10355
 laboneq/compiler/code_generator/measurement_calculator.py,sha256=w15OoQt0yXR4k3V2nvJT2CoNGtrPDeCiPoQazk5TZFc,17825
 laboneq/compiler/code_generator/sampled_event_handler.py,sha256=f5GlIAKgVDSST-nS7MpR93im0LvlbjpOYPOlZa0tLzA,30380
-laboneq/compiler/code_generator/seq_c_generator.py,sha256=oZ4-TzXQmrfYToNnRe-GPQa0A9ctlE4y2JsWj2yf918,19239
+laboneq/compiler/code_generator/seq_c_generator.py,sha256=cdaWiqI6rgg-xR_oY5qYNVW5AVfgaCk7Zawk7jFr-BE,18722
 laboneq/compiler/code_generator/seqc_tracker.py,sha256=bZPvLecbCXYH02TlTL7KkhOv6NXoMHOmS_kLZE9WzO8,6333
-laboneq/compiler/code_generator/signatures.py,sha256=A36tVPg7xJkTNPtvc0cF8KSCYYHVtfphyQqjqpQN0xs,9915
+laboneq/compiler/code_generator/signatures.py,sha256=fQWI4maz7IPPMexBPWLsU0dhhQqlVvnQhupGUG9w0Ns,10031
 laboneq/compiler/code_generator/utils.py,sha256=KJtRJg6wE8FPALrG4B8H7GRZa_7WqOrXroWW8kgSdBA,3500
-laboneq/compiler/code_generator/wave_compressor.py,sha256=BoCX_EAg6TN8VnTMPJIcP4JWX8QzhZnl4EMYw1m-yh8,7697
+laboneq/compiler/code_generator/wave_compressor.py,sha256=Wfg7pB_YsjeSPBso8C1kExSUSES82Y2VCDjbOMTyVA0,9102
 laboneq/compiler/code_generator/wave_index_tracker.py,sha256=700LQq60nX9Btcn9bj2SDn674qRmsxy_Nz6yy0qx1Y0,1476
 laboneq/compiler/common/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
 laboneq/compiler/common/awg_info.py,sha256=djhjq5t8JruHRi9hKk4rtBVH4KfMWRkuamcypmhP6WA,1093
 laboneq/compiler/common/awg_sampled_event.py,sha256=Sz21qx__YTdkpeBAhpfyVgT4ED1zUR4OiIn6GTnNVvw,1926
 laboneq/compiler/common/awg_signal_type.py,sha256=aXiZ_K-yaG1pPPUMh5IpOXn2rQJngQnTzwqP1LExtT8,480
 laboneq/compiler/common/compiler_settings.py,sha256=1Rr42CsHTmKtykUgOQuu0H56jCV4cGHAgoMb0nVuPFM,4015
 laboneq/compiler/common/device_type.py,sha256=QK48fFIH9-bcO25j6l4d-WrG1kpyapoTEZvHLzzsffI,6058
 laboneq/compiler/common/event_type.py,sha256=uFnpVFeUU9m-dEBgNzmo3Sj8SSoLwFOj9i_Wk37Kk2M,1624
 laboneq/compiler/common/play_wave_type.py,sha256=9olrAuZqSSq-3fDpUCwbH2IC2F1mYaZ64H_NG0J6eXM,229
 laboneq/compiler/common/pulse_parameters.py,sha256=zhIljy4MHaBGSFYR-28ksDetM39C5p006e8flU21ZWE,580
-laboneq/compiler/common/signal_obj.py,sha256=UBrf78oTS_MyH3YaPZudNqDvFJzoY5_Fw-MJIUcOXVA,2594
+laboneq/compiler/common/signal_obj.py,sha256=87PUbOLhI4vdpDdRTUYWNJK275tkozTPM0BPShROlNU,2541
 laboneq/compiler/common/trigger_mode.py,sha256=PfV_HskFUlk99bsngdjYz-b137e2qA6e1TNqA0Bjvbs,400
 laboneq/compiler/experiment_access/__init__.py,sha256=mb9ULouZiKIforKo2d458L6pvf0LmV4PXhmKhPBUj7g,154
 laboneq/compiler/experiment_access/acquire_info.py,sha256=bQrMObuyxABUpGTc0ubuUvOs15KzKJzos1dPw4B_PYs,222
 laboneq/compiler/experiment_access/device_info.py,sha256=HQBj1WpSt8TwHX5G_kE-1m5ulJ06-j_hdIIVamxHQDI,349
-laboneq/compiler/experiment_access/dsl_loader.py,sha256=_IIG-VcRcTpUILehAFyRoin4Qpq9eVnOHvY8nvvYMVc,45262
-laboneq/compiler/experiment_access/experiment_dao.py,sha256=Gn_2_3ZMCG8TLnA0Zv0rMD6NAvWXwUxE5eXBWCndKo4,16767
-laboneq/compiler/experiment_access/json_dumper.py,sha256=YNDUHHachBzw0-4FmCRQzMTeR5ys61xPaRgpvQoeQfg,14264
-laboneq/compiler/experiment_access/json_loader.py,sha256=4tK59zHBocRlaXcyBHQYjtMFJivsM9IHWfJ-P1txyVI,21043
-laboneq/compiler/experiment_access/loader_base.py,sha256=FEFxOs-_tS8ZMbLRAeaY7jDkFV6EmJvgxoKirI7kFo8,6182
+laboneq/compiler/experiment_access/dsl_loader.py,sha256=qakMUQYeSGZaH9NqN1bDSkDNvlnfnYoQ-oGS0S2QLU8,45124
+laboneq/compiler/experiment_access/experiment_dao.py,sha256=qJhN9vRGl0GYsIfBc8xuBxM4aR4-4jFYIkAOvFhsCmU,16726
+laboneq/compiler/experiment_access/json_dumper.py,sha256=jjVvU-2PPdF9avWQGkkK4IrhFmT20FojgbURa9EfQ5Q,14122
+laboneq/compiler/experiment_access/json_loader.py,sha256=XY7srlHpGcByKLJ8Btn3GRQr9Wx16i4dBVjPWUAa6EQ,20825
+laboneq/compiler/experiment_access/loader_base.py,sha256=YU27dCvNy3JRApvbtqmL6x4w36cZzJZjwyjg4dJwP2Y,6256
 laboneq/compiler/experiment_access/marker.py,sha256=2Okj9Q_Ukk02B-Z7_WDM6nHN-nuXw3qFjUNaw8LUMsI,270
 laboneq/compiler/experiment_access/oscillator_info.py,sha256=VvEyOttSTDd7-oxpbim4xmPJUwYEzjrsDXup9xLwI0k,286
 laboneq/compiler/experiment_access/param_ref.py,sha256=wqyyzAiSIEu2GVeNdZc-MtvdhdSDp1Quch8qBVIPppw,197
 laboneq/compiler/experiment_access/pulse_def.py,sha256=wC192cXc_oxtxj-xJS2tY2dHkDr_CAYrtIkcp45gj6E,1311
-laboneq/compiler/experiment_access/section_info.py,sha256=vRIw7KvrlNhXjh8ynUjGUer_DVJPxdo9FGBdDMWVuUY,851
+laboneq/compiler/experiment_access/section_info.py,sha256=4QCszplfb3FiWWqQZWLMkvc1yythBkpqu_6HdA0Sw0c,817
 laboneq/compiler/experiment_access/section_signal_pulse.py,sha256=ZGgbvNW3v-qIgyvcW34Lk31hyhFeNb_UjE6uIUXd8os,1069
 laboneq/compiler/experiment_access/signal_info.py,sha256=HLkN-Kq2vZrh5tg92RA3ZSSYaiRXXQecw01-NtXGR_Q,387
 laboneq/compiler/scheduler/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
 laboneq/compiler/scheduler/case_schedule.py,sha256=HwzkOLBBYQip5bDBxNApQnGITb5cgyLVsYezwhxCdCQ,3265
 laboneq/compiler/scheduler/interval_schedule.py,sha256=tp4CauVPr-hOXxtzvUQYZrmXcqJBY7UqQDPlDDo1S_0,7439
 laboneq/compiler/scheduler/loop_iteration_schedule.py,sha256=5RKVr5tmtYqcGx8DY_kichm2rjeHtXbMrthFzwzFE9U,3327
 laboneq/compiler/scheduler/loop_schedule.py,sha256=RUFiK0sMisFwB1NVL1fAphcxKGMjB1f0ZpMPAf5-_fk,8576
-laboneq/compiler/scheduler/match_schedule.py,sha256=MAvUzVbiMd5Zn9IWF4krOmoNElI5fE6MrF33hA6bk-Q,10452
+laboneq/compiler/scheduler/match_schedule.py,sha256=U67d7l60-qetl9v7BEaX3rbQvlzzfMLNYZ7fZAYC3rQ,10468
 laboneq/compiler/scheduler/oscillator_schedule.py,sha256=Iykf3E3wT7xXuH-hVk9_MwTHM7eWQFmhR3JzzQTd1eM,2248
 laboneq/compiler/scheduler/phase_reset_schedule.py,sha256=yLyoKe5S57LGcPMcgFxsBDyKjPROgCUdASTSPU-fQog,1761
 laboneq/compiler/scheduler/preorder_map.py,sha256=luqooLzAEbK2b0j8TIDcHsE3riHA_GFyhcSRerHUFUk,1808
 laboneq/compiler/scheduler/pulse_phase.py,sha256=poXl-PKFIO7X_xN3Qjqo-NWC-svaom3dWjetfKEsw8c,3821
 laboneq/compiler/scheduler/pulse_schedule.py,sha256=im2DdPgi2Q4pQq4Q-YnApyZyi04888iSOq03BRrzNds,6958
 laboneq/compiler/scheduler/reserve_schedule.py,sha256=WM-fLfdDnViVwB5U0TrrkiDKB0s3DSw3yUFLC5vyvQU,621
 laboneq/compiler/scheduler/root_schedule.py,sha256=2ErHbKUaD8f6xp42UdoCSaQ5AeZc5n4PNHaluspKRcE,1367
 laboneq/compiler/scheduler/sampling_rate_tracker.py,sha256=taR4AdTTaYNXfaEgM5hZNhL2VbcGnJCkx9gt4xAJg9E,1949
 laboneq/compiler/scheduler/schedule_data.py,sha256=f1m_AVtgmeOJ5nYgFw91OeCWauqB28MyewEovnNHkdw,1115
-laboneq/compiler/scheduler/scheduler.py,sha256=niev6cb8MQtcS4LuOd6icsZ-QUpI9U_GUiLGj1XTZk4,41127
+laboneq/compiler/scheduler/scheduler.py,sha256=rbrWG2msZJ-wigS4uvDSatqsUT_UOB2JnA_pdTrZjNs,41072
 laboneq/compiler/scheduler/section_schedule.py,sha256=UruX04LNrMUUAUoJ3RooT3zSquPW5Atfa18ds6n8sWw,13191
 laboneq/compiler/scheduler/utils.py,sha256=buFGd2oxNFr3hfGc8fx_dyMCbxTwimiSOuxCqeqSDRk,757
 laboneq/compiler/workflow/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
-laboneq/compiler/workflow/compiler.py,sha256=5ArB-ijAEEqmpMm6FAX0wUdaBrr5L8lUWs3seosGZzA,51030
+laboneq/compiler/workflow/compiler.py,sha256=RnTQKjJ7Et5MhjwjXz5v2Soqf5fqrl4-MGFhXLavHnA,47515
 laboneq/compiler/workflow/precompensation_helpers.py,sha256=dpRw6dGJcsDAv0uI48cfzso75IYHNVfP1NUkRhD-giI,12424
-laboneq/compiler/workflow/recipe_generator.py,sha256=lekirVjI87CDhXcWCfOwJpsSgek91DJGf9G2WyjEeh8,12522
+laboneq/compiler/workflow/realtime_compiler.py,sha256=6Qjl4z2xkbmnbRZY2MeMB6-CSGuWrhZOd0SJeJyMd0g,6847
+laboneq/compiler/workflow/recipe_generator.py,sha256=g9CzZEkX5Vfctu5j0iSr5K1_ZbxviumqLnVrqrsU0Qo,12441
 laboneq/contrib/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/bloch_simulator_pulse_plotter/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/bloch_simulator_pulse_plotter/inspector/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/bloch_simulator_pulse_plotter/inspector/update_inspect.py,sha256=dII-ZVAa3HumwKfHYGiARVBDCjaqJhGFy55XAjOPiaM,4511
 laboneq/contrib/bloch_simulator_pulse_plotter/plotter/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/bloch_simulator_pulse_plotter/plotter/plot_funs.py,sha256=3RjtFb3sxYokBP92COK53gCmBrCk9ubs8_xOb75fem4,3379
 laboneq/contrib/bloch_simulator_pulse_plotter/pulse_simulator/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
@@ -96,99 +99,112 @@
 laboneq/contrib/example_helpers/descriptors/hdawg_uhfqa_pqsc.py,sha256=CzjRnXjw4v_WMtSvY5xZbmLztyEHfAQlzMbgvZ8cAmE,956
 laboneq/contrib/example_helpers/descriptors/shfqc.py,sha256=Vu_W7gf5XigJBTq3QZV8u-mAVXt560OFbuIiNCX_G10,1887
 laboneq/contrib/example_helpers/descriptors/shfsg.py,sha256=aWkqMMBq90JCPAj0-uZadDEMziln_OsqxZSFBJpsf-E,1639
 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_hdawg_pqsc.py,sha256=ztHPSen0jfWqWzifanf-TmyXZ7P_R5-ssKXfOD_ASzo,2472
 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_pqsc.py,sha256=cH9gx4th7Gh_oC72Fs0U3XQL1DUW3ownAv3BYsJ4PnA,2160
 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_shfqc_hdawg_pqsc.py,sha256=PIPiyvyyMv9wwcKBf81xFhF1Pflol2WrS5fkfb21EKU,2708
 laboneq/contrib/example_helpers/plotting/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
-laboneq/contrib/example_helpers/plotting/plot_helpers.py,sha256=xvozYqVwDGKR6xnHaYBLxN4m5Hu3XqEi9In9vAIfJ5Q,11127
+laboneq/contrib/example_helpers/plotting/plot_helpers.py,sha256=yYgexGfC12FehKFFDro_uuAjKuEaKz_zvZRJFTAOcIY,12182
 laboneq/controller/__init__.py,sha256=gPuU9BwcRA-VFMRLtIzd9Y-KvLQhYv0czaGuo-uimjc,308
 laboneq/controller/attribute_value_tracker.py,sha256=Q-PznOOJHYue9gCwxM8bktkZse4FSGJcNrJINBqjItM,3380
 laboneq/controller/cache.py,sha256=sI4qtTQurYPWzMp7iW1oKwQp_GVftQX9isDkTNZ-bDE,1479
 laboneq/controller/communication.py,sha256=K-9sn7UABcGb9hGLM_8tLYtKWbNeSvUqcoubnBUTcvk,13604
-laboneq/controller/controller.py,sha256=SW_AQlq9In4iYVmyC6e1oD4yIa5a6P0ZHivzoMM-mEo,34028
+laboneq/controller/controller.py,sha256=UatTQTmZqF66kgNraEvp0QlLoSKMhTj1fnSALgkMasQ,30852
 laboneq/controller/laboneq_logging.py,sha256=9S7qvoF2MzOvw-BQLpHi7sLSe0v-xoAo0P0I_mbCPLU,4892
+laboneq/controller/near_time_runner.py,sha256=0RsFuXKbOShRpPInWW3BfscGEYZdFX8-qb3znqu0YpA,4671
 laboneq/controller/protected_session.py,sha256=v4T5NsQxE57E22hJltIumOnLAoBms0D7ZTtUYjGHGGM,337
-laboneq/controller/recipe_1_4_0.py,sha256=8T6XdPHMw0KBMP7Hx1c1z88dH82ms-PqiDTX5a-InBc,15188
-laboneq/controller/recipe_enums.py,sha256=uNjZPJci2KCleSh2zNYTOkUEfBpBK0spOU16GvaWj6Y,638
-laboneq/controller/recipe_processor.py,sha256=HJf4INxd56JHtP3sahnc1k7a2NtENn_hjemZCDOKeWs,21249
-laboneq/controller/results.py,sha256=b9Oy_F0GqSzHulNSWqt6ltUzXpYZ4JmC0BVIE176Qzc,1917
+laboneq/controller/recipe_1_4_0.py,sha256=csiCQdbuH-buQVpjJlmsqnRqfRrAT3VH7jU8UerUoII,12301
+laboneq/controller/recipe_enums.py,sha256=Tzp88VZKEmOUe5j9Z3Sq5FXRQhOhrdEa4lZwsmHFNbQ,529
+laboneq/controller/recipe_processor.py,sha256=HtOwKlubHuzzYJnvx4CefNTawjMFcJg9LQby3-GDpv0,21441
+laboneq/controller/results.py,sha256=S3eZ2xrXt2tly2M9TCrOstazN9oWNwB9xf0wDJJ-7go,1902
 laboneq/controller/toolkit_adapter.py,sha256=moZzwjnRUUbyT-7JL31EBtBh39VD3USx1SRolFS8v-g,1594
 laboneq/controller/util.py,sha256=fi5_nCRrmORASGaFlge4TN6gXAWZIiS0pinr9-DVjnA,1178
 laboneq/controller/versioning.py,sha256=IcmXytxA6OtbudyM2aK8gCgWLcuLbweru5wIafolpnU,281
 laboneq/controller/devices/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
-laboneq/controller/devices/device_collection.py,sha256=3NAj2v2Htyaofh-qoOQOsSMJPzFnb1y6z0PwVV48P7g,15391
+laboneq/controller/devices/device_collection.py,sha256=w6jA90eMIXZDcXXp85y12ekc3DoQwzclPSmaYWszRD0,15692
 laboneq/controller/devices/device_factory.py,sha256=CQmdrldqyhI7wCFw2aObszp9g3XhPaJZv9Y8U_VAdMY,1275
-laboneq/controller/devices/device_hdawg.py,sha256=9aSNOUIakFdAkEGSH4i5pZur4tL8FJ4iS1oCKkC9Y_w,24523
+laboneq/controller/devices/device_hdawg.py,sha256=H04dHZgNIsQBBp6XWKJSU9sBmDE4LFV2AyLTDUtGfP0,24400
 laboneq/controller/devices/device_nonqc.py,sha256=m1rpD0XgwgNChmIkzdOBFiyg4bbPWY-1b0ysrMLqLNs,491
-laboneq/controller/devices/device_pqsc.py,sha256=FkH6ZaKqQDoX_WmROL1czc_dTU5DP0nU6IkqShA30fo,8115
-laboneq/controller/devices/device_setup_dao.py,sha256=daW-WJHaqCuxxNF3Wtnzr0_ebL2X9cYo-WHTv_U0Bas,4137
-laboneq/controller/devices/device_shfppc.py,sha256=hUEGLYpFt4JHhmaR1NQvljlxU-8YxopEEnlKpm6Fg4Q,4344
-laboneq/controller/devices/device_shfqa.py,sha256=OsiHvUQ1EsiW5eMOQfGjq8kwjcCSGfvWMmDlxmR5v6c,42895
-laboneq/controller/devices/device_shfsg.py,sha256=1ThT7CgWXZkaH7O8PtXmPoIxQgNL2fBKX5d8Lju8FXw,21719
-laboneq/controller/devices/device_uhfqa.py,sha256=u1II0KmVXAnoWh7TLUhL139CkI8F9mdl5MRHJIdAa44,29618
-laboneq/controller/devices/device_zi.py,sha256=8aBRy3IMbTBl8bhWs5YEvDyowNwtsIzFhb5pTyVUPU8,37660
-laboneq/controller/devices/zi_emulator.py,sha256=Y2uZuFe020_fmG8fG_dyFk6HlUpK36fxwG6hrBMr4Lk,29590
+laboneq/controller/devices/device_pqsc.py,sha256=6HVcljbJvEpspB19rzzsbcXTXJRlbzYSNfNqWLa_R2E,7898
+laboneq/controller/devices/device_setup_dao.py,sha256=9XsGUnPALiOyg9T2ZB9TvTpA-VsdkMqkhoXbX3Yv-kc,4441
+laboneq/controller/devices/device_shf_base.py,sha256=V3dMo8SU2i3_MWDKNunQs0T1YI_jkX5Gs3xYcw1b2SE,2064
+laboneq/controller/devices/device_shfppc.py,sha256=nYaF3Q4DDGBdr0V2-jV1qqLHviVZ4OFbzg-6xcjn9_g,4408
+laboneq/controller/devices/device_shfqa.py,sha256=gS4UVg9kchX3pWK3lXozaDkkH2EcNxmDJAAZ0mFOJ3M,41523
+laboneq/controller/devices/device_shfsg.py,sha256=XRhQf9auynSLRtuHdLX38XttcpYsPw0bZZ_a5n6hiG8,20499
+laboneq/controller/devices/device_uhfqa.py,sha256=rS3FKel5Jby3ckwpgiAG0xbIsM_xuYxeHchWh_BvWYo,29497
+laboneq/controller/devices/device_zi.py,sha256=0T7obImVmWhI0g5IU2K_w3K2CMzoG817s8iNE8tl6JY,32396
+laboneq/controller/devices/zi_emulator.py,sha256=9zaa72zvCrHnCwFFV7JwklmB9d2QiuIs2VO8cUcvkho,29980
 laboneq/controller/devices/zi_node_monitor.py,sha256=2N2Q79sP-USY9-ovk5DHOXiO6Sov9QSzBGqdsyAPnuA,10358
 laboneq/core/__init__.py,sha256=nx0-aqsC4hdoO7jIj0Ut7yNTQbe5dme7jodU9wkd4N4,97
 laboneq/core/path.py,sha256=ZDMafOg44r5I3T-sW-iY6j7xrjYMbx12UsLoqbhg3Vw,2015
 laboneq/core/validators.py,sha256=pmtl8RdlBr-49CkxJseW1VrDtJU2gqLVBWSZdLrRpWc,1338
 laboneq/core/exceptions/__init__.py,sha256=8ZaME3lWkRJ7BZw1qVWGbt91jaklPd67iyIZ-zXoBpE,126
 laboneq/core/exceptions/laboneq_exception.py,sha256=bWRVbnLJiBszdNeEglRFp-z1Q3bb-irTIzf2vgTaBK0,123
 laboneq/core/serialization/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
 laboneq/core/serialization/simple_serialization.py,sha256=03qj5sZYadGGsqmd7qyCGmDizeRr8d91edo2Er6FT1Y,19090
 laboneq/core/types/__init__.py,sha256=fvF9SQu_JVfxc3et0G1RWE-FZvliRnYc_m6Ym6oavto,161
-laboneq/core/types/compiled_experiment.py,sha256=UNEhjGizBsy8pKOxCyKdeFLX4G3t-Y9oFjuaMR7vezI,5169
+laboneq/core/types/compiled_experiment.py,sha256=lozDc0EIOQX1iUuFSIyHPAdnjYj4izPnuSNtwLjbEHA,5075
 laboneq/core/types/uid.py,sha256=bly72s6lGrQLYLJ3sk-vjJgzGhbLLYuQ87HMR9BOG9I,1473
 laboneq/core/types/enums/__init__.py,sha256=RfmSFJUHNxbqCeYHZWeg9Vl5wAA9u8k-_LDMTOTBbmM,660
 laboneq/core/types/enums/acquisition_type.py,sha256=PpK4El9Gvmt7ojw6tCcTSkfrDkJxmpvZyE2wbkPooLg,934
 laboneq/core/types/enums/averaging_mode.py,sha256=skosaedPnNxrW_UGRpksM1uiT7tCRLNx-9I3SuvdlMY,213
 laboneq/core/types/enums/carrier_type.py,sha256=PEbKKDkeBlQuUJCF-TFytQHjZf_enLJUDOvImdwVBH8,188
 laboneq/core/types/enums/dsl_version.py,sha256=Ba_d-Bw4wPQOb7Nv6Uy1S5XFCvDBXkNWzOoiPokiVxs,227
 laboneq/core/types/enums/execution_type.py,sha256=5AndgsShuhqkXr64g3IOuXal_TvhCrVMl7PkblOrZ1U,185
-laboneq/core/types/enums/high_pass_compensation_clearing.py,sha256=1M6A-f1hF6O5AJuLiRiBxgMyerYajqq7y3CmBKzkaKk,223
+laboneq/core/types/enums/high_pass_compensation_clearing.py,sha256=x0F2mYFI5rT1-hEYylTZQRP31kas2PX0fsxkZ42oUaQ,333
 laboneq/core/types/enums/io_direction.py,sha256=RwJfnTnkhC6GyuoQ-SbdpySgeSkDreMpWkWlNGWwwY0,157
 laboneq/core/types/enums/io_signal_type.py,sha256=eZbqdP51PHnH77vn6MUup7igCrS3pnx-15x8MO50MAo,268
 laboneq/core/types/enums/mixer_type.py,sha256=iXF4i8-ovwBfJkppv4iB98ZmeV6bvpsZTRPr-emjwPM,316
 laboneq/core/types/enums/modulation_type.py,sha256=S7wsc5w0UiiGkgrI9uIbY2ICpn8G1syuE19h57OJtvk,200
 laboneq/core/types/enums/port_mode.py,sha256=1CdF7cSNb15P8ZgY54iPIOdwZuuDHwlC1HaJfSxchFk,152
 laboneq/core/types/enums/reference_clock_source.py,sha256=hN1gZKxh_ElHZOq3zl0nHyJaaKoCgixTc0fKcCKUy7E,188
 laboneq/core/types/enums/repetition_mode.py,sha256=hRnj_stjpVRDGTCHoN7q5kPffAm6OoTX9BWcoerl3A8,198
 laboneq/core/types/enums/section_alignment.py,sha256=nYuTh1r0PL35aQoLUgeOGTnZoAb6XhGPgVY4a70UMgc,170
 laboneq/core/utilities/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
 laboneq/core/utilities/compressed_formatter.py,sha256=PsOA_xZVu0cX4uAk33ax5ZPjCEJ1Dv2UspvjGCj6Si8,1813
 laboneq/core/utilities/pulse_sampler.py,sha256=eKdg1IcTwjoVmp7mKSSAu6eV80mYPgHaMUUr9AIWkZ4,8039
-laboneq/core/utilities/replace_pulse.py,sha256=LEWhHoF3s8klVXSaVO26gkthLuyJE_A5NRcZW8WGTx4,9808
+laboneq/core/utilities/replace_pulse.py,sha256=v5sA6qtAUU0cP1RMeYjiGVOEtZsCDQILcQA0IRmoPPE,9873
+laboneq/data/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/data/data_helper.py,sha256=ca5jUyF_lkiaRMPfPNyBmXumb5_TrHmoEW4NQkPIisg,3627
+laboneq/data/calibration/__init__.py,sha256=CUauhqJddoXpivkMrzIFsfQKXPSeN3YnKiY1p4tvtRg,1738
+laboneq/data/compilation_job/__init__.py,sha256=Y_JYiwAkCH1UN-Jek6NGNKmVvBK8DTJzFrY6wj3Y2RU,3199
+laboneq/data/execution_payload/__init__.py,sha256=GoYwGV2AUjqI8DxffEfaZ_Xe8vZsjATqnVz8--61NzY,3887
+laboneq/data/execution_payload/execution_payload_helper.py,sha256=pqwt_HmL67VTv6HTYSdOVs4j9MsOt99MbFcqkVptqJg,842
+laboneq/data/experiment_description/__init__.py,sha256=IyLHHANr1OMIl49rS-CWSkrAw4eYoUNm7BQtJuRqWL4,5188
+laboneq/data/experiment_description/experiment_helper.py,sha256=XekNd06WnP4oe51h90szF7VjHyoSw9JvBdqljNSzyxo,583
+laboneq/data/experiment_results/__init__.py,sha256=WPq3zHfdbaxiAUcLYf23cgaIVJ1VkMSrGpY1YkI-258,950
+laboneq/data/experiment_schedule/__init__.py,sha256=MiqtMp3ml2V4wwfTkQlzm1KYSaHSjr8J8f_051d34Uw,761
+laboneq/data/scheduled_experiment/__init__.py,sha256=vWDzi2fhnH9DNyfq3KBNjLNCG7RxMKe09tLAiwptnbU,1782
+laboneq/data/setup_description/__init__.py,sha256=L5L_rh81LvYqQcIKKJPhEp99A1ujx-S0txfkQLRU6So,3367
+laboneq/data/setup_description/setup_helper.py,sha256=vVlRJxe_Bt3XCnNbDj0-FvP3raYMjj4Xn7JGK_4Tdg8,2845
 laboneq/dsl/__init__.py,sha256=gsR9dv88edpbJLrwc_X2jj147IfVWpnTT10td01fPkY,178
-laboneq/dsl/laboneq_facade.py,sha256=xfeHLO9ywCpClZ1Jl_I_Z_IC5wDpr2tckFsJhPuy8PY,2929
+laboneq/dsl/laboneq_facade.py,sha256=uk6A352TiRfbFkOZgw7E23mjRCBPYnTIzsdwENfN6Yo,2947
 laboneq/dsl/parameter.py,sha256=AbR78048B3-jyYvq_A5rmBqaeg4v0C601f9EGFJzRN0,2552
 laboneq/dsl/session.py,sha256=P-mOhpv3-u5stl3oeRSjTn97b4Nm4M42gxw24HYzsT4,25670
 laboneq/dsl/utils.py,sha256=v0qlt2XA2CXiGK3Rpi_PC45YZGeQriRz-ShovaTXMBE,2296
 laboneq/dsl/calibration/__init__.py,sha256=3becZcLdza9jTczHmfBgbbaH238UfP9uPakbhe5kwto,529
 laboneq/dsl/calibration/amplifier_pump.py,sha256=H1L-uYlCL3sXTMXIbBFcWS9ln1mFiz5lCr6NnLUKODk,946
 laboneq/dsl/calibration/calibratable.py,sha256=DEx55rhplLTxoaf8-bGnmZqyO4eZdIyMptiLAGKEp7M,545
 laboneq/dsl/calibration/calibration.py,sha256=3t6v9XjyhsT8ZtZM5kIRIgfUy99OWk85JvcMFtDc-Ok,2313
 laboneq/dsl/calibration/calibration_item.py,sha256=JlPu54zS2NfivokgD4ICOhrw5e3Rhs5DO7pB0iDazpY,111
 laboneq/dsl/calibration/mixer_calibration.py,sha256=_ivXcsDgELxaC8zZ7E5caMhE-HZYSuuDyR5odaVImKw,992
 laboneq/dsl/calibration/observable.py,sha256=5zf7HE7e4MnrnHcgwAWMKkejOiVTZs4UCtlRiVn8OVw,3403
 laboneq/dsl/calibration/oscillator.py,sha256=3e_X5v9PSCOwLcr7nb-zUWj1OGjqIvsfxZWMFB_VDKE,2134
-laboneq/dsl/calibration/precompensation.py,sha256=N-GduIP4AVdKfxDH2rQ3zbYEarKx1rYrxO2Egb70Q9A,2650
+laboneq/dsl/calibration/precompensation.py,sha256=tDZHSsoZh_DSJH1BpZWcUiZMvkaZE9rhSI5czRtyh3M,3140
 laboneq/dsl/calibration/signal_calibration.py,sha256=798sV3mEz0ssBI4GYjNoNTIAuzBTf2rknvdMZBohQR0,5614
 laboneq/dsl/calibration/units.py,sha256=9W7YXV75G2VgNGSNserL_rsnEdjQugCuzg1gQmkvutU,553
 laboneq/dsl/device/__init__.py,sha256=uqx0Rho0xQ0vHzcP4no8R0OfjkK2ZdPllpVsZoAuH6Y,363
 laboneq/dsl/device/_device_setup_generator.py,sha256=sA2j1IKi3pId3yg5Ct4sp_tvkd4aZ7o8FX7fDdpKIgg,45826
 laboneq/dsl/device/connection.py,sha256=e_uMDO-7YrMKJkZEbizlTQZITsXU1--ceOYOZ0m40Xc,601
 laboneq/dsl/device/device_setup.py,sha256=hDYGDooO-rFxHsC7i1HD5kyzPvXzNSjrXBWkCTg0dMk,13663
 laboneq/dsl/device/device_setup_helper.py,sha256=KRaya8xtzjqzdn1SZ_NMCU7p_V-76Aj_S0evSzuey7c,2551
 laboneq/dsl/device/instrument.py,sha256=XjaPAcpKdPQx1z-QpAFwHLFERoK65-Rgb7SjIyW_zy8,1362
 laboneq/dsl/device/logical_signal_group.py,sha256=i12USV4K1ij8y_3SOYStnZE_z3Bo6G0-f03RtuBjO-w,1893
 laboneq/dsl/device/physical_channel_group.py,sha256=1u4c9TyfC5WZWkgQGTpDcbIc6hXcgKuNdE8AJcxbaRk,1729
 laboneq/dsl/device/ports.py,sha256=-jVPCUfRq1e2PHpPBrcHuUQcrrfv7kylzDUF9rZWTnQ,538
-laboneq/dsl/device/quantum_operations.py,sha256=cjiOhMFZT87b88P2pXK1MZSLvLT78oOVFs7PFvMAgZk,3422
-laboneq/dsl/device/qubits.py,sha256=zjEg3HIPvRU8giDSqI9i1vOISPtQSEPEKLez-CyoauA,4557
 laboneq/dsl/device/server.py,sha256=JOM2xKKWMwFWYPcAjoCoFIuF_4ZC73_fMiZXUhNSZPk,215
 laboneq/dsl/device/instruments/__init__.py,sha256=sl302P7-HQO6Y8NXCcN2-r5mfbGastN7Ugs6PfRA1wg,328
 laboneq/dsl/device/instruments/hdawg.py,sha256=xLmo7LJhGC61PDkv_ZYn37VD0bnRxC1Ag54ET_KRLE4,1778
 laboneq/dsl/device/instruments/nonqc.py,sha256=j6jLNrFifaKe1QDcQJcTVWMdQR7eBI345V7S-iWqhts,466
 laboneq/dsl/device/instruments/pqsc.py,sha256=JQrg31Gj6HRjUOYjDyG5m2A9ngrQOFcX0mHw_2BwsGk,948
 laboneq/dsl/device/instruments/shfppc.py,sha256=E_-2fesNBJ0E-qrrwSA5MK1TdL0Daht9OX2U0BeBtkg,927
 laboneq/dsl/device/instruments/shfqa.py,sha256=C6yaZvxr1xZwUegOILTNC8_B7a28O_GqsIYag-dCvYo,2248
@@ -201,48 +217,95 @@
 laboneq/dsl/device/servers/__init__.py,sha256=ZeYikalTjZXb_HDjfdGe6YHUuZAlDv0qqHZ0d1JLOE8,114
 laboneq/dsl/device/servers/data_server.py,sha256=URgMXwwmzNAPF3PrQBTE11dU7QLxGaJa0tIdi8F2BiQ,704
 laboneq/dsl/enums/__init__.py,sha256=GeDXWBzskaPr4MxVoeJp6kj-X5kVZA1yrbUw7wcV2F0,718
 laboneq/dsl/experiment/__init__.py,sha256=N159QRiB6rNL_RH6vzZwYqi4B91GTlX-JmmysAoQgMM,508
 laboneq/dsl/experiment/acquire.py,sha256=g4Pvm6T0qu8tH8LRTHhCZ1wb2K4Drc1rawNeNTRkS_E,972
 laboneq/dsl/experiment/call.py,sha256=eATarAz81C0QC5Ih-Uuh9PrS0g4rEF_vbQsrav_-I6Q,814
 laboneq/dsl/experiment/delay.py,sha256=98P3AePai3fqH1csDnWSxUN3EGJchuysX_2qnkCF2-Y,780
-laboneq/dsl/experiment/experiment.py,sha256=0xtihbOCTLtTD2eC7ZoQuMC2Xx9uZm0l32v2DNFy-oY,39761
+laboneq/dsl/experiment/experiment.py,sha256=eUkndC0frKHtbbx5jsUFOUrg47Mr2yTjCsn8N1zjymk,40011
 laboneq/dsl/experiment/experiment_signal.py,sha256=eHDHAu7Hv9xTSF-f9-YsJ1suZmZfaevS9anyLaBiOPY,8216
 laboneq/dsl/experiment/operation.py,sha256=kJPLIjNTFf_lJkVsOmASPi7GZVJ9CCZySdA2YDCmswU,401
 laboneq/dsl/experiment/play_pulse.py,sha256=yGd_-jzkuOK_i4A65mfoPfeG1IRKK8ZaDQE-E627Idw,1647
 laboneq/dsl/experiment/pulse.py,sha256=cdmMmMo1yGygx_5EkyemW6xO-8-FuIErugjN1PHiKrE,3953
 laboneq/dsl/experiment/pulse_library.py,sha256=kmvFKXNGXIVCnjFMsFqAdiUM5bk8u-grY4ZeuKWHJ8M,8194
 laboneq/dsl/experiment/reserve.py,sha256=tn1YEkW6E7BbBuG4SKveCmiAXrsYm2IeMUI2iDnwazs,890
 laboneq/dsl/experiment/section.py,sha256=0gg3PscVUPEoTEhYaE4bsX8qsTvxgXQ4RyKb_gop5q8,11431
 laboneq/dsl/experiment/set.py,sha256=4hEgxT9iYWNgDEEAFDS4D1GlgTsInRK3regArR4cnaU,640
 laboneq/dsl/experiment/utils.py,sha256=TiO1tKG5F8Zqx1lUz1rUPc3lNVE6UMPnniuLNoyMql8,323
+laboneq/dsl/quantum/__init__.py,sha256=NvineMWpjeAgy-1KhEkE0Ei9INuDe3AmsPsdbQe0Khk,224
+laboneq/dsl/quantum/quantum_operations.py,sha256=kb9rZDSllCSSflTZCcNHteZa7goD-Hilg9g0w32gRg0,3423
+laboneq/dsl/quantum/qubits.py,sha256=HZSaOHG-OI2Q5BrRmpHewZhmTSgw5CptG7hnGUSd_HM,10892
 laboneq/dsl/result/__init__.py,sha256=XAUfjo82SDzPK0s8ZZSJPTVRIF8b4smFBWhI5rwqBAQ,151
 laboneq/dsl/result/acquired_result.py,sha256=yNCpd1C8BnKeWbMCJHSVFOQzcYoy00-eLdLwjAEcFQk,1766
-laboneq/dsl/result/results.py,sha256=79EozB9G1ExCYAY8dFjEQdpDL82G5tJGKTdMH1XWRn8,7240
+laboneq/dsl/result/results.py,sha256=Loyay67WyhDB_fDCJ0zjPN2k18tvAOwCKXcIchhKLQE,7189
 laboneq/dsl/serialization/__init__.py,sha256=XVKLzoqNC9_psuftSgRNbbNmrcvTeJmWW5bIa-bmwRU,113
-laboneq/dsl/serialization/serializer.py,sha256=I4HJ5Qm2GBOxgEm_k7-e1-xd8vEz4m15CCpI4eP38fA,5392
+laboneq/dsl/serialization/serializer.py,sha256=2V6hFMW5TevU4m6T5GJZdsha2okNvE0KCNYvElsg2AA,5394
 laboneq/executor/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
 laboneq/executor/execution_from_experiment.py,sha256=eE1lzSHYQqZZqlM2TAyjm0ibP3ifeeNTIOazin9z96M,3819
 laboneq/executor/executor.py,sha256=xvJwDB-9hlPjD4dTPqfxN2uNVB_2o8ZoKLNWPQBgpQc,8152
+laboneq/implementation/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/implementation/compilation_service/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/implementation/compilation_service/compilation_service.py,sha256=bkthiJj5OpDDy2E7-5cXApuuuvsdEepx1AGOHu0q54k,1156
+laboneq/implementation/compilation_service/compilation_service_legacy.py,sha256=bgtE-Nzt6epqUkivxT9aNE8v8dxeg3lZZFh7dJbGizs,7894
+laboneq/implementation/data_storage/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/implementation/data_storage/l1q_database_wrapper.py,sha256=XIewgC1Gin2djDdSlz_DFQjaQ1s_dl6W_YnRABvx3K0,916
+laboneq/implementation/data_storage_service/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/implementation/data_storage_service/data_storage_service_sqlite_dict.py,sha256=CemktSIKDUVl2EHResIyU3aAJ_Ve70AJvHxSzMwkXEU,6103
+laboneq/implementation/experiment_workflow/__init__.py,sha256=AaKiWtIt7DgkOBZaLj_oOxrFACk6bWNIxqPdQd4UwOo,130
+laboneq/implementation/experiment_workflow/device_setup_generator.py,sha256=BtyCTvkijW2gr7CUaRXFxuVwDGSPXJBAKfoaDB-gaHI,16908
+laboneq/implementation/experiment_workflow/experiment_workflow.py,sha256=NC5eTQnDhae5rQRnooUBrnfL_LT8wtRoYAnlVhX-vhM,6106
+laboneq/implementation/legacy_adapters/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/implementation/legacy_adapters/dynamic_converter.py,sha256=sWsjce-ZD9uz0gKgaIicXe1NlHO0iTlmkFbi6q5Aqz0,3084
+laboneq/implementation/legacy_adapters/simple2.py,sha256=-Ye3LkRzavwAhi_bl3YbETkfWvrY_cPrdUz69Hg-G1I,950
+laboneq/implementation/legacy_adapters/converters_calibration/__init__.py,sha256=0RcULl5jNqdwM2Gqoo12x2XAQKygf8EEoWZ1PJZbCeI,7740
+laboneq/implementation/legacy_adapters/converters_calibration/post_process_calibration.py,sha256=vsxRzSBL2VJi5I3kJbUgnM4GOHoemTAvzVmijzWttzY,131
+laboneq/implementation/legacy_adapters/converters_experiment_description/__init__.py,sha256=6dQQFLZvFtASRTsZDfxi1Yr1B6BidoCPGc3ITwj6l4M,22847
+laboneq/implementation/legacy_adapters/converters_experiment_description/post_process_experiment_description.py,sha256=t1FQOO5S2w4iteG35Ryip6jlOtUPBJ-tEqA5fOBc_PE,1659
+laboneq/implementation/legacy_adapters/converters_experiment_results/__init__.py,sha256=MWmnjAIUheNFiIStmlVxUfO2Q22MqgFlKGqocqvG58g,1741
+laboneq/implementation/legacy_adapters/converters_experiment_results/post_process_experiment_results.py,sha256=vsxRzSBL2VJi5I3kJbUgnM4GOHoemTAvzVmijzWttzY,131
+laboneq/implementation/legacy_adapters/converters_scheduled_experiment/__init__.py,sha256=9ybevrSPbuLmJZjszERmB3i1T7JI-8DvCBCHcgDLD90,4376
+laboneq/implementation/legacy_adapters/converters_scheduled_experiment/post_process_scheduled_experiment.py,sha256=vsxRzSBL2VJi5I3kJbUgnM4GOHoemTAvzVmijzWttzY,131
+laboneq/implementation/legacy_adapters/converters_setup_description/__init__.py,sha256=xic3V54zuLyltVv1TPEpdSGp0UxTTho-uqboAhOn4H0,13804
+laboneq/implementation/legacy_adapters/converters_setup_description/post_process_setup_description.py,sha256=7PlpmIH1wcQpmbaZZNwmpCKGmjrjV7wCBiQ8l5bHpvE,5165
+laboneq/implementation/legacy_adapters/legacy_dsl_adapters/__init__.py,sha256=VqQQH_MyRUWwxW-pdkJSYkLk7mYvg8I_1IQ3Pyaa9fQ,9204
+laboneq/implementation/payload_builder/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/implementation/payload_builder/payload_builder.py,sha256=vuMCu2tH9bI50MTQ5SigiPGBo88osFfW0gSAhOimYkw,25577
+laboneq/implementation/runner/__init__.py,sha256=kbDoa0zD-iLYmGvh3f9ER9rSUW9UJxHzmdheeH4kxyg,105
+laboneq/implementation/runner/runner.py,sha256=Bqai465siIHt0SwsU6H94hek6sHpCnbsE85YZPqqfPQ,2293
+laboneq/implementation/runner/runner_legacy.py,sha256=PBgNcDC9DL4Duf8wUXqYKRdrYAvU9vjxmX9sNUDvFAc,14574
+laboneq/interfaces/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/interfaces/application_management/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/interfaces/application_management/laboneq_settings.py,sha256=AveKgiI8kTXggUoVS8BsCPDZF3STTSwNkOsSkWN21QA,384
+laboneq/interfaces/compilation_service/__init__.py,sha256=zB8QZ3xKM9mTzqQHFoKEmAbCkDBYhatxv3IZzqA7-KY,137
+laboneq/interfaces/compilation_service/compilation_service_api.py,sha256=QbYJLsbNtJt81vIz0J7SSJSNNCGQD3L3SO0xxB-fElQ,779
+laboneq/interfaces/data_storage/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/interfaces/data_storage/data_storage_api.py,sha256=4A3po4mvtpcYIJy1pKeUKIamknJ2-7SVQRwE3utEw9Y,2272
+laboneq/interfaces/experiment/__init__.py,sha256=dXziTVsjbygOsG0oulpw83gecI2RmpcVeCQbMmVv1Zw,120
+laboneq/interfaces/experiment/experiment_api.py,sha256=olBLbX-LMbfPFGkd4WGzkgQnlCic5z7JHi2b_-e-Tqw,2004
+laboneq/interfaces/payload_builder/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/interfaces/payload_builder/payload_builder_api.py,sha256=jliezqh7gJdH5Nw7qIMP0HHJxLopQa2hDp6vmUv9ygQ,892
+laboneq/interfaces/runner/__init__.py,sha256=3eHhVd6jL1C_XKdm6Uos7u8P7T_4MP6cnw2JMgXvqQE,77
+laboneq/interfaces/runner/runner_api.py,sha256=eHfo0TO_yZYchBQarIrALjUCmzNAxoHMeo-3oiUO4q4,766
+laboneq/interfaces/runner/runner_control_api.py,sha256=P53Yw82od4k6P8oceca9QbLLoa4Has3RiPoEeDdni54,793
 laboneq/openqasm3/__init__.py,sha256=zIfFQa39Ko4nUcnnLBmRilnUVJ9eeg022QoLpodiv2o,145
 laboneq/openqasm3/expression.py,sha256=DKk9nMo1cABcEb4kPJ3dOAKlsafr5O-rNh5TfbUHGkw,8903
 laboneq/openqasm3/gate_store.py,sha256=rF8qUBL6avuZYcGKAYVU85Xb3wwCFN69qYJEtwtZbTg,1671
 laboneq/openqasm3/namespace.py,sha256=c_rpWEw9MZALiu1ulKntBOaSSXQudd8HieQ2r-fU3qs,2593
-laboneq/openqasm3/openqasm3_importer.py,sha256=nkSJucZWi_qOVWUoy6H8VJLZg2yBDukSJS1GhDhynMU,15459
+laboneq/openqasm3/openqasm3_importer.py,sha256=jZc4TQ9FXP9cYtptw5lbkopk3soUhOPXE5C-7s4ol8w,15459
 laboneq/openqasm3/openqasm_error.py,sha256=rgkp6fT1tNrhVX8eCV-q1PLJUfGxkmT4gXEErJcSB-8,1732
 laboneq/openqasm3/reset_gate_factory.py,sha256=WnWPrS0E0NXXy1pbSryMw8KgswOoGm7IW71vhynXhKA,4850
 laboneq/openqasm3/signal_store.py,sha256=SJ3lvM5iWGi2HS7t64E2TbIsBZGS5JHdhJN0gX6bE8w,1517
 laboneq/pulse_sheet_viewer/__init__.py,sha256=F_gdqvR3iTbFH2-iGtGWPp2v2XpMu0c4SXEPEIJyQb0,127
 laboneq/pulse_sheet_viewer/event_graph_viewer.py,sha256=hKBUzFzimfz9YAFUYNYwrhwMscXHa-4M3BNa6id6SHE,2059
 laboneq/pulse_sheet_viewer/interactive_psv.py,sha256=D7pEX9C8mP9EZofE5L3aAAkX3lNFaEoHwBc_l2AHyec,2692
 laboneq/pulse_sheet_viewer/pulse_sheet_viewer.py,sha256=_O53T2cm8KWDhbUKoONuRb_9JOKyKvOqEMtQgrwlQPI,3288
 laboneq/pulse_sheet_viewer/pulse_sheet_viewer_template.html,sha256=TsX3r0W8qf_PKAw1pYreXQEcexRfzgL_FmbvOAFh06s,1443040
 laboneq/simulator/__init__.py,sha256=BuPOsR4Dwi6tSLAsG0lBeHzpOZFnCsNn93ohr-v9mZ8,152
-laboneq/simulator/output_simulator.py,sha256=OjbHVNNkrYITwZaJ58HaqAeM-ETeLP4y_ifA0aQXrGE,5904
-laboneq/simulator/seqc_parser.py,sha256=gVR7AEtmuJH2QDGnzA4LRkZPgr3iBorwWMk-CJ3cPGQ,40863
-laboneq/simulator/wave_scroller.py,sha256=P9YjG9w_td2SrZfQohIVcRe4Gf9MBI_-RgA615de99g,12500
-laboneq-2.7.0.dist-info/AUTHORS,sha256=Uu7pMg_oQJSHTrzjG8G3ApfutLIKqdOdjmtf5VZQILs,22
-laboneq-2.7.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-laboneq-2.7.0.dist-info/METADATA,sha256=PVXSv6mKgMP3JttTjgvdt6OdpNuUnaD3ZQ45AWurQHA,3188
-laboneq-2.7.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-laboneq-2.7.0.dist-info/top_level.txt,sha256=oZ0o6Elw6GJcR44azoSi8l6opKF-v5Ks1MLYbqpXJGA,8
-laboneq-2.7.0.dist-info/RECORD,,
+laboneq/simulator/output_simulator.py,sha256=4_jPSN8jYT3A3pW1_g5_1YnLnkPnTdfEu0249GApzu4,6090
+laboneq/simulator/seqc_parser.py,sha256=mZjEX7opXKvxjimhlIHHDNhikip0uWu_GJS9r7kB8Zc,41644
+laboneq/simulator/wave_scroller.py,sha256=9_xRKYi1deA8je4OAmJJsKmMpNEo9pGO-qJKEpf_3FY,17091
+laboneq-2.8.0.dist-info/AUTHORS,sha256=Uu7pMg_oQJSHTrzjG8G3ApfutLIKqdOdjmtf5VZQILs,22
+laboneq-2.8.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+laboneq-2.8.0.dist-info/METADATA,sha256=6QwBpj22m8DME8VbiSgEiu0LHgLA8FR9VtjRg3ra1-w,3255
+laboneq-2.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+laboneq-2.8.0.dist-info/top_level.txt,sha256=oZ0o6Elw6GJcR44azoSi8l6opKF-v5Ks1MLYbqpXJGA,8
+laboneq-2.8.0.dist-info/RECORD,,
```

