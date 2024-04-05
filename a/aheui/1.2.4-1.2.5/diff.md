# Comparing `tmp/aheui-1.2.4.tar.gz` & `tmp/aheui-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aheui-1.2.4.tar", last modified: Sun Mar 31 18:50:15 2024, max compression
+gzip compressed data, was "dist/aheui-1.2.5.tar", last modified: Fri Apr  5 15:00:51 2024, max compression
```

## Comparing `aheui-1.2.4.tar` & `aheui-1.2.5.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-03-31 18:50:15.000000 aheui-1.2.4/
--rw-r--r--   0 user       (501) staff       (20)     7603 2024-03-31 18:50:15.000000 aheui-1.2.4/PKG-INFO
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-03-31 18:50:15.000000 aheui-1.2.4/aheui.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     7603 2024-03-31 18:50:15.000000 aheui-1.2.4/aheui.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      392 2024-03-31 18:50:15.000000 aheui-1.2.4/aheui.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)       32 2024-03-31 18:50:15.000000 aheui-1.2.4/aheui.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       16 2024-03-31 18:50:15.000000 aheui-1.2.4/aheui.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-03-31 18:50:15.000000 aheui-1.2.4/aheui.egg-info/dependency_links.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-03-31 18:50:15.000000 aheui-1.2.4/aheui/
--rw-r--r--   0 user       (501) staff       (20)       18 2024-03-31 18:39:39.000000 aheui-1.2.4/aheui/version.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-03-31 05:03:26.000000 aheui-1.2.4/aheui/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     6859 2024-03-31 16:50:00.000000 aheui-1.2.4/aheui/_argparse.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-03-31 18:50:15.000000 aheui-1.2.4/aheui/int/
--rw-r--r--   0 user       (501) staff       (20)      401 2024-03-31 18:19:23.000000 aheui-1.2.4/aheui/int/smallint.py
--rw-r--r--   0 user       (501) staff       (20)      638 2024-03-31 18:19:23.000000 aheui-1.2.4/aheui/int/bigint.py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-03-31 05:03:26.000000 aheui-1.2.4/aheui/int/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    34104 2024-03-31 18:19:23.000000 aheui-1.2.4/aheui/compile.py
--rw-r--r--   0 user       (501) staff       (20)    15991 2024-03-31 18:19:23.000000 aheui-1.2.4/aheui/aheui.py
--rw-r--r--   0 user       (501) staff       (20)     1224 2024-03-31 16:50:00.000000 aheui-1.2.4/aheui/_compat.py
--rw-r--r--   0 user       (501) staff       (20)     1077 2024-03-31 16:50:00.000000 aheui-1.2.4/aheui/const.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-03-31 18:50:15.000000 aheui-1.2.4/bin/
--rwxr-xr-x   0 user       (501) staff       (20)      384 2024-03-31 18:32:13.000000 aheui-1.2.4/bin/aheui
--rwxr-xr-x   0 user       (501) staff       (20)      384 2024-03-31 18:32:13.000000 aheui-1.2.4/bin/aheui-py
--rw-r--r--   0 user       (501) staff       (20)        0 2024-03-31 16:01:29.000000 aheui-1.2.4/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)     5884 2024-03-31 05:03:26.000000 aheui-1.2.4/README.md
--rw-r--r--   0 user       (501) staff       (20)     1405 2024-03-31 18:49:29.000000 aheui-1.2.4/setup.py
--rw-r--r--   0 user       (501) staff       (20)       62 2024-03-31 18:50:15.000000 aheui-1.2.4/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-05 15:00:51.000000 aheui-1.2.5/
+-rw-r--r--   0 user       (501) staff       (20)     7697 2024-04-05 15:00:51.000000 aheui-1.2.5/PKG-INFO
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-05 15:00:51.000000 aheui-1.2.5/aheui.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     7697 2024-04-05 15:00:51.000000 aheui-1.2.5/aheui.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      454 2024-04-05 15:00:51.000000 aheui-1.2.5/aheui.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)       32 2024-04-05 15:00:51.000000 aheui-1.2.5/aheui.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       16 2024-04-05 15:00:51.000000 aheui-1.2.5/aheui.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-05 15:00:51.000000 aheui-1.2.5/aheui.egg-info/dependency_links.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-05 15:00:51.000000 aheui-1.2.5/aheui/
+-rw-r--r--   0 user       (501) staff       (20)       18 2024-04-05 09:24:12.000000 aheui-1.2.5/aheui/version.py
+-rw-r--r--   0 user       (501) staff       (20)     6319 2024-04-05 09:48:00.000000 aheui-1.2.5/aheui/option.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-03-31 05:03:26.000000 aheui-1.2.5/aheui/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1250 2024-04-05 09:24:12.000000 aheui-1.2.5/aheui/warning.py
+-rw-r--r--   0 user       (501) staff       (20)     4697 2024-04-05 09:24:12.000000 aheui-1.2.5/aheui/_argparse.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-05 15:00:51.000000 aheui-1.2.5/aheui/int/
+-rw-r--r--   0 user       (501) staff       (20)      731 2024-04-05 09:24:12.000000 aheui-1.2.5/aheui/int/smallint.py
+-rw-r--r--   0 user       (501) staff       (20)      892 2024-04-05 09:24:12.000000 aheui-1.2.5/aheui/int/bigint.py
+-rw-r--r--   0 user       (501) staff       (20)        0 2024-03-31 05:03:26.000000 aheui-1.2.5/aheui/int/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    34104 2024-04-05 09:24:12.000000 aheui-1.2.5/aheui/compile.py
+-rw-r--r--   0 user       (501) staff       (20)    13977 2024-04-05 09:48:00.000000 aheui-1.2.5/aheui/aheui.py
+-rw-r--r--   0 user       (501) staff       (20)     1857 2024-04-05 09:24:12.000000 aheui-1.2.5/aheui/_compat.py
+-rw-r--r--   0 user       (501) staff       (20)     1077 2024-04-05 06:42:15.000000 aheui-1.2.5/aheui/const.py
+-rw-r--r--   0 user       (501) staff       (20)     1327 2024-03-31 05:03:26.000000 aheui-1.2.5/LICENSE
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-05 15:00:51.000000 aheui-1.2.5/bin/
+-rwxr-xr-x   0 user       (501) staff       (20)      384 2024-04-05 09:05:25.000000 aheui-1.2.5/bin/aheui
+-rwxr-xr-x   0 user       (501) staff       (20)      384 2024-04-05 07:14:35.000000 aheui-1.2.5/bin/aheui-py
+-rwxr-xr-x   0 user       (501) staff       (20)      263 2024-04-05 09:24:14.000000 aheui-1.2.5/bin/ahsembler
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-05 15:00:51.000000 aheui-1.2.5/tests/
+-rw-r--r--   0 user       (501) staff       (20)     6713 2024-04-05 09:48:00.000000 aheui-1.2.5/tests/test_compile.py
+-rw-r--r--   0 user       (501) staff       (20)     6069 2024-04-05 09:24:12.000000 aheui-1.2.5/README.md
+-rw-r--r--   0 user       (501) staff       (20)     1333 2024-04-05 09:48:00.000000 aheui-1.2.5/setup.py
+-rw-r--r--   0 user       (501) staff       (20)       62 2024-04-05 15:00:51.000000 aheui-1.2.5/setup.cfg
```

### Comparing `aheui-1.2.4/PKG-INFO` & `aheui-1.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: aheui
-Version: 1.2.4
+Version: 1.2.5
 Summary: Aheui compiler & assembler toolkit.
 Home-page: https://github.com/aheui/rpaheui
 Author: Jeong YunWon
 Author-email: aheui@youknowone.org
 License: UNKNOWN
 Description: 알파희 - 알파희썬(rpython)으로 만든 엔터프라이즈급 고성능 아희
         ====
         
