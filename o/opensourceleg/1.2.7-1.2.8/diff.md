# Comparing `tmp/opensourceleg-1.2.7.tar.gz` & `tmp/opensourceleg-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.2.7.tar", max compression
+gzip compressed data, was "opensourceleg-1.2.8.tar", max compression
```

## Comparing `opensourceleg-1.2.7.tar` & `opensourceleg-1.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.7/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.7/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.7/opensourceleg/__init__.py
--rw-r--r--   0        0        0    22954 2023-06-06 02:22:42.448913 opensourceleg-1.2.7/opensourceleg/actuators.py
--rw-r--r--   0        0        0      136 2023-06-05 20:47:17.478958 opensourceleg-1.2.7/opensourceleg/ankle_encoder_map.npy
--rw-r--r--   0        0        0     1156 2023-06-06 13:48:00.772459 opensourceleg-1.2.7/opensourceleg/constants.py
--rw-r--r--   0        0        0      805 2023-06-06 13:04:42.094571 opensourceleg-1.2.7/opensourceleg/control.py
--rw-r--r--   0        0        0     6668 2023-06-07 03:52:26.170016 opensourceleg-1.2.7/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.7/opensourceleg/example.py
--rw-r--r--   0        0        0    10820 2023-06-06 14:59:16.262812 opensourceleg-1.2.7/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.7/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8513 2023-06-06 02:25:22.342625 opensourceleg-1.2.7/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.7/opensourceleg/logger.py
--rw-r--r--   0        0        0    17214 2023-06-07 03:50:21.478357 opensourceleg-1.2.7/opensourceleg/osl.py
--rw-r--r--   0        0        0    14963 2023-06-05 15:50:42.804893 opensourceleg-1.2.7/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.7/opensourceleg/thermal.py
--rw-r--r--   0        0        0    21242 2023-06-07 02:24:24.140310 opensourceleg-1.2.7/opensourceleg/tui.py
--rw-r--r--   0        0        0     4331 2023-06-05 20:47:20.793114 opensourceleg-1.2.7/opensourceleg/units.py
--rw-r--r--   0        0        0    11587 2023-06-06 02:26:59.481937 opensourceleg-1.2.7/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-06-07 03:53:10.358519 opensourceleg-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.8/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.8/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.8/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    22954 2023-06-08 20:35:27.080440 opensourceleg-1.2.8/opensourceleg/actuators.py
+-rw-r--r--   0        0        0      136 2023-06-05 20:47:17.478958 opensourceleg-1.2.8/opensourceleg/ankle_encoder_map.npy
+-rw-r--r--   0        0        0     1156 2023-06-08 20:36:58.593678 opensourceleg-1.2.8/opensourceleg/constants.py
+-rw-r--r--   0        0        0      805 2023-06-06 13:04:42.094571 opensourceleg-1.2.8/opensourceleg/control.py
+-rw-r--r--   0        0        0     7480 2023-06-08 20:40:33.324884 opensourceleg-1.2.8/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.8/opensourceleg/example.py
+-rw-r--r--   0        0        0    12114 2023-06-08 20:40:33.361500 opensourceleg-1.2.8/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.8/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8513 2023-06-06 02:25:22.342625 opensourceleg-1.2.8/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3715 2023-06-08 20:37:48.671909 opensourceleg-1.2.8/opensourceleg/logger.py
+-rw-r--r--   0        0        0    17657 2023-06-08 20:40:33.336090 opensourceleg-1.2.8/opensourceleg/osl.py
+-rw-r--r--   0        0        0    15011 2023-06-08 20:34:58.232056 opensourceleg-1.2.8/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.8/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21242 2023-06-07 02:24:24.140310 opensourceleg-1.2.8/opensourceleg/tui.py
+-rw-r--r--   0        0        0     4341 2023-06-07 17:03:13.722676 opensourceleg-1.2.8/opensourceleg/units.py
+-rw-r--r--   0        0        0    11587 2023-06-06 02:26:59.481937 opensourceleg-1.2.8/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-06-08 20:42:26.928688 opensourceleg-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.8/PKG-INFO
```

### Comparing `opensourceleg-1.2.7/LICENSE` & `opensourceleg-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.7/README.md` & `opensourceleg-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.7/opensourceleg/actuators.py` & `opensourceleg-1.2.8/opensourceleg/actuators.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.7/opensourceleg/constants.py` & `opensourceleg-1.2.8/opensourceleg/constants.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.7/opensourceleg/control.py` & `opensourceleg-1.2.8/opensourceleg/control.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.7/opensourceleg/demo.py` & `opensourceleg-1.2.8/opensourceleg/demo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 import time
 
 from opensourceleg.osl import OpenSourceLeg
 from opensourceleg.state_machine import Event, State
 
 # ------------- FSM PARAMETERS ---------------- #
 
