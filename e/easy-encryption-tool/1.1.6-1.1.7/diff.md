# Comparing `tmp/easy_encryption_tool-1.1.6-py3-none-any.whl.zip` & `tmp/easy_encryption_tool-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 38269 bytes, number of entries: 15
+Zip file size: 41098 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      253 b- defN 24-Apr-04 15:14 easy_encryption_tool/__init__.py
 -rw-r--r--  2.0 unx    20027 b- defN 24-Apr-04 15:39 easy_encryption_tool/aes_command.py
+-rw-r--r--  2.0 unx     8410 b- defN 24-Apr-05 16:05 easy_encryption_tool/cert_parse.py
 -rw-r--r--  2.0 unx      702 b- defN 24-Apr-04 08:28 easy_encryption_tool/command_perf.py
--rw-r--r--  2.0 unx     7420 b- defN 24-Apr-04 15:39 easy_encryption_tool/common.py
+-rw-r--r--  2.0 unx     7420 b- defN 24-Apr-05 05:45 easy_encryption_tool/common.py
 -rw-r--r--  2.0 unx    12652 b- defN 24-Apr-04 15:39 easy_encryption_tool/ecc_command.py
 -rw-r--r--  2.0 unx     4111 b- defN 24-Apr-04 15:39 easy_encryption_tool/hmac_command.py
--rw-r--r--  2.0 unx     2210 b- defN 24-Apr-04 15:39 easy_encryption_tool/main.py
--rw-r--r--  2.0 unx     2675 b- defN 24-Apr-04 15:39 easy_encryption_tool/random_str.py
+-rw-r--r--  2.0 unx     2284 b- defN 24-Apr-05 16:06 easy_encryption_tool/main.py
+-rw-r--r--  2.0 unx     2675 b- defN 24-Apr-05 05:45 easy_encryption_tool/random_str.py
 -rw-r--r--  2.0 unx    17736 b- defN 24-Apr-04 15:39 easy_encryption_tool/rsa_command.py
--rw-r--r--  2.0 unx      870 b- defN 24-Apr-04 15:39 easy_encryption_tool/tool_version.py
--rw-r--r--  2.0 unx    59150 b- defN 24-Apr-04 15:41 easy_encryption_tool-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 15:41 easy_encryption_tool-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       83 b- defN 24-Apr-04 15:41 easy_encryption_tool-1.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 24-Apr-04 15:41 easy_encryption_tool-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1366 b- defN 24-Apr-04 15:41 easy_encryption_tool-1.1.6.dist-info/RECORD
-15 files, 129368 bytes uncompressed, 35967 bytes compressed:  72.2%
+-rw-r--r--  2.0 unx      870 b- defN 24-Apr-05 05:45 easy_encryption_tool/tool_version.py
+-rw-r--r--  2.0 unx    59779 b- defN 24-Apr-05 16:07 easy_encryption_tool-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 16:07 easy_encryption_tool-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       83 b- defN 24-Apr-05 16:07 easy_encryption_tool-1.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-05 16:07 easy_encryption_tool-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1457 b- defN 24-Apr-05 16:07 easy_encryption_tool-1.1.7.dist-info/RECORD
+16 files, 138572 bytes uncompressed, 38652 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: easy_encryption_tool/__init__.py
 Comment: 
 
 Filename: easy_encryption_tool/aes_command.py
 Comment: 
 
+Filename: easy_encryption_tool/cert_parse.py
+Comment: 
+
 Filename: easy_encryption_tool/command_perf.py
 Comment: 
 
 Filename: easy_encryption_tool/common.py
 Comment: 
 
 Filename: easy_encryption_tool/ecc_command.py
@@ -24,23 +27,23 @@
 
 Filename: easy_encryption_tool/rsa_command.py
 Comment: 
 
 Filename: easy_encryption_tool/tool_version.py
 Comment: 
 
