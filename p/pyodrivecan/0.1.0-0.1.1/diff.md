# Comparing `tmp/pyodrivecan-0.1.0.tar.gz` & `tmp/pyodrivecan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodrivecan-0.1.0.tar", last modified: Fri Mar 29 23:13:14 2024, max compression
+gzip compressed data, was "pyodrivecan-0.1.1.tar", last modified: Fri Apr  5 00:33:18 2024, max compression
```

## Comparing `pyodrivecan-0.1.0.tar` & `pyodrivecan-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:13:14.966220 pyodrivecan-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-29 23:13:07.000000 pyodrivecan-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-29 23:13:14.966220 pyodrivecan-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-29 23:13:14.966220 pyodrivecan-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-29 23:13:07.000000 pyodrivecan-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:13:14.962220 pyodrivecan-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:13:14.962220 pyodrivecan-0.1.0/src/pyodrivecan/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-29 23:13:07.000000 pyodrivecan-0.1.0/src/pyodrivecan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-03-29 23:13:07.000000 pyodrivecan-0.1.0/src/pyodrivecan/odrivedatabase.py
--rw-r--r--   0 runner    (1001) docker     (127)    44369 2024-03-29 23:13:07.000000 pyodrivecan-0.1.0/src/pyodrivecan/pyodrivecan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:13:14.966220 pyodrivecan-0.1.0/src/pyodrivecan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-29 23:13:14.000000 pyodrivecan-0.1.0/src/pyodrivecan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-29 23:13:14.000000 pyodrivecan-0.1.0/src/pyodrivecan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 23:13:14.000000 pyodrivecan-0.1.0/src/pyodrivecan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 23:13:14.000000 pyodrivecan-0.1.0/src/pyodrivecan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 23:13:14.000000 pyodrivecan-0.1.0/src/pyodrivecan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:33:18.433115 pyodrivecan-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/src/pyodrivecan/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/src/pyodrivecan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/src/pyodrivecan/odrivedatabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48375 2024-04-05 00:33:12.000000 pyodrivecan-0.1.1/src/pyodrivecan/pyodrivecan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:33:18.437115 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 00:33:18.000000 pyodrivecan-0.1.1/src/pyodrivecan.egg-info/top_level.txt
```

### Comparing `pyodrivecan-0.1.0/LICENSE` & `pyodrivecan-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodrivecan-0.1.0/PKG-INFO` & `pyodrivecan-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodrivecan
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for controlling O-Drive Motor Controller using can with Python.
 Home-page: https://github.com/dylanballback/ODriveCan
 Author: Dylan Ballback
 Author-email: dylanballback19@gmail.com
 License: mit
 Keywords: O-Drive,CAN,Python
 Classifier: Topic :: Printing
```

### Comparing `pyodrivecan-0.1.0/setup.cfg` & `pyodrivecan-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyodrivecan-0.1.0/src/pyodrivecan/odrivedatabase.py` & `pyodrivecan-0.1.1/src/pyodrivecan/odrivedatabase.py`

 * *Files identical despite different names*

### Comparing `pyodrivecan-0.1.0/src/pyodrivecan/pyodrivecan.py` & `pyodrivecan-0.1.1/src/pyodrivecan/pyodrivecan.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 class ODriveCAN:
     """
     A class for setting up O-Drive motor controllers using CAN communication with Python on a Raspberry Pi with the Waveshare RS485 CAN HAT.
 
     Attributes:
         canBusID           (str): The CAN Bus ID, which should be "can0" by default. If multiple CAN buses are present on the device, this can be modified accordingly.
         canBusType         (str): The CAN communication type as defined by the python-can package. By default, "socketcan" is used.
+        self.canBitRate    (int): The CAN Bit Rate or Bus Speed, by Default O-Drive GUI has this set to 250000 bits/s
         nodeID             (int): The node ID of the O-Drive controller on the CAN network.
         position           (float, optional): The current position of the motor in revolutions. Defaults to None.
         velocity           (float, optional): The current velocity of the motor in revolutions per second. Defaults to None.
         torque_target      (float, optional): The target torque for the motor. Defaults to None.
         torque_estimate    (float, optional): The estimated torque of the motor. Defaults to None.
         bus_voltage        (float, optional): The current bus voltage of the O-Drive. Defaults to None.
         bus_current        (float, optional): The current bus current of the O-Drive. Defaults to None.
@@ -92,14 +93,15 @@
     can_setup_done = False
 
     def __init__(
             self,
             nodeID,
             canBusID="can0",
             canBusType="socketcan",
+            canBitRate=250000,
             position=None,
             velocity=None,
             torque_target=None,
             torque_estimate=None,
             bus_voltage=None,
             bus_current=None,
             iq_setpoint=None,
@@ -110,14 +112,15 @@
             database='odrive_data.db',
             active_error = None,
             disarm_reason = None
             ):
     
         self.canBusID = canBusID
         self.canBusType = canBusType
+        self.canBitRate = canBitRate
         self.nodeID = nodeID
         self.canBus = can.interface.Bus(canBusID, bustype=canBusType)
         self.database = OdriveDatabase(database)
         self.collected_data = []  # Initialize an empty list to store data
         self.start_time = time.time()  # Capture the start time when the object is initialized
         self.latest_data = {}
         self.running = True
@@ -214,15 +217,15 @@
 
         Raises:
             Exception: If the setup process fails after retrying, including after a reset and restart attempt.
         """
         
 
         # Commands for setting up, resetting, and restarting the CAN interface
