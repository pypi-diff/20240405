# Comparing `tmp/pyimg4-0.8.tar.gz` & `tmp/pyimg4-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimg4-0.8.tar", max compression
+gzip compressed data, was "pyimg4-0.8.2.tar", max compression
```

## Comparing `pyimg4-0.8.tar` & `pyimg4-0.8.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-08-22 20:30:12.666847 pyimg4-0.8/LICENSE
--rw-r--r--   0        0        0     1946 2023-08-22 20:30:12.666847 pyimg4-0.8/README.md
--rw-r--r--   0        0        0      223 2023-08-22 20:30:12.666847 pyimg4-0.8/pyimg4/__init__.py
--rw-r--r--   0        0        0    23939 2023-08-22 20:30:12.666847 pyimg4-0.8/pyimg4/__main__.py
--rw-r--r--   0        0        0    43290 2023-08-22 20:30:12.666847 pyimg4-0.8/pyimg4/_parser.py
--rw-r--r--   0        0        0      313 2023-08-22 20:30:12.666847 pyimg4-0.8/pyimg4/_types.py
--rw-r--r--   0        0        0     1291 2023-08-22 20:30:12.666847 pyimg4-0.8/pyimg4/errors.py
--rw-r--r--   0        0        0     1323 2023-08-22 20:30:12.666847 pyimg4-0.8/pyproject.toml
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 pyimg4-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-05 00:40:55.494810 pyimg4-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1861 2024-04-05 00:40:55.494810 pyimg4-0.8.2/README.md
+-rw-r--r--   0        0        0      183 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/__init__.py
+-rw-r--r--   0        0        0    28418 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/__main__.py
+-rw-r--r--   0        0        0     1273 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/errors.py
+-rw-r--r--   0        0        0    45343 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/parser.py
+-rw-r--r--   0        0        0      313 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyimg4/types.py
+-rw-r--r--   0        0        0     1377 2024-04-05 00:40:55.494810 pyimg4-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3241 1970-01-01 00:00:00.000000 pyimg4-0.8.2/PKG-INFO
```

### Comparing `pyimg4-0.8/LICENSE` & `pyimg4-0.8.2/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 adam
+Copyright (c) 2024 m1sta
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyimg4-0.8/README.md` & `pyimg4-0.8.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   <a href="https://github.com/m1stadev/PyIMG4/blob/master/LICENSE">
     <image src="https://img.shields.io/github/license/m1stadev/PyIMG4">
   </a>
   <a href="https://github.com/m1stadev/PyIMG4/stargazers">
     <image src="https://img.shields.io/github/stars/m1stadev/PyIMG4">
   </a>
   <a href="https://github.com/m1stadev/PyIMG4">
-    <image src="https://img.shields.io/tokei/lines/github/m1stadev/PyIMG4">
+    <image src="https://tokei.rs/b1/github/m1stadev/PyIMG4?category=code&lang=python&style=flat">
   </a>
   <a href="https://github.com/m1stadev/PyIMG4">
     <image src="https://img.shields.io/github/actions/workflow/status/m1stadev/PyIMG4/.github/workflows/python-tests.yml">
   </a>
     <br>
 </p>
 
@@ -29,36 +29,31 @@
 ```
 Usage: pyimg4 [OPTIONS] COMMAND [ARGS]...
 
   A Python CLI tool for parsing Apple's Image4 format.
 
 Options:
   --version  Show the version and exit.
-  --help     Show this message and exit.
+  -h, --help     Show this message and exit.
 
 Commands:
   im4m  Image4 manifest commands.
   im4p  Image4 payload commands.
   im4r  Image4 restore info commands.
   img4  Image4 commands.
 ```
 
 ## Requirements
 - Python 3.8 or higher