-BODY_WEIGHT = 80
+BODY_WEIGHT = 60
 
 # STATE 1: EARLY STANCE
 
-KNEE_K_ESTANCE = 250
-KNEE_B_ESTANCE = 1000
+KNEE_K_ESTANCE = 99.372
+KNEE_B_ESTANCE = 3.180
 KNEE_THETA_ESTANCE = 5
 
 LOAD_LSTANCE: float = -1.0 * BODY_WEIGHT * 0.25
 ANKLE_THETA_ESTANCE_TO_LSTANCE = 6.0
 
-ANKLE_K_ESTANCE = 50
+ANKLE_K_ESTANCE = 19.874
 ANKLE_B_ESTANCE = 0
 ANKLE_THETA_ESTANCE = -2
 
 # --------------------------------------------- #
 # STATE 2: LATE STANCE
 
-KNEE_K_LSTANCE = 250
-KNEE_B_LSTANCE = 400
+KNEE_K_LSTANCE = 99.372
+KNEE_B_LSTANCE = 1.272
 KNEE_THETA_LSTANCE = 8
 
 LOAD_ESWING: float = -1.0 * BODY_WEIGHT * 0.15
 
-ANKLE_K_LSTANCE = 200
-ANKLE_B_LSTANCE = 20
+ANKLE_K_LSTANCE = 79.498
+ANKLE_B_LSTANCE = 0.063
 ANKLE_THETA_LSTANCE = -20
 
 # --------------------------------------------- #
 # STATE 3: EARLY SWING
 
-KNEE_K_ESWING = 100
-KNEE_B_ESWING = 20
-KNEE_THETA_ESWING = 65
+KNEE_K_ESWING = 39.749
+KNEE_B_ESWING = 0.063
+KNEE_THETA_ESWING = 60
 
-KNEE_THETA_ESWING_TO_LSWING = 55
+KNEE_THETA_ESWING_TO_LSWING = 50
 KNEE_DTHETA_ESWING_TO_LSWING = 3
 
-ANKLE_K_ESWING = 20
-ANKLE_B_ESWING = 0
+ANKLE_K_ESWING = 7.949
+ANKLE_B_ESWING = 0.0
 ANKLE_THETA_ESWING = 25
 
 # --------------------------------------------- #
 # STATE 4: LATE SWING
 
-KNEE_K_LSWING = 40
-KNEE_B_LSWING = 1200
+KNEE_K_LSWING = 15.899
+KNEE_B_LSWING = 3.816
 KNEE_THETA_LSWING = 5
 
 LOAD_ESTANCE: float = -1.0 * BODY_WEIGHT * 0.4
 KNEE_THETA_LSWING_TO_ESTANCE = 30
 
