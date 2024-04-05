# Comparing `tmp/pyserilog-0.2.0a3-py3-none-any.whl.zip` & `tmp/pyserilog-0.2.0a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 70520 bytes, number of entries: 113
+Zip file size: 70586 bytes, number of entries: 113
 -rw-rw-rw-  2.0 fat       97 b- defN 23-Mar-25 04:26 pyserilog/__init__.py
 -rw-rw-rw-  2.0 fat      194 b- defN 23-Mar-25 04:26 pyserilog/guard.py
 -rw-rw-rw-  2.0 fat     5466 b- defN 24-Apr-04 12:41 pyserilog/ilogger.py
 -rw-rw-rw-  2.0 fat     9312 b- defN 23-Mar-26 15:34 pyserilog/logger_configuration.py
 -rw-rw-rw-  2.0 fat      298 b- defN 23-Mar-25 04:26 pyserilog/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-25 04:26 pyserilog/capturing/__init__.py
 -rw-rw-rw-  2.0 fat     2211 b- defN 23-Mar-26 15:34 pyserilog/capturing/depth_limiter.py
@@ -103,13 +103,13 @@
 -rw-rw-rw-  2.0 fat     2910 b- defN 23-Mar-27 16:33 pyserilog/rendering/message_template_renderer.py
 -rw-rw-rw-  2.0 fat      674 b- defN 23-Mar-27 16:33 pyserilog/rendering/padding.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-04 13:26 pyserilog/settings/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-04 13:26 pyserilog/settings/key_value_paies/__init__.py
 -rw-rw-rw-  2.0 fat     1642 b- defN 23-Mar-26 11:28 pyserilog/settings/key_value_paies/callable_configuration_method_finder.py
 -rw-rw-rw-  2.0 fat    13526 b- defN 23-Mar-26 15:34 pyserilog/settings/key_value_paies/key_value_pair_settings.py
 -rw-rw-rw-  2.0 fat     1652 b- defN 23-Mar-25 10:33 pyserilog/settings/key_value_paies/setting_value_conversions.py
--rw-rw-rw-  2.0 fat     5427 b- defN 24-Apr-04 13:13 pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
--rw-rw-rw-  2.0 fat      628 b- defN 24-Apr-04 13:30 pyserilog-0.2.0a3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 13:30 pyserilog-0.2.0a3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-04 13:30 pyserilog-0.2.0a3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    10841 b- defN 24-Apr-04 13:30 pyserilog-0.2.0a3.dist-info/RECORD
-113 files, 185157 bytes uncompressed, 52778 bytes compressed:  71.5%
+-rw-rw-rw-  2.0 fat     5630 b- defN 24-Apr-04 13:49 pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
+-rw-rw-rw-  2.0 fat      628 b- defN 24-Apr-04 13:50 pyserilog-0.2.0a4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 13:50 pyserilog-0.2.0a4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-04 13:50 pyserilog-0.2.0a4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    10841 b- defN 24-Apr-04 13:50 pyserilog-0.2.0a4.dist-info/RECORD
+113 files, 185360 bytes uncompressed, 52844 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -321,20 +321,20 @@
 
 Filename: pyserilog/settings/key_value_paies/setting_value_conversions.py
 Comment: 
 
 Filename: pyserilog/settings/key_value_paies/surrogate_configuration_methods.py
 Comment: 
 
-Filename: pyserilog-0.2.0a3.dist-info/METADATA
+Filename: pyserilog-0.2.0a4.dist-info/METADATA
 Comment: 
 
-Filename: pyserilog-0.2.0a3.dist-info/WHEEL
+Filename: pyserilog-0.2.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: pyserilog-0.2.0a3.dist-info/top_level.txt
+Filename: pyserilog-0.2.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyserilog-0.2.0a3.dist-info/RECORD
+Filename: pyserilog-0.2.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyserilog/settings/key_value_paies/surrogate_configuration_methods.py