-        setup_command = ["sudo", "ip", "link", "set", self.canBusID, "up", "type", "can", "bitrate", "250000"]
+        setup_command = ["sudo", "ip", "link", "set", self.canBusID, "up", "type", "can", "bitrate", str(self.canBitRate)]
         reset_command = ["sudo", "/sbin/ip", "link", "set", self.canBusID, "down"]
         restart_command = ["sudo", "ip", "link", "set", self.canBusID, "type", "can", "restart-ms", "100"]
         # Command to dump CAN messages for verification
        
         
         try:
             # First, check if the CAN interface is already operational.
@@ -251,14 +254,15 @@
                     print("CAN setup verified successfully after reset and restart.")
                 else:
                     raise Exception("Failed to verify CAN setup after reset and restart.")
             else:
                 print(f"Error setting up CAN interface: {e.stderr}")
                 raise
 
+
 #----------------------------- CAN Bus Setup for Raspberry Pi END -----------------------------------------
 
 
     
     def initCanBus(self):
         """
         Initalize connection to CAN Bus
@@ -278,19 +282,19 @@
     def flush_can_buffer(self):
         """
         Flushes the CAN receive buffer to clear any pending messages.
 
         Example:
             >>> odrive_can.flush_can_buffer()
             ...
-            ... I have cleared all CAN Messages on the BUS!
+            ... CAN BUS Flushed.
         """
         #Flush CAN RX buffer to ensure no old pending messages.
         while not (self.canBus.recv(timeout=0) is None): pass
-        print("I have cleared all CAN Messages on the BUS!")
+        print("CAN BUS Flushed.")
 
 
     #Shutdown can bus at the end of a program. 
     def bus_shutdown(self):
         """
         Run this method at the end of your program to shundown the can bus to prevent can errors.
 
@@ -373,15 +377,15 @@
                     is_extended_id=False
                 ),
                 timeout=0.5  # Timeout of 0.5 seconds
             )
             print(f"Axis state set command sent for {axis_state_name} ({axis_requested_state}) to ODrive {self.nodeID}.")
             
             # Now we wait for a heartbeat message to confirm the new state
-            print(f"Waiting for confirmation from ODrive {self.nodeID}...")
+            #print(f"Waiting for confirmation from ODrive {self.nodeID}...")
             start_time = time.time()
             while time.time() - start_time < 5:  # Wait for up to 5 seconds for confirmation
                 msg = self.canBus.recv(timeout=0.5)  # Adjust timeout as needed
                 if msg and (msg.arbitration_id == (self.nodeID << 5 | 0x01)):  # 0x01: Heartbeat
                     _, state, _, _ = struct.unpack('<IBBB', bytes(msg.data[:7]))
                     if state == axis_requested_state:
                         print(f"Confirmation received: ODrive {self.nodeID} is now in state {axis_state_name}.")
@@ -398,14 +402,62 @@
                     print(f"No confirmation received from ODrive {self.nodeID}. Please check the device.")
                     return
 
         except Exception as e:
             print(f"Error setting axis state for ODrive {self.nodeID}: {str(e)}")
 
 