-ANKLE_K_LSWING = 20
-ANKLE_B_LSWING = 0
+ANKLE_K_LSWING = 7.949
+ANKLE_B_LSWING = 0.0
 ANKLE_THETA_LSWING = 15
 
 # ------------- FSM TRANSITIONS --------------- #
 
 
 def estance_to_lstance(osl: OpenSourceLeg) -> bool:
     """
@@ -246,14 +246,41 @@
         destination=early_stance,
         event=heel_strike,
         callback=lswing_to_estance,
     )
 
     osl.add_tui()
 
+    osl.log.add_attributes(class_instance=osl, attributes_str=["timestamp"])
+    osl.log.add_attributes(
+        class_instance=osl.knee,
+        attributes_str=[
+            "output_position",
+            "motor_current",
+            "joint_torque",
+            "motor_voltage",
+            "accelx",
+        ],
+    )
+
+    osl.log.add_attributes(
+        class_instance=osl.ankle,
+        attributes_str=[
+            "output_position",
+            "motor_current",
+            "joint_torque",
+            "motor_voltage",
+            "accelx",
+        ],
+    )
+    osl.log.add_attributes(class_instance=osl.loadcell, attributes_str=["fz"])
+    osl.log.add_attributes(
+        class_instance=osl.state_machine, attributes_str=["current_state_name"]
+    )
+
     with osl:
         osl.home()
-        osl.run(set_state_machine_parameters=True)
+        osl.run(set_state_machine_parameters=True, log_data=True)
 
 
 if __name__ == "__main__":
     state_machine_controller()
```

### Comparing `opensourceleg-1.2.7/opensourceleg/joints.py` & `opensourceleg-1.2.8/opensourceleg/joints.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,14 +70,25 @@
 
     def home(
         self,
         homing_voltage: int = 2000,
         homing_frequency: int = 100,
     ) -> None:
 
+        """
+
+        This method homes the joint by moving it to the zero position.
+        The zero position is defined as the position where the joint is fully extended.
+        This method will also make an encoder map if one does not exist.
+
+        Args:
+            homing_voltage (int): voltage in mV to use for homing
+            homing_frequency (int): frequency in Hz to use for homing
+        """
+
         is_homing = True
 
         CURRENT_THRESHOLD = 5000
         VELOCITY_THRESHOLD = 0.001
 
         self.set_mode(mode="voltage")
         homing_direction = -1.0
@@ -286,14 +297,44 @@
             kp=kp,
             ki=ki,
             K=K / (self.gear_ratio**2),
             B=B / (self.gear_ratio**2),
             ff=ff,
         )
 
+    def convert_to_joint_impedance(
+        self,
+        K: float = 100,
+        B: float = 40,
+    ):
+        joint_stiffness = (K / constants.NM_PER_RAD_TO_K) * self.gear_ratio**2
+        joint_damping = (B / constants.NM_S_PER_RAD_TO_B) * self.gear_ratio**2
+
+        return joint_stiffness, joint_damping
+
+    def convert_to_motor_impedance(
+        self,
+        K: float = 100,
+        B: float = 40,
+    ):
+        motor_stiffness = K / constants.NM_PER_RAD_TO_K
+        motor_damping = B / constants.NM_S_PER_RAD_TO_B
+
+        return motor_stiffness, motor_damping
+
+    def convert_to_pid_impedance(
+        self,
+        K: float = 0.08922,
+        B: float = 0.0038070,
+    ):
+        pid_stiffness = (K / self.gear_ratio**2) * constants.NM_PER_RAD_TO_K
+        pid_damping = (B / self.gear_ratio**2) * constants.NM_S_PER_RAD_TO_B
+
+        return pid_stiffness, pid_damping
+
     def update_set_points(self) -> None:
         self.set_mode(mode=self.control_mode_sp)
 
     @property
     def name(self) -> str:
         return self._name
```

### Comparing `opensourceleg-1.2.7/opensourceleg/loadcell.py` & `opensourceleg-1.2.8/opensourceleg/loadcell.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.7/opensourceleg/logger.py` & `opensourceleg-1.2.8/opensourceleg/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,26 +10,25 @@
     Methods:
         __init__(self, class_instance: object, file_path: str, logger: logging.Logger = None) -> None
         log(self) -> None
     """
 
     def __init__(
         self,
-        file_path: str = "./osl.log",
+        file_path: str = "./osl",
         log_format: str = "[%(asctime)s] %(levelname)s: %(message)s",
     ) -> None:
 
-        self._file_path: str = file_path
+        self._file_path: str = file_path + ".log"
 
         self._class_instances = []
         self._attributes = []
 
-        self._file = open(self._file_path + ".csv", "w")
+        self._file = open(file_path + ".csv", "w")
         self._writer = csv.writer(self._file)
