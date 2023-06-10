# Comparing `tmp/pioreactor_relay_plugin-0.4.0-py3-none-any.whl.zip` & `tmp/pioreactor_relay_plugin-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5168 bytes, number of entries: 10
+Zip file size: 5170 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       53 b- defN 22-Aug-26 19:03 pioreactor_relay_plugin/__init__.py
 -rw-r--r--  2.0 unx      104 b- defN 23-Jan-19 01:10 pioreactor_relay_plugin/additional_config.ini
--rw-r--r--  2.0 unx     2869 b- defN 23-May-20 01:57 pioreactor_relay_plugin/relay.py
+-rw-r--r--  2.0 unx     2903 b- defN 23-Jun-10 22:53 pioreactor_relay_plugin/relay.py
 -rw-r--r--  2.0 unx      409 b- defN 23-May-20 01:57 pioreactor_relay_plugin/ui/contrib/jobs/relay.yaml
--rw-r--r--  2.0 unx     1061 b- defN 23-May-20 01:58 pioreactor_relay_plugin-0.4.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1642 b- defN 23-May-20 01:58 pioreactor_relay_plugin-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-20 01:58 pioreactor_relay_plugin-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-May-20 01:58 pioreactor_relay_plugin-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 23-May-20 01:58 pioreactor_relay_plugin-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 23-May-20 01:58 pioreactor_relay_plugin-0.4.0.dist-info/RECORD
-10 files, 7292 bytes uncompressed, 3464 bytes compressed:  52.5%
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-10 22:54 pioreactor_relay_plugin-0.4.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1642 b- defN 23-Jun-10 22:54 pioreactor_relay_plugin-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 22:54 pioreactor_relay_plugin-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-10 22:54 pioreactor_relay_plugin-0.4.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-10 22:54 pioreactor_relay_plugin-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jun-10 22:54 pioreactor_relay_plugin-0.4.1.dist-info/RECORD
+10 files, 7326 bytes uncompressed, 3466 bytes compressed:  52.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: pioreactor_relay_plugin/relay.py
 Comment: 
 
 Filename: pioreactor_relay_plugin/ui/contrib/jobs/relay.yaml
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.4.0.dist-info/LICENSE.txt
+Filename: pioreactor_relay_plugin-0.4.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.4.0.dist-info/METADATA
+Filename: pioreactor_relay_plugin-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.4.0.dist-info/WHEEL
+Filename: pioreactor_relay_plugin-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.4.0.dist-info/entry_points.txt
+Filename: pioreactor_relay_plugin-0.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.4.0.dist-info/top_level.txt
+Filename: pioreactor_relay_plugin-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pioreactor_relay_plugin-0.4.0.dist-info/RECORD
+Filename: pioreactor_relay_plugin-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioreactor_relay_plugin/relay.py

```diff
@@ -7,15 +7,14 @@
 from pioreactor.hardware import PWM_TO_PIN
 from pioreactor.utils.pwm import PWM
 from pioreactor.whoami import get_latest_experiment_name
 from pioreactor.whoami import get_unit_name
 
 
 class Relay(BackgroundJobWithDodgingContrib):
-
     published_settings = {
         "is_relay_on": {"datatype": "boolean", "settable": True},
     }
 
     job_name = "relay"
 
     def __init__(self, unit, experiment, start_on=True):
@@ -38,15 +37,15 @@
         self.pwm.lock()
 
     def on_init_to_ready(self):
         super().on_init_to_ready()
         self.logger.debug(f"Starting relay {'ON' if self.is_relay_on else 'OFF'}.")
         self.pwm.start(self.duty_cycle)
 
-    def set_relay_on(self, value: bool):
+    def set_is_relay_on(self, value: bool):
         if value == self.is_relay_on:
             return
 
         if value:
             self._set_duty_cycle(100)
             self.is_relay_on = True
         else:
@@ -57,44 +56,46 @@
         self.duty_cycle = new_duty_cycle
 
         if hasattr(self, "pwm"):
             self.pwm.change_duty_cycle(self.duty_cycle)
 
     def on_ready_to_sleeping(self):
         super().on_ready_to_sleeping()
-        self.set_relay_on(False)
+        self.set_is_relay_on(False)
 
     def on_sleeping_to_ready(self):
         super().on_sleeping_to_ready()
-        self.set_relay_on(True)
+        self.set_is_relay_on(True)
 
     def on_disconnected(self):
         super().on_disconnected()
-        self.set_relay_on(False)
+        self.set_is_relay_on(False)
         self.pwm.cleanup()
 
     def action_to_do_before_od_reading(self):
-        self.set_relay_on(False)
+        self.set_is_relay_on(False)
 
     def action_to_do_after_od_reading(self):
-        self.set_relay_on(True)
+        self.set_is_relay_on(True)
 
 
 @click.command(name="relay")
 @click.option(
     "-s",
     "--start-on",
     default=config.getint("relay.config", "start_on", fallback=1),
     type=click.BOOL,
 )
 def click_relay(start_on: bool):
     """
     Start the relay
     """
     job = Relay(
-        unit=get_unit_name(), experiment=get_latest_experiment_name(), start_on=bool(start_on)
+        unit=get_unit_name(),
+        experiment=get_latest_experiment_name(),
+        start_on=bool(start_on),
     )
     job.block_until_disconnected()
 
 
 if __name__ == "__main__":
     click_relay()
```