+#----------------------------------------- Check Axis State Idle --------------------------------------------------------
+            
+    def is_odrive_idle(self):
+        """
+        Checks if the ODrive is in the IDLE state.
+
+        Returns:
+            bool: True if the ODrive is in the IDLE state, False otherwise.
+        """
+        state_names = {
+            0: "undefined",
+            1: "idle",
+            2: "startup_sequence",
+            3: "full_calibration_sequence",
+            4: "motor_calibration",
+            6: "encoder_index_search",
+            7: "encoder_offset_calibration",
+            8: "closed_loop_control",
+            9: "lockin_spin",
+            10: "encoder_dir_find",
+            11: "homing",
+            12: "encoder_hall_polarity_calibration",
+            13: "encoder_hall_phase_calibration",
+            14: "anticogging_calibration"
+        }
+        idle_state_code = 1  # The code for the IDLE state
+
+        # Send a command to request the current state, or just wait for the next heartbeat message
+        print(f"Checking if ODrive {self.nodeID} is in IDLE state...")
+        start_time = time.time()
+        while time.time() - start_time < 5:  # Wait for up to 5 seconds for a heartbeat message
+            msg = self.canBus.recv(timeout=0.5)  # Adjust timeout as needed
+            if msg and (msg.arbitration_id == (self.nodeID << 5 | 0x01)):  # 0x01: Heartbeat
+                _, state, _, _ = struct.unpack('<IBBB', bytes(msg.data[:7]))
+                if state == idle_state_code:
+                    print(f"ODrive {self.nodeID} is in IDLE state.")
+                    return True
+                else:
+                    actual_state_name = state_names.get(state, "Unknown State")
+                    print(f"ODrive {self.nodeID} is in {actual_state_name} state.")
+                    return False
+            elif msg:
+                continue  # Skip any non-heartbeat messages
+
+        print(f"No state information received from ODrive {self.nodeID}.")
+        return False
+
+
 #----------------------------------------- Set Controller Mode --------------------------------------------------------
 
     def set_controller_mode(self, control_mode_name, input_mode_name="pass_through"):
             """
             Sets the control mode and input mode of the ODrive controller using descriptive names.
 
             Control Modes:
@@ -538,14 +590,62 @@
                 timeout=0.5 
             )
             print(f"Cleared errors for ODrive {self.nodeID}. LED flash is {'enabled' if identify else 'disabled'}.")
         except Exception as e:
             print(f"Error sending Clear_Errors command to ODrive {self.nodeID}: {str(e)}")
 
 
+#-------------------------------------- Reboot O-Drive  ------------------------------------------------
+
+    def reboot_save(self, action='save'):
+        """
+        Reboots the ODrive or performs related actions based on the specified action parameter.
+
+        Parameters:
+            action (str): The action to be performed, which can be one of the following:
+                        'reboot': Reboot the ODrive.
+                        'save': Save the configuration to persistent storage.
+                        'erase': Erase the configuration.
+                        'dfu': Enter DFU (Device Firmware Upgrade) mode.
+
+        Command ID: 0x16 (Host → ODrive)
+
+        Note: The axis must be in the IDLE state before performing this action.
+        """
+        actions = {
+            'reboot': 0,
+            'save': 1,
+            'erase': 2,
+            'dfu': 3
+        }
+
+        if action not in actions:
+            print(f"Invalid action specified: {action}. Must be one of {list(actions.keys())}.")
+            return
+
+        # Check if ODrive is in IDLE state before proceeding
+        if not self.is_odrive_idle():
+            print(f"ODrive {self.nodeID} is not in IDLE state. Cannot perform {action} action.")
+            return
+
+        command_id = 0x16  # Command ID for reboot actions
+        action_byte = actions[action]
+        message_data = struct.pack('<B', action_byte)
+
+        try:
+            self.canBus.send(can.Message(
+                arbitration_id=(self.nodeID << 5 | command_id),
+                data=message_data,
+                is_extended_id=False
+            ))
+            print(f"{action.capitalize()} command sent to ODrive {self.nodeID}.")
+        except Exception as e:
+            print(f"Error sending {action} command to ODrive {self.nodeID}: {str(e)}")
+
+
 
 #-------------------------------------- Set Absoulte Postion  ------------------------------------------------
     def set_absolute_position(self, position=None):
         """
         Sends a command to the ODrive to set the motor to an absolute position. If no position is specified,
         the motor will be set to the last known position.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyodrivecan-0.1.0/src/pyodrivecan.egg-info/PKG-INFO` & `pyodrivecan-0.1.1/src/pyodrivecan.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodrivecan
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for controlling O-Drive Motor Controller using can with Python.
 Home-page: https://github.com/dylanballback/ODriveCan
 Author: Dylan Ballback
 Author-email: dylanballback19@gmail.com
 License: mit
 Keywords: O-Drive,CAN,Python
 Classifier: Topic :: Printing
```