-Filename: easy_encryption_tool-1.1.6.dist-info/METADATA
+Filename: easy_encryption_tool-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: easy_encryption_tool-1.1.6.dist-info/WHEEL
+Filename: easy_encryption_tool-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: easy_encryption_tool-1.1.6.dist-info/entry_points.txt
+Filename: easy_encryption_tool-1.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.1.6.dist-info/top_level.txt
+Filename: easy_encryption_tool-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.1.6.dist-info/RECORD
+Filename: easy_encryption_tool-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## easy_encryption_tool/main.py

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 # @Time: 2024-03-30 15:41:41
 
 import click
 
-from easy_encryption_tool import aes_command, ecc_command, hmac_command, random_str, rsa_command, tool_version
+from easy_encryption_tool import aes_command, cert_parse, ecc_command, hmac_command, random_str, rsa_command, tool_version
 
 """
 name (str): 命令组的名称。如果未提供，将使用装饰的函数的名称。
 
 commands (dict): 一个字典，其中键是命令名称，值是命令函数。这允许你在装饰器内部直接定义命令，而不是通过单独的 @click.command() 装饰器。
 
 invoke_without_command (bool): 如果为 True，则在没有提供子命令的情况下调用组时，将调用组函数本身。
@@ -46,9 +46,11 @@
 
 ecc_command.ecc_group.add_command(ecc_command.generate)
 ecc_command.ecc_group.add_command(ecc_command.key_exchange)
 ecc_command.ecc_group.add_command(ecc_command.ecc_sign)
 ecc_command.ecc_group.add_command(ecc_command.ecc_verify)
 encryption_tool.add_command(ecc_command.ecc_group)
 
+encryption_tool.add_command(cert_parse.parse_x509_cert_file)
+
 if __name__ == '__main__':
     encryption_tool()
```

## Comparing `easy_encryption_tool-1.1.6.dist-info/METADATA` & `easy_encryption_tool-1.1.7.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: easy-encryption-tool
-Version: 1.1.6
+Version: 1.1.7
 Home-page: https://cloud.tencent.com/developer/article/2155922
 Author: bowenerchen
 Author-email: bowener.chen@gmail.com
 License: MIT
 Keywords: encryption cli tool security aes hmac ecc rsa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: cryptography
 
 # 易加密（easy_encryption_tool）
 
+## 工具的安装
+
+`pip install easy-encryption-tool`
+
+项目地址：[easy-encryption-tool · PyPI](https://pypi.org/project/easy-encryption-tool/)
+
 ## 工具支持的命令
 
 ```python
 ❯ easy_encryption_tool --help
 
 Usage: easy_encryption_tool [OPTIONS] COMMAND [ARGS]...
 
@@ -30,24 +36,38 @@
   ecc         ecc签名验签和密钥交换验证工具
   hmac        hmac消息验证码工具
   random-str  随机字符串生成器
   rsa         rsa加解密和签名验签工具
   version     展示当前版本信息以及运行时信息
 ```
 
+## 设置easy_encryption_tool 自动补全
+
+参考：https://click.palletsprojects.com/en/8.1.x/shell-completion/
+
+### 手动设置(以 zsh 举例)
+
+```python
+# ZSH
+# 1. 执行命令生成~/.easy_encryption_tool_complete.sh文件
+_EASY_ENCRYPTION_TOOL_COMPLETE=zsh_source easy_encryption_tool >~/.easy_encryption_tool_complete.sh
+
+# 2. 在.zshrc 文件中引用生成的文件
+#    使用 vim 或其他编辑器打开~.zshrc 文件，添加下面的语句到文件中，然后保存退出
+. ~/.easy_encryption_tool_complete.sh
+
+# 3. 使配置在当前shell session 中生效
+source ~/.zshrc
+```
+
+
+
 ## 显示版本
 
 ```python
-# 展示版本信息，包括：
-# 工具版本
-# python解释器版本
-# 操作系统
-# cpu
-# 字节序
-# 作者信息
 ❯ easy_encryption_tool version
 
 ------ 7906e795524f2b7c begin@2024-04-04_15:02:59.590 ------
 tool-version:v1.0.0
 python:3.11.4 (main, Jul  5 2023, 08:54:11) [Clang 14.0.6 ]
 os:darwin
 chip:macOS-14.3.1-arm64-arm-64bit
```

## Comparing `easy_encryption_tool-1.1.6.dist-info/RECORD` & `easy_encryption_tool-1.1.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 easy_encryption_tool/__init__.py,sha256=XXlLRfi0r0AnF5kNBOg1dCUmiy0l3jFsPHmpvQPUB48,253
 easy_encryption_tool/aes_command.py,sha256=CbhUaS5d_5pRnsaZV7VSi6CAsAkzLP1k2ZUwcBWgCuc,20027
+easy_encryption_tool/cert_parse.py,sha256=Opcq6jW47IPy5xrI8EVo030lEEh5vppaqg2OQAiiDtA,8410
 easy_encryption_tool/command_perf.py,sha256=cMRgLVDiu9qdjVDXEl-WOOi1iNfWVu56Ee_tLC_6hOE,702
 easy_encryption_tool/common.py,sha256=vY5pMJsCOwK8sej5NXWr2ScSg7w2FJLlYkncawji8sM,7420
 easy_encryption_tool/ecc_command.py,sha256=g76LOqS-UILqXSgFZhqw_1qAXpXDZRUNslcmAQHmkpk,12652
 easy_encryption_tool/hmac_command.py,sha256=mQaZ9dDsh3q4KNEhkyht8bVPcT5LD0Oq8b2tEpqxWKg,4111
-easy_encryption_tool/main.py,sha256=e3YHOsFViRrS_TMd6Pv8wLu4EaZO4GFvuUPnDV0zLs8,2210
+easy_encryption_tool/main.py,sha256=c5iXQa3r2Sq1U6O8UX_9XyE_PrFb1NHz-EYzCk2Ye34,2284
 easy_encryption_tool/random_str.py,sha256=Mz8QkU8w-TrKWxLKhevXtic9_EPryeYlJcrEhXaQcVA,2675
 easy_encryption_tool/rsa_command.py,sha256=QsAJUo69Yo8EpZ3mbu4mbIR50NGPoRXfzZPtHJAOIGg,17736
 easy_encryption_tool/tool_version.py,sha256=Gz2mCkhX1Ztrpr_TaTBkyVWs9Yk3gX8QxxlgkB4ga0A,870
-easy_encryption_tool-1.1.6.dist-info/METADATA,sha256=gBPwfRBVST_P2Z8FcIcQyi5wvEvdEc0cnKw10G9kLSU,59150
-easy_encryption_tool-1.1.6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-easy_encryption_tool-1.1.6.dist-info/entry_points.txt,sha256=qrNi4Ml3z53yoZNoOEQFVofyZCmLG_sUQSytiejkJYY,83
-easy_encryption_tool-1.1.6.dist-info/top_level.txt,sha256=2RdeCo7jNerQyfXisv2UZytrMsfSAwsyef13Mq3TkMU,21
-easy_encryption_tool-1.1.6.dist-info/RECORD,,
+easy_encryption_tool-1.1.7.dist-info/METADATA,sha256=BpUmbsHyTENy5Fs2ye2mfoGGJDBJxUOM4NR-_H3J1Wg,59779
+easy_encryption_tool-1.1.7.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+easy_encryption_tool-1.1.7.dist-info/entry_points.txt,sha256=qrNi4Ml3z53yoZNoOEQFVofyZCmLG_sUQSytiejkJYY,83
+easy_encryption_tool-1.1.7.dist-info/top_level.txt,sha256=2RdeCo7jNerQyfXisv2UZytrMsfSAwsyef13Mq3TkMU,21
+easy_encryption_tool-1.1.7.dist-info/RECORD,,
```