```diff
@@ -8,14 +8,15 @@
 from pyserilog.configuration.logger_sink_configuration import LoggerSinkConfiguration
 from pyserilog.configuration.logger_audit_sink_configuration import LoggerAuditSinkConfiguration
 from pyserilog.core.ilog_event_filter import ILogEventFilter
 from pyserilog.core.idestructuring_policy import IDestructuringPolicy
 from pyserilog.core.ilog_event_sink import ILogEventSink
 from pyserilog.core.ilog_event_enricher import ILogEventEnricher
 from pyserilog.core.logging_level_switch import LoggingLevelSwitch
+from pyserilog.core.sinks.secondary_logger_sink import SecondaryLoggerSink
 from pyserilog.events.level_alias import LevelAlias
 from pyserilog.events.log_event_level import LogEventLevel
 
 
 class WriteToSurrogateConfigurationMethods:
     @staticmethod
     def sink(logger_sink_configuration: LoggerSinkConfiguration, sink: ILogEventSink,
@@ -25,16 +26,19 @@
 
     @staticmethod
     def logger(logger_sink_configuration: LoggerSinkConfiguration,
                configure_logger: Callable[[LoggerConfiguration], types.NoneType],
                restricted_to_minimum_level: LogEventLevel = LevelAlias.minimum,
                level_switch: LoggingLevelSwitch = None) -> LoggerConfiguration:
         configure = LoggerConfiguration().minimum_level.level_is(LevelAlias.minimum)
-        logger = configure_logger(configure)
-        return logger_sink_configuration.logger(logger, restricted_to_minimum_level, level_switch)
+        configure_logger(configure)
+        sub_logger = configure.create_logger()
+
+        secondary_sink = SecondaryLoggerSink(sub_logger, attempt_dispose=True)
+        return logger_sink_configuration.sink(secondary_sink, restricted_to_minimum_level, level_switch)
 
 
 class AuditToSurrogateConfigurationMethods:
     @staticmethod
     def sink(audit_sink_configuration: LoggerAuditSinkConfiguration, sink: ILogEventSink,
              restricted_to_minimum_level: LogEventLevel = LevelAlias.minimum,
              level_switch: LoggingLevelSwitch = None) -> LoggerConfiguration:
```

## Comparing `pyserilog-0.2.0a3.dist-info/METADATA` & `pyserilog-0.2.0a4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserilog
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: python version of serilog a structured logging library
 Home-page: UNKNOWN
 Author: Reza Sadeghi
 Author-email: rezasadeghikhas@gmail.com
 License: Apache2
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `pyserilog-0.2.0a3.dist-info/RECORD` & `pyserilog-0.2.0a4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -102,12 +102,12 @@
 pyserilog/rendering/message_template_renderer.py,sha256=HY0CaF6OuYlDHFw0gGrwgHstghX1IZEMPbtUrOqtVHg,2910
 pyserilog/rendering/padding.py,sha256=T6rCLbmZC2P1BUhX5SEqN0nILXOf-Red-V2KVcCtKbI,674
 pyserilog/settings/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyserilog/settings/key_value_paies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyserilog/settings/key_value_paies/callable_configuration_method_finder.py,sha256=nVM5Vw-PL1-ZuE10Bh_Hx4vgKt3sGQBGQvKFreD3ee4,1642
 pyserilog/settings/key_value_paies/key_value_pair_settings.py,sha256=6HsKeOqYAw4biKQ1ftJxpGjEAVfA9WuPD5fF4KdxxAs,13526
 pyserilog/settings/key_value_paies/setting_value_conversions.py,sha256=VuL5eS3jbvRLsaSL1idEGvm3gCxQZOCvR6LuC7CL5EI,1652
-pyserilog/settings/key_value_paies/surrogate_configuration_methods.py,sha256=vZPRfzU6aBxISJaKygi_EB6ma9ZUhIWLBjb5XQ2ZKuI,5427
-pyserilog-0.2.0a3.dist-info/METADATA,sha256=0tI2aaGbNAyACVCGmO7AEzeHNYQE1-DiAZtFgd5RX9U,628
-pyserilog-0.2.0a3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyserilog-0.2.0a3.dist-info/top_level.txt,sha256=hPeO21itJn_SAW-X2aIdIo_cgIiyUrxcxrYpP7xQu88,10
-pyserilog-0.2.0a3.dist-info/RECORD,,
+pyserilog/settings/key_value_paies/surrogate_configuration_methods.py,sha256=HkOe5rahROzt3596pq1sxh8HAhX9vAtzACVl29GokhI,5630
+pyserilog-0.2.0a4.dist-info/METADATA,sha256=lOnYf4Ypu3PAG551xLWRFj43rVCchd_WkBxzb_7LZGI,628
+pyserilog-0.2.0a4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyserilog-0.2.0a4.dist-info/top_level.txt,sha256=hPeO21itJn_SAW-X2aIdIo_cgIiyUrxcxrYpP7xQu88,10
+pyserilog-0.2.0a4.dist-info/RECORD,,
```

