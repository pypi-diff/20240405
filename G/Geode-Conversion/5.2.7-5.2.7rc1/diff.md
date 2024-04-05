# Comparing `tmp/Geode_Conversion-5.2.7-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Conversion-5.2.7rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1631603 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      171 b- defN 24-Apr-05 00:34 geode_conversion/__init__.py
--rw-rw-rw-  2.0 fat      178 b- defN 24-Apr-05 00:34 geode_conversion/model.py
--rw-rw-rw-  2.0 fat  4042752 b- defN 24-Apr-05 00:35 geode_conversion/bin/Geode-Conversion_model.dll
--rw-rw-rw-  2.0 fat   150528 b- defN 24-Apr-05 00:35 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1990 b- defN 24-Apr-05 00:35 Geode_Conversion-5.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-05 00:35 Geode_Conversion-5.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-05 00:35 Geode_Conversion-5.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      731 b- defN 24-Apr-05 00:35 Geode_Conversion-5.2.7.dist-info/RECORD
-8 files, 4196467 bytes uncompressed, 1630315 bytes compressed:  61.2%
+Zip file size: 1631629 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      171 b- defN 24-Apr-04 17:51 geode_conversion/__init__.py
+-rw-rw-rw-  2.0 fat      178 b- defN 24-Apr-04 17:51 geode_conversion/model.py
+-rw-rw-rw-  2.0 fat  4042752 b- defN 24-Apr-04 17:51 geode_conversion/bin/Geode-Conversion_model.dll
+-rw-rw-rw-  2.0 fat   150528 b- defN 24-Apr-04 17:51 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1996 b- defN 24-Apr-04 17:51 Geode_Conversion-5.2.7rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-04 17:51 Geode_Conversion-5.2.7rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-04 17:51 Geode_Conversion-5.2.7rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      743 b- defN 24-Apr-04 17:51 Geode_Conversion-5.2.7rc1.dist-info/RECORD
+8 files, 4196485 bytes uncompressed, 1630317 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: geode_conversion/bin/Geode-Conversion_model.dll
 Comment: 
 
 Filename: geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Conversion-5.2.7.dist-info/METADATA
+Filename: Geode_Conversion-5.2.7rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-5.2.7.dist-info/WHEEL
+Filename: Geode_Conversion-5.2.7rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Conversion-5.2.7.dist-info/top_level.txt
+Filename: Geode_Conversion-5.2.7rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Conversion-5.2.7.dist-info/RECORD
+Filename: Geode_Conversion-5.2.7rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_conversion/bin/Geode-Conversion_model.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802e27f4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Apr  5 00:34:56 2024
+Time/Date		Thu Apr  4 17:51:37 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002e6e00
 SizeOfInitializedData	00000000000f6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002e27f4
@@ -397794,15 +397794,15 @@
    180154f8e:	test   %rax,%rax
    180154f91:	je     0x180154fd1
    180154f93:	movq   $0x1,(%rax)
    180154f9a:	movb   $0x0,0x8(%rax)
    180154f9e:	xor    %eax,%eax
    180154fa0:	mov    %rax,0x10(%rdi)
    180154fa4:	mov    %rbx,0x10(%rdi)
-   180154fa8:	lea    0x22fa29(%rip),%rax        # 0x1803849d8
+   180154fa8:	lea    0x22f9c9(%rip),%rax        # 0x180384978
    180154faf:	mov    %rax,0x18(%rdi)
    180154fb3:	mov    %r13,0x40(%rdi)
    180154fb7:	lea    0xf8(%rbp),%rax
    180154fbe:	mov    %rax,0x48(%rdi)
    180154fc2:	movsd  %xmm6,0x50(%rdi)
    180154fc7:	mov    %r14d,0x58(%rdi)
    180154fcb:	mov    %r12d,0x5c(%rdi)
@@ -397870,15 +397870,15 @@
    1801550b9:	test   %rax,%rax
    1801550bc:	je     0x1801550fc
    1801550be:	movq   $0x1,(%rax)
    1801550c5:	movb   $0x0,0x8(%rax)
    1801550c9:	xor    %eax,%eax
    1801550cb:	mov    %rax,0x10(%rdi)
    1801550cf:	mov    %rbx,0x10(%rdi)
-   1801550d3:	lea    0x22f8de(%rip),%rax        # 0x1803849b8
+   1801550d3:	lea    0x22f91e(%rip),%rax        # 0x1803849f8
    1801550da:	mov    %rax,0x18(%rdi)
    1801550de:	mov    %r13,0x40(%rdi)
    1801550e2:	lea    0xf8(%rbp),%rax
    1801550e9:	mov    %rax,0x48(%rdi)
    1801550ed:	movsd  %xmm6,0x50(%rdi)
    1801550f2:	mov    %r15d,0x58(%rdi)
    1801550f6:	mov    %r12d,0x5c(%rdi)
