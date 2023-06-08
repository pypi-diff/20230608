# Comparing `tmp/aiida-aurora-0.2.0.tar.gz` & `tmp/aiida_aurora-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-aurora-0.2.0.tar", last modified: Tue Aug  9 16:24:36 2022, max compression
+gzip compressed data, was "aiida_aurora-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida-aurora-0.2.0.tar` & `aiida_aurora-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,61 @@
--rw-r--r--   0        0        0     1070 2022-01-12 17:18:42.983936 aiida-aurora-0.2.0/LICENSE
--rw-r--r--   0        0        0     6365 2022-01-12 17:22:44.785959 aiida-aurora-0.2.0/README.md
--rw-r--r--   0        0        0       83 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/__init__.py
--rw-r--r--   0        0        0       84 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/calculations/__init__.py
--rw-r--r--   0        0        0     5906 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/calculations/cycler.py
--rw-r--r--   0        0        0     3320 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/calculations/fake.py
--rw-r--r--   0        0        0     1592 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/cli.py
--rw-r--r--   0        0        0      230 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/data/__init__.py
--rw-r--r--   0        0        0     4117 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/data/battery.py
--rw-r--r--   0        0        0     2424 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/data/control.py
--rw-r--r--   0        0        0     2314 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/data/experiment.py
--rw-r--r--   0        0        0     2710 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/helpers.py
--rw-r--r--   0        0        0     5750 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/parsers.py
--rw-r--r--   0        0        0    17111 2022-08-09 16:21:44.094920 aiida-aurora-0.2.0/aiida_aurora/scheduler.py
--rw-r--r--   0        0        0     3538 2022-08-09 16:21:44.098919 aiida-aurora-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7677 1970-01-01 00:00:00.000000 aiida-aurora-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2023-06-08 14:37:01.364612 aiida_aurora-0.3.1/.coveragerc
+-rwxr-xr-x   0        0        0      195 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.github/install_aiida_github.sh
+-rw-r--r--   0        0        0     2157 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      753 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.github/workflows/publish-on-pypi.yml
+-rw-r--r--   0        0        0      142 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.gitignore
+-rw-r--r--   0        0        0      942 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      119 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.readthedocs.yml
+-rw-r--r--   0        0        0      232 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.style.yapf
+-rw-r--r--   0        0        0     1070 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/LICENSE
+-rw-r--r--   0        0        0       35 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/MANIFEST.in
+-rw-r--r--   0        0        0     6365 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/README.md
+-rw-r--r--   0        0        0       83 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/calculations/__init__.py
+-rw-r--r--   0        0        0     7147 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/calculations/cycler.py
+-rw-r--r--   0        0        0     3396 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/calculations/fake.py
+-rw-r--r--   0        0        0     1592 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/cli.py
+-rw-r--r--   0        0        0      246 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/data/__init__.py
+-rw-r--r--   0        0        0     4117 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/data/battery.py
+-rw-r--r--   0        0        0     2362 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/data/control.py
+-rw-r--r--   0        0        0     2322 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/data/experiment.py
+-rw-r--r--   0        0        0     2696 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/helpers.py
+-rw-r--r--   0        0        0     6271 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/parsers.py
+-rw-r--r--   0        0        0    15913 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/scheduler.py
+-rw-r--r--   0        0        0       49 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/utils/__init__.py
+-rw-r--r--   0        0        0     9221 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/utils/cycling_analysis.py
+-rw-r--r--   0        0        0     1263 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/utils/plot.py
+-rw-r--r--   0        0        0      172 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/workflows/__init__.py
+-rw-r--r--   0        0        0    12454 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/workflows/stress_test.py
+-rw-r--r--   0        0        0    32366 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/workflows/stress_test_defaults.json
+-rw-r--r--   0        0        0        7 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/docs/.gitignore
+-rwxr-xr-x   0        0        0     1541 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/docs/Makefile
+-rwxr-xr-x   0        0        0    11606 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/docs/source/conf.py
+-rw-r--r--   0        0        0     2814 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/docs/source/developer_guide/index.rst
+-rw-r--r--   0        0        0    76300 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/images/AiiDA_transparent_logo.png
+-rwxr-xr-x   0        0        0     1274 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/index.rst
+-rw-r--r--   0        0        0     1263 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/user_guide/get_started.rst
+-rw-r--r--   0        0        0       94 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/user_guide/index.rst
+-rw-r--r--   0        0        0      243 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/user_guide/tutorial.rst
+-rw-r--r--   0        0        0      275 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/code_ketchup-0.2rc2.yml
+-rw-r--r--   0        0        0      292 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/code_monitor.yml
+-rw-r--r--   0        0        0      280 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_ddm07162.yml
+-rw-r--r--   0        0        0      329 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_ddm07162_config.yaml
+-rw-r--r--   0        0        0      336 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_localhost-verdi.yml
+-rw-r--r--   0        0        0       41 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_localhost-verdi_config.yaml
+-rw-r--r--   0        0        0      276 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_localhost.yml
+-rw-r--r--   0        0        0       41 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_localhost_config.yaml
+-rwxr-xr-x   0        0        0      517 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/setup.sh
+-rw-r--r--   0        0        0     2761 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/stress_test/batteries.json
+-rw-r--r--   0        0        0     4683 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/stress_test/submit_test.py
+-rw-r--r--   0        0        0      139 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/fake_aurora_server/batt.json
+-rw-r--r--   0        0        0      147 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/fake_aurora_server/exp.json
+-rwxr-xr-x   0        0        0     3001 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/fake_aurora_server/server.py
+-rw-r--r--   0        0        0     3676 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      485 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/input_files/__init__.py
+-rw-r--r--   0        0        0       27 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/input_files/file1.txt
+-rw-r--r--   0        0        0       27 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/input_files/file2.txt
+-rw-r--r--   0        0        0     1107 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/test_calculations.py
+-rw-r--r--   0        0        0     1151 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/test_cli.py
+-rw-r--r--   0        0        0     7677 1970-01-01 00:00:00.000000 aiida_aurora-0.3.1/PKG-INFO
```

### Comparing `aiida-aurora-0.2.0/LICENSE` & `aiida_aurora-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-aurora-0.2.0/README.md` & `aiida_aurora-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aiida-aurora-0.2.0/aiida_aurora/calculations/cycler.py` & `aiida_aurora-0.3.1/aiida_aurora/calculations/cycler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,164 @@
 """
-Calculations provided by aiida_aurora.
-
-Register calculations via the "aiida.calculations" entry point in setup.json.
+Battery cycling experiment CalcJobs.
 """
-from importlib import import_module
+from typing import Optional
 
+from aurora.schemas.dgbowl_schemas import conversion_map, payload_models
 import yaml
 
 from aiida.common import datastructures
 from aiida.engine import CalcJob
-from aiida.orm import ArrayData, SinglefileData
+from aiida.engine.processes.exit_code import ExitCode
+from aiida.orm import ArrayData, Node, SinglefileData
 
