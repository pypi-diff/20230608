# Comparing `tmp/qiskit_braket_provider-0.0.3.tar.gz` & `tmp/qiskit_braket_provider-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_braket_provider-0.0.3.tar", last modified: Wed Nov 23 21:13:13 2022, max compression
+gzip compressed data, was "qiskit_braket_provider-0.0.4.tar", last modified: Thu Jun  8 19:04:14 2023, max compression
```

## Comparing `qiskit_braket_provider-0.0.3.tar` & `qiskit_braket_provider-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 21:13:13.381343 qiskit_braket_provider-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11416 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2943 2022-11-23 21:13:13.381343 qiskit_braket_provider-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1980 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 21:13:13.377343 qiskit_braket_provider-0.0.3/qiskit_braket_provider/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 21:13:13.381343 qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/
--rw-r--r--   0 runner    (1001) docker     (122)      680 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13165 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8649 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/braket_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4107 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/braket_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/braket_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 21:13:13.377343 qiskit_braket_provider-0.0.3/qiskit_braket_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2943 2022-11-23 21:13:13.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      796 2022-11-23 21:13:13.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-23 21:13:13.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      131 2022-11-23 21:13:13.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2022-11-23 21:13:13.000000 qiskit_braket_provider-0.0.3/qiskit_braket_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2022-11-23 21:13:13.381343 qiskit_braket_provider-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 21:13:13.381343 qiskit_braket_provider-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 21:13:13.381343 qiskit_braket_provider-0.0.3/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/tests/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3751 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/tests/providers/mocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/tests/providers/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8512 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/tests/providers/test_braket_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/tests/providers/test_braket_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     2554 2022-11-23 21:13:04.000000 qiskit_braket_provider-0.0.3/tests/providers/test_braket_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:04:14.141635 qiskit_braket_provider-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-08 19:04:14.141635 qiskit_braket_provider-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:04:14.141635 qiskit_braket_provider-0.0.4/qiskit_braket_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:04:14.141635 qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/braket_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/braket_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/braket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:04:14.141635 qiskit_braket_provider-0.0.4/qiskit_braket_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-08 19:04:14.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-08 19:04:14.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:04:14.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-08 19:04:14.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 19:04:14.000000 qiskit_braket_provider-0.0.4/qiskit_braket_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 19:04:14.145635 qiskit_braket_provider-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:04:14.141635 qiskit_braket_provider-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:04:14.141635 qiskit_braket_provider-0.0.4/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/tests/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/tests/providers/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/tests/providers/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/tests/providers/test_braket_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/tests/providers/test_braket_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-08 19:04:04.000000 qiskit_braket_provider-0.0.4/tests/providers/test_braket_provider.py
```

### Comparing `qiskit_braket_provider-0.0.3/LICENSE.txt` & `qiskit_braket_provider-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.0.3/PKG-INFO` & `qiskit_braket_provider-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_braket_provider
-Version: 0.0.3
+Version: 0.0.4
 Summary: Qiskit-Braket provider to execute Qiskit programs on AWS quantum computing hardware devices through Amazon Braket.
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: qiskit braket sdk quantum
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qiskit_braket_provider-0.0.3/README.md` & `qiskit_braket_provider-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/__init__.py` & `qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/adapter.py` & `qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """Util function for provider."""
 from typing import Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 from braket.aws import AwsDevice