-        self._writer.writerow(self._attributes)
 
         self._log_levels = {
             "DEBUG": logging.DEBUG,
             "INFO": logging.INFO,
             "WARNING": logging.WARNING,
             "ERROR": logging.ERROR,
             "CRITICAL": logging.CRITICAL,
@@ -93,32 +92,32 @@
         self._class_instances.append(class_instance)
         self._attributes.append(attributes_str)
 
     def data(self) -> None:
         """
         Logs the attributes of the class instance to the csv file
         """
+        header_data = []
+        data = []
 
         if not self._is_logging:
             for class_instance, attributes in zip(
                 self._class_instances, self._attributes
             ):
-                self._writer.writerow(
-                    row=[
-                        f"{class_instance.__class__.__name__}: {attribute}"
-                        for attribute in attributes
-                    ]
-                )
+                for attribute in attributes:
+                    header_data.append(f"{attribute}")
+
+            self._writer.writerow(header_data)
             self._is_logging = True
 
         for class_instance, attributes in zip(self._class_instances, self._attributes):
-            self._writer.writerow(
-                row=[getattr(class_instance, attribute) for attribute in attributes]
-            )
+            for attribute in attributes:
+                data.append(getattr(class_instance, attribute))
 
+        self._writer.writerow(data)
         self._file.flush()
 
     def close(self) -> None:
         """
         Closes the csv file
         """
         self._file.close()
```

### Comparing `opensourceleg-1.2.7/opensourceleg/osl.py` & `opensourceleg-1.2.8/opensourceleg/osl.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         if OpenSourceLeg._instance is None:
             OpenSourceLeg()
         return OpenSourceLeg._instance
 
     def __init__(
         self,
         frequency: int = 200,
-        file_name: str = "./osl.log",
+        file_name: str = "osl",
     ) -> None:
         """
         Initialize the OSL class.
 
         Parameters
         ----------
         frequency : int, optional
@@ -61,24 +61,28 @@
         self._is_sm_running: bool = False
         self._is_homed: bool = False
 
         self._knee: Joint = None  # type: ignore
         self._ankle: Joint = None  # type: ignore
         self._loadcell: Loadcell = None  # type: ignore
 
+        self._log_data: bool = False
+
         self.log = Logger(
             file_path=file_name, log_format="[%(asctime)s] %(levelname)s: %(message)s"
         )
 
         self.clock = SoftRealtimeLoop(dt=1.0 / self._frequency, report=False, fade=0.1)
         self._units: UnitsDefinition = DEFAULT_UNITS
 
         self.tui = None
         self.state_machine = None
 
+        self._timestamp: float = time.time()
+
     def __enter__(self) -> None:
 
         if self.has_knee:
             self._knee.start()
 
         if self.has_ankle:
             self._ankle.start()
@@ -301,54 +305,62 @@
                 )
                 self.__exit__(type=None, value=None, tb=None)
                 exit()
 
         if self.has_loadcell:
             self._loadcell.update()
 
+        if self._log_data:
+            self.log.data()
+
         if self.has_state_machine:
 
             if self.is_homed and not self.is_sm_running:
                 self.state_machine.start()
                 self._is_sm_running = True
 
-            self.state_machine.update()  # type: ignore
+            if self.is_sm_running:
+                self.state_machine.update()  # type: ignore
 
             if set_state_machine_parameters:
                 if self.has_knee and self.state_machine.current_state.is_knee_active:  # type: ignore
 
                     if self.knee.mode != self.knee.modes["impedance"]:  # type: ignore
                         self.knee.set_mode(mode="impedance")  # type: ignore
                         self.knee.set_impedance_gains()  # type: ignore
 
-                    self.knee.set_impedance_gains(  # type: ignore
+                    self.knee.set_joint_impedance(  # type: ignore
                         K=self.state_machine.current_state.knee_stiffness,  # type: ignore
                         B=self.state_machine.current_state.knee_damping,  # type: ignore
                     )
 
                     self.knee.set_output_position(  # type: ignore
                         position=self.state_machine.current_state.knee_theta  # type: ignore
                     )
 
                 if self.has_ankle and self.state_machine.current_state.is_ankle_active:  # type: ignore
 
                     if self.ankle.mode != self.ankle.modes["impedance"]:  # type: ignore
                         self.ankle.set_mode(mode="impedance")  # type: ignore
                         self.ankle.set_impedance_gains()  # type: ignore
 
-                    self.ankle.set_impedance_gains(  # type: ignore
+                    self.ankle.set_joint_impedance(  # type: ignore
                         K=self.state_machine.current_state.ankle_stiffness,  # type: ignore
                         B=self.state_machine.current_state.ankle_damping,  # type: ignore
                     )
 
                     self.ankle.set_output_position(  # type: ignore
                         position=self.state_machine.current_state.ankle_theta  # type: ignore
                     )
 
-    def run(self, set_state_machine_parameters: bool = False) -> None:
+            self._timestamp = time.time()
+
+    def run(
+        self, set_state_machine_parameters: bool = False, log_data: bool = False
+    ) -> None:
         """
         Run the OpenSourceLeg instance: update the joints, loadcell, and state machine.
         If the instance has a TUI, run the TUI.
         If the instance has a state machine and if set_state_machine_parameters is True,
         set the joint impedance gains and equilibrium angles to the current state's values.
 
         Parameters
@@ -363,14 +375,17 @@
                 self._is_sm_running = True
         else:
             osl.log.warn(
                 f"[OSL] Please run the homing routine by calling `osl.home()` before starting the state-machine."
             )
             exit()
 
+        if log_data:
+            self._log_data = True
+
         self.update(set_state_machine_parameters=set_state_machine_parameters)
 
         time.sleep(0.1)
 
         if not self.has_tui:
             self.update(set_state_machine_parameters=set_state_machine_parameters)
 
@@ -444,19 +459,19 @@
         self.log.debug("[OSL] Emergency stop activated.")
 
         if self.has_tui:
             self.tui.quit()  # type: ignore
 
     def home(self) -> None:
         if self.has_knee:
-            self.log.debug(msg="[OSL] Homing knee joint.")
+            self.log.info(msg="[OSL] Homing knee joint.")
             self.knee.home()  # type: ignore
 
         if self.has_ankle:
-            self.log.debug(msg="[OSL] Homing ankle joint.")
+            self.log.info(msg="[OSL] Homing ankle joint.")
             self.ankle.home()  # type: ignore
 
         self._is_homed = True
 
     def calibrate_loadcell(self) -> None:
         self.log.debug(msg="[OSL] Calibrating loadcell.")
         if self.has_loadcell:
@@ -482,14 +497,21 @@
 
         if self.has_ankle:
             self.ankle.set_mode(mode="voltage")  # type: ignore
             self.ankle.set_voltage(value=0, force=True)  # type: ignore
 
             time.sleep(0.1)
 
+    def log_data(self):
+        self._log_data = True
+
+    @property
+    def timestamp(self) -> float:
+        return self._timestamp
+
     @property
     def knee(self):
         if self.has_knee:
             return self._knee
         else:
             self.log.warning(msg="[OSL] Knee is not connected.")
```

### Comparing `opensourceleg-1.2.7/opensourceleg/state_machine.py` & `opensourceleg-1.2.8/opensourceleg/state_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 class State:
     """
     A class to represent a state in a finite state machine.
 
     Args:
         name (str): Name of the state
         is_knee_active (bool): Whether the knee is active. Default: False
-        knee_stiffness (float): Knee stiffness
-        knee_damping (float): Knee damping
+        knee_stiffness (float): Knee stiffness in Nm/rad
+        knee_damping (float): Knee damping in Nm/rad/sec
         knee_equilibrium_angle (float): Knee equilibrium angle
         is_ankle_active (bool): Whether the ankle is active. Default: False
-        ankle_stiffness (float): Ankle stiffness
-        ankle_damping (float): Ankle damping
+        ankle_stiffness (float): Ankle stiffness in Nm/rad
+        ankle_damping (float): Ankle damping in Nm/rad/sec
         ankle_equilibrium_angle (float): Ankle equilibrium angle
         minimum_time_in_state (float): Minimum time spent in the state in seconds. Default: 2.0
 
     Note:
         The knee and ankle impedance parameters are only used if the
         corresponding joint is active. You can also set custom data
         using the `set_custom_data` method.
```

### Comparing `opensourceleg-1.2.7/opensourceleg/thermal.py` & `opensourceleg-1.2.8/opensourceleg/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.7/opensourceleg/tui.py` & `opensourceleg-1.2.8/opensourceleg/tui.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.7/opensourceleg/units.py` & `opensourceleg-1.2.8/opensourceleg/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,13 +160,13 @@
         "current": "mA",
         "voltage": "mV",
         "gravity": "m/s^2",
         "temperature": "C",
     }
 )
 
-if __name__ == "__main__":
-    units: UnitsDefinition = DEFAULT_UNITS
-    units["temperature"] = "F"  # type: ignore
+# if __name__ == "__main__":
+#     units: UnitsDefinition = DEFAULT_UNITS
+#     units["temperature"] = "F"  # type: ignore
 
-    print(units.convert_to_default_units(value=80, attribute="temperature"))
-    print(units.convert_from_default_units(value=0, attribute="temperature"))
+#     print(units.convert_to_default_units(value=80, attribute="temperature"))
+#     print(units.convert_from_default_units(value=0, attribute="temperature"))
```

### Comparing `opensourceleg-1.2.7/opensourceleg/utilities.py` & `opensourceleg-1.2.8/opensourceleg/utilities.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.7/pyproject.toml` & `opensourceleg-1.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.2.7"
+version = "1.2.8"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.2.7/PKG-INFO` & `opensourceleg-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.2.7
+Version: 1.2.8
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