@@ -416305,15 +416305,15 @@
    180164ae3:	jne    0x180164aa0
    180164ae5:	jmp    0x180164c42
    180164aea:	movq   $0x1,0x80(%rbp)
    180164af5:	movb   $0x0,0x88(%rbp)
    180164afc:	xor    %eax,%eax
    180164afe:	mov    %rax,0x90(%rbp)
    180164b05:	mov    %rax,0x90(%rbp)
-   180164b0c:	lea    0x21fee5(%rip),%rax        # 0x1803849f8
+   180164b0c:	lea    0x21fec5(%rip),%rax        # 0x1803849d8
    180164b13:	mov    %rax,0x98(%rbp)
    180164b1a:	mov    %r13,0xc0(%rbp)
    180164b21:	lea    0x10(%rbp),%rax
    180164b25:	mov    %rax,0xc8(%rbp)
    180164b2c:	mov    %r12,0xd0(%rbp)
    180164b33:	mov    0x80(%rbp),%rax
    180164b3a:	inc    %rax
@@ -416610,15 +416610,15 @@
    180164f43:	jne    0x180164eb0
    180164f49:	jmp    0x1801650b2
    180164f4e:	movq   $0x1,0x80(%rbp)
    180164f59:	movb   $0x0,0x88(%rbp)
    180164f60:	xor    %eax,%eax
    180164f62:	mov    %rax,0x90(%rbp)
    180164f69:	mov    %rax,0x90(%rbp)
-   180164f70:	lea    0x21fa01(%rip),%rax        # 0x180384978
+   180164f70:	lea    0x21fa41(%rip),%rax        # 0x1803849b8
    180164f77:	mov    %rax,0x98(%rbp)
    180164f7e:	mov    %r13,0xc0(%rbp)
    180164f85:	lea    0x30(%rbp),%rax
    180164f89:	mov    %rax,0xc8(%rbp)
    180164f90:	mov    %r15,0xd0(%rbp)
    180164f97:	mov    0x80(%rbp),%rax
    180164f9e:	inc    %rax
@@ -1081001,20 +1081001,21 @@
    180384959:	rex.WR cmp %r8b,0x1(%rax)
    180384960:	rex.XB outsl %ds:(%rsi),(%dx)
    180384962:	outsb  %ds:(%rsi),(%dx)
    180384963:	jbe    0x1803849ca
    180384965:	jb     0x1803849da
    180384967:	imul   $0x0,0x6e(%rdi),%ebp
    18038496e:	add    %al,(%rax)
-   180384970:	movabs 0xc00000000180384c,%al
-   180384979:	rex.X adc $0x80,%al
-   18038497c:	add    %eax,(%rax)
+   180384970:	movabs 0xe00000000180384c,%al
+   180384979:	pop    %rax
+   18038497a:	(bad)
+   18038497b:	addb   $0x0,(%rcx)
    18038497e:	add    %al,(%rax)
-   180384980:	nop
-   180384981:	jge    0x180384999
+   180384980:	lock pop %rcx
+   180384982:	(bad)
    180384983:	addb   $0x0,(%rcx)
    180384986:	add    %al,(%rax)
    180384988:	push   %rax
    180384989:	rex.XB adc $0x80,%al
    18038498c:	add    %eax,(%rax)
    18038498e:	add    %al,(%rax)
    180384990:	add    %al,0x14(%rbx)
@@ -1081026,47 +1081027,46 @@
    1803849a6:	add    %al,(%rax)
    1803849a8:	adc    %dh,0x16(%rbp)
    1803849ab:	addb   $0x0,(%rcx)
    1803849ae:	add    %al,(%rax)
    1803849b0:	add    %al,0x14(%rbx)
    1803849b3:	addb   $0x0,(%rcx)
    1803849b6:	add    %al,(%rax)
-   1803849b8:	loopne 0x180384a12
-   1803849ba:	(bad)
-   1803849bb:	addb   $0x0,(%rcx)
+   1803849b8:	rolb   $0x80,0x14(%rdx)
+   1803849bc:	add    %eax,(%rax)
    1803849be:	add    %al,(%rax)