## Comparing `pioreactor_relay_plugin-0.4.0.dist-info/LICENSE.txt` & `pioreactor_relay_plugin-0.4.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pioreactor_relay_plugin-0.4.0.dist-info/METADATA` & `pioreactor_relay_plugin-0.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pioreactor-relay-plugin
-Version: 0.4.0
+Version: 0.4.1
 Summary: Turn the PWM channels into a simple on/off relay for additional hardware.
 Home-page: https://github.com/CamDavidsonPilon/pioreactor-relay-plugin
 Author: Kelly Tran, Cam Davidson-Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `pioreactor_relay_plugin-0.4.0.dist-info/RECORD` & `pioreactor_relay_plugin-0.4.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pioreactor_relay_plugin/__init__.py,sha256=nzaA-lKGw3qkVWG-sUeDh3T3kL9Qn6uk055B38nfLKI,53
 pioreactor_relay_plugin/additional_config.ini,sha256=2NDiRYnY_lF3_dB0ZwD7ExMO23toseu-cKrNjguRFWg,104
-pioreactor_relay_plugin/relay.py,sha256=6_nS4Jmg6vfL-ekoHrlfry2F8BOFGpY42L6_jrNd9ic,2869
+pioreactor_relay_plugin/relay.py,sha256=qtOexoNB0UfO5aadroMzgKOkYn34AUrIa8IA4XPJdm4,2903
 pioreactor_relay_plugin/ui/contrib/jobs/relay.yaml,sha256=I9HtWsGN33F55myl4bUIBR-PvF3cTTtwD2LP09PX_XI,409
-pioreactor_relay_plugin-0.4.0.dist-info/LICENSE.txt,sha256=Ln7xVAOPmdFrbD7I-uwGZgbLrRdLxzhv4hPqZwVLzOM,1061
-pioreactor_relay_plugin-0.4.0.dist-info/METADATA,sha256=ZF48VY5VAFO1sUsg_9LUApxdTj2eLBz6d7bFx5fza-A,1642
-pioreactor_relay_plugin-0.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pioreactor_relay_plugin-0.4.0.dist-info/entry_points.txt,sha256=eoInJCHltj2GDoz1keQngjmowbJ8e1OHV6b8si2G5x4,71
-pioreactor_relay_plugin-0.4.0.dist-info/top_level.txt,sha256=ycPmfjvugfCgM68hl_LSwxvU5fKcmHeDoY0ZKS1HKNM,24
-pioreactor_relay_plugin-0.4.0.dist-info/RECORD,,
+pioreactor_relay_plugin-0.4.1.dist-info/LICENSE.txt,sha256=Ln7xVAOPmdFrbD7I-uwGZgbLrRdLxzhv4hPqZwVLzOM,1061
+pioreactor_relay_plugin-0.4.1.dist-info/METADATA,sha256=XD2eg8CgBSyW9l1JXtRHddiFmd5PKyJ-22ZzPAx-NHI,1642
+pioreactor_relay_plugin-0.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pioreactor_relay_plugin-0.4.1.dist-info/entry_points.txt,sha256=eoInJCHltj2GDoz1keQngjmowbJ8e1OHV6b8si2G5x4,71
+pioreactor_relay_plugin-0.4.1.dist-info/top_level.txt,sha256=ycPmfjvugfCgM68hl_LSwxvU5fKcmHeDoY0ZKS1HKNM,24
+pioreactor_relay_plugin-0.4.1.dist-info/RECORD,,
```