-- Python development headers (`python3-dev` on Debian-based OSes)
 
 ## Installation
 - Install from [PyPI](https://pypi.org/project/pyimg4/):
     - ```python3 -m pip install pyimg4```
-    - If you would like to use the compression features of PyIMG4, install the required libraries:
+    - If you would like to use the compression features of PyIMG4, install the optional libraries:
       - ```python3 -m pip install pyimg4[compression]```
 - Local installation:
     - `./install.sh`
     - Requires [Poetry](https://python-poetry.org)
 
-## TODO
-- Write documentation
-- Add logging
-
 ## Support
 
 For any questions/issues you have, [open an issue](https://github.com/m1stadev/PyIMG4/issues) or join my [Discord](https://m1sta.xyz/discord).
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
                      [https://github.com/m1stadev/PyIMG4]
                              ************ PPyyIIMMGG44 ************
 
          A Python library/CLI tool for parsing Apple's _I_m_a_g_e_4_ _f_o_r_m_a_t.
 ## Usage ``` Usage: pyimg4 [OPTIONS] COMMAND [ARGS]... A Python CLI tool for
-parsing Apple's Image4 format. Options: --version Show the version and exit. --
-help Show this message and exit. Commands: im4m Image4 manifest commands. im4p
-Image4 payload commands. im4r Image4 restore info commands. img4 Image4
-commands. ``` ## Requirements - Python 3.8 or higher - Python development
-headers (`python3-dev` on Debian-based OSes) ## Installation - Install from
-[PyPI](https://pypi.org/project/pyimg4/): - ```python3 -m pip install pyimg4```
-- If you would like to use the compression features of PyIMG4, install the
-required libraries: - ```python3 -m pip install pyimg4[compression]``` - Local
-installation: - `./install.sh` - Requires [Poetry](https://python-poetry.org)
-## TODO - Write documentation - Add logging ## Support For any questions/issues
-you have, [open an issue](https://github.com/m1stadev/PyIMG4/issues) or join my
-[Discord](https://m1sta.xyz/discord).
+parsing Apple's Image4 format. Options: --version Show the version and exit. -
+h, --help Show this message and exit. Commands: im4m Image4 manifest commands.
+im4p Image4 payload commands. im4r Image4 restore info commands. img4 Image4
+commands. ``` ## Requirements - Python 3.8 or higher ## Installation - Install
+from [PyPI](https://pypi.org/project/pyimg4/): - ```python3 -m pip install
+pyimg4``` - If you would like to use the compression features of PyIMG4,
+install the optional libraries: - ```python3 -m pip install pyimg4
+[compression]``` - Local installation: - `./install.sh` - Requires [Poetry]
+(https://python-poetry.org) ## Support For any questions/issues you have, [open
+an issue](https://github.com/m1stadev/PyIMG4/issues) or join my [Discord]
+(https://m1sta.xyz/discord).
```

### Comparing `pyimg4-0.8/pyimg4/__main__.py` & `pyimg4-0.8.2/pyimg4/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 from typing import BinaryIO, Optional
 
 import click
 
 import pyimg4
 from pyimg4 import Compression, Keybag
 
+CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
-@click.group()
+
+@click.group(context_settings=CONTEXT_SETTINGS)
 @click.version_option(message=f'PyIMG4 {pyimg4.__version__}')
 def cli():
-    '''A Python CLI tool for parsing Apple's Image4 format.'''
+    """A Python CLI tool for parsing Apple's Image4 format."""
 
     sys.tracebacklimit = 0
 
 
 @cli.group()
 def im4m() -> None:
-    '''Image4 manifest commands.'''
+    """Image4 manifest commands."""
 
     pass
 
 
 @im4m.command('info')
 @click.option(
     '-i',
@@ -36,15 +38,15 @@
     '-v',
     '--verbose',
     'verbose',
     is_flag=True,
     help='Increase verbosity.',
 )
 def im4m_info(input_: BinaryIO, verbose: bool) -> None:
-    '''Print available information on an Image4 manifest.'''
+    """Print available information on an Image4 manifest."""
 
     click.echo(f'Reading {input_.name}...')
 
     try:
         im4m = pyimg4.IM4M(input_.read())
     except:
         raise click.BadParameter(f'Failed to parse Image4 manifest file: {input_.name}')
@@ -120,46 +122,46 @@
     '-v',
     '--verbose',
     'verbose',
     is_flag=True,
     help='Increase verbosity.',
 )
 def im4m_verify(input_: BinaryIO, build_manifest: BinaryIO, verbose: bool) -> None:
-    '''Verify an Image4 manifest with a provided build manifest.'''
+    """Verify an Image4 manifest with a provided build manifest."""
 
     click.echo(f'Reading {input_.name}...')
 
     try:
         im4m = pyimg4.IM4M(input_.read())
     except:
         raise click.BadParameter(f'Failed to parse Image4 manifest file: {input_.name}')
 
     click.echo(f'Reading {build_manifest.name}...')
 
     try:
         manifest = plistlib.load(build_manifest)
-    except:
+    except plistlib.InvalidFileException:
         raise click.BadParameter(
             f'Failed to parse build manifest file: {build_manifest.name}'
         )
 
     for identity in manifest['BuildIdentities']:
         if not (
             int(identity['ApBoardID'], 16) == im4m.board_id
             and int(identity['ApChipID'], 16) == im4m.chip_id
         ):
             if verbose:
                 click.echo(
-                    f"Skipping build identity {manifest['BuildIdentities'].index(identity)}..."
+                    f"Skipping build identity {manifest['BuildIdentities'].index(identity) + 1}..."
                 )
 
             continue
 
         click.echo(
-            f"Selected build identity: {manifest['BuildIdentities'].index(identity)}"
+            f"Selected build identity: {manifest['BuildIdentities'].index(identity) + 1}"
         )
         for name, image_info in identity['Manifest'].items():
             if 'Digest' not in image_info.keys():
                 if verbose:
                     click.echo(f'Component: {name} has no hash, skipping...')
 
                 continue
@@ -182,17 +184,89 @@
             click.echo(f"Build ID: {identity['Info']['BuildNumber']}")
             click.echo(f"Restore type: {identity['Info']['RestoreBehavior']}")
             return
 
     click.echo('Image4 manifest is not valid for the provided build manifest!')
 
 
+@im4m.command('extract')
+@click.option(
+    '-i',
+    '--input',
+    'input_',
+    type=click.File('rb'),
+    help='Input SHSH blob file.',
+    required=True,
+)
+@click.option(
+    '-o',
+    '--output',
+    'output',
+    type=click.File('wb'),
+    help='Output file.',
+    required=True,
+)
+@click.option(
+    '-u',
+    '--update',
+    'install_type',
+    flag_value='updateInstall',
+    help='Extract update Image4 manifest (if available).',
+)
+@click.option(
+    '-n',
+    '--no-nonce',
+    'install_type',
+    flag_value='noNonce',
+    help='Extract no-nonce Image4 manifest (if available).',
+)
+def im4m_extract(
+    input_: BinaryIO, output: BinaryIO, install_type: Optional[str]
+) -> None:
+    """Extract an Image4 manifest from an SHSH blob."""
+
+    try:
+        data = plistlib.load(input_)
+    except plistlib.InvalidFileException:
+        raise click.BadParameter(f'Failed to read SHSH blob: {input_.name}')
+
+    if install_type == 'updateInstall':
+        if 'updateInstall' not in data.keys():
+            raise click.BadParameter(
+                f'SHSH blob does not contain an update Image4 manifest: {input_.name}'
+            )
+
+        data = data['updateInstall']
+    elif install_type == 'noNonce':
+        if 'noNonce' not in data.keys():
+            raise click.BadParameter(
+                f'SHSH blob does not contain a no-nonce Image4 manifest: {input_.name}'
+            )
+
+        data = data['noNonce']
+
+    if 'ApImg4Ticket' not in data.keys():
+        raise click.BadParameter(
+            f'SHSH blob does not contain an Image4 manifest: {input_.name}'
+        )
+
+    try:
+        im4m = pyimg4.IM4M(data['ApImg4Ticket'])
+    except:
+        raise click.BadParameter(
+            f'Failed to parse Image4 manifest in SHSH blob: {input_.name}'
+        )
+
+    output.write(im4m.output())
+    click.echo(f'Image4 manifest outputted to: {output.name}')
+
+
 @cli.group()
 def im4p() -> None:
-    '''Image4 payload commands.'''
+    """Image4 payload commands."""
 
     pass
 
 
 @im4p.command('create')
 @click.option(
     '-i',
@@ -213,36 +287,36 @@
 @click.option(
     '-d',
     '--description',
     type=str,
     help='Description to set.',
 )
 @click.option(
-    '--extra',
-    type=click.File('rb'),
-    help='Extra IM4P payload data to set (requires --lzss).',
-)
-@click.option(
     '--lzss', 'compression_type', flag_value='LZSS', help='LZSS compress the data.'
 )
 @click.option(
     '--lzfse',
     'compression_type',
     flag_value='LZFSE',
     help='LZFSE compress the data.',
 )
+@click.option(
+    '--extra',
+    type=click.File('rb'),
+    help='Extra IM4P payload data to set (requires --lzss).',
+)
 def im4p_create(
     input_: BinaryIO,
     output: BinaryIO,
     fourcc: str,
     description: Optional[str],
-    extra: Optional[BinaryIO],
     compression_type: Optional[str],
+    extra: Optional[BinaryIO],
 ) -> None:
-    '''Create an Image4 payload file.'''
+    """Create an Image4 payload file."""
 
     if len(fourcc) != 4:
         raise click.BadParameter('FourCC must be 4 characters long')
 
     click.echo(f'Reading {input_.name}...')
 
     try:
@@ -267,15 +341,15 @@
                 f'Payload is already {im4p.payload.compression.name} compressed'
             )
 
         click.echo(f'Compressing payload using {compression_type.name}...')
         im4p.payload.compress(compression_type)
 
     output.write(im4p.output())
-    click.echo(f'IM4P outputted to: {output.name}')
+    click.echo(f'Image4 payload outputted to: {output.name}')
 
 
 @im4p.command('extract')
 @click.option(
     '-i',
     '--input',
     'input_',
@@ -308,32 +382,32 @@
     input_: BinaryIO,
     output: BinaryIO,
     extra: Optional[BinaryIO],
     decompress: bool,
     iv: Optional[str],
     key: Optional[str],
 ) -> None:
-    '''Extract data from an Image4 payload.'''
+    """Extract data from an Image4 payload."""
 
     click.echo(f'Reading {input_.name}...')
 
     try:
         im4p = pyimg4.IM4P(input_.read())
     except:
         raise click.BadParameter(f'Failed to parse Image4 payload file: {input_.name}')
 
     if iv is None and key is None:
-        if im4p.payload.encrypted == True:
+        if im4p.payload.encrypted is True:
             click.echo('[NOTE] Image4 payload data is encrypted')
 
     elif iv is None or key is None:
-        if im4p.payload.encrypted == True:
+        if im4p.payload.encrypted is True:
             raise click.BadParameter('You must specify both the IV and the key')
 
-    elif im4p.payload.encrypted == True:
+    elif im4p.payload.encrypted is True:
         click.echo('[NOTE] Image4 payload data is encrypted, decrypting...')
 
         if iv.lower().startswith('0x'):
             iv = iv[2:]
 
         if key.lower().startswith('0x'):
             key = key[2:]
@@ -394,44 +468,47 @@
     '-v',
     '--verbose',
     'verbose',
     is_flag=True,
     help='Increase verbosity.',
 )
 def im4p_info(input_: BinaryIO, verbose: bool) -> None:
-    '''Print available information on an Image4 payload.'''
+    """Print available information on an Image4 payload."""
 
     click.echo(f'Reading {input_.name}...')
 
     try:
         im4p = pyimg4.IM4P(input_.read())
     except:
         raise click.BadParameter(f'Failed to parse Image4 payload file: {input_.name}')
 
     click.echo('Image4 payload info:')
     click.echo(f'  FourCC: {im4p.fourcc}')
     click.echo(f'  Description: {im4p.description}')
-    click.echo(f'  Data size: {round(len(im4p.payload) / 1000, 2)}KB')
+
+    if verbose:
+        payload_size = len(im4p.payload)
+    else:
+        payload_size = f'{round(len(im4p.payload) / 1000, 2)}KB'
+    click.echo(f'  Data size: {payload_size}')
 
     if im4p.payload.compression != pyimg4.Compression.NONE:
         compression_type = (
             'LZFSE'
             if im4p.payload.compression
             in (pyimg4.Compression.LZFSE, pyimg4.Compression.LZFSE_ENCRYPTED)
-            else im4p.payload.compression
+            else im4p.payload.compression.name
         )
         click.echo(f'  Data compression type: {compression_type}')
 
-        if im4p.payload.compression == pyimg4.Compression.LZSS:
-            im4p.payload.decompress()
-            payload_size = len(im4p.payload)
+        if verbose:
+            payload_size = im4p.payload.size
         else:
-            payload_size = im4p.payload.get_lzfse_payload_size()
-
-        click.echo(f'  Data size (uncompressed): {round(payload_size / 1000, 2)}KB')
+            payload_size = f'{round(im4p.payload.size / 1000, 2)}KB'
+        click.echo(f'  Data size (uncompressed): {payload_size}')
 
     click.echo(f'  Encrypted: {im4p.payload.encrypted}')
     if im4p.payload.encrypted:
         click.echo(f'  Keybags ({len(im4p.payload.keybags)}):')
         for k, kb in enumerate(im4p.payload.keybags):
             click.echo(f'    Type: {kb.type.name}')
             click.echo(f'    IV: {kb.iv.hex()}')
@@ -455,15 +532,15 @@
             click.echo(
                 f"\n  Properties ({len(im4p.properties)}): {', '.join(i.fourcc for i in im4p.properties)}"
             )
 
 
 @cli.group()
 def im4r() -> None:
-    '''Image4 restore info commands.'''
+    """Image4 restore info commands."""
 
     pass
 
 
 @im4r.command('create')
 @click.option(
     '-g',
@@ -476,15 +553,15 @@
     '-o',
     '--output',
     type=click.File('wb'),
     required=True,
     help='File to output Image4 restore info to.',
 )
 def im4r_create(boot_nonce: str, output: BinaryIO) -> None:
-    '''Create an Image4 restore info file.'''
+    """Create an Image4 restore info file."""
 
     click.echo(f'Creating Image4 restore info file with boot nonce: {boot_nonce}...')
 
     if boot_nonce.lower().startswith('0x'):
         boot_nonce = boot_nonce[2:]
 
     try:
@@ -514,15 +591,15 @@
     '-v',
     '--verbose',
     'verbose',
     is_flag=True,
     help='Increase verbosity.',
 )
 def im4r_info(input_: BinaryIO, verbose: bool) -> None:
-    '''Print available information on an Image4 restore info file.'''
+    """Print available information on an Image4 restore info file."""
 
     click.echo(f'Reading {input_.name}...')
 
     try:
         im4r = pyimg4.IM4R(input_.read())
     except:
         raise click.BadParameter(
@@ -547,25 +624,52 @@
                     click.echo()
         else:
             click.echo(f"  Properties ({len(extra_props)}): {', '.join(extra_props)}")
 
 
 @cli.group()
 def img4() -> None:
-    '''Image4 commands.'''
+    """Image4 commands."""
 
     pass
 
 
 @img4.command('create')
 @click.option(
+    '-i',
+    '--input',
+    'input_',
+    type=click.File('rb'),
+    help='Input file.',
+)
+@click.option('-f', '--fourcc', type=str, help='FourCC to set.')
+@click.option(
+    '-d',
+    '--description',
+    type=str,
+    help='Description to set.',
+)
+@click.option(
+    '--lzss', 'compression_type', flag_value='LZSS', help='LZSS compress the data.'
+)
+@click.option(
+    '--lzfse',
+    'compression_type',
+    flag_value='LZFSE',
+    help='LZFSE compress the data.',
+)
+@click.option(
+    '--extra',
+    type=click.File('rb'),
+    help='Extra IM4P payload data to set (requires --lzss).',
+)
+@click.option(
     '-p',
     '--im4p',
     type=click.File('rb'),
-    required=True,
     help='Input Image4 payload file.',
 )
 @click.option(
     '-m',
     '--im4m',
     type=click.File('rb'),
     required=True,
@@ -584,79 +688,127 @@
     type=str,
     help='Boot nonce to set in Image4 restore info.',
 )
 @click.option(
     '-o', '--output', type=click.File('wb'), required=True, help='Output file.'
 )
 def img4_create(
-    im4p: BinaryIO,
+    input_: Optional[BinaryIO],
+    fourcc: Optional[str],
+    description: Optional[str],
+    compression_type: Optional[str],
+    extra: Optional[BinaryIO],
+    im4p: Optional[BinaryIO],
     im4m: BinaryIO,
     im4r: Optional[BinaryIO],
     boot_nonce: Optional[str],
     output: BinaryIO,
 ):
-    '''Create an Image4 file.'''
+    """Create an Image4 file."""
 
-    click.echo(f'Reading {im4p.name}...')
+    if all(i is None for i in (input_, im4p, im4m, im4r, boot_nonce)):
+        raise click.BadParameter('You must specify at least one input file')
 
-    try:
-        im4p = pyimg4.IM4P(im4p.read())
-    except:
-        raise click.BadParameter(f'Failed to parse Image4 payload file: {im4p.name}')
+    img4 = pyimg4.IMG4()
+    if im4p is not None:
+        click.echo(f'Reading {im4p.name}...')
 
-    click.echo(f'Reading {im4m.name}...')
+        try:
+            im4p = pyimg4.IM4P(im4p.read())
+        except:
+            raise click.BadParameter(
+                f'Failed to parse Image4 payload file: {im4p.name}'
+            )
 
-    try:
-        im4m = pyimg4.IM4M(im4m.read())
-    except:
-        raise click.BadParameter(f'Failed to parse Image4 manifest file: {im4m.name}')
+        img4.im4p = im4p
+
+    elif input_ is not None:
+        click.echo(f'Reading {input_.name}...')
+        im4p = pyimg4.IM4P(
+            fourcc=fourcc, description=description, payload=input_.read()
+        )
+
+        if extra is not None:
+            click.echo(f'Reading extra Image4 payload data: {extra.name}...')
+            im4p.payload.extra = extra.read()
+
+        if compression_type is not None:
+            compression_type = getattr(Compression, compression_type)
+            click.echo(f'Compressing payload using {compression_type.name}...')
+            im4p.payload.compress(compression_type)
+
+        img4.im4p = im4p
+
+    if im4m is not None:
+        click.echo(f'Reading {im4m.name}...')
+
+        try:
+            im4m = pyimg4.IM4M(im4m.read())
+        except:
+            raise click.BadParameter(
+                f'Failed to parse Image4 manifest file: {im4m.name}'
+            )
+
+        img4.im4m = im4m
 
     if im4r is not None:
         click.echo(f'Reading {im4r.name}...')
 
         try:
             im4r = pyimg4.IM4R(im4r.read())
         except:
             raise click.BadParameter(
                 f'Failed to parse Image4 restore info file: {im4r.name}'
             )
 
+        img4.im4r = im4r
+
     elif boot_nonce is not None:
         click.echo(f'Creating Image4 restore info with boot nonce: {boot_nonce}...')
 
         if boot_nonce.lower().startswith('0x'):
             boot_nonce = boot_nonce[2:]
 
         try:
             boot_nonce = bytes.fromhex(boot_nonce)
         except TypeError:
             raise click.BadParameter('Boot nonce must be a hex string')
 
         if len(boot_nonce) != 8:
             raise click.BadParameter('Boot nonce must be 8 bytes long')
 
-        im4r = pyimg4.IM4R(boot_nonce=boot_nonce)
-
-    click.echo('Creating Image4...')
-    img4 = pyimg4.IMG4(im4p=im4p, im4m=im4m, im4r=im4r)
+        img4.im4r = pyimg4.IM4R(boot_nonce=boot_nonce)
 
+    click.echo('Outputting Image4...')
     output.write(img4.output())
     click.echo(f'Image4 file outputted to: {output.name}')
 
 
 @img4.command('extract')
 @click.option(
     '-i',
     '--input',
     'input_',
     type=click.File('rb'),
     help='Input Image4 file.',
     required=True,
 )
 @click.option(
+    '-r',
+    '--raw',
+    'raw',
+    type=click.File('wb'),
+    help='File to output Image4 payload data to.',
+)
+@click.option(
+    '--extra',
+    type=click.File('wb'),
+    help='File to output extra Image4 payload data to.',
+)
+@click.option(
     '-p',
     '--im4p',
     type=click.File('wb'),
     help='File to output Image4 payload to.',
 )
 @click.option(
     '-m',
@@ -668,30 +820,43 @@
     '-r',
     '--im4r',
     type=click.File('wb'),
     help='File to output Image4 restore info to.',
 )
 def img4_extract(
     input_: BinaryIO,
+    raw: Optional[BinaryIO],
+    extra: Optional[BinaryIO],
     im4p: Optional[BinaryIO],
     im4m: Optional[BinaryIO],
     im4r: Optional[BinaryIO],
 ) -> None:
-    '''Extract Image4 manifest/payload/restore info from an Image4 file.'''
+    """Extract Image4 manifest/payload/restore info from an Image4 file."""
 
     click.echo(f'Reading {input_.name}...')
 
     try:
         img4 = pyimg4.IMG4(input_.read())
     except:
         raise click.BadParameter(f'Failed to parse Image4 file: {input_.name}')
 
-    if all(i is None for i in (im4p, im4m, im4r)):
+    if all(i is None for i in (raw, extra, im4p, im4m, im4r)):
         raise click.BadParameter('You must specify at least one output file')
 
+    if raw is not None:
+        raw.write(img4.im4p.payload.data)
+        click.echo(f'Extracted Image4 payload data to: {raw.name}')
+
+    if extra is not None:
+        if img4.im4p.payload.extra is None:
+            raise click.BadParameter('No extra Image4 payload data found')
+
+        extra.write(img4.im4p.payload.extra)
+        click.echo(f'Extracted extra Image4 payload data to: {extra.name}')
+
     if im4p is not None:
         if img4.im4p is None:
             raise click.BadParameter('Image4 payload not found in Image4 file')
 
         im4p.write(img4.im4p.output())
         click.echo(f'Extracted Image4 payload to: {im4p.name}')
 
@@ -723,15 +888,15 @@
     '-v',
     '--verbose',
     'verbose',
     is_flag=True,
     help='Increase verbosity.',
 )
 def img4_info(input_: BinaryIO, verbose: bool) -> None:
-    '''Print available information on an Image4 file.'''
+    """Print available information on an Image4 file."""
 
     click.echo(f'Reading {input_.name}...')
 
     try:
         img4 = pyimg4.IMG4(input_.read())
     except:
         raise click.BadParameter(f'Failed to parse Image4 file: {input_.name}')
@@ -740,15 +905,15 @@
 
     click.echo('  Image4 payload info:')
     click.echo(f'    FourCC: {img4.im4p.fourcc}')
     click.echo(f'    Description: {img4.im4p.description}')
     click.echo(f'    Data size: {round(len(img4.im4p.payload) / 1000, 2)}KB')
 
     if (
-        img4.im4p.payload.encrypted == False
+        img4.im4p.payload.encrypted is False
         and img4.im4p.payload.compression != pyimg4.Compression.NONE
     ):
         click.echo(f'    Data compression type: {img4.im4p.payload.compression.name}')
 
         img4.im4p.payload.decompress()
         click.echo(
             f'    Data size (uncompressed): {round(len(img4.im4p.payload) / 1000, 2)}KB'
```

### Comparing `pyimg4-0.8/pyimg4/_parser.py` & `pyimg4-0.8.2/pyimg4/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,58 @@
+from sys import platform
 from typing import Any, List, Optional, Tuple, Union
 from zlib import adler32
 
 import asn1
 from Crypto.Cipher import AES
 
-from ._types import *
-from .errors import *
+from .errors import CompressionError, UnexpectedDataError, UnexpectedTagError
+from .types import Compression, KeybagType, Payload
 
 try:
     import lzss
 
-    have_lzss = True
+    _have_lzss = True
 except ImportError:
-    have_lzss = False
+    _have_lzss = False
 
-try:
-    import liblzfse
+_have_lzfse = False
+if platform == 'Darwin':
+    try:
+        import apple_compress
 
-    have_lzfse = True
-except ImportError:
-    have_lzfse = False
+        def _lzfse_decompress(data: bytes, decmp_size: Optional[int] = None) -> bytes:
+            return apple_compress.decompress(
+                data,
+                algorithm=apple_compress.Algorithm.LZFSE_IBOOT,
+                decmp_size=decmp_size,
+            )
+
+        def _lzfse_compress(data: bytes) -> bytes:
+            return apple_compress.compress(
+                data, algorithm=apple_compress.Algorithm.LZFSE_IBOOT
+            )
+
+        _have_lzfse = True
+    except ImportError:
+        pass
+
+if _have_lzfse is False:
+    try:
+        import liblzfse
+
+        def _lzfse_decompress(data: bytes, _: Optional[int] = None) -> bytes:
+            return liblzfse.decompress(data)
+
+        def _lzfse_compress(data: bytes) -> bytes:
+            return liblzfse.compress(data)
+
+        _have_lzfse = True
+    except ImportError:
+        pass
 
 
 class _PyIMG4:
     def __init__(self, data: Optional[bytes] = None) -> None:
         self._data = data
 
         self._decoder = asn1.Decoder()
@@ -110,32 +139,28 @@
 
     @property
     def value(self) -> Any:
         return self._value
 
     def output(self) -> bytes:
         self._encoder.start()
-        self._encoder.enter(
+        with self._encoder.construct(
             int(bytes(self.fourcc, 'ascii').hex(), 16), asn1.Classes.Private
-        )
-        self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-
-        self._encoder.write(
-            self.fourcc,
-            asn1.Numbers.IA5String,
-            asn1.Types.Primitive,
-            asn1.Classes.Universal,
-        )
-
-        self._encoder.write(
-            self.value, None, asn1.Types.Primitive, asn1.Classes.Universal
-        )
+        ):
+            with self._encoder.construct(asn1.Numbers.Sequence, asn1.Classes.Universal):
+                self._encoder.write(
+                    self.fourcc,
+                    asn1.Numbers.IA5String,
+                    asn1.Types.Primitive,
+                    asn1.Classes.Universal,
+                )
 
-        for _ in range(2):
-            self._encoder.leave()
+                self._encoder.write(
+                    self.value, None, asn1.Types.Primitive, asn1.Classes.Universal
+                )
 
         return self._encoder.output()
 
 
 class _PropertyGroup(_PyIMG4):
     _property = _Property
 
@@ -220,42 +245,38 @@
             raise TypeError(f'No {self._property.__name__} or fourcc provided.')
 
     def output(self) -> bytes:
         if len(self.properties) == 0:
             raise ValueError('No properties are set')
 
         self._encoder.start()
-        self._encoder.enter(
+        with self._encoder.construct(
             int(bytes(self.fourcc, 'ascii').hex(), 16), asn1.Classes.Private
-        )
-        self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-
-        self._encoder.write(
-            self.fourcc,
-            asn1.Numbers.IA5String,
-            asn1.Types.Primitive,
-            asn1.Classes.Universal,
-        )
-
-        self._encoder.enter(asn1.Numbers.Set, asn1.Classes.Universal)
-        for prop in self.properties:
-            self._decoder.start(prop.output())
-            self._encoder.enter(self._decoder.peek().nr, asn1.Classes.Private)
-
-            self._decoder.enter()
-            self._encoder.write(
-                self._decoder.read()[1],
-                asn1.Numbers.Sequence,
-                asn1.Types.Constructed,
-                asn1.Classes.Universal,
-            )
-            self._encoder.leave()
+        ):
+            with self._encoder.construct(asn1.Numbers.Sequence, asn1.Classes.Universal):
+                self._encoder.write(
+                    self.fourcc,
+                    asn1.Numbers.IA5String,
+                    asn1.Types.Primitive,
+                    asn1.Classes.Universal,
+                )
 
-        for _ in range(3):
-            self._encoder.leave()
+                with self._encoder.construct(asn1.Numbers.Set, asn1.Classes.Universal):
+                    for prop in self.properties:
+                        self._decoder.start(prop.output())
+                        with self._encoder.construct(
+                            self._decoder.peek().nr, asn1.Classes.Private
+                        ):
+                            self._decoder.enter()
+                            self._encoder.write(
+                                self._decoder.read()[1],
+                                asn1.Numbers.Sequence,
+                                asn1.Types.Constructed,
+                                asn1.Classes.Universal,
+                            )
 
         return self._encoder.output()
 
 
 class Data(_PyIMG4):
     def get_type(self) -> Optional[Union['IMG4', 'IM4P', 'IM4M', 'IM4R']]:
         self._decoder.start(self._data)
@@ -497,67 +518,61 @@
         if len(self.properties) == 0:
             raise ValueError('No properties are set')
 
         if len(self.images) == 0:
             raise ValueError('No images are set')
 
         self._encoder.start()
-        self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-
-        self._encoder.write(
-            'IM4M',
-            asn1.Numbers.IA5String,
-            asn1.Types.Primitive,
-            asn1.Classes.Universal,
-        )
-
-        self._encoder.write(
-            0,
-            asn1.Numbers.Integer,
-            asn1.Types.Primitive,
-            asn1.Classes.Universal,
-        )
-
-        self._encoder.enter(asn1.Numbers.Set, asn1.Classes.Universal)
-
-        manp = ManifestImageProperties(fourcc='MANP')
-        for prop in self.properties:
-            manp.add_property(prop)
-
-        manb = ManifestImageProperties(fourcc='MANB')
-        manb._properties = [manp, *self.images]
-        self._decoder.start(manb.output())
-        self._encoder.enter(self._decoder.peek().nr, asn1.Classes.Private)
-
-        self._decoder.enter()
-        self._encoder.write(
-            self._decoder.read()[1],
-            asn1.Numbers.Sequence,
-            asn1.Types.Constructed,
-            asn1.Classes.Universal,
-        )
+        with self._encoder.construct(asn1.Numbers.Sequence, asn1.Classes.Universal):
+            self._encoder.write(
+                'IM4M',
+                asn1.Numbers.IA5String,
+                asn1.Types.Primitive,
+                asn1.Classes.Universal,
+            )
 
-        for _ in range(2):
-            self._encoder.leave()
+            self._encoder.write(
+                0,
+                asn1.Numbers.Integer,
+                asn1.Types.Primitive,
+                asn1.Classes.Universal,
+            )
 
-        self._encoder.write(
-            self.signature,
-            asn1.Numbers.OctetString,
-            asn1.Types.Primitive,
-            asn1.Classes.Universal,
-        )
+            with self._encoder.construct(asn1.Numbers.Set, asn1.Classes.Universal):
+                manp = ManifestImageProperties(fourcc='MANP')
+                for prop in self.properties:
+                    manp.add_property(prop)
+
+                manb = ManifestImageProperties(fourcc='MANB')
+                manb._properties = [manp, *self.images]
+                self._decoder.start(manb.output())
+                with self._encoder.construct(
+                    self._decoder.peek().nr, asn1.Classes.Private
+                ):
+                    self._decoder.enter()
+                    self._encoder.write(
+                        self._decoder.read()[1],
+                        asn1.Numbers.Sequence,
+                        asn1.Types.Constructed,
+                        asn1.Classes.Universal,
+                    )
 
-        self._encoder.write(
-            self.certificates,
-            asn1.Numbers.Sequence,
-            asn1.Types.Constructed,
-            asn1.Classes.Universal,
-        )
+            self._encoder.write(
+                self.signature,
+                asn1.Numbers.OctetString,
+                asn1.Types.Primitive,
+                asn1.Classes.Universal,
+            )
 
-        self._encoder.leave()
+            self._encoder.write(
+                self.certificates,
+                asn1.Numbers.Sequence,
+                asn1.Types.Constructed,
+                asn1.Classes.Universal,
+            )
         return self._encoder.output()
 
 
 class RestoreProperty(_Property):
     pass
 
 
@@ -595,43 +610,38 @@
         self.add_property(RestoreProperty(fourcc='BNCN', value=boot_nonce))
 
     def output(self) -> bytes:
         if len(self.properties) == 0:
             raise ValueError('No properties are set')
 
         self._encoder.start()
-        self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-
-        self._encoder.write(
-            self.fourcc,
-            asn1.Numbers.IA5String,
-            asn1.Types.Primitive,
-            asn1.Classes.Universal,
-        )
-
-        self._encoder.enter(asn1.Numbers.Set, asn1.Classes.Universal)
-
-        if self.boot_nonce is not None:
-            self.boot_nonce = self.boot_nonce[::-1]
-
-        for prop in self.properties:
-            self._decoder.start(prop.output())
-            self._encoder.enter(self._decoder.peek().nr, asn1.Classes.Private)
-
-            self._decoder.enter()
+        with self._encoder.construct(asn1.Numbers.Sequence, asn1.Classes.Universal):
             self._encoder.write(
-                self._decoder.read()[1],
-                asn1.Numbers.Sequence,
-                asn1.Types.Constructed,
+                self.fourcc,
+                asn1.Numbers.IA5String,
+                asn1.Types.Primitive,
                 asn1.Classes.Universal,
             )
-            self._encoder.leave()
 
-        for _ in range(2):
-            self._encoder.leave()
+            with self._encoder.construct(asn1.Numbers.Set, asn1.Classes.Universal):
+                if self.boot_nonce is not None:
+                    self.boot_nonce = self.boot_nonce[::-1]
+
+                for prop in self.properties:
+                    self._decoder.start(prop.output())
+                    with self._encoder.construct(
+                        self._decoder.peek().nr, asn1.Classes.Private
+                    ):
+                        self._decoder.enter()
+                        self._encoder.write(
+                            self._decoder.read()[1],
+                            asn1.Numbers.Sequence,
+                            asn1.Types.Constructed,
+                            asn1.Classes.Universal,
+                        )
 
         return self._encoder.output()
 
 
 class IMG4(_PyIMG4):
     def __init__(
         self,
@@ -727,49 +737,51 @@
             raise UnexpectedDataError('IM4R or bytes', im4r)
 
         self._im4r = IM4R(im4r) if isinstance(im4r, bytes) else im4r
 
     def output(self) -> bytes:
         self._encoder.start()
 
-        self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-        self._encoder.write(
-            'IMG4', asn1.Numbers.IA5String, asn1.Types.Primitive, asn1.Classes.Universal
-        )
-
-        if self.im4p is None:
-            raise ValueError('No IM4P is set.')
+        with self._encoder.construct(asn1.Numbers.Sequence, asn1.Classes.Universal):
+            self._encoder.write(
+                'IMG4',
+                asn1.Numbers.IA5String,
+                asn1.Types.Primitive,
+                asn1.Classes.Universal,
+            )
 
-        self._decoder.start(self.im4p.output())
-        self._encoder.write(
-            self._decoder.read()[1],
-            asn1.Numbers.Sequence,
-            asn1.Types.Constructed,
-            asn1.Classes.Universal,
-        )
+            if self.im4p is None:
+                raise ValueError('No IM4P is set.')
 
-        if self.im4m is None:
-            raise ValueError('No IM4M is set.')
+            self._decoder.start(self.im4p.output())
+            self._encoder.write(
+                self._decoder.read()[1],
+                asn1.Numbers.Sequence,
+                asn1.Types.Constructed,
+                asn1.Classes.Universal,
+            )
 
-        self._encoder.write(
-            self.im4m.output(),
-            0,
-            asn1.Types.Constructed,
-            asn1.Classes.Context,
-        )
+            if self.im4m is None:
+                raise ValueError('No IM4M is set.')
 
-        if self.im4r is not None:
             self._encoder.write(
-                self.im4r.output(),
-                1,
+                self.im4m.output(),
+                0,
                 asn1.Types.Constructed,
                 asn1.Classes.Context,
             )
 
-        self._encoder.leave()
+            if self.im4r is not None:
+                self._encoder.write(
+                    self.im4r.output(),
+                    1,
+                    asn1.Types.Constructed,
+                    asn1.Classes.Context,
+                )
+
         return self._encoder.output()
 
 
 class PayloadProperty(_Property):
     pass
 
 
@@ -855,15 +867,15 @@
         if not self._decoder.eof() and self._decoder.peek().nr == asn1.Numbers.Sequence:
             self._decoder.enter()
 
             if (
                 self._decoder.peek().nr == asn1.Numbers.Integer
                 and self._decoder.read()[1] == 1
             ):
-                self.payload.set_lzfse_payload_size(self._decoder.read()[1])
+                self.payload.size = self._decoder.read()[1]
 
             self._decoder.leave()
 
         if not self._decoder.eof() and self._decoder.peek().cls == asn1.Classes.Context:
             self._decoder.enter()
 
             if self._decoder.peek().nr != asn1.Numbers.Sequence:
@@ -953,109 +965,113 @@
                 self._properties.remove(prop)
             else:
                 raise ValueError(f'Property "{fourcc}" not found')
 
     def output(self) -> bytes:
         self._encoder.start()
 
-        self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-        self._encoder.write(
-            'IM4P', asn1.Numbers.IA5String, asn1.Types.Primitive, asn1.Classes.Universal
-        )
-
-        if self.fourcc is None:
-            raise ValueError('No fourcc is set.')
-
-        self._encoder.write(
-            self.fourcc,
-            asn1.Numbers.IA5String,
-            asn1.Types.Primitive,
-            asn1.Classes.Universal,
-        )
-
-        self._encoder.write(
-            self.description,
-            asn1.Numbers.IA5String,
-            asn1.Types.Primitive,
-            asn1.Classes.Universal,
-        )
-
-        if self.payload is None:
-            raise ValueError('No payload is set.')
-
-        for i in self.payload.output():
-            if i is None:
-                continue
-
+        with self._encoder.construct(asn1.Numbers.Sequence, asn1.Classes.Universal):
             self._encoder.write(
-                i,
-                asn1.Numbers.OctetString,
+                'IM4P',
+                asn1.Numbers.IA5String,
                 asn1.Types.Primitive,
                 asn1.Classes.Universal,
             )
 
-        if self.payload.compression in (Compression.LZFSE, Compression.LZFSE_ENCRYPTED):
-            self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-
-            self._encoder.write(
-                1,
-                asn1.Numbers.Integer,
-                asn1.Types.Primitive,
-                asn1.Classes.Universal,
-            )
+            if self.fourcc is None:
+                raise ValueError('No fourcc is set.')
 
             self._encoder.write(
-                self.payload.get_lzfse_payload_size(),
-                asn1.Numbers.Integer,
+                self.fourcc,
+                asn1.Numbers.IA5String,
                 asn1.Types.Primitive,
                 asn1.Classes.Universal,
             )
 
-            self._encoder.leave()
-
-        if len(self.properties) > 0:
-            self._encoder.enter(0, asn1.Classes.Context)
-            self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-
             self._encoder.write(
-                'PAYP',
+                self.description,
                 asn1.Numbers.IA5String,
                 asn1.Types.Primitive,
                 asn1.Classes.Universal,
             )
 
-            self._encoder.enter(asn1.Numbers.Set, asn1.Classes.Universal)
-            for prop in self.properties:
-                self._decoder.start(prop.output())
-                self._encoder.enter(self._decoder.peek().nr, asn1.Classes.Private)
+            if self.payload is None:
+                raise ValueError('No payload is set.')
+
+            for i in self.payload.output():
+                if i is None:
+                    continue
 
-                self._decoder.enter()
                 self._encoder.write(
-                    self._decoder.read()[1],
-                    asn1.Numbers.Sequence,
-                    asn1.Types.Constructed,
+                    i,
+                    asn1.Numbers.OctetString,
+                    asn1.Types.Primitive,
                     asn1.Classes.Universal,
                 )
-                self._encoder.leave()
 
-            for _ in range(3):
-                self._encoder.leave()
+            if self.payload.compression in (
+                Compression.LZFSE,
+                Compression.LZFSE_ENCRYPTED,
+            ):
+                with self._encoder.construct(
+                    asn1.Numbers.Sequence, asn1.Classes.Universal
+                ):
+                    self._encoder.write(
+                        1,
+                        asn1.Numbers.Integer,
+                        asn1.Types.Primitive,
+                        asn1.Classes.Universal,
+                    )
+
+                    self._encoder.write(
+                        self.payload.size,
+                        asn1.Numbers.Integer,
+                        asn1.Types.Primitive,
+                        asn1.Classes.Universal,
+                    )
+
+            if len(self.properties) > 0:
+                with self._encoder.construct(0, asn1.Classes.Context):
+                    with self._encoder.construct(
+                        asn1.Numbers.Sequence, asn1.Classes.Universal
+                    ):
+                        self._encoder.write(
+                            'PAYP',
+                            asn1.Numbers.IA5String,
+                            asn1.Types.Primitive,
+                            asn1.Classes.Universal,
+                        )
+
+                        with self._encoder.construct(
+                            asn1.Numbers.Set, asn1.Classes.Universal
+                        ):
+                            for prop in self.properties:
+                                self._decoder.start(prop.output())
+                                with self._encoder.construct(
+                                    self._decoder.peek().nr, asn1.Classes.Private
+                                ):
+                                    self._decoder.enter()
+                                    self._encoder.write(
+                                        self._decoder.read()[1],
+                                        asn1.Numbers.Sequence,
+                                        asn1.Types.Constructed,
+                                        asn1.Classes.Universal,
+                                    )
 
-        self._encoder.leave()
         return self._encoder.output()
 
 
 class Keybag(_PyIMG4):
     def __init__(
         self,
         data: Optional[bytes] = None,
         *,
         iv: bytes = None,
         key: bytes = None,
-        type_: KeybagType = KeybagType.PRODUCTION  # Assume PRODUCTION if not provided
+        type_: KeybagType = KeybagType.PRODUCTION,  # Assume PRODUCTION if not provided
     ) -> None:
         super().__init__(data)
 
         if iv and key:
             self.iv = iv
             self.key = key
             self.type = type_
@@ -1064,15 +1080,15 @@
             self._parse()
 
         else:
             raise TypeError('No data or IV/Key provided.')
 
     def __repr__(self) -> str:
         return (
-            f"Keybag(iv={self.iv.hex()}, key={self.key.hex()}, type={self.type.name})"
+            f'Keybag(iv={self.iv.hex()}, key={self.key.hex()}, type={self.type.name})'
         )
 
     def _parse(self) -> None:
         self._decoder.start(self._data)
 
         if self._decoder.peek().nr != asn1.Numbers.Integer:
             raise UnexpectedTagError(self._decoder.peek(), asn1.Numbers.Integer)
@@ -1131,67 +1147,99 @@
         if not isinstance(type_, KeybagType):
             raise UnexpectedDataError('KeybagType', type_)
 
         self._type = type_
 
 
 class IM4PData(_PyIMG4):
-    def __init__(self, data: bytes) -> None:
+    def __init__(
+        self, data: bytes, *, size: int = 0, extra: Optional[bytes] = None
+    ) -> None:
         super().__init__(data)
 
         self._keybags = []
-        self.extra: Optional[bytes] = None
-        self._lzfse_payload_size: Optional[int] = None
+        self.extra = extra
+
+        self._detect_compression(size, data)
+        if self.compression == Compression.LZSS:
+            self._parse_complzss_header()
+        elif self.compression not in (Compression.NONE, Compression.LZFSE_ENCRYPTED):
+            self.size = len(self._decompress_data(data, self.compression, size))
+        else:
+            self.size = size
 
     def __len__(self) -> int:
-        return len(self.output().data)
+        return len(self.data)
 
     def __repr__(self) -> str:
         repr_ = f'IM4PData(payload length={hex(len(self))}, encrypted={self.encrypted}'
         if self.compression != Compression.NONE:
             repr_ += f', compression={self.compression.name}'
 
         return f'{repr_})'
 
-    def _create_complzss_header(self) -> bytes:
+    def _create_complzss_header(self, comp_size: int) -> bytes:
         header = bytearray(b'complzss')
         header += adler32(self._data).to_bytes(4, 'big')
-        header += len(self._data).to_bytes(4, 'big')
-        header += len(lzss.compress(self._data)).to_bytes(4, 'big')
+        header += self.size.to_bytes(4, 'big')
+        header += comp_size.to_bytes(4, 'big')
         header += int(1).to_bytes(4, 'big')
         header += bytearray(0x180 - len(header))
 
         return bytes(header)
 
+    def _decompress_data(
+        self, data: bytes, compression: Compression, size: Optional[int] = None
+    ) -> bytes:
+        if compression == Compression.LZSS:
+            if not _have_lzss:
+                raise RuntimeError('pylzss not installed, cannot use LZSS compression')
+
+            return lzss.decompress(data)
+
+        elif self.compression == Compression.LZFSE:
+            if not _have_lzfse:
+                raise RuntimeError(
+                    'apple-compress/pyliblzfse not installed, cannot use LZFSE compression'
+                )
+
+            return _lzfse_decompress(self._data, size)
+
+    def _detect_compression(self, size: int, data: bytes) -> None:
+        if self.encrypted and size > 0:
+            self._compression = Compression.LZFSE_ENCRYPTED
+
+        elif data.startswith(b'complzss'):
+            self._compression = Compression.LZSS
+
+        elif data.startswith(b'bvx2') and b'bvx$' in self._data:
+            self._compression = Compression.LZFSE
+
+        else:
+            self._compression = Compression.NONE
+
     def _parse_complzss_header(self) -> None:
+        self.size = int(self._data[0xC:0x10].hex(), 16)
         cmp_len = int(self._data[0x10:0x14].hex(), 16)
 
         if (
             cmp_len < len(self._data) - 0x180
         ):  # iOS 9+ A7-A9 kernelcache, so KPP is appended to the LZSS-compressed data
             extra_len = len(self._data) - cmp_len - 0x180
             self.extra = self._data[-extra_len:]
 
             self._data = self._data[:-extra_len]
 
-        self._data = self._data[0x180:]
-
     @property
     def compression(self) -> Compression:
-        if self.encrypted and self._lzfse_payload_size is not None:
-            return Compression.LZFSE_ENCRYPTED
+        return self._compression
 
-        if self._data.startswith(b'complzss'):
-            return Compression.LZSS
-
-        elif self._data.startswith(b'bvx2') and b'bvx$' in self._data:
-            return Compression.LZFSE
-
-        else:
-            return Compression.NONE
+    @property
+    def data(self) -> bytes:
+        return self._data
 
     @property
     def encrypted(self) -> bool:
         return len(self.keybags) > 0
 
     @property
     def extra(self) -> Optional[bytes]:
@@ -1204,14 +1252,31 @@
 
         self._extra = extra
 
     @property
     def keybags(self) -> Tuple[Optional[Keybag]]:
         return tuple(self._keybags)
 
+    @property
+    def size(self) -> int:
+        return self._size
+
+    @size.setter
+    def size(self, size: int) -> None:
+        if not isinstance(size, int):
+            raise UnexpectedDataError('int', size)
+
+        if size < 0:
+            raise ValueError('Size cannot be less than 0.')
+
+        if 0 < size < len(self.data):
+            raise ValueError('Size cannot be less than the length of the payload data.')
+
+        self._size = size
+
     def add_keybag(self, keybag: Keybag) -> None:
         if not isinstance(keybag, Keybag):
             raise UnexpectedDataError('Keybag', keybag)
 
         if any(kbag.type == keybag.type for kbag in self.keybags):
             raise ValueError(
                 f'There is already a {keybag.type.name.lower()} keybag added.'
@@ -1244,142 +1309,86 @@
                 raise ValueError(f'There is no {type_.name.lower()} keybag added.')
 
     def compress(self, compression: Compression) -> None:
         if compression in (
             Compression.NONE,
             Compression.LZFSE_ENCRYPTED,
         ):
-            raise CompressionError('A valid compression type must be specified.')
+            raise ValueError('A valid compression type must be specified.')
 
-        elif self.compression in (
-            Compression.LZSS,
-            Compression.LZFSE,
-            Compression.LZFSE_ENCRYPTED,
-        ):
-            raise CompressionError(
-                f"Payload is already {compression.name.replace('_ENCRYPTED', '')}-compressed."
-            )
+        if self.encrypted is True:
+            raise CompressionError('Cannot compress encrypted payload.')
 
+        elif self.compression in (Compression.LZSS, Compression.LZFSE):
+            raise CompressionError(f'Payload is already {compression.name}-compressed.')
+
+        self.size = len(self._data)
         if compression == Compression.LZSS:
-            if not have_lzss:
+            if not _have_lzss:
                 raise RuntimeError('pylzss not installed, cannot use LZSS compression')
 
-            self._data = self._create_complzss_header() + lzss.compress(self._data)
-
-            if self.extra is not None:
-                self._data += self.extra
+            comp_data = lzss.compress(self._data)
+            self._data = self._create_complzss_header(len(comp_data)) + comp_data
 
         elif compression == Compression.LZFSE:
-            if not have_lzfse:
+            if not _have_lzfse:
                 raise RuntimeError(
-                    'pyliblzfse not installed, cannot use LZFSE compression'
+                    'apple-compress/pyliblzfse not installed, cannot use LZFSE compression'
                 )
 
-            payload_size = len(self._data)
-            self._data = liblzfse.compress(self._data)
-            # Cannot set LZFSE payload size until after compression
-            self.set_lzfse_payload_size(payload_size)
-
-            if self.compression != Compression.LZFSE:  # If bvx2 header isn't present
-                self._lzfse_payload_size = None
-                self._data = liblzfse.decompress(self._data)
-
+            comp_data = _lzfse_compress(self._data)
+            if not (comp_data.startswith(b'bvx2') and b'bvx$' in comp_data):
                 raise CompressionError('Failed to LZFSE-compress payload.')
 
-        if self.compression != Compression.LZFSE:
-            self._lzfse_payload_size = None
+            self._data = comp_data
+
+        self._detect_compression(self.size, self._data)
+
+        if self.extra is not None:
+            self._data += self.extra
 
     def decompress(self) -> None:
         if self.compression == Compression.NONE:
             raise CompressionError('Payload is not compressed.')
 
-        if self.encrypted == True:
+        elif self.compression == Compression.LZFSE_ENCRYPTED:
             raise CompressionError('Cannot decompress encrypted payload.')
 
-        elif self.compression == Compression.LZSS:
-            if not have_lzss:
-                raise RuntimeError('pylzss not installed, cannot use LZSS compression')
-
-            self._parse_complzss_header()
-            self._data = lzss.decompress(self._data)
-
-        elif self.compression == Compression.LZFSE:
-            if not have_lzfse:
-                raise RuntimeError(
-                    'pyliblzfse not installed, cannot use LZFSE compression'
-                )
-
-            self._lzfse_payload_size = None
-            self._data = liblzfse.decompress(self._data)
+        self._data = self._decompress_data(self._data, self.compression, self.size)
+        self._compression = Compression.NONE
+        self._detect_compression(self.size, self._data)
 
     def decrypt(self, kbag: Keybag) -> None:
-        try:
-            self._data = AES.new(kbag.key, AES.MODE_CBC, kbag.iv).decrypt(self._data)
-            self._keybags = []
-        except:
-            raise AESError('Failed to decrypt payload.')
-
-    def get_lzfse_payload_size(self) -> int:
-        if self._lzfse_payload_size is None:
-            if self.compression == Compression.LZFSE:
-                self.set_lzfse_payload_size(len(liblzfse.decompress(self._data)))
-
-            elif self.encrypted:
-                raise AttributeError(
-                    'Cannot get LZFSE payload size of encrypted payload.'
-                )
-
-            else:
-                raise CompressionError(
-                    'Cannot get LZFSE payload size of non-LZFSE-compressed payload.'
-                )
-
-        return self._lzfse_payload_size
-
-    def set_lzfse_payload_size(self, size: int) -> None:
-        # If the compression is LZFSE_ENCRYPTED, the payload size is already set.
-        if self._lzfse_payload_size is not None:
-            raise AttributeError('Unable to set LZFSE payload size more than once.')
-
-        if size is not None and not isinstance(size, int):
-            raise UnexpectedDataError('int', size)
-
-        # If the payload isn't LZFSE-compressed nor encrypted, the payload size can't be set.
-        if self.compression != Compression.LZFSE and self.encrypted == False:
-            raise CompressionError(
-                'Cannot set LZFSE payload size of non-LZFSE-compressed payload.'
-            )
-
-        self._lzfse_payload_size = size
+        self._data = AES.new(kbag.key, AES.MODE_CBC, kbag.iv).decrypt(self._data)
+        self._keybags = []
 
     def output(self) -> Payload:
         kbag_data = None
         if self.encrypted:
             self._encoder.start()
-            self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-
-            for kbag in self.keybags:
-                self._encoder.enter(asn1.Numbers.Sequence, asn1.Classes.Universal)
-                self._encoder.write(
-                    self.keybags.index(kbag) + 1,
-                    asn1.Numbers.Integer,
-                    asn1.Types.Primitive,
-                    asn1.Classes.Universal,
-                )
-                self._encoder.write(
-                    kbag.iv,
-                    asn1.Numbers.OctetString,
-                    asn1.Types.Primitive,
-                    asn1.Classes.Universal,
-                )
-                self._encoder.write(
-                    kbag.key,
-                    asn1.Numbers.OctetString,
-                    asn1.Types.Primitive,
-                    asn1.Classes.Universal,
-                )
-                self._encoder.leave()
+            with self._encoder.construct(asn1.Numbers.Sequence, asn1.Classes.Universal):
+                for kbag in self.keybags:
+                    with self._encoder.construct(
+                        asn1.Numbers.Sequence, asn1.Classes.Universal
+                    ):
+                        self._encoder.write(
+                            self.keybags.index(kbag) + 1,
+                            asn1.Numbers.Integer,
+                            asn1.Types.Primitive,
+                            asn1.Classes.Universal,
+                        )
+                        self._encoder.write(
+                            kbag.iv,
+                            asn1.Numbers.OctetString,
+                            asn1.Types.Primitive,
+                            asn1.Classes.Universal,
+                        )
+                        self._encoder.write(
+                            kbag.key,
+                            asn1.Numbers.OctetString,
+                            asn1.Types.Primitive,
+                            asn1.Classes.Universal,
+                        )
 
-            self._encoder.leave()
             kbag_data = self._encoder.output()
 
         return Payload(self._data, kbag_data)
```

### Comparing `pyimg4-0.8/pyimg4/errors.py` & `pyimg4-0.8.2/pyimg4/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, NoReturn, Union
+from typing import Any, Union
 
 from asn1 import Classes, Numbers, Tag
 
 
 class _PyIMG4Error(Exception):
     pass
 
@@ -12,29 +12,29 @@
 
 
 class CompressionError(_PyIMG4Error):
     pass
 
 
 class UnexpectedDataError(_PyIMG4Error, ValueError):
-    def __init__(self, expect: str, real: Any) -> NoReturn:
+    def __init__(self, expect: str, real: Any) -> None:
         if not isinstance(real, (float, int)) and len(real) > 15:
             real = f'<{type(real).__name__} with len of {len(real)}>'
 
         super().__init__(
-            f"Expected data: {expect}, got: {real.hex() if isinstance(real, bytes) else real}"
+            f'Expected data: {expect}, got: {real.hex() if isinstance(real, bytes) else real}'
         )
 
 
 class UnexpectedTagError(_PyIMG4Error, ValueError):
-    def __init__(self, tag: Tag, valid: Union[Classes, Numbers]) -> NoReturn:
+    def __init__(self, tag: Tag, valid: Union[Classes, Numbers]) -> None:
         try:
             tag_type = next(t.name for t in Numbers if t.value == tag.nr)
         except StopIteration:
             tag_type = f"{next(t.name for t in Classes if t.value == tag.cls)} {tag.nr if tag.cls == Classes.Private else ''}"
 
         if isinstance(valid, Numbers):
             expected_type = next(t.name for t in Numbers if t.value == valid)
         if isinstance(valid, Classes):
             expected_type = next(t.name for t in Classes if t.value == tag.cls)
 
-        super().__init__(f"Expected tag of type {expected_type}, got {tag_type}")
+        super().__init__(f'Expected tag of type {expected_type}, got {tag_type}')
```

### Comparing `pyimg4-0.8/pyproject.toml` & `pyimg4-0.8.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyimg4"
-version = "0.8"
+version = "0.8.2"
 description = "A Python library/CLI tool for parsing Apple's Image4 format."
 authors = ["m1stadev <adamhamdi31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/m1stadev/PyIMG4"
 keywords = ["ios", "jailbreak", "iboot", "img4", "image4"]
 classifiers = [
@@ -21,34 +21,36 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 asn1 = "^2.7.0"
 click = "^8.1.7"
 pycryptodome = "^3.18.0"
 pyliblzfse = {version = "^0.4.1", optional = true}
-pylzss = {version = "^0.3.1", optional = true}
+pylzss = {version = "^0.3.4", optional = true}
+apple-compress = {version = "^0.2.3", optional = true}
 
 [tool.poetry.extras]
-compression = ["pyliblzfse", "pylzss"]
+compression = ["apple-compress", "pyliblzfse", "pylzss"]
 
 [tool.poetry.dev-dependencies]
-black = "^23.7.0"
-isort = "^5.12.0"
 pytest = "^7.4.0"
 remotezip = "^0.12.1"
 
-[tool.black]
-skip-string-normalization = true
-
-[tool.isort]
-profile = "black"
-src_paths = ["examples", "pyimg4", "tests"]
-
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
+[tool.ruff]
+target-version = "py38"
+
+[tool.ruff.lint]
+extend-select = ["I"]
+ignore = ["E722"]
+
+[tool.ruff.format]
+quote-style = "single"
+
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/m1stadev/PyIMG4/issues"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyimg4-0.8/PKG-INFO` & `pyimg4-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimg4
-Version: 0.8
+Version: 0.8.2
 Summary: A Python library/CLI tool for parsing Apple's Image4 format.
 Home-page: https://github.com/m1stadev/PyIMG4
 License: MIT
 Keywords: ios,jailbreak,iboot,img4,image4
 Author: m1stadev
 Author-email: adamhamdi31@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,21 +14,23 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Provides-Extra: compression
+Requires-Dist: apple-compress (>=0.2.3,<0.3.0) ; extra == "compression"
 Requires-Dist: asn1 (>=2.7.0,<3.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: pyliblzfse (>=0.4.1,<0.5.0) ; extra == "compression"
-Requires-Dist: pylzss (>=0.3.1,<0.4.0) ; extra == "compression"
+Requires-Dist: pylzss (>=0.3.4,<0.4.0) ; extra == "compression"
 Project-URL: Bug Tracker, https://github.com/m1stadev/PyIMG4/issues
 Project-URL: Repository, https://github.com/m1stadev/PyIMG4
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src=".github/assets/icon.png" alt="https://github.com/m1stadev/PyIMG4" width=256px> 
 </p>
@@ -40,15 +42,15 @@
   <a href="https://github.com/m1stadev/PyIMG4/blob/master/LICENSE">
     <image src="https://img.shields.io/github/license/m1stadev/PyIMG4">
   </a>
   <a href="https://github.com/m1stadev/PyIMG4/stargazers">
     <image src="https://img.shields.io/github/stars/m1stadev/PyIMG4">
   </a>
   <a href="https://github.com/m1stadev/PyIMG4">
-    <image src="https://img.shields.io/tokei/lines/github/m1stadev/PyIMG4">
+    <image src="https://tokei.rs/b1/github/m1stadev/PyIMG4?category=code&lang=python&style=flat">
   </a>
   <a href="https://github.com/m1stadev/PyIMG4">
     <image src="https://img.shields.io/github/actions/workflow/status/m1stadev/PyIMG4/.github/workflows/python-tests.yml">
   </a>
     <br>
 </p>
 
@@ -60,37 +62,32 @@
 ```
 Usage: pyimg4 [OPTIONS] COMMAND [ARGS]...
 
   A Python CLI tool for parsing Apple's Image4 format.
 
 Options:
   --version  Show the version and exit.
-  --help     Show this message and exit.
+  -h, --help     Show this message and exit.
 
 Commands:
   im4m  Image4 manifest commands.
   im4p  Image4 payload commands.
   im4r  Image4 restore info commands.
   img4  Image4 commands.
 ```
 
 ## Requirements
 - Python 3.8 or higher
-- Python development headers (`python3-dev` on Debian-based OSes)
 
 ## Installation
 - Install from [PyPI](https://pypi.org/project/pyimg4/):
     - ```python3 -m pip install pyimg4```
-    - If you would like to use the compression features of PyIMG4, install the required libraries:
+    - If you would like to use the compression features of PyIMG4, install the optional libraries:
       - ```python3 -m pip install pyimg4[compression]```
 - Local installation:
     - `./install.sh`
     - Requires [Poetry](https://python-poetry.org)
 
-## TODO
-- Write documentation
-- Add logging
-
 ## Support
 
 For any questions/issues you have, [open an issue](https://github.com/m1stadev/PyIMG4/issues) or join my [Discord](https://m1sta.xyz/discord).
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: pyimg4 Version: 0.8 Summary: A Python library/CLI
+Metadata-Version: 2.1 Name: pyimg4 Version: 0.8.2 Summary: A Python library/CLI
 tool for parsing Apple's Image4 format. Home-page: https://github.com/m1stadev/
 PyIMG4 License: MIT Keywords: ios,jailbreak,iboot,img4,image4 Author: m1stadev
 Author-email: adamhamdi31@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Utilities Provides-Extra: compression
-Requires-Dist: asn1 (>=2.7.0,<3.0.0) Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: pycryptodome (>=3.18.0,<4.0.0) Requires-Dist: pyliblzfse
-(>=0.4.1,<0.5.0) ; extra == "compression" Requires-Dist: pylzss
-(>=0.3.1,<0.4.0) ; extra == "compression" Project-URL: Bug Tracker, https://
-github.com/m1stadev/PyIMG4/issues Project-URL: Repository, https://github.com/
-m1stadev/PyIMG4 Description-Content-Type: text/markdown
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Topic :: Utilities Provides-Extra: compression Requires-Dist: apple-compress
+(>=0.2.3,<0.3.0) ; extra == "compression" Requires-Dist: asn1 (>=2.7.0,<3.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist: pycryptodome
+(>=3.18.0,<4.0.0) Requires-Dist: pyliblzfse (>=0.4.1,<0.5.0) ; extra ==
+"compression" Requires-Dist: pylzss (>=0.3.4,<0.4.0) ; extra == "compression"
+Project-URL: Bug Tracker, https://github.com/m1stadev/PyIMG4/issues Project-
+URL: Repository, https://github.com/m1stadev/PyIMG4 Description-Content-Type:
+text/markdown
                      [https://github.com/m1stadev/PyIMG4]
                              ************ PPyyIIMMGG44 ************
 
          A Python library/CLI tool for parsing Apple's _I_m_a_g_e_4_ _f_o_r_m_a_t.
 ## Usage ``` Usage: pyimg4 [OPTIONS] COMMAND [ARGS]... A Python CLI tool for
-parsing Apple's Image4 format. Options: --version Show the version and exit. --
-help Show this message and exit. Commands: im4m Image4 manifest commands. im4p
-Image4 payload commands. im4r Image4 restore info commands. img4 Image4
-commands. ``` ## Requirements - Python 3.8 or higher - Python development
-headers (`python3-dev` on Debian-based OSes) ## Installation - Install from
-[PyPI](https://pypi.org/project/pyimg4/): - ```python3 -m pip install pyimg4```
-- If you would like to use the compression features of PyIMG4, install the
-required libraries: - ```python3 -m pip install pyimg4[compression]``` - Local
-installation: - `./install.sh` - Requires [Poetry](https://python-poetry.org)
-## TODO - Write documentation - Add logging ## Support For any questions/issues
-you have, [open an issue](https://github.com/m1stadev/PyIMG4/issues) or join my
-[Discord](https://m1sta.xyz/discord).
+parsing Apple's Image4 format. Options: --version Show the version and exit. -
+h, --help Show this message and exit. Commands: im4m Image4 manifest commands.
+im4p Image4 payload commands. im4r Image4 restore info commands. img4 Image4
+commands. ``` ## Requirements - Python 3.8 or higher ## Installation - Install
+from [PyPI](https://pypi.org/project/pyimg4/): - ```python3 -m pip install
+pyimg4``` - If you would like to use the compression features of PyIMG4,
+install the optional libraries: - ```python3 -m pip install pyimg4
+[compression]``` - Local installation: - `./install.sh` - Requires [Poetry]
+(https://python-poetry.org) ## Support For any questions/issues you have, [open
+an issue](https://github.com/m1stadev/PyIMG4/issues) or join my [Discord]
+(https://m1sta.xyz/discord).
```