-from braket.circuits import Circuit, Instruction, gates, result_types
+from braket.circuits import (
+    Circuit,
+    FreeParameter,
+    Instruction,
+    gates,
+    result_types,
+    observables,
+)
 from braket.device_schema import (
     DeviceActionType,
     GateModelQpuParadigmProperties,
     JaqcdDeviceActionProperties,
+    OpenQASMDeviceActionProperties,
 )
 from braket.device_schema.ionq import IonqDeviceCapabilities
 from braket.device_schema.oqc import OqcDeviceCapabilities
 from braket.device_schema.rigetti import RigettiDeviceCapabilities
 from braket.device_schema.simulators import (
     GateModelSimulatorDeviceCapabilities,
     GateModelSimulatorParadigmProperties,
@@ -40,26 +48,28 @@
     SdgGate,
     SGate,
     SwapGate,
     SXdgGate,
     SXGate,
     TdgGate,
     TGate,
+    UGate,
     U1Gate,
     U2Gate,
     U3Gate,
     XGate,
     YGate,
     ZGate,
 )
 from qiskit.transpiler import InstructionProperties, Target
 
 from qiskit_braket_provider.exception import QiskitBraketException
 
 qiskit_to_braket_gate_names_mapping = {
+    "u": "u",
     "u1": "u1",
     "u2": "u2",
     "u3": "u3",
     "p": "phaseshift",
     "cx": "cnot",
     "x": "x",
     "y": "y",
@@ -85,14 +95,21 @@
     "rxx": "xx",
     "ryy": "yy",
     "ecr": "ecr",
 }
 
 
 qiskit_gate_names_to_braket_gates: Dict[str, Callable] = {
+    "u": lambda theta, phi, lam: [
+        gates.Rz(lam),
+        gates.Rx(pi / 2),
+        gates.Rz(theta),
+        gates.Rx(-pi / 2),
+        gates.Rz(phi),
+    ],
     "u1": lambda lam: [gates.Rz(lam)],
     "u2": lambda phi, lam: [gates.Rz(lam), gates.Ry(pi / 2), gates.Rz(phi)],
     "u3": lambda theta, phi, lam: [
         gates.Rz(lam),
         gates.Rx(pi / 2),
         gates.Rz(theta),
         gates.Rx(-pi / 2),
@@ -124,14 +141,15 @@
     "rxx": lambda angle: [gates.XX(angle)],
     "ryy": lambda angle: [gates.YY(angle)],
     "ecr": lambda: [gates.ECR()],
 }
 
 
 qiskit_gate_name_to_braket_gate_mapping: Dict[str, Optional[QiskitInstruction]] = {
+    "u": UGate(Parameter("theta"), Parameter("phi"), Parameter("lam")),
     "u1": U1Gate(Parameter("theta")),
     "u2": U2Gate(Parameter("theta"), Parameter("lam")),
     "u3": U3Gate(Parameter("theta"), Parameter("phi"), Parameter("lam")),
     "h": HGate(),
     "ccnot": CCXGate(),
     "cnot": CXGate(),
     "cphaseshift": CPhaseGate(Parameter("theta")),
@@ -229,16 +247,18 @@
 
     properties = device.properties
     # gate model devices
     if isinstance(
         properties,
         (IonqDeviceCapabilities, RigettiDeviceCapabilities, OqcDeviceCapabilities),
     ):
-        action_properties: JaqcdDeviceActionProperties = properties.action.get(
-            DeviceActionType.JAQCD
+        action_properties: OpenQASMDeviceActionProperties = (
+            properties.action.get(DeviceActionType.OPENQASM)
+            if properties.action.get(DeviceActionType.OPENQASM)
+            else properties.action.get(DeviceActionType.JAQCD)
         )
         paradigm: GateModelQpuParadigmProperties = properties.paradigm
         connectivity = paradigm.connectivity
         instructions: List[QiskitInstruction] = []
 
         for operation in action_properties.supportedOperations:
             instruction = _op_to_instruction(operation)
@@ -343,29 +363,35 @@
     quantum_circuit = Circuit()
     for qiskit_gates in circuit.data:
         name = qiskit_gates[0].name
         if name == "measure":
             # TODO: change Probability result type for Sample for proper functioning # pylint:disable=fixme
             # Getting the index from the bit mapping
             quantum_circuit.add_result_type(
-                result_types.Probability(
+                # pylint:disable=fixme
+                result_types.Sample(
+                    observable=observables.Z(),
                     target=[
                         circuit.find_bit(qiskit_gates[1][0]).index,
                         circuit.find_bit(qiskit_gates[2][0]).index,
-                    ]
+                    ],
                 )
             )
         elif name == "barrier":
             # This does not exist
             pass
         else:
             params = []
             if hasattr(qiskit_gates[0], "params"):
                 params = qiskit_gates[0].params
 
+            for i, param in enumerate(params):
+                if isinstance(param, Parameter):
+                    params[i] = FreeParameter(param.name)
+
             for gate in qiskit_gate_names_to_braket_gates[name](*params):
                 instruction = Instruction(
                     # Getting the index from the bit mapping
                     operator=gate,
                     target=[circuit.find_bit(i).index for i in qiskit_gates[1]],
                 )
                 quantum_circuit += instruction
```

### Comparing `qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/braket_backend.py` & `qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/braket_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """AWS Braket backends."""
 
 
 import datetime
 import logging
 from abc import ABC
 from typing import Iterable, Union, List
-import pkg_resources
 
 from braket.aws import AwsDevice, AwsQuantumTaskBatch, AwsQuantumTask
 from braket.circuits import Circuit
 from braket.devices import LocalSimulator
 from braket.tasks.local_quantum_task import LocalQuantumTask
 from qiskit import QuantumCircuit
 from qiskit.providers import BackendV2, QubitProperties, Options, Provider
@@ -17,14 +16,15 @@
 from .adapter import (
     aws_device_to_target,
     local_simulator_to_target,
     convert_qiskit_to_braket_circuits,
     wrap_circuits_in_verbatim_box,
 )
 from .braket_job import AWSBraketJob
+from .. import version
 from ..exception import QiskitBraketException
 
 logger = logging.getLogger(__name__)
 
 
 TASK_ID_DIVIDER = ";"
 
@@ -49,15 +49,15 @@
             >>> device = LocalSimulator(name="braket_sv")      #Local State Vector Simulator
             >>> device = LocalSimulator(name="braket_dm")      #Local Density Matrix Simulator
 
         Args:
             name: name of backend
             **fields: extra fields
         """
-        super().__init__(name="sv_simulator", **fields)
+        super().__init__(name=name, **fields)
         self.backend_name = name
         self._aws_device = LocalSimulator(backend=self.backend_name)
         self._target = local_simulator_to_target(self._aws_device)
         self.status = self._aws_device.status
 
     @property
     def target(self):
@@ -97,20 +97,21 @@
 
     def control_channel(self, qubits: Iterable[int]):
         raise NotImplementedError(f"Control channel is not supported by {self.name}.")
 
     def run(
         self, run_input: Union[QuantumCircuit, List[QuantumCircuit]], **options
     ) -> AWSBraketJob:
-
         convert_input = (
             [run_input] if isinstance(run_input, QuantumCircuit) else list(run_input)
         )
         circuits: List[Circuit] = list(convert_qiskit_to_braket_circuits(convert_input))
         shots = options["shots"] if "shots" in options else 1024
+        if shots == 0:
+            circuits = list(map(lambda x: x.state_vector(), circuits))
         tasks = []
         try:
             for circuit in circuits:
                 task: Union[LocalQuantumTask] = self._aws_device.run(
                     task_specification=circuit, shots=shots
                 )
                 tasks.append(task)
@@ -169,16 +170,15 @@
             provider=provider,
             name=name,
             description=description,
             online_date=online_date,
             backend_version=backend_version,
             **fields,
         )
-        pkg_version = pkg_resources.get_distribution("qiskit-braket-provider").version
-        user_agent = f"QiskitBraketProvider/{pkg_version}"
+        user_agent = f"QiskitBraketProvider/{version.__version__}"
         device.aws_session.add_braket_user_agent(user_agent)
         self._device = device
         self._target = aws_device_to_target(device=device)
 
     def retrieve_job(self, job_id: str) -> AWSBraketJob:
         """Return a single job submitted to AWS backend.
```

### Comparing `qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/braket_job.py` & `qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/braket_job.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,24 +37,36 @@
     """
     experiment_results: List[ExperimentResult] = []
 
     # For each task the results is get and filled into an ExperimentResult object
     for task in tasks:
         if task.state() in AwsQuantumTask.RESULTS_READY_STATES:
             result: GateModelQuantumTaskResult = task.result()
-            counts = {
-                k[::-1]: v for k, v in dict(result.measurement_counts).items()
-            }  # convert to little-endian
-            data = ExperimentResultData(
-                counts=counts,
-                memory=[
-                    "".join(shot_result[::-1].astype(str))
-                    for shot_result in result.measurements
-                ],
-            )
+
+            if result.task_metadata.shots == 0:
+                statevector = result.values[
+                    result._result_types_indices[
+                        "{'type': <Type.statevector: 'statevector'>}"
+                    ]
+                ]
+                data = ExperimentResultData(
+                    statevector=statevector,
+                )
+            else:
+                counts = {
+                    k[::-1]: v for k, v in dict(result.measurement_counts).items()
+                }  # convert to little-endian
+
+                data = ExperimentResultData(
+                    counts=counts,
+                    memory=[
+                        "".join(shot_result[::-1].astype(str))
+                        for shot_result in result.measurements
+                    ],
+                )
         else:
             return None
 
         experiment_result = ExperimentResult(
             shots=result.task_metadata.shots,
             success=True,
             status=task.state(),
```

### Comparing `qiskit_braket_provider-0.0.3/qiskit_braket_provider/providers/braket_provider.py` & `qiskit_braket_provider-0.0.4/qiskit_braket_provider/providers/braket_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
          BraketBackend[Lucy],
          BraketBackend[SV1],
          BraketBackend[TN1],
          BraketBackend[dm1]]
     """
 
     def backends(self, name=None, **kwargs):
-
         if kwargs.get("local"):
             return [BraketLocalBackend(name="default")]
         names = [name] if name else None
         devices = AwsDevice.get_devices(names=names, **kwargs)
         # filter by supported devices
         # gate models are only supported
         supported_devices = [
```

### Comparing `qiskit_braket_provider-0.0.3/qiskit_braket_provider.egg-info/PKG-INFO` & `qiskit_braket_provider-0.0.4/qiskit_braket_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-braket-provider
-Version: 0.0.3
+Version: 0.0.4
 Summary: Qiskit-Braket provider to execute Qiskit programs on AWS quantum computing hardware devices through Amazon Braket.
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: qiskit braket sdk quantum
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qiskit_braket_provider-0.0.3/qiskit_braket_provider.egg-info/SOURCES.txt` & `qiskit_braket_provider-0.0.4/qiskit_braket_provider.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 qiskit_braket_provider/__init__.py
 qiskit_braket_provider/exception.py
+qiskit_braket_provider/version.py
 qiskit_braket_provider.egg-info/PKG-INFO
 qiskit_braket_provider.egg-info/SOURCES.txt
 qiskit_braket_provider.egg-info/dependency_links.txt
 qiskit_braket_provider.egg-info/requires.txt
 qiskit_braket_provider.egg-info/top_level.txt
 qiskit_braket_provider/providers/__init__.py
 qiskit_braket_provider/providers/adapter.py
```

### Comparing `qiskit_braket_provider-0.0.3/setup.py` & `qiskit_braket_provider-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """Setup file for Qiskit-Braket provider."""
 import os
+from typing import Any, Dict, Optional
+
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 version_path = os.path.abspath(
-    os.path.join(os.path.dirname(__file__), "qiskit_braket_provider", "VERSION.txt")
+    os.path.join(os.path.dirname(__file__), "qiskit_braket_provider", "version.py")
 )
 
-with open(version_path, "r") as fd:
-    version = fd.read().rstrip()
+version_dict: Optional[Dict[str, Any]] = {}
+with open(version_path) as fp:
+    exec(fp.read(), version_dict)
+version = version_dict["__version__"]
 
 setuptools.setup(
     name="qiskit_braket_provider",
     description="Qiskit-Braket provider to execute Qiskit "
     "programs on AWS quantum computing "
     "hardware devices through Amazon Braket.",
     long_description=long_description,
```

### Comparing `qiskit_braket_provider-0.0.3/tests/providers/mocks.py` & `qiskit_braket_provider-0.0.4/tests/providers/mocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
                 "windowStartHour": "11:00",
                 "windowEndHour": "12:00",
             }
         ],
         "shotsRange": [1, 10],
     },
     "action": {
-        "braket.ir.jaqcd.program": {
-            "actionType": "braket.ir.jaqcd.program",
+        "braket.ir.openqasm.program": {
+            "actionType": "braket.ir.openqasm.program",
             "version": ["1"],
             "supportedOperations": ["H"],
         }
     },
     "paradigm": {
         "qubitCount": 30,
         "nativeGateSet": ["ccnot", "cy"],
```

### Comparing `qiskit_braket_provider-0.0.3/tests/providers/test_braket_backend.py` & `qiskit_braket_provider-0.0.4/tests/providers/test_braket_backend.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests for AWS Braket backends."""
 import unittest
+from typing import Dict, List
 from unittest import TestCase
 from unittest.mock import Mock
-import pkg_resources
 
 from botocore import errorfactory
 from qiskit import QuantumCircuit, transpile, BasicAer
 from qiskit.algorithms import VQE, VQEResult
 from qiskit.algorithms.optimizers import (
     SLSQP,
 )
@@ -17,35 +17,58 @@
     X,
     Z,
 )
 from qiskit.result import Result
 from qiskit.transpiler import Target
 from qiskit.utils import QuantumInstance
 
-from qiskit_braket_provider import AWSBraketProvider
+from qiskit_braket_provider import AWSBraketProvider, version
 from qiskit_braket_provider.providers import AWSBraketBackend, BraketLocalBackend
 from qiskit_braket_provider.providers.adapter import aws_device_to_target
 from tests.providers.mocks import RIGETTI_MOCK_GATE_MODEL_QPU_CAPABILITIES
 
 
+def combine_dicts(
+    dict1: Dict[str, float], dict2: Dict[str, float]
+) -> Dict[str, List[float]]:
+    """Combines dictionaries with different keys.
+
+    Args:
+        dict1: first
+        dict2: second
+
+    Returns:
+        merged dicts with list of keys
+    """
+    combined_dict: Dict[str, List[float]] = {}
+    for key in dict1.keys():
+        if key in combined_dict:
+            combined_dict[key].append(dict1[key])
+        else:
+            combined_dict[key] = [dict1[key]]
+    for key in dict2.keys():
+        if key in combined_dict:
+            combined_dict[key].append(dict2[key])
+        else:
+            combined_dict[key] = [dict2[key]]
+    return combined_dict
+
+
 class TestAWSBraketBackend(TestCase):
     """Tests BraketBackend."""
 
     def test_device_backend(self):
         """Tests device backend."""
         device = Mock()
         device.properties = RIGETTI_MOCK_GATE_MODEL_QPU_CAPABILITIES
         backend = AWSBraketBackend(device)
         self.assertTrue(backend)
         self.assertIsInstance(backend.target, Target)
         self.assertIsNone(backend.max_circuits)
-        user_agent = (
-            f"QiskitBraketProvider/"
-            f"{pkg_resources.get_distribution('qiskit-braket-provider').version}"
-        )
+        user_agent = f"QiskitBraketProvider/" f"{version.__version__}"
         device.aws_session.add_braket_user_agent.assert_called_with(user_agent)
         with self.assertRaises(NotImplementedError):
             backend.drive_channel(0)
         with self.assertRaises(NotImplementedError):
             backend.acquire_channel(0)
         with self.assertRaises(NotImplementedError):
             backend.measure_channel(0)
@@ -63,14 +86,19 @@
         with self.assertRaises(NotImplementedError):
             backend.acquire_channel(0)
         with self.assertRaises(NotImplementedError):
             backend.measure_channel(0)
         with self.assertRaises(NotImplementedError):
             backend.control_channel([0, 1])
 
+    def test_local_backend_output(self):
+        """Test local backend output"""
+        first_backend = BraketLocalBackend(name="braket_dm")
+        self.assertEqual(first_backend.backend_name, "braket_dm")
+
     def test_local_backend_circuit(self):
         """Tests local backend with circuit."""
         backend = BraketLocalBackend(name="default")
         circuits = []
 
         # Circuit 0
         q_c = QuantumCircuit(2)
@@ -91,14 +119,30 @@
         # Result 0
         self.assertEqual(results[0].get_counts(), {"11": 1024})
         # Result 1
         _00 = results[1].get_counts()["00"]
         _11 = results[1].get_counts()["11"]
         self.assertEqual(_00 + _11, 1024)
 
+    def test_local_backend_circuit_shots0(self):
+        """Tests local backend with circuit with shots=0."""
+        backend = BraketLocalBackend(name="default")
+
+        circuit = QuantumCircuit(2)
+        circuit.x(0)
+        circuit.cx(0, 1)
+
+        result = backend.run(circuit, shots=0).result()
+
+        statevector = result.get_statevector()
+        self.assertEqual(statevector[0], 0.0 + 0.0j)
+        self.assertEqual(statevector[1], 0.0 + 0.0j)
+        self.assertEqual(statevector[2], 0.0 + 0.0j)
+        self.assertEqual(statevector[3], 1.0 + 0.0j)
+
     def test_vqe(self):
         """Tests VQE."""
         local_simulator = BraketLocalBackend(name="default")
 
         h2_op = (
             (-1.052373245772859 * I ^ I)
             + (0.39793742484318045 * I ^ Z)
@@ -143,19 +187,34 @@
                 )
                 aer_result = (
                     aer_backend.run(transpiled_aer_circuit, shots=1000)
                     .result()
                     .get_counts()
                 )
 
-                self.assertEqual(
-                    sorted([k for k, v in braket_result.items() if v > 50]),
-                    sorted([k for k, v in aer_result.items() if v > 0.05]),
+                combined_results = combine_dicts(
+                    {k: float(v) / 1000.0 for k, v in braket_result.items()}, aer_result
                 )
-                self.assertIsInstance(braket_result, dict)
+
+                for key, values in combined_results.items():
+                    if len(values) == 1:
+                        self.assertTrue(
+                            values[0] < 0.05,
+                            f"Missing {key} key in one of the results.",
+                        )
+                    else:
+                        percent_diff = abs(
+                            ((float(values[0]) - values[1]) / values[0]) * 100
+                        )
+                        abs_diff = abs(values[0] - values[1])
+                        self.assertTrue(
+                            percent_diff < 10 or abs_diff < 0.05,
+                            f"Key {key} with percent difference {percent_diff} "
+                            f"and absolute difference {abs_diff}. Original values {values}",
+                        )
 
     @unittest.skip("Call to external resources.")
     def test_retrieve_job(self):
         """Tests retrieve job by id."""
         backend = AWSBraketProvider().get_backend("SV1")
         circuits = [
             transpile(
```

### Comparing `qiskit_braket_provider-0.0.3/tests/providers/test_braket_job.py` & `qiskit_braket_provider-0.0.4/tests/providers/test_braket_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.0.3/tests/providers/test_braket_provider.py` & `qiskit_braket_provider-0.0.4/tests/providers/test_braket_provider.py`

 * *Files identical despite different names*