-   1803849c0:	and    %bl,0x16(%rcx)
+   1803849c0:	nop
+   1803849c1:	jge    0x1803849d9
    1803849c3:	addb   $0x0,(%rcx)
    1803849c6:	add    %al,(%rax)
    1803849c8:	push   %rax
    1803849c9:	rex.XB adc $0x80,%al
    1803849cc:	add    %eax,(%rax)
    1803849ce:	add    %al,(%rax)
    1803849d0:	add    %al,0x14(%rbx)
    1803849d3:	addb   $0x0,(%rcx)
    1803849d6:	add    %al,(%rax)
-   1803849d8:	loopne 0x180384a32
-   1803849da:	(bad)
-   1803849db:	addb   $0x0,(%rcx)
+   1803849d8:	rolb   $0x80,0x14(%rdx)
+   1803849dc:	add    %eax,(%rax)
    1803849de:	add    %al,(%rax)
-   1803849e0:	lock pop %rcx
-   1803849e2:	(bad)
+   1803849e0:	lock jge 0x1803849f9
    1803849e3:	addb   $0x0,(%rcx)
    1803849e6:	add    %al,(%rax)
    1803849e8:	push   %rax
    1803849e9:	rex.XB adc $0x80,%al
    1803849ec:	add    %eax,(%rax)
    1803849ee:	add    %al,(%rax)
    1803849f0:	add    %al,0x14(%rbx)
    1803849f3:	addb   $0x0,(%rcx)
    1803849f6:	add    %al,(%rax)
-   1803849f8:	rolb   $0x80,0x14(%rdx)
-   1803849fc:	add    %eax,(%rax)
+   1803849f8:	loopne 0x180384a52
+   1803849fa:	(bad)
+   1803849fb:	addb   $0x0,(%rcx)
    1803849fe:	add    %al,(%rax)
-   180384a00:	lock jge 0x180384a19
+   180384a00:	and    %bl,0x16(%rcx)
    180384a03:	addb   $0x0,(%rcx)
    180384a06:	add    %al,(%rax)
    180384a08:	push   %rax
    180384a09:	rex.XB adc $0x80,%al
    180384a0c:	add    %eax,(%rax)
    180384a0e:	add    %al,(%rax)
    180384a10:	add    %al,0x14(%rbx)
@@ -1082477,16 +1082477,15 @@
    1803859ba:	(bad)
    1803859bb:	(bad)
    1803859bc:	(bad)
    1803859bd:	(bad)
    1803859be:	(bad)
    1803859bf:	incl   (%rax)
    1803859c1:	add    %al,(%rax)
-   1803859c3:	add    %dh,(%rax)
-   1803859c5:	rex.RXB pcmpgtd (%r8),%mm0
+   1803859c3:	add    %ch,0x660ee8(%rcx)
    1803859c9:	add    %al,(%rax)
    1803859cb:	add    %cl,-0x78000000(%rip)        # 0x1083859d1
    1803859d1:	add    (%rax),%eax
    1803859d3:	add    %dh,%ah
    1803859d5:	xchg   %bh,(%rax)
    1803859d7:	add    %dh,%ah
    1803859d9:	js     0x180385a13
```

## Comparing `Geode_Conversion-5.2.7.dist-info/METADATA` & `Geode_Conversion-5.2.7rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Geode-Conversion
-Version: 5.2.7
+Version: 5.2.7rc1
 Summary: Conversion module for Geode-solutions OpenGeode modules
 Home-page: https://github.com/Geode-solutions/Geode-Conversion
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core ==14.*,>=14.18.1
+Requires-Dist: opengeode-core ==14.*,>=14.18.1rc1
 
 <h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Conversion OpenGeode module</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.2.7 Summary: Conversion
-module for Geode-solutions OpenGeode modules Home-page: https://github.com/
-Geode-solutions/Geode-Conversion Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: opengeode-core ==14.*,>=14.18.1
+Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.2.7rc1 Summary:
+Conversion module for Geode-solutions OpenGeode modules Home-page: https://
+github.com/Geode-solutions/Geode-Conversion Author: Geode-solutions Author-
+email: contact@geode-solutions.com License: Proprietary Platform: UNKNOWN
+Description-Content-Type: text/markdown Requires-Dist: opengeode-core
+==14.*,>=14.18.1rc1
                ************ GGeeooddee--CCoonnvveerrssiioonnbbyy GGeeooddee--ssoolluuttiioonnss ************
                      ******** CCoonnvveerrssiioonn OOppeennGGeeooddee mmoodduullee ********
             [Build Status][Deploy Status][Coverage Status][Version]
               [Windows support][Ubuntu support][Red Hat support]
  [Language][License][Semantic-release]_[_S_l_a_c_k_ _i_n_v_i_t_e_]Copyright (c) 2019 - 2024,
                                 Geode-solutions
```