-from aiida_aurora.data.battery import BatterySample, BatteryState
-from aiida_aurora.data.control import TomatoSettings
-from aiida_aurora.data.experiment import CyclingSpecs
+from aiida_aurora.data.battery import BatterySampleData, BatteryStateData
+from aiida_aurora.data.control import TomatoSettingsData
+from aiida_aurora.data.experiment import CyclingSpecsData
 
 
 class BatteryCyclerExperiment(CalcJob):
     """
     AiiDA calculation plugin for the tomato instrument automation package.
     https://github.com/dgbowl/tomato
     """
-    _INPUT_PAYLOAD_YAML_FILE = 'payload.yaml'
-    _INPUT_PAYLOAD_VERSION = '0.2'
-    _OUTPUT_FILE_PREFIX = 'results'
+
+    _INPUT_PAYLOAD_YAML_FILE = "payload.yaml"
+    _INPUT_PAYLOAD_VERSION = "0.2"
+    _OUTPUT_FILE_PREFIX = "results"
 
     @classmethod
     def define(cls, spec):
         """Define inputs and outputs of the calculation."""
-        # yapf: disable
         super().define(spec)
 
         # set default values for AiiDA options
-        spec.inputs['metadata']['options']['resources'].default = {  # REQUIRED?
-            'num_machines': 1,
+        spec.inputs["metadata"]["options"]["resources"].default = {  # REQUIRED?
+            "num_machines": 1,
         }
-        spec.inputs['metadata']['options']['parser_name'].default = 'aurora'
-        spec.inputs['metadata']['options']['withmpi'].default = False
-        spec.inputs['metadata']['options']['input_filename'].default = cls._INPUT_PAYLOAD_YAML_FILE
+        spec.inputs["metadata"]["options"]["parser_name"].default = "aurora"
+        spec.inputs["metadata"]["options"]["withmpi"].default = False
+        spec.inputs["metadata"]["options"]["input_filename"].default = cls._INPUT_PAYLOAD_YAML_FILE
         # spec.inputs['metadata']['options']['scheduler_stderr'].default = ''
         # spec.inputs['metadata']['options']['scheduler_stdout'].default = ''
 
         # new ports
-        spec.input('metadata.options.output_filename', valid_type=str, default=cls._OUTPUT_FILE_PREFIX)
-        spec.input('battery_sample', valid_type=BatterySample, help='Battery sample used.')
-        spec.input('technique', valid_type=CyclingSpecs, help='Experiment specifications.')
-        spec.input('control_settings', valid_type=TomatoSettings, help='Experiment control settings.')
-        spec.output('results', valid_type=ArrayData, help='Results of the experiment.')
-        spec.output('raw_data', valid_type=SinglefileData, help='Raw data retrieved.')
-        # spec.output('battery_state', valid_type=BatteryState, help='State of the battery after the experiment.')
-
-        spec.exit_code(300, 'ERROR_MISSING_OUTPUT_FILES', message='Experiment did not produce any kind of output file.')
-        spec.exit_code(301, 'ERROR_MISSING_JSON_FILE', message='Experiment did not produce an output json file.')
-        spec.exit_code(302, 'ERROR_MISSING_ZIP_FILE', message='Experiment did not produce a zip file with raw data.')
-        spec.exit_code(311, 'ERROR_COMPLETED_ERROR', message='The tomato job was marked as completed with an error.')
-        spec.exit_code(312, 'ERROR_COMPLETED_CANCELLED', message='The tomato job was marked as cancelled.')
-        spec.exit_code(400, 'ERROR_PARSING_JSON_FILE', message='Parsing of json file failed.')
+        spec.input(
+            "metadata.options.output_filename",
+            valid_type=str,
+            default=cls._OUTPUT_FILE_PREFIX,
+        )
+        spec.input("battery_sample", valid_type=BatterySampleData, help="Battery sample used.")
+        spec.input("technique", valid_type=CyclingSpecsData, help="Experiment specifications.")
+        spec.input("control_settings", valid_type=TomatoSettingsData, help="Experiment control settings.")
+        spec.output("results", valid_type=ArrayData, help="Results of the experiment.")
+        spec.output("raw_data", valid_type=SinglefileData, help="Raw data retrieved.")
+        # spec.output('battery_state', valid_type=BatteryStateData, help='State of the battery after the experiment.')
+
+        # Unrecoverable errors: required retrieved files could not be read, parsed or are otherwise incomplete
+        spec.exit_code(300, "ERROR_OUTPUT_FILES_MISSING", message="Experiment did not produce any kind of output file.")
+        spec.exit_code(301, "ERROR_OUTPUT_JSON_MISSING", message="Experiment did not produce an output JSON file.")
+        spec.exit_code(
+            311, "ERROR_OUTPUT_JSON_READ", message="The output JSON file could not be read. Raw data may be available."
+        )
+        spec.exit_code(
+            312,
+            "ERROR_OUTPUT_JSON_PARSE",
+            message="The output JSON file could not be parsed. Raw data may be available."
+        )
+
+        # Warnings: JSON file with data was retrieved, but something went different than expected
+        spec.exit_code(
+            302,
+            "WARNING_OUTPUT_ZIP_MISSING",
+            message="Experiment did not produce a ZIP file with raw data, but the JSON file was parsed."
+        )
+        spec.exit_code(
+            501,
+            "WARNING_COMPLETED_ERROR",
+            message="The tomato job was marked as completed with an error, but some files were retrieved."
+        )
+        spec.exit_code(
+            502,
+            "WARNING_COMPLETED_CANCELLED",
+            message="The tomato job was marked as cancelled, but some files were retrieved."
+        )
 
     def prepare_for_submission(self, folder):
         """
         Create input files.
 
         :param folder: an `aiida.common.folders.Folder` where the plugin should temporarily place all files
             needed by the calculation.
         :return: `aiida.common.datastructures.CalcInfo` instance
         """
 
         # if connecting to a Windows PowerShell computer, change the extension of the submit script to '.ps1'
-        if self.inputs.code.computer.transport_type == 'sshtowin':
-            submit_script_filename = self.node.get_option('submit_script_filename')
-            if not submit_script_filename.endswith('.ps1'):
-                if submit_script_filename.endswith('.sh'):
-                    submit_script_filename = submit_script_filename[:-3] + '.ps1'
+        if self.inputs.code.computer.transport_type == "sshtowin":
+            submit_script_filename = self.node.get_option("submit_script_filename")
+            if not submit_script_filename.endswith(".ps1"):
+                if submit_script_filename.endswith(".sh"):
+                    submit_script_filename = submit_script_filename[:-3] + ".ps1"
                 else:
-                    submit_script_filename(submit_script_filename + '.ps1')
-                self.node.backend_entity.set_attribute('submit_script_filename', submit_script_filename)
+                    submit_script_filename(submit_script_filename + ".ps1")
+                self.node.backend_entity.set_attribute("submit_script_filename", submit_script_filename)
 
         # prepare the payload
-        # TODO: use dgbowl_schemas module
-        ## from dgbowl_schemas.tomato.payload_0_1.tomato import Tomato
-        ## - should 'version: "0.1"' be written in the submit script?
-        ## - name of the file containing the sample and method
-        tomato_schema_module = import_module(f"aurora.schemas.tomato_{self._INPUT_PAYLOAD_VERSION.replace('.', 'p')}")
-        TomatoSchema = tomato_schema_module.tomato.Tomato
+        TomatoPayload = payload_models[self._INPUT_PAYLOAD_VERSION]
 
         tomato_dict = self.inputs.control_settings.get_dict()
-        if tomato_dict['output']['prefix'] is None:
-            tomato_dict['output']['prefix'] = self._OUTPUT_FILE_PREFIX
+        if tomato_dict["output"]["prefix"] is None:
+            tomato_dict["output"]["prefix"] = self._OUTPUT_FILE_PREFIX
         else:
-            self._OUTPUT_FILE_PREFIX = tomato_dict['output']['prefix']
-        payload = tomato_schema_module.TomatoPayload(
-            version = self._INPUT_PAYLOAD_VERSION,
-            sample = tomato_schema_module.sample.convert_batterysample_to_sample(self.inputs.battery_sample.get_dict()),
-            method = tomato_schema_module.method.convert_electrochemsequence_to_method_list(
-                self.inputs.technique.get_dict()),
-            tomato = TomatoSchema(**tomato_dict),
+            self._OUTPUT_FILE_PREFIX = tomato_dict["output"]["prefix"]
+
+        payload = TomatoPayload(
+            version=self._INPUT_PAYLOAD_VERSION,
+            sample=conversion_map[self._INPUT_PAYLOAD_VERSION]["sample"](self.inputs.battery_sample.get_dict()),
+            method=conversion_map[self._INPUT_PAYLOAD_VERSION]["method"](self.inputs.technique.get_dict()),
+            tomato=conversion_map[self._INPUT_PAYLOAD_VERSION]["tomato"](**tomato_dict),
         )
-        with folder.open(self.options.input_filename, 'w', encoding='utf8') as handle:
-            handle.write(yaml.dump(payload.dict()))
+
+        # HOTFIX: Better to fix beforehand (to-do)
+        payload_dict = payload.dict()
+
+        if 'method' in payload_dict:
+            new_methods = []
+
+            for old_method in payload_dict['method']:
+                new_method = dict(old_method)
+                if 'loop' == new_method['technique']:
+                    new_method['goto'] = new_method['goto'] - 1
+                new_methods.append(new_method)
+
+            payload_dict['method'] = new_methods
+        # END HOTFIX
+
+        with folder.open(self.options.input_filename, "w", encoding="utf8") as handle:
+            handle.write(yaml.dump(payload_dict))
 
         codeinfo = datastructures.CodeInfo()
 
         # the calculation code should be 'ketchup', so we add the following `cmdline_params`
         # in order to submit the payload to tomato
-        codeinfo.cmdline_params = ['submit', '--jobname', '$JOB_TITLE', self._INPUT_PAYLOAD_YAML_FILE]
+        codeinfo.cmdline_params = [
+            "submit",
+            "--jobname",
+            "$JOB_TITLE",
+            self._INPUT_PAYLOAD_YAML_FILE,
+        ]
         codeinfo.code_uuid = self.inputs.code.uuid
         codeinfo.withmpi = self.inputs.metadata.options.withmpi
 
         # Prepare a `CalcInfo` to be returned to the engine
         calcinfo = datastructures.CalcInfo()
         calcinfo.codes_info = [codeinfo]
         calcinfo.local_copy_list = []
-        calcinfo.retrieve_list = [f'{self._OUTPUT_FILE_PREFIX}.json']
-        calcinfo.retrieve_temporary_list = [f'{self._OUTPUT_FILE_PREFIX}.zip']
+        calcinfo.retrieve_list = [f"{self._OUTPUT_FILE_PREFIX}.json"]
+        calcinfo.retrieve_temporary_list = [f"{self._OUTPUT_FILE_PREFIX}.zip"]
 
         return calcinfo
+
+    def parse_scheduler_output(self, retrieved: Node) -> Optional[ExitCode]:
+        """Parse the output of the scheduler if that functionality has been implemented for the plugin."""
+        # Tomato scheduler does not return any output that should be parsed
+        return None
```

### Comparing `aiida-aurora-0.2.0/aiida_aurora/calculations/fake.py` & `aiida_aurora-0.3.1/aiida_aurora/calculations/fake.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,89 @@
 """
-Calculations provided by aiida_aurora.
-
-Register calculations via the "aiida.calculations" entry point in setup.json.
+Dummy CalcJobs to simulate a battery experiment.
 """
 from aiida.common import datastructures
 from aiida.engine import CalcJob
 # from aiida.orm import SinglefileData
 from aiida.orm import Dict
 
-from aiida_aurora.data.battery import BatterySample, BatteryState
-from aiida_aurora.data.experiment import CyclingSpecs
+from aiida_aurora.data.battery import BatterySampleData, BatteryStateData
+from aiida_aurora.data.experiment import CyclingSpecsData
 
 
 class BatteryFakeExperiment(CalcJob):
     """
     AiiDA calculation plugin for the fake_aurora_server script.
 
     Simple AiiDA plugin that sends input data as json files to the fake Aurora server API script.
     """
-    _INPUT_BATTERY_JSON_FILE = 'battery.json'
-    _INPUT_EXPERIMENT_JSON_FILE = 'experiment.json'
-    _OUTPUT_JSON_FILE = 'output.json'
-    _DEFAULT_STDOUT_FILE = 'output.log'
+
+    _INPUT_BATTERY_JSON_FILE = "battery.json"
+    _INPUT_EXPERIMENT_JSON_FILE = "experiment.json"
+    _OUTPUT_JSON_FILE = "output.json"
+    _DEFAULT_STDOUT_FILE = "output.log"
 
     @classmethod
     def define(cls, spec):
         """Define inputs and outputs of the calculation."""
-        # yapf: disable
         super().define(spec)
 
         # set default values for AiiDA options
-        spec.inputs['metadata']['options']['resources'].default = {
-            'num_machines': 1,
-            'num_mpiprocs_per_machine': 1,
+        spec.inputs["metadata"]["options"]["resources"].default = {
+            "num_machines": 1,
+            "num_mpiprocs_per_machine": 1,
         }
-        spec.inputs['metadata']['options']['parser_name'].default = 'aurora'
+        spec.inputs["metadata"]["options"]["parser_name"].default = "aurora"
 
         # new ports
-        spec.input('metadata.options.output_filename', valid_type=str, default=cls._DEFAULT_STDOUT_FILE)
-        spec.input('battery_sample', valid_type=BatterySample, help='Battery sample used.')
-        spec.input('exp_specs', valid_type=CyclingSpecs, help='Experiment specifications.')
-        spec.output('results', valid_type=Dict, help='Results of the experiment.')  # a proper type should be defined
-        #spec.output('battery_state', valid_type=BatteryState, help='State of the battery after the experiment.')
-
-        spec.exit_code(300, 'ERROR_MISSING_OUTPUT_FILES', message='Calculation did not produce all expected output files.')
+        spec.input(
+            "metadata.options.output_filename",
+            valid_type=str,
+            default=cls._DEFAULT_STDOUT_FILE,
+        )
+        spec.input("battery_sample", valid_type=BatterySampleData, help="Battery sample used.")
+        spec.input("exp_specs", valid_type=CyclingSpecsData, help="Experiment specifications.")
+        spec.output("results", valid_type=Dict, help="Results of the experiment.")  # a proper type should be defined
+        # spec.output('battery_state', valid_type=BatteryStateData, help='State of the battery after the experiment.')
+
+        spec.exit_code(
+            300, "ERROR_MISSING_OUTPUT_FILES", message="Calculation did not produce all expected output files."
+        )
 
     def prepare_for_submission(self, folder):
         """
         Create input files.
 
         :param folder: an `aiida.common.folders.Folder` where the plugin should temporarily place all files
             needed by the calculation.
         :return: `aiida.common.datastructures.CalcInfo` instance
         """
 
-        with open(self._INPUT_BATTERY_JSON_FILE, 'w') as handle:
+        with open(self._INPUT_BATTERY_JSON_FILE, "w") as handle:
             handle.write(self.inputs.battery_sample.get_json())
-        with open(self._INPUT_EXPERIMENT_JSON_FILE, 'w') as handle:
+        with open(self._INPUT_EXPERIMENT_JSON_FILE, "w") as handle:
             handle.write(self.inputs.exp_specs.get_json())
 
         codeinfo = datastructures.CodeInfo()
         # codeinfo.cmdline_params = self.inputs.parameters.cmdline_params(
         #     file1_name=self.inputs.file1.filename,
         #     file2_name=self.inputs.file2.filename)
-        codeinfo.cmdline_params = [self._INPUT_BATTERY_JSON_FILE, self._INPUT_EXPERIMENT_JSON_FILE,
-                    '-o', self._OUTPUT_JSON_FILE]
+        codeinfo.cmdline_params = [
+            self._INPUT_BATTERY_JSON_FILE,
+            self._INPUT_EXPERIMENT_JSON_FILE,
+            "-o",
+            self._OUTPUT_JSON_FILE,
+        ]
         codeinfo.code_uuid = self.inputs.code.uuid
         codeinfo.stdout_name = self.metadata.options.output_filename
         codeinfo.withmpi = self.inputs.metadata.options.withmpi
 
         # Prepare a `CalcInfo` to be returned to the engine
         calcinfo = datastructures.CalcInfo()
         calcinfo.codes_info = [codeinfo]
         calcinfo.local_copy_list = []
-        calcinfo.retrieve_list = [self.metadata.options.output_filename, self._OUTPUT_JSON_FILE]
+        calcinfo.retrieve_list = [
+            self.metadata.options.output_filename,
+            self._OUTPUT_JSON_FILE,
+        ]
 
         return calcinfo
```

### Comparing `aiida-aurora-0.2.0/aiida_aurora/cli.py` & `aiida_aurora-0.3.1/aiida_aurora/cli.py`

 * *Files identical despite different names*

### Comparing `aiida-aurora-0.2.0/aiida_aurora/data/battery.py` & `aiida_aurora-0.3.1/aiida_aurora/data/battery.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,74 +2,72 @@
 Data types provided by plugin
 
 Register data types via the "aiida.data" entry point in setup.json.
 """
 
 import json
 
-from aurora.schemas.data_schemas import BatterySample as BatterySampleSchema
-from aurora.schemas.data_schemas import BatteryState as BatteryStateSchema
+from aurora.schemas.battery import BatterySample as BatterySampleSchema
+from aurora.schemas.battery import BatteryState as BatteryStateSchema
 import yaml
 
 from aiida.orm import Dict
 
 
-class BatterySample(Dict):  # pylint: disable=too-many-ancestors
+class BatterySampleData(Dict):  # pylint: disable=too-many-ancestors
     """
     A battery sample data object.
 
     This class represents a battery sample.
     """
 
     # "pydantic" schema to add automatic validation
     schema = BatterySampleSchema
 
     # pylint: disable=redefined-builtin
     def __init__(self, dict=None, **kwargs):
         """
         Constructor for the data class
 
-        Usage: ``BatterySample(dict{...})``
+        Usage: ``BatterySampleData(dict{...})``
 
         :param parameters_dict: dictionary with battery specifications
         :param type parameters_dict: dict
         """
         dict = self.validate(dict)
         super().__init__(dict=dict, **kwargs)
         if not self.label:
             self.label = self.dict["metadata"].get("name")
 
     def validate(self, parameters_dict):  # pylint: disable=no-self-use
         """Validate command line options.
 
         Uses the voluptuous package for validation. Find out about allowed keys using::
 
-            print(BatterySample.schema)
+            print(BatterySampleData.schema)
 
         :param parameters_dict: dictionary with battery specifications
         :param type parameters_dict: dict
         :returns: validated dictionary
         """
         d = BatterySampleSchema(**parameters_dict).dict()
         # Manual fix to convert date-times to ISO string format
         # TODO integrate this into the data schema
-        d["metadata"]["creation_datetime"] = d["metadata"][
-            "creation_datetime"
-        ].isoformat()
+        d["metadata"]["creation_datetime"] = d["metadata"]["creation_datetime"].isoformat()
         return d
 
     def get_json(self):
-        """Get a JSON file containing the BatterySample specs."""
+        """Get a JSON file containing the BatterySampleData specs."""
 
         # this can be customized to fit the desired format
         object_to_be_serialized = self.get_dict()
         return json.dumps(object_to_be_serialized)
 
     def get_yaml(self):
-        """Get a YAML file containing the BatterySample specs."""
+        """Get a YAML file containing the BatterySampleData specs."""
 
         # this can be customized to fit the desired format
         object_to_be_serialized = {"sample": self.get_dict()}
         return yaml.dump(object_to_be_serialized)
 
     def __str__(self):
         """String representation of node.
@@ -80,15 +78,15 @@
             {'ignore-case': True}
         """
         string = super().__str__()
         string += "\n" + str(self.get_dict())
         return string
 
 
-class BatteryState(Dict):  # pylint: disable=too-many-ancestors
+class BatteryStateData(Dict):  # pylint: disable=too-many-ancestors
     """
     A battery state data object.
 
     This class represents a battery state.
     It consists of a battery sample and a state id.
     """
 
@@ -96,28 +94,28 @@
     schema = BatteryStateSchema
 
     # pylint: disable=redefined-builtin
     def __init__(self, dict=None, **kwargs):
         """
         Constructor for the data class
 
-        Usage: ``BatteryState(dict{...})``
+        Usage: ``BatteryStateData(dict{...})``
 
         :param parameters_dict: dictionary with battery specifications
         :param type parameters_dict: dict
         """
         dict = self.validate(dict)
         super().__init__(dict=dict, **kwargs)
 
     def validate(self, parameters_dict):  # pylint: disable=no-self-use
         """Validate command line options.
 
         Uses the voluptuous package for validation. Find out about allowed keys using::
 
-            print(BatteryState.schema)
+            print(BatteryStateData.schema)
 
         :param parameters_dict: dictionary with battery specifications
         :param type parameters_dict: dict
         :returns: validated dictionary
         """
         return BatteryStateSchema(parameters_dict).dict()
```

### Comparing `aiida-aurora-0.2.0/aiida_aurora/data/control.py` & `aiida_aurora-0.3.1/aiida_aurora/data/control.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 """
 A dummy experiment specifications class.
 """
-
-from importlib import import_module
 import json
 
+from aurora.schemas.dgbowl_schemas import conversion_map
 import yaml
 
 from aiida.orm import Dict
 
 TOMATO_PAYLOAD_VERSION = "0.2"
-tomato_schema_module = import_module(
-    f"aurora.schemas.tomato_{TOMATO_PAYLOAD_VERSION.replace('.', 'p')}"
-)
-TomatoSchema = tomato_schema_module.tomato.Tomato
+TomatoSchema = conversion_map[TOMATO_PAYLOAD_VERSION]["tomato"]
 
 
-class TomatoSettings(Dict):  # pylint: disable=too-many-ancestors
+class TomatoSettingsData(Dict):  # pylint: disable=too-many-ancestors
     """
     An experiment specification object.
 
     This class represents the specifications used in an experiment.
     """
 
     # "pydantic" schema  to add automatic validation
     schema = TomatoSchema
 
     # pylint: disable=redefined-builtin
     def __init__(self, dict=None, **kwargs):
         """
         Constructor for the data class
 
-        Usage: ``TomatoSettings(dict{...})``
+        Usage: ``TomatoSettingsData(dict{...})``
 
         :param parameters_dict: dictionary with battery specifications
         :param type parameters_dict: dict
         """
         dict = self.validate(dict)
         super().__init__(dict=dict, **kwargs)
         # if not self.label:
         #     self.label = self.dict['metadata'].get('name')
 
     def validate(self, parameters_dict):  # pylint: disable=no-self-use
         """Validate command line options.
 
         Uses the voluptuous package for validation. Find out about allowed keys using::
 
-            print(TomatoSettings.schema)
+            print(TomatoSettingsData.schema)
 
         :param parameters_dict: dictionary with battery specifications
         :param type parameters_dict: dict
         :returns: validated dictionary
         """
         return TomatoSchema(**parameters_dict).dict()
 
@@ -58,15 +54,15 @@
         """Get a JSON file containing the DummyExperimentSpecs specs."""
 
         # this can be customized to fit the desired format
         object_to_be_serialized = self.get_dict()
         return json.dumps(object_to_be_serialized)
 
     def get_yaml(self):
-        """Get a YAML file containing the TomatoSettings specs."""
+        """Get a YAML file containing the TomatoSettingsData specs."""
 
         # this can be customized to fit the desired format
         object_to_be_serialized = {"tomato": self.get_dict()}
         return yaml.dump(object_to_be_serialized)
 
     def __str__(self):
         """String representation of node.
```

### Comparing `aiida-aurora-0.2.0/aiida_aurora/data/experiment.py` & `aiida_aurora-0.3.1/aiida_aurora/data/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from aurora.schemas.cycling import ElectroChemSequence as ElectroChemSequenceSchema
 import yaml
 
 from aiida.orm import Dict
 
 
-class CyclingSpecs(Dict):  # pylint: disable=too-many-ancestors
+class CyclingSpecsData(Dict):  # pylint: disable=too-many-ancestors
     """
     An experiment specification object.
 
     This class represents the specifications used in an experiment.
     """
 
     # "pydantic" schema  to add automatic validation
@@ -52,15 +52,15 @@
         """Get a JSON file containing the DummyExperimentSpecs specs."""
 
         # this can be customized to fit the desired format
         object_to_be_serialized = self.get_dict()
         return json.dumps(object_to_be_serialized)
 
     def get_yaml(self):
-        """Get a YAML file containing the BatterySample specs."""
+        """Get a YAML file containing the BatterySampleData specs."""
 
         # this can be customized to fit the desired format
         object_to_be_serialized = {"method": self.get_dict()}
         return yaml.dump(object_to_be_serialized)
 
     def __str__(self):
         """String representation of node.
```

### Comparing `aiida-aurora-0.2.0/aiida_aurora/helpers.py` & `aiida_aurora-0.3.1/aiida_aurora/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,15 @@
     try:
         executable = executables[entry_point]
     except KeyError as exc:
         raise KeyError(
             f"Entry point '{entry_point}' not recognized. Allowed values: {list(executables.keys())}"
         ) from exc
 
-    codes = Code.objects.find(
-        filters={"label": executable}
-    )  # pylint: disable=no-member
+    codes = Code.objects.find(filters={"label": executable})  # pylint: disable=no-member
     if codes:
         return codes[0]
 
     path = get_path_to_executable(executable)
     code = Code(
         input_plugin_name=entry_point,
         remote_computer_exec=[computer, path],
```

### Comparing `aiida-aurora-0.2.0/aiida_aurora/parsers.py` & `aiida_aurora-0.3.1/aiida_aurora/parsers.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,28 @@
 from aiida.plugins import CalculationFactory
 
 BatteryCyclerExperiment = CalculationFactory("aurora.cycler")
 
 
 class TomatoParser(Parser):
     """
-    Parser class for parsing output of calculation.
+    Parser class for parsing the output of a BatteryCyclerExperiment generated by tomato.
+    Two files should be found in the working directory:
+      - a ZIP file, containing the raw data
+      - a JSON file, containing the data pre-processed by tomato & yadg
+
+    Priority is to retrieve the parsed JSON file.
+    The raw data ZIP file is also retained if found.
     """
 
     def __init__(self, node):
         """
         Initialize Parser instance
 
-        Checks that the ProcessNode being passed was produced by a DiffCalculation.
+        Checks that the ProcessNode being passed was produced by a BatteryCyclerExperiment.
 
         :param node: ProcessNode of calculation
         :param type node: :class:`aiida.orm.ProcessNode`
         """
         super().__init__(node)
         if not issubclass(node.process_class, BatteryCyclerExperiment):
             raise exceptions.ParsingError("Can only parse BatteryCyclerExperiment")
@@ -40,65 +46,65 @@
         """
         Parse outputs, store results in database.
 
         :returns: an exit code, if parsing fails (or nothing if parsing succeeds)
         """
         retrieved_temporary_folder = kwargs["retrieved_temporary_folder"]
         output_json_filename = self.node.get_option("output_filename") + ".json"
-        output_zip_filename = os.path.join(
-            retrieved_temporary_folder, self.node.get_option("output_filename") + ".zip"
-        )
+        output_zip_filename = os.path.join(retrieved_temporary_folder, self.node.get_option("output_filename") + ".zip")
 
         files_retrieved = self.retrieved.list_object_names()
 
         # Check that zip file is present
         if os.path.isfile(output_zip_filename):
             try:
                 self.logger.debug(f"Storing '{output_zip_filename}'")
                 output_raw_data_node = SinglefileData(output_zip_filename)
                 self.out("raw_data", output_raw_data_node)
                 output_raw_data_node_created = True
             except Exception:
-                self.logger.warning(
-                    f"The raw data zip file '{output_zip_filename}' could not be read."
-                )
+                self.logger.warning(f"The raw data zip file '{output_zip_filename}' could not be read.")
                 output_raw_data_node_created = False
         else:
-            self.logger.warning(
-                f"The raw data zip file '{output_zip_filename}' is missing."
-            )
+            self.logger.warning(f"The raw data zip file '{output_zip_filename}' is missing.")
             output_raw_data_node_created = False
 
         # Check that json file is present
         if not output_json_filename in files_retrieved:
-            self.logger.error(
-                f"The output json file '{output_json_filename}' is missing."
-            )
+            self.logger.error(f"The output json file '{output_json_filename}' is missing.")
             if output_raw_data_node_created:
-                return self.exit_codes.ERROR_MISSING_JSON_FILE
-            return self.exit_codes.ERROR_MISSING_OUTPUT_FILES
+                # only json file is missing
+                return self.exit_codes.ERROR_OUTPUT_JSON_MISSING
+            # both files are missing
+            return self.exit_codes.ERROR_OUTPUT_FILES_MISSING
 
         # If a json file was found, parse it and add output node
         try:
             self.logger.debug(f"Parsing '{output_json_filename}'")
             with self.retrieved.open(output_json_filename, "r") as handle:
-                output_results_node = self.parse_tomato_results(
-                    json.load(handle), self.logger
-                )
+                output_results_node = self.parse_tomato_results(json.load(handle), self.logger)
             self.out("results", output_results_node)
-        except Exception:
+        except OSError:
+            self.logger.error(f"Error opening the json file '{output_json_filename}'.")
+            return self.exit_codes.ERROR_OUTPUT_JSON_READ
+        except json.JSONDecodeError:
             self.logger.error(f"Error parsing json file '{output_json_filename}'.")
-            return self.exit_codes.ERROR_PARSING_JSON_FILE
+            return self.exit_codes.ERROR_OUTPUT_JSON_PARSE
 
-        # check that the zip file is there. Is it already stored in a SinglefileData node??
+        # If found, the zip file was already stored in a SinglefileData node
         if not output_raw_data_node_created:
-            return self.exit_codes.ERROR_MISSING_ZIP_FILE
+            return self.exit_codes.WARNING_OUTPUT_ZIP_MISSING
 
-        # TODO: other checks:  jobs completed with error or cancelled
-        # ......
+        # If files were retrieved and parsed by the job was completed with error or cancelled,
+        # use the specific error codes
+        job_annotation = self.node.get_attribute("last_job_info").get("annotation")
+        if job_annotation == "Completed with error":
+            return self.exit_codes.WARNING_COMPLETED_ERROR
+        elif job_annotation == "Cancelled":
+            return self.exit_codes.WARNING_COMPLETED_CANCELLED
 
         return ExitCode(0)
 
     @staticmethod
     def parse_tomato_results(data_dic, logger=None):
         """
         Parse results.json file.
@@ -108,41 +114,30 @@
           - `data` is split in steps, physical quantity name, and n/s/u identifier (nominal value, std error, units)
             The name of each array is:  `'step{step_number}_{raw_quantity_name}_{identifier}'`
         """
         array_dic = {}
         for imstep, mstep in enumerate(data_dic["steps"]):  # method step
             raw_qty_names = list(mstep["data"][0]["raw"].keys())
             if logger:
-                logger.debug(
-                    f"parse_tomato_results: step {imstep}: {list(raw_qty_names)}"
-                )
+                logger.debug(f"parse_tomato_results: step {imstep}: {list(raw_qty_names)}")
             for raw_qty_name in raw_qty_names:
                 # substitute any special character with underscores
                 raw_qty_name_cleaned = re.sub("[^0-9a-zA-Z_]", "_", raw_qty_name)
                 if isinstance(mstep["data"][0]["raw"][raw_qty_name], dict):
                     for identifier in mstep["data"][0]["raw"][raw_qty_name].keys():
-                        array_dic[
-                            f"step{imstep}_{raw_qty_name_cleaned}_{identifier}"
-                        ] = np.array(
-                            [
-                                step["raw"][raw_qty_name][identifier]
-                                for step in mstep["data"]
-                            ]
-                        )
+                        array_dic[f"step{imstep}_{raw_qty_name_cleaned}_{identifier}"] = np.array([
+                            step["raw"][raw_qty_name][identifier] for step in mstep["data"]
+                        ])
                 else:
-                    array_dic[f"step{imstep}_{raw_qty_name_cleaned}"] = np.array(
-                        [step["raw"][raw_qty_name] for step in mstep["data"]]
-                    )
-            array_dic[f"step{imstep}_uts"] = np.array(
-                [step["uts"] for step in mstep["data"]]
-            )
+                    array_dic[f"step{imstep}_{raw_qty_name_cleaned}"] = np.array([
+                        step["raw"][raw_qty_name] for step in mstep["data"]
+                    ])
+            array_dic[f"step{imstep}_uts"] = np.array([step["uts"] for step in mstep["data"]])
         if logger:
-            logger.debug(
-                f"parse_tomato_results: arrays stored: {list(array_dic.keys())}"
-            )
+            logger.debug(f"parse_tomato_results: arrays stored: {list(array_dic.keys())}")
 
         node = ArrayData()
         for key, value in array_dic.items():
             node.set_array(key, value)
             node.set_attribute_many(data_dic["metadata"])
 
         return node
```

### Comparing `aiida-aurora-0.2.0/aiida_aurora/scheduler.py` & `aiida_aurora-0.3.1/aiida_aurora/scheduler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Plugin for the Tomato scheduler.
 """
 import datetime
 import re
 
+import yaml
+
 from aiida.common import exceptions
 from aiida.common.escaping import escape_for_bash
 from aiida.common.extendeddicts import AttributeDict
 from aiida.schedulers import Scheduler, SchedulerError
 from aiida.schedulers.datastructures import JobInfo, JobResource, JobState
 
 # There is no "job owner" in tomato.
@@ -28,16 +30,22 @@
     "qw": JobState.QUEUED,
     "r": JobState.RUNNING,
     "c": JobState.DONE,
     "ce": JobState.DONE,
     "cd": JobState.DONE,
 }
 
-# ketchup submit returns "jobid = {jobid}"
-_TOMATO_SUBMITTED_REGEXP = re.compile(r"(.*:\s*)?(jobid\s+=)\s+(?P<jobid>\d+)")
+_MAP_ANNOTATION_TOMATO = {
+    "q": "Queued",
+    "qw": "Queued, matching pipeline found",
+    "r": "Running",
+    "c": "Completed successfully",
+    "ce": "Completed with error",
+    "cd": "Cancelled",
+}
 
 
 class TomatoResource(JobResource):
     """Class for Tomato job resources."""
 
     @classmethod
     def validate_resources(cls, **kwargs):
@@ -104,22 +112,23 @@
         if user:
             raise exceptions.FeatureNotAvailable("Cannot query by user")
 
         if jobs:
             if isinstance(jobs, str):
                 command = f"{self.KETCHUP} status {escape_for_bash(jobs)}"
             else:
+                command = f"{self.KETCHUP} status "
                 try:
-                    command = " && ".join(f"{self.KETCHUP} status {j}" for j in jobs)
-                except TypeError:
+                    command += " ".join(f"{j}" for j in jobs)
+                except TypeError as e:
                     raise TypeError(
                         "If provided, the 'jobs' variable must be a string or an iterable of strings"
-                    )
+                    ) from e
         else:
-            command = f"{self.KETCHUP} status queue"
+            command = f"{self.KETCHUP} status queue -v"
 
         self._logger.debug(f"ketchup command: {command}")
         return command
 
     def _get_detailed_job_info_command(self, job_id):
         """Return the command to run to get the detailed information on a job,
         even after the job has finished.
@@ -142,17 +151,15 @@
         if job_tmpl.job_name:
             # I leave only letters, numbers, dots, dashes and underscores
             # Note: I don't compile the regexp, I am going to use it only once
             job_title = re.sub(r"[^a-zA-Z0-9_.-]+", "", job_tmpl.job_name)
 
             # prepend a 'j' (for 'job') before the string if the string
             # is now empty or does not start with a valid charachter
-            if not job_title or (
-                job_title[0] not in string.ascii_letters + string.digits
-            ):
+            if not job_title or (job_title[0] not in string.ascii_letters + string.digits):
                 job_title = f"j{job_title}"
 
             # Truncate to the first 128 characters
             # Nothing is done if the string is shorter.
             job_title = job_title[:128]
             if job_tmpl.shell_type == "powershell":
                 header = f"$JOB_TITLE='{job_title}'"
@@ -200,34 +207,22 @@
         for code_info in codes_info:
             command_to_exec_list = []
             for arg in code_info.cmdline_params:
                 command_to_exec_list.append(arg)
                 # command_to_exec_list.append(escape_for_bash(arg))
             command_to_exec = " ".join(command_to_exec_list)
 
-            stdin_str = (
-                f"< {escape_for_bash(code_info.stdin_name)}"
-                if code_info.stdin_name
-                else ""
-            )
-            stdout_str = (
-                f"> {escape_for_bash(code_info.stdout_name)}"
-                if code_info.stdout_name
-                else ""
-            )
+            stdin_str = (f"< {escape_for_bash(code_info.stdin_name)}" if code_info.stdin_name else "")
+            stdout_str = (f"> {escape_for_bash(code_info.stdout_name)}" if code_info.stdout_name else "")
 
             join_files = code_info.join_files
             if join_files:
                 stderr_str = "2>&1"
             else:
-                stderr_str = (
-                    f"2> {escape_for_bash(code_info.stderr_name)}"
-                    if code_info.stderr_name
-                    else ""
-                )
+                stderr_str = (f"2> {escape_for_bash(code_info.stderr_name)}" if code_info.stderr_name else "")
 
             output_string = f"{command_to_exec} {stdin_str} {stdout_str} {stderr_str}"
 
             list_of_runlines.append(output_string)
 
         self.logger.debug(f"_get_run_line output: {list_of_runlines}")
 
@@ -252,138 +247,108 @@
                 f"""stderr='{stderr.strip()}'"""
             )
         if stderr.strip():
             self.logger.warning(
                 f"ketchup returned exit code 0 (_parse_joblist_output function) but non-empty stderr='{stderr.strip()}'"
             )
 
-        jobdata_raw = [l for l in stdout.splitlines() if l]
+        # remove all empty lines and lines containing 'ERROR'
+        jobdata_raw = "\n".join(l for l in stdout.splitlines() if l and "ERROR" not in l)
+
+        def convert_datetime(dt):
+            if isinstance(dt, datetime.datetime):
+                return dt
+            try:
+                return datetime.datetime.fromisoformat(dt)
+            except Exception:
+                return None
 
         # Create dictionary and parse specific fields
         job_list = []
 
-        if "=========" in jobdata_raw[1]:
+        if "===========================" in jobdata_raw:
             # the command was 'ketchup status queue'
+            jobdata_raw = jobdata_raw.splitlines()
             if len(jobdata_raw) > 2:
                 for line in jobdata_raw[2:]:
                     job = line.split()
                     this_job = JobInfo()
                     this_job.job_id = job[0]
                     this_job.title = job[1]
 
                     try:
                         this_job.job_state = _MAP_STATUS_TOMATO[job[2]]
+                        this_job.annotation = _MAP_ANNOTATION_TOMATO[job[2]]
                     except KeyError:
-                        self.logger.warning(
-                            f"Unrecognized job_state '{job[2]}' for job id {this_job.job_id}"
-                        )
+                        self.logger.warning(f"Unrecognized job_state '{job[2]}' for job id {this_job.job_id}")
                         this_job.job_state = JobState.UNDETERMINED
 
                     if len(job) == 3:
                         this_job.pipeline = None
                     elif len(job) == 4:
                         this_job.pipeline = job[3]
                     else:
-                        raise ValueError(
-                            f"More than 4 columns returned by ketchup status queue\n{job}"
-                        )
+                        raise ValueError(f"More than 4 columns returned by ketchup status queue\n{job}")
 
                     # Everything goes here anyway for debugging purposes
                     this_job.raw_data = job
 
                     # I append to the list of jobs to return
                     job_list.append(this_job)
             else:
                 pass  # there are no jobs in the queue
 
-        elif "jobid =" in jobdata_raw[0]:
-            # the command was 'ketchup status {jobid} && ...'
-            this_job = None
-            for raw_line in jobdata_raw:
-                line = list(map(str.strip, raw_line.split("=")))  # split line at '='
-                if "jobid" in line[0]:
-                    if this_job:
-                        job_list.append(this_job)  # append previous job read
-                    this_job = JobInfo()
-                    this_job.job_id = line[1]
-                elif "jobname" in line[0]:
-                    this_job.title = line[1]
-                elif "status" in line[0]:
-                    try:
-                        this_job.job_state = _MAP_STATUS_TOMATO[line[1]]
-                    except KeyError:
-                        self.logger.warning(
-                            f"Unrecognized job_state '{line[1]}' for job id {this_job.job_id}"
-                        )
-                        this_job.job_state = JobState.UNDETERMINED
-                elif "submitted at" in line[0]:
-                    try:
-                        this_job.submission_time = datetime.datetime.fromisoformat(
-                            line[1]
-                        )
-                    except (ValueError, IndexError):
-                        self.logger.warning(
-                            f"Error parsing submission_time for job id {this_job.job_id}"
-                        )
-                elif "executed at" in line[0]:
-                    try:
-                        this_job.dispatch_time = datetime.datetime.fromisoformat(
-                            line[1]
-                        )
-                    except (ValueError, IndexError):
-                        self.logger.warning(
-                            f"Error parsing dispatch_time for job id {this_job.job_id}"
-                        )
-                elif "completed at" in line[0]:
-                    try:
-                        this_job.finish_time = datetime.datetime.fromisoformat(line[1])
-                    except (ValueError, IndexError):
-                        self.logger.warning(
-                            f"Error parsing finished_time for job id {this_job.job_id}"
-                        )
-                elif "with pipeline" in line[0]:
-                    this_job.allocated_machines = [(line[1])]
-                elif "with PID" in line[0]:
-                    pass
-                else:
-                    self.logger.warning(f"Unrecognized line: {line}")
+        else:
+            # the command was 'ketchup status {jobid} ...'
+            # the output is yaml-formatted
+            jobdata_parsed = yaml.full_load(jobdata_raw)
+
+            for this_job_dict in jobdata_parsed:
+                this_job = JobInfo()
+                this_job.job_id = str(this_job_dict["jobid"])
+                this_job.title = this_job_dict["jobname"]
+                try:
+                    this_job_status = this_job_dict["status"]
+                    this_job.job_state = _MAP_STATUS_TOMATO[this_job_status]
+                    this_job.annotation = _MAP_ANNOTATION_TOMATO[this_job_status]
+                except KeyError:
+                    self.logger.warning(f"Unrecognized job_state '{this_job_status}' for job id {this_job.job_id}")
+                    this_job.job_state = JobState.UNDETERMINED
+
+                # yaml parses iso-format datetime strings automatically:
+                this_job.submission_time = convert_datetime(this_job_dict.get("submitted"))
+                this_job.dispatch_time = convert_datetime(this_job_dict.get("executed"))
+                this_job.finish_time = convert_datetime(this_job_dict.get("completed"))
+                this_job.allocated_machines = this_job_dict.get("pipeline")
+                # ignored: this_job_dict.get("pid")
 
-            job_list.append(this_job)  # append last job
+                job_list.append(this_job)  # append last job
 
         return job_list
 
     def _parse_submit_output(self, retval, stdout, stderr):
         """Parse the output of the submit command returned by calling the `_get_submit_command` command.
 
         :return: a string with the job ID.
         """
         if retval != 0:
-            self._logger.error(
-                f"Error in _parse_submit_output: retval={retval}; stdout={stdout}; stderr={stderr}"
-            )
-            raise SchedulerError(
-                f"Error during submission, retval={retval}; stdout={stdout}; stderr={stderr}"
-            )
+            self._logger.error(f"Error in _parse_submit_output: retval={retval}; stdout={stdout}; stderr={stderr}")
+            raise SchedulerError(f"Error during submission, retval={retval}; stdout={stdout}; stderr={stderr}")
 
         if stderr.strip():
-            self._logger.warning(
-                f"in _parse_submit_output there was some text in stderr: {stderr}"
-            )
+            self._logger.warning(f"in _parse_submit_output there was some text in stderr: {stderr}")
 
-        # I check for a valid string in the output.
-        # See comments near the regexp above.
-        # I check for the first line that matches.
-        for line in stdout.split("\n"):
-            match = _TOMATO_SUBMITTED_REGEXP.match(line.strip())
-            if match:
-                return match.group("jobid")
-        # If I am here, no valid line could be found.
-        self.logger.error(
-            f"in _parse_submit_output: unable to find the job id: {stdout}"
-        )
+        # I check for the jobid in the output
+        stdout_dict = yaml.full_load(stdout)
+        if "jobid" in stdout_dict:
+            self._logger.debug(f"The submitted jobid is {stdout_dict['jobid']}")
+            return stdout_dict["jobid"]
+
+        # If I am here, no jobid was found
+        self.logger.error(f"in _parse_submit_output: unable to find the job id: {stdout}")
         raise SchedulerError(
             "Error during submission, could not retrieve the jobID from ketchup output; see log for more info."
         )
 
     def _get_kill_command(self, jobid):
         """Return the command to kill the job with specified jobid."""
 
@@ -395,28 +360,22 @@
 
     def _parse_kill_output(self, retval, stdout, stderr):
         """Parse the output of the kill command.
 
         :return: True if everything seems ok, False otherwise.
         """
         if retval != 0:
-            self._logger.error(
-                f"Error in _parse_kill_output: retval={retval}; stdout={stdout}; stderr={stderr}"
-            )
+            self._logger.error(f"Error in _parse_kill_output: retval={retval}; stdout={stdout}; stderr={stderr}")
             return False
 
         if stderr.strip():
-            self._logger.warning(
-                f"in _parse_kill_output there was some text in stderr: {stderr}"
-            )
+            self._logger.warning(f"in _parse_kill_output there was some text in stderr: {stderr}")
 
         if stdout.strip():
-            self._logger.warning(
-                f"in _parse_kill_output there was some text in stdout: {stdout}"
-            )
+            self._logger.warning(f"in _parse_kill_output there was some text in stdout: {stdout}")
 
         return True
 
     def parse_output(self, detailed_job_info, stdout, stderr):
         """Parse the output of the scheduler.
 
         :param detailed_job_info: dictionary with the output returned by the `Scheduler.get_detailed_job_info` command.
```

### Comparing `aiida-aurora-0.2.0/pyproject.toml` & `aiida_aurora-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -46,23 +46,26 @@
     "sphinxcontrib-contentui",
     "sphinxcontrib-details-directive",
     "furo",
     "markupsafe<2.1"
 ]
 
 [project.entry-points."aiida.data"]