-        [![Build Status](https://travis-ci.org/aheui/rpaheui.svg?branch=master)](https://travis-ci.org/aheui/rpaheui)
+        [![Build Status](https://github.com/aheui/rpaheui/workflows/CI/badge.svg)](https://github.com/aheui/rpaheui/actions?query=workflow%3ACI)
         
         * English: [README.en.md](https://github.com/aheui/rpaheui/blob/master/README.en.md)
         * Working log (English): [LOG.md](https://github.com/aheui/rpaheui/blob/master/LOG.md)
         
         * 빌드 및 실행 영상: [Youtube](https://www.youtube.com/watch?v=mjoj69i_f8s)
         * 2015 한국 파이콘: [PyPy/RPython으로 20배 빨라지는 JIT 아희 인터프리터](http://www.slideshare.net/YunWonJeong/pypyrpython-20-jit)
         
@@ -27,16 +27,17 @@
         아직 파이썬을 모르세요? [알파희 개발자가 번역한 책](http://www.yes24.com/24/Goods/15240210?Acode=101)으로 파이썬을 공부해 봅시다.
         
         * 알파희썬이란?: [http://rpython.readthedocs.org][rpython]
         
         
         ```
         git clone https://github.com/aheui/rpaheui
-        make # set RPYTHON in Makefile. You can get pypy by: hg clone http://bitbucket.org/pypy/pypy
-        ./aheui-c <your-aheui-code>
+        make # RPYTHON 환경변수 설정 필요. rpython은 pypy 소스코드를 내려받으면 포함되어 있습니다. 버전은 github actions 설정을 참고해 주세요.
+        ./bin/aheui-c <아희 코드 파일>
+        ./bin/aheui-bigint-c <큰 정수가 필요한 아희 코드 파일>
         ```
         
         JIT로 속도 올리기
         ----
         
         PyPy 기술은 PyPy를 CPython보다 빠르게 동작하게 만듭니다. ([http://speed.pypy.org/](http://speed.pypy.org/) 참고)
         
@@ -133,12 +134,10 @@
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `aheui-1.2.4/aheui.egg-info/PKG-INFO` & `aheui-1.2.5/aheui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: aheui
-Version: 1.2.4
+Version: 1.2.5
 Summary: Aheui compiler & assembler toolkit.
 Home-page: https://github.com/aheui/rpaheui
 Author: Jeong YunWon
 Author-email: aheui@youknowone.org
 License: UNKNOWN
 Description: 알파희 - 알파희썬(rpython)으로 만든 엔터프라이즈급 고성능 아희
         ====
         
-        [![Build Status](https://travis-ci.org/aheui/rpaheui.svg?branch=master)](https://travis-ci.org/aheui/rpaheui)
+        [![Build Status](https://github.com/aheui/rpaheui/workflows/CI/badge.svg)](https://github.com/aheui/rpaheui/actions?query=workflow%3ACI)
         
         * English: [README.en.md](https://github.com/aheui/rpaheui/blob/master/README.en.md)
         * Working log (English): [LOG.md](https://github.com/aheui/rpaheui/blob/master/LOG.md)
         
         * 빌드 및 실행 영상: [Youtube](https://www.youtube.com/watch?v=mjoj69i_f8s)
         * 2015 한국 파이콘: [PyPy/RPython으로 20배 빨라지는 JIT 아희 인터프리터](http://www.slideshare.net/YunWonJeong/pypyrpython-20-jit)
         
@@ -27,16 +27,17 @@
         아직 파이썬을 모르세요? [알파희 개발자가 번역한 책](http://www.yes24.com/24/Goods/15240210?Acode=101)으로 파이썬을 공부해 봅시다.
         
         * 알파희썬이란?: [http://rpython.readthedocs.org][rpython]
         
         
         ```
         git clone https://github.com/aheui/rpaheui
-        make # set RPYTHON in Makefile. You can get pypy by: hg clone http://bitbucket.org/pypy/pypy
-        ./aheui-c <your-aheui-code>
+        make # RPYTHON 환경변수 설정 필요. rpython은 pypy 소스코드를 내려받으면 포함되어 있습니다. 버전은 github actions 설정을 참고해 주세요.
+        ./bin/aheui-c <아희 코드 파일>
+        ./bin/aheui-bigint-c <큰 정수가 필요한 아희 코드 파일>
         ```
         
         JIT로 속도 올리기
         ----
         
         PyPy 기술은 PyPy를 CPython보다 빠르게 동작하게 만듭니다. ([http://speed.pypy.org/](http://speed.pypy.org/) 참고)
         
@@ -133,12 +134,10 @@
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `aheui-1.2.4/aheui/_argparse.py` & `aheui-1.2.5/aheui/option.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,161 +1,151 @@
 # flake8: noqa: E501
 
 from __future__ import absolute_import
 
+import os
+from aheui._argparse import ArgumentParser
+from aheui._compat import bigint, PY3
 from aheui.version import VERSION
-
-
-class ParserError(Exception):
-    __description__ = ''
-
-    def __init__(self, desc=''):
-        self.desc = desc
-
-    def message(self):
-        return self.__description__ + self.desc
-
-
-class TooFewArgumentError(ParserError):
-    __description__ = 'too few arguments: '
-
-
-class TooManyArgumentError(ParserError):
-    __description__ = 'too many arguments: '
-
-
-class ArgumentNotInChoicesError(ParserError):
-    __description__ = 'argument is not in choices: '
-
-
-class InformationException(ParserError):
-    __description__ = ''
-
-
-class HelpException(InformationException):
-    __description__ = ''
-
-
-class ArgumentParser(object):
-    def __init__(self, **kwargs):
-        self.kwargs = kwargs
-        self.arguments = []
-
-    def add_argument(self, *names, **kwargs):
-        if 'dest' not in kwargs:
-            name = names[0]
-            while name[0] == '-':
-                name = name[1:]
-            kwargs['dest'] = name
-        if 'narg' not in kwargs:
-            kwargs['narg'] = '1'
-        if 'choices' not in kwargs:
-            kwargs['choices'] = ''
-        if 'description' not in kwargs:
-            kwargs['description'] = ''
-        if 'full_description' not in kwargs:
-            kwargs['full_description'] = ''
-        self.arguments.append((names, kwargs))
-
-    def _parse_args(self, args):
-        parsed = {}
-        nonparsed = []
-        idx = 0
-        while idx < len(args):
-            arg = args[idx]
-            done = False
-            for names, opt in self.arguments:
-                dest = opt['dest']
-                choices = opt['choices']
-                for name in list(names):
-                    if arg.startswith(name):
-                        narg = int(opt['narg'])
-                        if narg <= 0:
-                            idx += 1
-                            parsed[dest] = 'yes'
-                            done = True
-                            if narg < 0:
-                                if opt['dest'] == 'help':
-                                    raise HelpException('')
-                                else:
-                                    raise InformationException(opt['message'])
-                        elif name.startswith('--'):
-                            if '=' not in arg:
-                                raise TooFewArgumentError(name)
-                            argname, arg = arg.split('=', 1)
-                            if choices:
-                                if arg not in choices:
-                                    raise ArgumentNotInChoicesError('%s (given: %s / expected: %s)' % (name, arg, choices))
-                            parsed[dest] = arg
-                            idx += 1
-                            done = True
-                        elif name.startswith('-'):
-                            if name == arg:
-                                arg = args[idx + 1]
-                                parsed[dest] = arg
-                                idx += 2
-                            else:
-                                parsed[dest] = arg[len(name):]
-                                idx += 1
-                            done = True
-                    if done:
-                        break
-                if done:
-                    break
-            if not done:
-                nonparsed.append(arg)
-                idx += 1
-        for names, opt in self.arguments:
-            dest = opt['dest']
-            if dest not in parsed:
-                parsed[dest] = opt['default']
-        return parsed, nonparsed
-
-    def parse_args(self, args):
-        import os
-        try:
-            return self._parse_args(args)
-        except HelpException:
-            os.write(2, 'usage: %s [option] ... file\n\n' % self.kwargs.get('prog', args[0]))
-            for names, opt in self.arguments:
-                name = names[0] if names[0] == names[1] else ('%s,%s' % names[0:2])
-                os.write(2, '%s%s: %s' % (name, ' ' * (12 - len(name)), opt['description']))
-                if int(opt['narg']) > 0 and opt['default']:
-                    os.write(2, ' (default: %s)' % opt['default'])
-                if opt['choices']:
-                    os.write(2, ' (choices: %s)' % opt['choices'])
-                if opt['full_description']:
-                    os.write(2, '\n')
-                    os.write(2, opt['full_description'])
-                os.write(2, '\n')
-        except InformationException as e:
-            os.write(2, '%s\n' % e.desc)
-        except ParserError as e:
-            prog = self.kwargs.get('prog', args[0])
-            os.write(2, '%s: error: %s\n' % (prog, e.message()))
-        return {}, []
+from aheui import compile
 
 
 parser = ArgumentParser(prog='aheui')
-parser.add_argument('--opt', '-O', default='2', choices='0,1,2', description='Set optimization level.', full_description="""\t0: No optimization.
+parser.add_argument('--opt', '-O', default='1', choices='0,1,2', description='Set optimization level.', full_description="""\t0: No optimization.
 \t1: Quickly resolve deadcode by rough stacksize emulation and merge constant operations.
 \t2: Perfectly resolve deadcode by stacksize emulation, reserialize code chunks and merge constant operations.
 """)
-parser.add_argument('--source', '-S', default='auto', choices='auto,bytecode,asm,asm+comment,text', description='Set source filetype.', full_description="""\t- `auto`: Guess the source type. `bytecode` if `.aheuic` or `End of bytecode` pattern in source. `asm` is `.aheuis`. `text` if `.aheui`. `text` is default.
+parser.add_argument('--source', '-S', default='auto', choices='auto,bytecode,asm,text', description='Set source filetype.', full_description="""\t- `auto`: Guess the source type. `bytecode` if `.aheuic` or `End of bytecode` pattern in source. `asm` is `.aheuis`. `text` if `.aheui`. `text` is default.
 \t- `bytecode`: Aheui bytecode. (Bytecode representation of `ahsembly`.
 \t- `asm`: See `ahsembly`.
 \t- `asm+comment`: Same as `asm` with comments.
 \t- usage: `--source=asm`, `-Sbytecode` or `-S text`
 """)
-parser.add_argument('--target', '-T', default='run', choices='run,bytecode,asm', description='Set target filetype.', full_description="""\t- `run`: Run given code.
+parser.add_argument('--target', '-T', default='run', choices='run,bytecode,asm,asm+comment', description='Set target filetype.', full_description="""\t- `run`: Run given code.
 \t- `bytecode`: Aheui bytecode. (Bytecode representation of `ahsembly`.
 \t- `asm`: See `ahsembly`.
 \t- usage: `--target=asm`, `-Tbytecode` or `-T run`
 """)
 parser.add_argument('--output', '-o', default='', description='Output file. Default is ``. See details for each target. If the value is `-`, it is standard output.', full_description="""\t- `run` target: This option is not availble and ignored.
 \t- `bytecode` target: Default value is `.aheuic`
 \t- `asm` target: Default value is `.aheuis`
 """)
 parser.add_argument('--cmd', '-c', default='', description='Program passed in as string')
 parser.add_argument('--no-c', '--no-c', narg='0', default='no', description='Do not generate `.aheuic` file automatically.', full_description='\tWhat is .aheuic? https://github.com/aheui/snippets/commit/cbb5a12e7cd2db771538ab28dfbc9ad1ada86f35\n')
-parser.add_argument('--version', '-v', narg='-1', default='no', description='Show program version', message=VERSION)
+parser.add_argument('--warning-limit', '--warning-limit', default='', description='Set repetitive warning limit. '' fallbacks to environment variable `RPAHEUI_WARNING_LIMIT`. 0 means no warning. -1 means no limit. Default is 3.')
+parser.add_argument('--trace-limit', '--trace-limit', default='', description='Set JIT trace limit. '' fallbacks to environment variable `RPAHEUI_TRACE_LIMIT`.')
+parser.add_argument('--version', '-v', narg='-1', default='no', description='Show program version', message=('%s %s' % (VERSION, bigint.NAME)).encode('utf-8'))
 parser.add_argument('--help', '-h', narg='-1', default='no', description='Show this help text')
+
+
+def kwarg_or_environ(kwargs, environ, arg_key, env_key):
+    if arg_key in kwargs and kwargs[arg_key] != '':
+        return (1, kwargs[arg_key])
+    try:
+        return (2, environ[env_key])
+    except KeyError:
+        return (0, '')
+
+
+def kwarg_or_environ_int(kwargs, environ, arg_key, env_key, default):
+    source, arg = kwarg_or_environ(kwargs, environ, arg_key, env_key)
+    if source == 0:
+        return default
+    try:
+        value = int(arg)
+    except ValueError:
+        if source == 1:
+            msg = b'The value of --%s="%s" is not a valid integer\n' % (arg_key, arg)
+        elif source == 2:
+            msg = b'The value %s="%s" is not a valid integer\n' % (env_key, arg)
+        else:
+            assert False
+        os.write(2, msg)
+        raise
+    return value
+
+
+def process_options(argv, environ):
+    def open_r(filename):
+        return os.open(filename, os.O_RDONLY, 0o777)
+
+    kwargs, args = parser.parse_args(argv)
+    if not args:
+        raise SystemExit()
+
+    cmd = kwargs['cmd']
+    if cmd == '':
+        if len(args) != 2:
+            os.write(2, b'aheui: error: no input files\n')
+            raise SystemExit()
+        filename = args[1]
+        if filename == '-':
+            fp = 0
+            contents = compile.read(fp)
+        else:
+            fp = open_r(filename)
+            contents = compile.read(fp)
+            os.close(fp)
+    else:
+        if len(args) != 1:
+            os.write(2, b'aheui: error: --cmd,-c but input file found\n')
+            raise SystemExit()
+        if PY3:
+            cmd = cmd.encode('utf-8')
+        contents = cmd
+        filename = '-'
+
+    source = kwargs['source']
+    if source == 'auto':
+        if filename.endswith('.aheui'):
+            source = 'text'
+        elif filename.endswith('.aheuic'):
+            source = 'bytecode'
+        elif filename.endswith('.aheuis'):
+            source = 'asm'
+        elif b'\xff\xff\xff\xff' in contents:
+            source = 'bytecode'
+        else:
+            source = 'text'
+
+    opt_level = kwargs['opt']
+
+    target = kwargs['target']
+    need_aheuic = target == 'run' and kwargs['no-c'] == 'no'\
+        and filename != '-' and not filename.endswith('.aheuic')
+
+    if need_aheuic:
+        aheuic_output = filename
+        if aheuic_output.endswith('.aheui'):
+            aheuic_output += 'c'
+        else:
+            aheuic_output += '.aheuic'
+    else:
+        aheuic_output = None
+
+    output = kwargs['output']
+    comment_aheuis = False
+    if output == '':
+        if target == 'bytecode':
+            output = filename
+            if output.endswith('.aheui'):
+                output += 'c'
+            else:
+                output += '.aheuic'
+        elif target in ['asm', 'asm+comment']:
+            output = filename
+            if output != '-':
+                if output.endswith('.aheui'):
+                    output += 's'
+                else:
+                    output += '.aheuis'
+            comment_aheuis = target == 'asm+comment'
+        elif target == 'run':
+            output = '-'
+        else:
+            os.write(2, b'aheui: error: --target,-t must be one of "bytecode", "asm", "asm+comment", "run"\n')  # noqa: E501
+            raise SystemExit()
+
+    warning_limit = kwarg_or_environ_int(kwargs, environ, 'warning-limit', 'RPAHEUI_WARNING_LIMIT', 3)
+    trace_limit = kwarg_or_environ_int(kwargs, environ, 'trace-limit', 'RPAHEUI_TRACE_LIMIT', -1)
+
+    return cmd, source, contents, opt_level, target, aheuic_output, comment_aheuis, output, warning_limit, trace_limit
```

### Comparing `aheui-1.2.4/aheui/compile.py` & `aheui-1.2.5/aheui/compile.py`

 * *Files identical despite different names*

### Comparing `aheui-1.2.4/aheui/aheui.py` & `aheui-1.2.5/aheui/aheui.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # coding: utf-8
 
 from __future__ import absolute_import
 
 import os
 
 from aheui import const as c
-from aheui._compat import jit, unichr, ord, _unicode
-from aheui import _argparse
+from aheui._compat import jit, unichr, ord, _unicode, bigint, PYR
 from aheui import compile
-from aheui.int import smallint as bigint  # import `bigint` to enable bigint
+from aheui.option import process_options
+from aheui.warning import WarningPool
 
 
 def get_location(pc, stackok, is_queue, program):
     """Add debug information.
 
     PYPYLOG=jit-log-opt,jit-backend,jit-summary:<filename>
     """
@@ -27,20 +27,21 @@
 driver = jit.JitDriver(
     greens=['pc', 'stackok', 'is_queue', 'program'],
     reds=['stacksize', 'storage', 'selected'],
     get_printable_location=get_location)
 
 
 DEBUG = False  # debug flag for `rpaheui`
+MINUS1 = bigint.fromlong(-1)
 
 
 class Link(object):
     """Element unit for stack and queue."""
 
-    def __init__(self, next, value=bigint.fromlong(-1)):
+    def __init__(self, next, value=MINUS1):
         self.value = value
         self.next = next
 
 
 class LinkedList(object):
     """Common linked list for storages"""
 
@@ -56,19 +57,14 @@
         return value
 
     def swap(self):
         node1 = self.head
         node2 = node1.next
         node1.value, node2.value = node2.value, node1.value
 
-    def pop_longlong(self):
-        big_r = self.pop()
-        r = bigint.tolonglong(big_r)
-        return r
-
     def add(self):
         r1, r2 = self._get_2_values()
         r = bigint.add(r2, r1)
         self._put_value(r)
 
     def sub(self):
         r1, r2 = self._get_2_values()
@@ -215,18 +211,18 @@
 input_buffer = InputBuffer()
 
 
 @jit.dont_look_inside
 def read_utf8(input_buffer=input_buffer):
     """Get a utf-8 character from standard input.
 
-    The length of utf-8 character is detectable in first byte.
-    If decode fails, it means it is a broken character.
-    Non-utf-8 character input is undefined in aheui.
-    Let's put -1 in this implementaion.
+    The length of a UTF-8 character can be detected in the first byte.
+    If decoding fails, it indicates that the character is broken.
+    In Aheui, non-UTF-8 character input is undefined.
+    In this implementation, let's assign -1.
     """
     input_buffer.load(1)
     head = input_buffer.look(1)
     if head:
         v = ord(head[0])
         if v >= 0x80:
             if (v & 0xf0) == 0xf0:
@@ -278,28 +274,35 @@
     assert len(numchars) > 0
     if negative:
         numchars.insert(0, b'-')
     num = bigint.fromstr(b''.join(numchars))
     return num
 
 
-@jit.dont_look_inside
-def write_number(value):
-    os.write(outfp, _unicode(value).encode('utf-8'))
+def write_number(value_str):
+    os.write(outfp, value_str)
 
 
-@jit.dont_look_inside
-def write_utf8(value):
-    if not (0 <= value < 0x110000):
-        msg = b'[Warning] Undefined behavior: unicode %x out of range\n' % value
-        os.write(errfp, msg)
-        value = 0xfffd
-    os.write(outfp, unichr(value).encode('utf-8'))
+def write_utf8(warnings, value):
+    REPLACE_CHAR = unichr(0xfffd).encode('utf-8')
+
+    if bigint.is_unicodepoint(value):
+        codepoint = bigint.toint(value)
+        unicode_char = unichr(codepoint)
+        bytes = unicode_char.encode('utf-8')
+    else:
+        bytes = REPLACE_CHAR
+
+    os.write(outfp, bytes)
 
 
+def warn_utf8_range(warnings, value):
+    warnings.warn(b'write-utf8-range', value)
+    os.write(outfp, unichr(0xfffd).encode('utf-8'))
+
 class Program(object):
     _immutable_fields_ = ['labels[**]', 'opcodes[*]', 'values[*]', 'size']
 
     def __init__(self, lines, label_map):
         self.opcodes = [line[0] for line in lines]
         self.values = [line[1] for line in lines]
         self.size = len(lines)
@@ -320,18 +323,18 @@
     @jit.elidable
     def get_label(self, pc):
         return self.labels[self.get_operand(pc)]
 
 
 outfp = 1
 errfp = 2
+warnings = WarningPool()
 
 
 def mainloop(program, debug):
-    jit.set_param(driver, 'trace_limit', 30000)
     program = jit.promote(program)
     jit.assert_green(program)
     pc = 0
     stacksize = 0
     is_queue = False
     storage = Storage()
     storage = jit.promote(storage)
@@ -385,40 +388,44 @@
             value = program.get_operand(pc)
             selected = storage[value]
             stacksize = len(selected)
             is_queue = value == c.VAL_QUEUE
         elif op == c.OP_MOV:
             r = selected.pop()
             value = program.get_operand(pc)
-            storage[value].push(r)
+            targeted = storage[value]
+            targeted.push(r)
+            if selected == targeted:
+                stacksize += 1
         elif op == c.OP_CMP:
             selected.cmp()
         elif op == c.OP_BRPOP1 or op == c.OP_BRPOP2 or op == c.OP_JMP or op == c.OP_BRZ:
             if op == c.OP_BRPOP1 or op == c.OP_BRPOP2:
                 jump = not stackok
             elif op == c.OP_JMP:
                 jump = True
             elif op == c.OP_BRZ:
-                jump = 0 == selected.pop_longlong()
+                top = selected.pop()
+                jump = bigint.is_zero(top)
             else:
                 assert False
             if jump:
                 value = program.get_label(pc)
                 pc = value
                 stackok = program.get_req_size(pc) <= stacksize
                 driver.can_enter_jit(
                     pc=pc, stackok=stackok, is_queue=is_queue, program=program,
                     stacksize=stacksize, storage=storage, selected=selected)
                 continue
         elif op == c.OP_POPNUM:
-            r = selected.pop_longlong()
-            write_number(r)
+            r = selected.pop()
+            write_number(bigint.str(r))
         elif op == c.OP_POPCHAR:
-            r = selected.pop_longlong()
-            write_utf8(r)
+            r = selected.pop()
+            write_utf8(warnings, r)
         elif op == c.OP_PUSHNUM:
             num = read_number()
             selected.push(num)
         elif op == c.OP_PUSHCHAR:
             char = read_utf8()
             selected.push(char)
         elif op == c.OP_NONE:
@@ -427,113 +434,32 @@
             break
         else:
             os.write(errfp, (u'Missing operator: %s' % _unicode(op)).encode('utf-8'))
             assert False
         pc += 1
 
     if len(selected) > 0:
-        return int(selected.pop_longlong())
+        return bigint.toint(selected.pop())
     else:
         return 0
 
 
-def process_opt(argv):
-    def open_r(filename):
-        return os.open(filename, os.O_RDONLY, 0o777)
-
-    parser = _argparse.parser
-    kwargs, args = parser.parse_args(argv)
-    if not args:
-        raise SystemExit()
-
-    cmd = kwargs['cmd']
-    if cmd == '':
-        if len(args) != 2:
-            os.write(2, b'aheui: error: no input files\n')
-            raise SystemExit()
-        filename = args[1]
-        if filename == '-':
-            fp = 0
-            contents = compile.read(fp)
-        else:
-            fp = open_r(filename)
-            contents = compile.read(fp)
-            os.close(fp)
-    else:
-        if len(args) != 1:
-            os.write(2, b'aheui: error: --cmd,-c but input file found\n')
-            raise SystemExit()
-        contents = cmd
-        filename = '-'
-
-    source = kwargs['source']
-    if source == 'auto':
-        if filename.endswith('.aheui'):
-            source = 'text'
-        elif filename.endswith('.aheuic'):
-            source = 'bytecode'
-        elif filename.endswith('.aheuis'):
-            source = 'asm'
-        elif '\xff\xff\xff\xff' in contents:
-            source = 'bytecode'
-        else:
-            source = 'text'
-
-    opt_level = kwargs['opt']
-
-    target = kwargs['target']
-    need_aheuic = target == 'run' and kwargs['no-c'] == 'no'\
-        and filename != '-' and not filename.endswith('.aheuic')
-
-    if need_aheuic:
-        aheuic_output = filename
-        if aheuic_output.endswith('.aheui'):
-            aheuic_output += 'c'
-        else:
-            aheuic_output += '.aheuic'
-    else:
-        aheuic_output = None
-
-    output = kwargs['output']
-    comment_aheuis = False
-    if output == '':
-        if target == 'bytecode':
-            output = filename
-            if output.endswith('.aheui'):
-                output += 'c'
-            else:
-                output += '.aheuic'
-        elif target in ['asm', 'asm+comment']:
-            output = filename
-            if output.endswith('.aheui'):
-                output += 's'
-            else:
-                output += '.aheuis'
-            comment_aheuis = target == 'asm+comment'
-        elif target == 'run':
-            output = '-'
-        else:
-            os.write(2, b'aheui: error: --target,-t must be one of "bytecode", "asm", "asm+comment", "run"\n')  # noqa: E501
-            raise SystemExit()
-
-    return cmd, source, contents, opt_level, target, aheuic_output, comment_aheuis, output
-
-
 def open_w(filename):
     return os.open(filename, os.O_WRONLY | os.O_CREAT, 0o644)
 
 
 def prepare_compiler(contents, opt_level=2, source='code', aheuic_output=None, add_debug_info=False):
     compiler = compile.Compiler()
     if source == 'bytecode':
         compiler.read_bytecode(contents)
     elif source == 'asm':
         compiler.read_asm(contents.decode('utf-8'))
     else:
-        compiler.compile(contents.decode('utf-8'), add_debug_info=add_debug_info)
+        contents = contents.decode('utf-8')
+        compiler.compile(contents, add_debug_info=add_debug_info)
 
     if opt_level == 0:
         pass
     elif opt_level == 1:
         compiler.optimize1()
     elif opt_level == 2:
         compiler.optimize2()
@@ -552,22 +478,28 @@
         except Exception:
             pass
     return compiler
 
 
 def entry_point(argv):
     try:
-        cmd, source, contents, str_opt_level, target, aheuic_output, comment_aheuis, output = process_opt(argv)
+        cmd, source, contents, str_opt_level, target, aheuic_output, comment_aheuis, output, warning_limit, trace_limit = process_options(argv, os.environ)
     except SystemExit:
         return 1
 
+    warnings.limit = warning_limit
+    if trace_limit >= 0:
+        jit.set_param(driver, 'trace_limit', trace_limit)
+
     add_debug_info = DEBUG or target != 'run'  # debug flag for user program
     compiler = prepare_compiler(contents, int(str_opt_level), source, aheuic_output, add_debug_info)
     outfp = 1 if output == '-' else open_w(output)
     if target == 'run':
+        if not PYR:
+            warnings.warn(b'no-rpython')
         program = Program(compiler.lines, compiler.label_map)
         exitcode = mainloop(program, compiler.debug)
     elif target in ['asm', 'asm+comment']:
         asm = compiler.write_asm(commented=comment_aheuis).encode('utf-8')
         os.write(outfp, asm)
         os.close(outfp)
         exitcode = 0
```

### Comparing `aheui-1.2.4/aheui/const.py` & `aheui-1.2.5/aheui/const.py`

 * *Files identical despite different names*

### Comparing `aheui-1.2.4/README.md` & `aheui-1.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 알파희 - 알파희썬(rpython)으로 만든 엔터프라이즈급 고성능 아희
 ====
 
-[![Build Status](https://travis-ci.org/aheui/rpaheui.svg?branch=master)](https://travis-ci.org/aheui/rpaheui)
+[![Build Status](https://github.com/aheui/rpaheui/workflows/CI/badge.svg)](https://github.com/aheui/rpaheui/actions?query=workflow%3ACI)
 
 * English: [README.en.md](https://github.com/aheui/rpaheui/blob/master/README.en.md)
 * Working log (English): [LOG.md](https://github.com/aheui/rpaheui/blob/master/LOG.md)
 
 * 빌드 및 실행 영상: [Youtube](https://www.youtube.com/watch?v=mjoj69i_f8s)
 * 2015 한국 파이콘: [PyPy/RPython으로 20배 빨라지는 JIT 아희 인터프리터](http://www.slideshare.net/YunWonJeong/pypyrpython-20-jit)
 
@@ -19,16 +19,17 @@
 아직 파이썬을 모르세요? [알파희 개발자가 번역한 책](http://www.yes24.com/24/Goods/15240210?Acode=101)으로 파이썬을 공부해 봅시다.
 
 * 알파희썬이란?: [http://rpython.readthedocs.org][rpython]
 
 
 ```
 git clone https://github.com/aheui/rpaheui
-make # set RPYTHON in Makefile. You can get pypy by: hg clone http://bitbucket.org/pypy/pypy
-./aheui-c <your-aheui-code>
+make # RPYTHON 환경변수 설정 필요. rpython은 pypy 소스코드를 내려받으면 포함되어 있습니다. 버전은 github actions 설정을 참고해 주세요.
+./bin/aheui-c <아희 코드 파일>
+./bin/aheui-bigint-c <큰 정수가 필요한 아희 코드 파일>
 ```
 
 JIT로 속도 올리기
 ----
 
 PyPy 기술은 PyPy를 CPython보다 빠르게 동작하게 만듭니다. ([http://speed.pypy.org/](http://speed.pypy.org/) 참고)
```

### Comparing `aheui-1.2.4/setup.py` & `aheui-1.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,36 +25,35 @@
     version=get_version(),
     description='Aheui compiler & assembler toolkit.',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     author='Jeong YunWon',
     author_email='aheui@youknowone.org',
     url='https://github.com/aheui/rpaheui',
-    packages=(
+    packages=[
         'aheui',
         'aheui/int',
-    ),
+    ],
     package_data={
         'aheui': ['version.py']
     },
     install_requires=[
     ],
     tests_require=tests_require,
     extras_require={
         'tests': tests_require,
     },
     scripts=[
         'bin/aheui-py',
         'bin/aheui',
+        'bin/ahsembler',
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