-"aurora.batterysample" = "aiida_aurora.data.battery:BatterySample"
-"aurora.batterystate" = "aiida_aurora.data.battery:BatteryState"
-"aurora.cyclingspecs" = "aiida_aurora.data.experiment:CyclingSpecs"
-"aurora.tomatosettings" = "aiida_aurora.data.control:TomatoSettings"
+"aurora.batterysample" = "aiida_aurora.data.battery:BatterySampleData"
+"aurora.batterystate" = "aiida_aurora.data.battery:BatteryStateData"
+"aurora.cyclingspecs" = "aiida_aurora.data.experiment:CyclingSpecsData"
+"aurora.tomatosettings" = "aiida_aurora.data.control:TomatoSettingsData"
 
 [project.entry-points."aiida.calculations"]
 "aurora.fake" = "aiida_aurora.calculations.fake:BatteryFakeExperiment"
 "aurora.cycler" = "aiida_aurora.calculations.cycler:BatteryCyclerExperiment"
 
+[project.entry-points.'aiida.workflows']
+'aurora.stress_test' = 'aiida_aurora.workflows.stress_test:StressTestWorkChain'
+
 [project.entry-points."aiida.parsers"]
 "aurora" = "aiida_aurora.parsers:TomatoParser"
 
 [project.entry-points."aiida.schedulers"]
 "tomato" = "aiida_aurora.scheduler:TomatoScheduler"
 
 [project.entry-points."aiida.cmdline.data"]
```

### Comparing `aiida-aurora-0.2.0/PKG-INFO` & `aiida_aurora-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-aurora
-Version: 0.2.0
+Version: 0.3.1
 Summary: AiiDA plugin for the Aurora platform.
 Keywords: aiida,plugin,aurora
 Author-email: Loris Ercole <loris.ercole@epfl.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
```

