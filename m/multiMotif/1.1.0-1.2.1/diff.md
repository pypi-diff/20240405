# Comparing `tmp/multiMotif-1.1.0.tar.gz` & `tmp/multiMotif-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiMotif-1.1.0.tar", last modified: Sun Feb  4 09:11:58 2024, max compression
+gzip compressed data, was "multiMotif-1.2.1.tar", last modified: Fri Apr  5 04:44:50 2024, max compression
```

## Comparing `multiMotif-1.1.0.tar` & `multiMotif-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 09:11:58.355072 multiMotif-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-04 09:11:49.000000 multiMotif-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-02-04 09:11:58.355072 multiMotif-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-02-04 09:11:49.000000 multiMotif-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 09:11:58.351072 multiMotif-1.1.0/multiMotif/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 09:11:49.000000 multiMotif-1.1.0/multiMotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54152 2024-02-04 09:11:49.000000 multiMotif-1.1.0/multiMotif/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 09:11:58.351072 multiMotif-1.1.0/multiMotif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-02-04 09:11:58.000000 multiMotif-1.1.0/multiMotif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-04 09:11:58.000000 multiMotif-1.1.0/multiMotif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 09:11:58.000000 multiMotif-1.1.0/multiMotif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-04 09:11:58.000000 multiMotif-1.1.0/multiMotif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-04 09:11:58.000000 multiMotif-1.1.0/multiMotif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-04 09:11:58.000000 multiMotif-1.1.0/multiMotif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 09:11:58.355072 multiMotif-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-04 09:11:49.000000 multiMotif-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:44:50.887712 multiMotif-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 04:44:41.000000 multiMotif-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-05 04:44:50.887712 multiMotif-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-04-05 04:44:41.000000 multiMotif-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:44:50.887712 multiMotif-1.2.1/multiMotif/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 04:44:41.000000 multiMotif-1.2.1/multiMotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71656 2024-04-05 04:44:41.000000 multiMotif-1.2.1/multiMotif/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:44:50.887712 multiMotif-1.2.1/multiMotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 04:44:50.000000 multiMotif-1.2.1/multiMotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:44:50.887712 multiMotif-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-05 04:44:41.000000 multiMotif-1.2.1/setup.py
```

### Comparing `multiMotif-1.1.0/LICENSE` & `multiMotif-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multiMotif-1.1.0/PKG-INFO` & `multiMotif-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: multiMotif
-Version: 1.1.0
+Version: 1.2.1
 Summary: A Computational Tool for Variable Motif scanning and Sequence-based Relative Position Visualization of Search Results in Sequences.
-Home-page: https://github.com/Sienna-L/multiMotif
+Home-page: https://github.com/SainanLuo/multiMotif
 Author: Sainan Luo
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython>=1.78
 Requires-Dist: matplotlib>=3.3
 Requires-Dist: numpy>=1.19
 Requires-Dist: pandas>=1.1
+Requires-Dist: plotly>=5.18.0
 
 # VariaMotif
  Scanning and visualization for variable gap motifs.
 
 ## Installation
 
 To install VariaMotif, you can use [pip](https://pip.pypa.io/en/stable/installation/):
```

### Comparing `multiMotif-1.1.0/README.md` & `multiMotif-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `multiMotif-1.1.0/multiMotif/main.py` & `multiMotif-1.2.1/multiMotif/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,196 +1,119 @@
 import argparse
-from Bio import SeqIO
+from itertools import groupby
 import multiprocessing
-import pandas as pd
-import matplotlib
-matplotlib.use('Agg')  # Set non-interactive backend to prevent X11 window creation
-import matplotlib.pyplot as plt
-import numpy as np
-from matplotlib.patches import Patch
-from Bio.SeqRecord import SeqRecord
-import math
 from concurrent.futures import ProcessPoolExecutor, as_completed
-from itertools import groupby
+import math
 import csv
 
-def get_extract_sequences_args(parser):
-    parser.add_argument("-fna", "--fna", type=str, help="Input a FASTA file such genome sequence")
-    parser.add_argument("-gff", "--gff", type=str, help="Input a annotation file, such as a .gff")
-    parser.add_argument("-up", "--upstream", dest="upstream", type=int, default=400, help="For the promoter option: specify the upstream length from gene start location (optional, default is 400)")
-    parser.add_argument("-down", "--downstream", dest="downstream", type=int, default=0, help="For promoter option: specify the downstream length from gene start location  (optional, default is 0)")
-    parser.add_argument("--promoter", dest="promoter", action="store_true", help="Extract promoter sequences")
-    parser.add_argument("--orf", dest="orf", action="store_true", help="Extract ORF sequences")
-    parser.add_argument('-o', '--output', type=str, help='Output sequence file')
+import numpy as np
+import pandas as pd
+from Bio.SeqRecord import SeqRecord
+from Bio import SeqIO
+import plotly.graph_objects as go
+from plotly.subplots import make_subplots
 
-def get_single_args(parser):
+def get_singleMotif_args(parser):
     single = parser.add_argument_group("Option for single motif scanning")
     single.add_argument('-f', '--fasta', type=str, help='Input FASTA file containing sequences for motif scanning')
     single.add_argument('-motif', type=str, help='Input motif sequences')
     single.add_argument('-m', '--mismatches', default=0, type=int, help='Maximum allowed mismatches motif scanning. Default is 0')
     single.add_argument('-d', '--direction', type=str, default='+', choices=['+,-', '+', '-'], help='Search direction: both, forward (default), or reverse')
     single.add_argument('-o', '--output_dir', type=str, help='Output directory for result files')
 
-    motif_display = parser.add_argument_group("Options for motif display")
-    motif_display.add_argument('-i', '--image', action="store_true", help='Display motif in sequence: Default is not to display.')
-    motif_display.add_argument('-r', '--display_both_directions', action='store_true', help='Display motifs from both + and - strands.Default is the forward strand (+).')
-
-    # Variable motif type arguments
     motif_group = parser.add_argument_group("Motif Type")
     motif_group.add_argument('-DNA', action="store_true", help="Search for DNA motifs")
     motif_group.add_argument('-RNA', action="store_true", help="Search for RNA motifs")
     motif_group.add_argument('-protein', action="store_true", help="Search for protein motifs")
 
+    motif_display = parser.add_argument_group("Options for motif display")
+    motif_display.add_argument('-i', '--image', action="store_true", help='Display motif in sequence: Default is not to display.')
+    motif_display.add_argument('-r', '--display_both_directions', action='store_true', help='Display motifs from both + and - strands.Default is the forward strand (+).')
+    motif_display.add_argument("-gff", "--gff", type=str, help="Input a annotation file, such as a .gff")
+    motif_display.add_argument("-motif_up", "--motif_up", dest="motif_up", type=int, default=2000, help="For the promoter option: specify the upstream length from motif start location (optional, default is 2000)")
+    motif_display.add_argument("-motif_down", "--motif_down", dest="motif_down", type=int, default=2000, help="For promoter option: specify the downstream length from motif end location  (optional, default is 2000)")    
+
     fimo = parser.add_argument_group("Compare with fimo result")
-    fimo.add_argument("-fimo_path", "--fimo_path", type=str, default=False, help="Path to Fimo result file (e.g., /path/to/fimo.tsv).")
+    fimo.add_argument("-fimo_path", "--fimo_path", type=str, help="Path to Fimo result file (e.g., /path/to/fimo.tsv).")
 
-def get_multiple_args(parser):
+def get_multiMotif_args(parser):
     parser.add_argument('-l', '--motiflist', type=str, help='Input file containing motifs list in order')
     parser.add_argument('-f', '--fasta', type=str, help='Input FASTA file containing sequences for motif scanning')
+    parser.add_argument('-m', '--mismatches', type=int, help='Maximum allowed mismatches for complete motif. Default is equal to the sum of submotif mismatches.')
     parser.add_argument('-d', '--direction', type=str, default='+', choices=['+,-', '+', '-'], help='Search direction: both, forward (default), or reverse')
     parser.add_argument('-n', '--mis_motif_nums', default=0, type=int, help='Allow how many motifs could be lost')
-    
-    motif_display = parser.add_argument_group("Options for motif display")
-    motif_display.add_argument('-i', '--image', action="store_true", help='Display motif in sequence: Default is not to display.')
-    motif_display.add_argument('-r', '--display_both_directions', action='store_true', help='Display motifs from both + and - strands.Default is the forward strand (+).')
+    parser.add_argument("-necessary", "--necessary", type=str, help="A file: a comma-separated line containing all required motifs.Not set by default")
+
 
-    # Variable motif type arguments
     motif_group = parser.add_argument_group("Motif Type")
     motif_group.add_argument('-DNA', action="store_true", help="Search for DNA motifs")
     motif_group.add_argument('-RNA', action="store_true", help="Search for RNA motifs")
     motif_group.add_argument('-protein', action="store_true", help="Search for protein motifs")
 
-    parser.add_argument('-o', '--output_dir', type=str, help='Output directory for result files')
-
-def get_regulator_args(parser):
-    parser.add_argument('-f', '--fasta', type=str, help='Input FASTA file containing sequences for motif scanning')
-    parser.add_argument('-motif1', type=str, help='Input motif1 sequence')
-    parser.add_argument('-m1', '--mismatch1', default=0, type=int, help='Maximum allowed mismatches for -motif1. Default is 0')
-    parser.add_argument('-motif2', default="None", type=str, help='Input motif1 sequence. Default is "None"')
-    parser.add_argument('-m2', '--mismatch2', default=0, type=int, help='Maximum allowed mismatches for -motif2. Default is 0')
-    parser.add_argument('-m', '--mismatches', default=0, type=int, help='Maximum allowed mismatches for complete motif. Default is equal to the sum of submotif mismatches.')
-    parser.add_argument('-min_g', '--min_gap', default=0, type=int, help='Minimum gap length between motif1 and motif2. Default is 0')
-    parser.add_argument('-max_g', '--max_gap', default=50, type=int, help='Maximum gap length between motif1 and motif2. Default is 50')
-    parser.add_argument('-d', '--direction', type=str, default='+', choices=['+,-', '+', '-'], help='Search direction: both, forward (default), or reverse')    
-
     motif_display = parser.add_argument_group("Options for motif display")
     motif_display.add_argument('-i', '--image', action="store_true", help='Display motif in sequence: Default is not to display.')
     motif_display.add_argument('-r', '--display_both_directions', action='store_true', help='Display motifs from both + and - strands.Default is the forward strand (+).')
+    motif_display.add_argument("-gff", "--gff", type=str, help="Input a annotation file, such as a .gff")
+    motif_display.add_argument("-motif_up", "--motif_up", dest="motif_up", type=int, default=2000, help="For the promoter option: specify the upstream length from motif start location (optional, default is 2000)")
+    motif_display.add_argument("-motif_down", "--motif_down", dest="motif_down", type=int, default=2000, help="For promoter option: specify the downstream length from motif end location  (optional, default is 2000)")
+
+    regulator_group = parser.add_argument_group("regulator")
+    regulator_group.add_argument("--regulator", dest="regulator", action="store_true", help="Choose to scan regultor variable gap motifs")
+    regulator_group.add_argument('-min_g', '--min_gap', default=0, type=int, help='Minimum gap length between motif1 and motif2. Default is 0')
+    regulator_group.add_argument('-max_g', '--max_gap', default=50, type=int, help='Maximum gap length between motif1 and motif2. Default is 50')
 
-    # Variable motif type arguments
-    motif_group = parser.add_argument_group("Motif Type")
-    motif_group.add_argument('-DNA', action="store_true", help="Search for DNA motifs")
-    motif_group.add_argument('-RNA', action="store_true", help="Search for RNA motifs")
-    motif_group.add_argument('-protein', action="store_true", help="Search for protein motifs")
-
-    # Output arguments
-    parser.add_argument('-o', '--output_dir', type=str, help='Output file for motif scanning result and Output file prefix for display')
+    parser.add_argument('-o', '--output_dir', type=str, help='Output directory for result files')
 
-def get_VisualMotif_args(parser):
+def get_visualMotif_args(parser):
     parser.add_argument('-t', '--table', dest='table_file', help='Input table file')
     parser.add_argument('-r', '--display_both_directions', action='store_true', help='Display motifs from both + and - strands.Default is the forward strand (+).')
     parser.add_argument('-o', '--output_dir', type=str, help='Output directory for result files')
 
+    genome_group = parser.add_argument_group("gene_display")
+    genome_group.add_argument("-gff", "--gff", type=str, help="Input a annotation file, such as a .gff")
+    genome_group.add_argument("-motif_up", "--motif_up", dest="motif_up", type=int, default=2000, help="For the promoter option: specify the upstream length from motif start location (optional, default is 2000)")
+    genome_group.add_argument("-motif_down", "--motif_down", dest="motif_down", type=int, default=2000, help="For promoter option: specify the downstream length from motif end location  (optional, default is 2000)")
+
+def get_extract_sequences_args(parser):
+    parser.add_argument("-fna", "--fna", type=str, help="Input a FASTA file containing the genome sequence")
+    parser.add_argument("-gff", "--gff", type=str, help="Input a annotation file(.gff)")
+    parser.add_argument("-up", "--upstream", dest="upstream", type=int, default=400, help="For the promoter option: specify the upstream length from gene start location (optional, default is 400)")
+    parser.add_argument("-down", "--downstream", dest="downstream", type=int, default=0, help="For promoter option: specify the downstream length from gene start location  (optional, default is 0)")
+    parser.add_argument("--promoter", dest="promoter", action="store_true", help="Extract promoter sequences")
+    parser.add_argument("--orf", dest="orf", action="store_true", help="Extract ORF sequences")
+    parser.add_argument('-o', '--output', type=str, help='Output sequence file')
+
 def get_args():
     parser = argparse.ArgumentParser(description='VariaMotif for motif scanning')
-
-    # Create subparsers
     subparsers = parser.add_subparsers(help='sub-command help')
 
-    # Subparser for extract_sequences
+    singleMotif_parser = subparsers.add_parser('singleMotif', help='Scanning for single motif')
+    get_singleMotif_args(singleMotif_parser)
+    singleMotif_parser.set_defaults(func=singleMotif_function)
+
+    multiMotif_parser = subparsers.add_parser('multiMotif', help='Scanning more than two ordered motifs')
+    get_multiMotif_args(multiMotif_parser)
+    multiMotif_parser.set_defaults(func=multiMotif_function)
+
+    visualMotif_parser = subparsers.add_parser('visualMotif', help='Visualization:display motif in sequence')
+    get_visualMotif_args(visualMotif_parser)
+    visualMotif_parser.set_defaults(func=visualMotif_function)
+
     extract_sequences_parser = subparsers.add_parser('extract_sequences', help='Extract Sequences')
     get_extract_sequences_args(extract_sequences_parser)
     extract_sequences_parser.set_defaults(func=extract_sequences_function)
 
-    # Subparser for fix
-    single_parser = subparsers.add_parser('single', help='Scanning for single motif')
-    get_single_args(single_parser)
-    single_parser.set_defaults(func=single_function)
-
-    # Subparser for variable
-    regulator_parser = subparsers.add_parser('regulator', help='Scanning for regultor variable gap motifs')
-    get_regulator_args(regulator_parser)
-    regulator_parser.set_defaults(func=regulator_function)
-
-    # Subparser for manyMotifs
-    multiple_parser = subparsers.add_parser('multiple', help='Scanning more than two ordered motifs')
-    get_multiple_args(multiple_parser)
-    multiple_parser.set_defaults(func=multiple_function)
-
-    # Subparser for VisualMotif
-    VisualMotif_parser = subparsers.add_parser('VisualMotif', help='Visualization:display motif in sequence')
-    get_VisualMotif_args(VisualMotif_parser)
-    VisualMotif_parser.set_defaults(func=VisualMotif_function)
-
-    # Parse the command line arguments
     args = parser.parse_args()
 
-    # Call the appropriate function based on the subparser
     if hasattr(args, 'func'):
         args.func(args)
     else:
-        # If no subcommand is provided, print the help message
         parser.print_help()
-    
-
-def extract_sequences_function(args):
-    if args.output is None:
-        raise ValueError("Output file path is required.")
-    sequences = SeqIO.to_dict(SeqIO.parse(args.fna, "fasta"))
-    # Open output file for writing
-    output_handle = open(args.output, "w")
-    # Process GFF file
-    with open(args.gff, "r") as gff_handle:
-        for line in gff_handle:
-            line = line.strip()
-            if line.startswith("#"):
-                continue
-            fields = line.split("\t")
-            feature_type = fields[2]
-            strand = fields[6]
-            if feature_type == "CDS":
-                seq_name = fields[0]
-                seq_start = int(fields[3])
-                seq_end = int(fields[4])
-                attributes = fields[8].split(";")
-                cds_id = parent = gene = product = "None"
-
-                for attr in attributes:
-                    if attr.startswith("ID="):
-                        cds_id = attr[3:]
-                    elif attr.startswith("Parent="):
-                        parent = attr[7:]
-                    elif attr.startswith("gene="):
-                        gene = attr[5:]
-                    elif attr.startswith("product="):
-                        product = attr[8:]
-                if seq_name in sequences:
-                    sequence = sequences[seq_name].seq
-                    if args.promoter:
-                        if strand == "-":
-                            start = max(seq_end - args.downstream, 0)
-                            end = start + args.upstream + args.downstream
-                            seq_fragment = sequence[start:end].reverse_complement()
-                        else:
-                            start = max(seq_start - args.upstream, 0)
-                            end = start + args.upstream + args.downstream
-                            seq_fragment = sequence[start:end]
-                    elif args.orf:
-                        if strand == "-":
-                            seq_fragment = sequence[seq_start - 1:seq_end].reverse_complement()
-                        else:
-                            seq_fragment = sequence[seq_start - 1:seq_end]
-                    else:
-                        continue
-                    seq_record = SeqRecord(seq_fragment, id=f"{seq_name}|{cds_id}|{parent}|{gene}|{seq_start}|{seq_end}|{strand}|{product}",description="")
-                    SeqIO.write(seq_record, output_handle, "fasta")
-    # Close output file
-    output_handle.close()
 
-def single_function(args):
+def singleMotif_function(args):
     fasta_file_path = args.fasta
     output_dir = args.output_dir
     all_results = []
     filtered_results = []
     motif = args.motif
     max_mismatches = args.mismatches
     direction = args.direction
@@ -220,15 +143,15 @@
     if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) < 500000:
         if direction == '+' or direction == '+,-':
             motif_results = pool.starmap(search_motif, [(record, motif, max_mismatches, len(motif)) for record in records])
             motif_results = [item for sublist in motif_results for item in sublist]
             all_results.extend(motif_results)
         if direction == '-' or direction == '+,-':
             motif_results = pool.starmap(reverse_search_fix, [(record, motif, max_mismatches, len(motif)) for record in records])
-            motif_results = [item for sublist in motif_results for item in sublist] #Flatten the list
+            motif_results = [item for sublist in motif_results for item in sublist]
             all_results.extend(motif_results)
         all_results = sorted(all_results, key=lambda x: (x['sequence_id'], x['start']))
 
         seen_positions = set()
         unique_positions = set()
         for result in all_results:
             key = (result['sequence_id'], result['start'])           
@@ -249,15 +172,15 @@
     else:
         with open(output_file_path1,'w') as output_file:
             output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tmismatches\tmatched_sequence\n")
             for result in filtered_results:
                 result['motif']=f"single_{result['motif']}"
                 output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\n")
     if args.image:
-        plot_motifs_to_single_chart(output_file_path1, output_file_path1, display_both_directions=args.display_both_directions)
+        plot_motifs_to_single_chart(output_file_path1, output_file_path1, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
 
     fimo_results=[]
     fimo_results_filter=[]
     if args.fimo_path:
         output_file_path2 = f"{output_dir}/fimo.out"
         records = list(SeqIO.parse(fasta_file_path, "fasta"))
         file_path=args.fimo_path
@@ -304,18 +227,18 @@
                 unique_positions.add(key)
                 fimo_results_filter.append(result)
 
         if not fimo_results_filter:
             print("#No Result")
         else:
             with open(output_file_path2,'w') as output_file:
-                output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tmismatches\tmatched_sequence\n")
+                output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tp-value\tq-value\tmatched_sequence\n")
                 for result in fimo_results_filter:
                     output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['p-value']}\t{result['q-value']}\t{result['fragment']}\n")
-        plot_motifs_to_single_chart(output_file_path2, output_file_path2, display_both_directions=args.display_both_directions)
+        plot_motifs_to_single_chart(output_file_path2, output_file_path2, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
 
         output_file_path3 = f"{output_dir}/merge.out"
         merged_results = []
         seen_keys = set()
         for result in filtered_results:
             key = f"{result['sequence_id']}_{result['sequence_length']}_{result['start']}_{result['end']}_{result['strand']}"
             if key not in seen_keys:
@@ -331,194 +254,258 @@
                     if all(str(merged_result[k]) == str(result[k]) for k in ('sequence_id', 'sequence_length', 'start', 'end', 'strand')):
                         merged_result['motif'] = merged_result['motif'].replace('single', 'both')
 
         with open(output_file_path3,'w') as output_file:
             output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\n")
             for result in merged_results:
                 output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\n")
-        plot_motifs_to_single_chart(output_file_path3, output_file_path3, display_both_directions=args.display_both_directions)
+        plot_motifs_to_single_chart(output_file_path3, output_file_path3, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
 
-def multiple_function(args):
-    fasta_file_path = args.fasta
-    motiflist = args.motiflist
-    direction = args.direction
-    output_dir = args.output_dir
-    n=args.mis_motif_nums
-    pool = multiprocessing.Pool(multiprocessing.cpu_count())
-    records = list(SeqIO.parse(fasta_file_path, "fasta"))
-    all_results = []
-    motif_results_pre = []
-    output_file_path1 = f"{output_dir}/multiMotifs_list.out"
-    output_file_path2 = f"{output_dir}/multiMotifs_statistics.out"    
+def multiMotif_function(args):
+    if not args.regulator:
+        fasta_file_path = args.fasta
+        motiflist = args.motiflist
+        direction = args.direction
+        output_dir = args.output_dir
+        n=args.mis_motif_nums
+        pool = multiprocessing.Pool(multiprocessing.cpu_count())
+        records = list(SeqIO.parse(fasta_file_path, "fasta"))
+        all_results = []
+        motif_results_pre = []
+        output_file_path1 = f"{output_dir}/multiMotifs_list.out"
+        output_file_path2 = f"{output_dir}/multiMotifs_statistics.out"    
 
-    with open(motiflist, 'r') as file:
-        line_count = sum(1 for line in file)
-    if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) >= 500000:
         with open(motiflist, 'r') as file:
-            for line_number, line in enumerate(file, start=1):
-                motif = line.strip().split('\t')[0]
-                max_mismatches = int(line.strip().split('\t')[1])
-                if direction == '+' or direction == '+,-':  
-                    motif_results_pre = process_genome_file_forward(fasta_file_path, motif, max_mismatches)
-                    for result in motif_results_pre:
-                        result['motif_type'] = line_number
-                    all_results.extend(motif_results_pre)
-                if direction == '-' or direction == '+,-':
-                    motif_results_pre = process_genome_file_reverse(fasta_file_path, motif, max_mismatches)
-                    for result in motif_results_pre:
-                        result['motif_type'] = line_number
-                    all_results.extend(motif_results_pre)
-        all_results = sorted(all_results, key=lambda x: (x['motif_type'], x['sequence_id'], x['start']))
-    if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) < 500000:
-        with open(motiflist, 'r') as file:
-            for line_number, line in enumerate(file, start=1):
-                motif = line.strip().split('\t')[0]
-                max_mismatches = int(line.strip().split('\t')[1])
-                if direction == '+' or direction == '+,-':
-                    motif_results = pool.starmap(search_motif, [(record, motif, max_mismatches, len(motif)) for record in records])
+            line_count = sum(1 for line in file)
+        if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) >= 500000:
+            with open(motiflist, 'r') as file:
+                for line_number, line in enumerate(file, start=1):
+                    motif = line.strip().split('\t')[0]
+                    max_mismatches = int(line.strip().split('\t')[1])
+                    if direction == '+' or direction == '+,-':  
+                        motif_results_pre = process_genome_file_forward(fasta_file_path, motif, max_mismatches)
+                        for result in motif_results_pre:
+                            result['motif_type'] = line_number
+                        all_results.extend(motif_results_pre)
+                    if direction == '-' or direction == '+,-':
+                        motif_results_pre = process_genome_file_reverse(fasta_file_path, motif, max_mismatches)
+                        for result in motif_results_pre:
+                            result['motif_type'] = line_number
+                        all_results.extend(motif_results_pre)
+            all_results = sorted(all_results, key=lambda x: (x['motif_type'], x['sequence_id'], x['start']))
+
+        if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) < 500000:
+            with open(motiflist, 'r') as file:
+                for line_number, line in enumerate(file, start=1):
+                    motif = line.strip().split('\t')[0]
+                    max_mismatches = int(line.strip().split('\t')[1])
+                    if direction == '+' or direction == '+,-':
+                        motif_results = pool.starmap(search_motif, [(record, motif, max_mismatches, len(motif)) for record in records])
+                        motif_results = [item for sublist in motif_results for item in sublist]
+                        for result in motif_results:
+                            result['motif_type'] = line_number
+                        all_results.extend(motif_results)
+                    if direction == '-' or direction == '+,-':
+                        motif_results = pool.starmap(reverse_search_fix, [(record, motif, max_mismatches, len(motif)) for record in records])
+                        motif_results = [item for sublist in motif_results for item in sublist]
+                        for result in motif_results:
+                            result['motif_type'] = line_number
+                        all_results.extend(motif_results)
+            all_results = sorted(all_results, key=lambda x: (x['motif_type'], x['sequence_id'], x['start']))
+        if args.protein:
+            with open(motiflist, 'r') as file:
+                for line_number, line in enumerate(file, start=1):
+                    motif = line.strip().split('\t')[0]
+                    max_mismatches = int(line.strip().split('\t')[1])
+                    motif_results = pool.starmap(search_motif_protein, [(record, motif, max_mismatches, len(motif)) for record in records])
                     motif_results = [item for sublist in motif_results for item in sublist]
                     for result in motif_results:
                         result['motif_type'] = line_number
                     all_results.extend(motif_results)
-                if direction == '-' or direction == '+,-':
-                    motif_results = pool.starmap(reverse_search_fix, [(record, motif, max_mismatches, len(motif)) for record in records])
-                    motif_results = [item for sublist in motif_results for item in sublist] #Flatten the list
-                    for result in motif_results:
-                        result['motif_type'] = line_number
-                    all_results.extend(motif_results)
-        all_results = sorted(all_results, key=lambda x: (x['motif_type'], x['sequence_id'], x['start']))
-    if args.protein:
-        with open(motiflist, 'r') as file:
-            for line_number, line in enumerate(file, start=1):
-                motif = line.strip().split('\t')[0]
-                max_mismatches = int(line.strip().split('\t')[1])
-                motif_results = pool.starmap(search_motif_protein, [(record, motif, max_mismatches, len(motif)) for record in records])
-                motif_results = [item for sublist in motif_results for item in sublist]
-                for result in motif_results:
-                    result['motif_type'] = line_number
-                all_results.extend(motif_results)
-        all_results = sorted(all_results, key=lambda x: (x['motif_type'], x['sequence_id'], x['start']))
-    if not all_results:
-        print("#No Result")
-    else:
-        with open(output_file_path1,'w') as output_file:
-            output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tmismatches\tmatched_sequence\tmotif_type\n")
-            for result in all_results:
-                output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\t{result['motif_type']}\n")
+            all_results = sorted(all_results, key=lambda x: (x['motif_type'], x['sequence_id'], x['start']))
+        if not all_results:
+            print("#No Result")
+        else:
+            with open(output_file_path1,'w') as output_file:
+                output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tmismatches\tmatched_sequence\tmotif_type\n")
+                for result in all_results:
+                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\t{result['motif_type']}\n")
 
-    filtered_results = []
-    seen_positions = set()
-    unique_positions = set()
+        filtered_results = []
+        seen_positions = set()
+        unique_positions = set()
 
-    for result in all_results:
-        key = (result['sequence_id'], result['start'], result['motif_type'])
-    
-        if key not in seen_positions and result['strand'] == '+':
-            seen_positions.add(key)
-            filtered_results.append(result)
-        elif key not in seen_positions:
-            unique_positions.add(key)
-            filtered_results.append(result)
-
-    motif_nums = line_count - n
-    manyMotifs_results = []
-    filtered_results_sorted = sorted(filtered_results, key=lambda x: x['sequence_id'])
-
-    grouped_results = groupby(filtered_results_sorted, key=lambda x: x['sequence_id'])
-    grouped_results_list = [(key,list(group)) for key, group in grouped_results]
-    manyMotifs_results_pre1 = pool.starmap(filter_rows, [(group, motif_nums) for key, group in grouped_results_list])
-    manyMotifs_results_pre2 = [item for sublist in manyMotifs_results_pre1 if sublist is not None for item in sublist]
-    manyMotifs_results.extend(manyMotifs_results_pre2)
-    manyMotifs_results = sorted(manyMotifs_results, key=lambda x: x['sequence_id'])
-    
-    if not manyMotifs_results:
-        print("#No Result")
-    else:
-        with open(output_file_path2,'w') as output_file:
-            output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tmismatches\tmatched_sequence\tmotif_type\n")
-            for result in manyMotifs_results:
-                output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\t{result['motif_type']}\n")
+        for result in all_results:
+            key = (result['sequence_id'], result['start'], result['motif_type'])
+        
+            if key not in seen_positions and result['strand'] == '+':
+                seen_positions.add(key)
+                filtered_results.append(result)
+            elif key not in seen_positions:
+                unique_positions.add(key)
+                filtered_results.append(result)
 
-    if args.image:
-        plot_motifs_to_single_chart(output_file_path2, output_file_path2, display_both_directions=args.display_both_directions)
+        motif_nums = line_count - n
+        manyMotifs_results = []
 
-def regulator_function(args):
-    fasta_file_path = args.fasta
-    motif1 = args.motif1
-    motif2 = args.motif2
-    max_mismatch1 = args.mismatch1
-    max_mismatch2 = args.mismatch2
-    min_gap = args.min_gap
-    max_gap = args.max_gap
-    direction = args.direction
-    pool = multiprocessing.Pool(multiprocessing.cpu_count())
-    records = list(SeqIO.parse(fasta_file_path, "fasta"))
-    all_results = []
-    output_dir = args.output_dir    
-    output_file_path = f"{output_dir}/regulator_variable_gap.out"
+        filtered_results_sorted = sorted(filtered_results, key=lambda x: (x['sequence_id'],x['start']))
+        grouped_results = groupby(filtered_results_sorted, key=lambda x: x['sequence_id'])
+        grouped_results_list = [(key,list(group)) for key, group in grouped_results]
+        manyMotifs_results_pre1 = pool.starmap(filter_rows, [(group, motif_nums,line_count,args.necessary) for key, group in grouped_results_list])
+        manyMotifs_results_pre2 = [item for sublist in manyMotifs_results_pre1 if sublist is not None for item in sublist]    
+        manyMotifs_results.extend(manyMotifs_results_pre2)
+        manyMotifs_results= [item for sublist in manyMotifs_results if sublist is not None for item in sublist]
+        manyMotifs_results = sorted(manyMotifs_results, key=lambda x: x['sequence_id'])
+        
+        if not manyMotifs_results:
+            print("#No Result")
+        else:
+            with open(output_file_path2,'w') as output_file:
+                output_file.write("Sequence_ID\tSequence_Length\tmotif\tstart\tend\tstrand\tmismatches\tmatched_sequence\tmotif_type\n")
+                for result in manyMotifs_results:
+                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['mismatches']}\t{result['fragment']}\t{result['motif_type']}\n")
 
-    if args.mismatches is None:
-        args.mismatches = max_mismatch1 + max_mismatch2
-        max_mismatches = args.mismatches
-    else:
-        max_mismatches = args.mismatches
+        if args.image:
+            plot_motifs_to_single_chart(output_file_path2, output_file_path2, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
 
-    if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) >= 5000:
-        if direction == '+' or direction == '+,-':  
-            motif1_results_pre = process_genome_file_forward(fasta_file_path, motif1, max_mismatch1)
-            motif1_results = sorted(motif1_results_pre, key=lambda x: (x['seq_name'], x['start']))
-            motif2_results_pre = process_genome_file_forward(fasta_file_path, motif2, max_mismatch2)
-            motif2_results = sorted(motif2_results_pre, key=lambda x: (x['seq_name'], x['start']))
-            num_chunks = multiprocessing.cpu_count()
-            chunk_size = max(len(motif1_results) // num_chunks,1)
-            chunks = [motif1_results[i:i + chunk_size] for i in range(0, len(motif1_results), chunk_size)]
-                
-            for record in records:
-                combined_results = pool.starmap(combine_results_forward, [(record, motif1_results_chunk, motif2_results, max_mismatches, min_gap, max_gap) for motif1_results_chunk in chunks])
+    if args.regulator:
+        motiflist = args.motiflist
+        with open(motiflist, 'r') as file:
+            lines = file.readlines()
+        motif1,max_mismatch1_str = lines[0].strip().split('\t')
+        motif2,max_mismatch2_str = lines[1].strip().split('\t')
+        max_mismatch1 = int(max_mismatch1_str) if max_mismatch1_str else 0 
+        max_mismatch2 = int(max_mismatch2_str) if max_mismatch2_str else 0 
+
+        fasta_file_path = args.fasta
+        min_gap = args.min_gap
+        max_gap = args.max_gap
+        direction = args.direction
+        pool = multiprocessing.Pool(multiprocessing.cpu_count())
+        records = list(SeqIO.parse(fasta_file_path, "fasta"))
+        all_results = []
+        output_dir = args.output_dir    
+        output_file_path = f"{output_dir}/regulator_variable_gap.out"
+
+        if args.mismatches is None:
+            args.mismatches = max_mismatch1 + max_mismatch2
+            max_mismatches = args.mismatches
+        else:
+            max_mismatches = args.mismatches
+
+        if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) >= 500000:
+            if direction == '+' or direction == '+,-':  
+                motif1_results_pre = process_genome_file_forward(fasta_file_path, motif1, max_mismatch1)
+                motif1_results = sorted(motif1_results_pre, key=lambda x: (x['sequence_id'], x['start']))
+                motif2_results_pre = process_genome_file_forward(fasta_file_path, motif2, max_mismatch2)
+                motif2_results = sorted(motif2_results_pre, key=lambda x: (x['sequence_id'], x['start']))
+                num_chunks = multiprocessing.cpu_count()
+                chunk_size = max(len(motif1_results) // num_chunks,1)
+                chunks = [motif1_results[i:i + chunk_size] for i in range(0, len(motif1_results), chunk_size)]
+                    
+                for record in records:
+                    combined_results = pool.starmap(combine_results_forward, [(record, motif1_results_chunk, motif2_results, max_mismatches, min_gap, max_gap) for motif1_results_chunk in chunks])
+                    combined_results = [item for sublist in combined_results for item in sublist]
+                    all_results.extend(combined_results)		                   
+            if direction == '-' or direction == '+,-':  
+                motif1_results_pre = process_genome_file_reverse(fasta_file_path, motif1, max_mismatch1)
+                motif1_results = sorted(motif1_results_pre, key=lambda x: (x['sequence_id'], x['start']))
+                motif2_results_pre = process_genome_file_reverse(fasta_file_path, motif2, max_mismatch2)
+                motif2_results = sorted(motif2_results_pre, key=lambda x: (x['sequence_id'], x['start']))
+                num_chunks = multiprocessing.cpu_count()
+                chunk_size = max(len(motif1_results) // num_chunks,1)
+                chunks = [motif1_results[i:i + chunk_size] for i in range(0, len(motif1_results), chunk_size)]             
+                for record in records:
+                    combined_results = pool.starmap(combine_results_reverse, [(record, motif1_results_chunk, motif2_results, max_mismatches, min_gap, max_gap) for motif1_results_chunk in chunks])
+                    combined_results = [item for sublist in combined_results for item in sublist]
+                    all_results.extend(combined_results)
+        if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) < 500000:
+            if direction == '+' or direction == '+,-':
+                combined_results = pool.starmap(process_record_DNA_forward, [(record, motif1, motif2, max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap) for record in records])
                 combined_results = [item for sublist in combined_results for item in sublist]
-                all_results.extend(combined_results)		                   
-        if direction == '-' or direction == '+,-':  
-            motif1_results_pre = process_genome_file_reverse(fasta_file_path, motif1, max_mismatch1)
-            motif1_results = sorted(motif1_results_pre, key=lambda x: (x['seq_name'], x['start']))
-            motif2_results_pre = process_genome_file_reverse(fasta_file_path, motif2, max_mismatch2)
-            motif2_results = sorted(motif2_results_pre, key=lambda x: (x['seq_name'], x['start']))
-            num_chunks = multiprocessing.cpu_count()
-            chunk_size = max(len(motif1_results) // num_chunks,1)
-            chunks = [motif1_results[i:i + chunk_size] for i in range(0, len(motif1_results), chunk_size)]             
-            for record in records:
-                combined_results = pool.starmap(combine_results_reverse, [(record, motif1_results_chunk, motif2_results, max_mismatches, min_gap, max_gap) for motif1_results_chunk in chunks])
+                all_results.extend(combined_results)
+            if direction == '-' or direction == '+,-':
+                combined_results = pool.starmap(process_record_DNA_reverse, [(record, motif1, motif2, max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap) for record in records])
                 combined_results = [item for sublist in combined_results for item in sublist]
                 all_results.extend(combined_results)
-    if (args.DNA or args.RNA) and calculate_average_length(fasta_file_path) < 500000:
-        if direction == '+' or direction == '+,-':
-            combined_results = pool.starmap(process_record_DNA_forward, [(record, motif1, motif2, max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap) for record in records])
-            combined_results = [item for sublist in combined_results for item in sublist] #Flatten the list
+        if args.protein:
+            combined_results = pool.starmap(process_record_protein, [(record, motif1, motif2, max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap) for record in records])
+            combined_results = [item for sublist in combined_results for item in sublist]
             all_results.extend(combined_results)
-        if direction == '-' or direction == '+,-':
-            combined_results = pool.starmap(process_record_DNA_reverse, [(record, motif1, motif2, max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap) for record in records])
-            combined_results = [item for sublist in combined_results for item in sublist] #Flatten the list
-            all_results.extend(combined_results)
-    if args.protein:
-        combined_results = pool.starmap(process_record_protein, [(record, motif1, motif2, max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap) for record in records])
-        combined_results = [item for sublist in combined_results for item in sublist] #Flatten the list
-        all_results.extend(combined_results)
-    if not all_results:
-        print("# No Result")
-    else:
-        with open(output_file_path, 'w') as output_file:
-            output_file.write("Sequence_ID\tSequence_Length\tMotif\tstart\tend\tstrand\tmotif1_mismatch\tfragment1\tmotif2_mismatch\tfragment2\tmismatches\tgap_length\tmatched_sequence\n")
-            for result in all_results:
-                output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['motif1_mismatch']}\t{result['fragment1']}\t{result['motif2_mismatch']}\t{result['fragment2']}\t{result['mismatch']}\t{result['gap_length']}\t{result['sequence']}\n")
-    if args.image:
-        plot_motifs_to_single_chart(output_file_path, output_file_path, display_both_directions=args.display_both_directions)
+        if not all_results:
+            print("# No Result")
+        else:
+            with open(output_file_path, 'w') as output_file:
+                output_file.write("Sequence_ID\tSequence_Length\tMotif\tstart\tend\tstrand\tmotif1_mismatch\tfragment1\tmotif2_mismatch\tfragment2\tmismatches\tgap_length\tmatched_sequence\n")
+                for result in all_results:
+                    output_file.write(f"{result['sequence_id']}\t{result['sequence_length']}\t{result['motif']}\t{result['start']}\t{result['end']}\t{result['strand']}\t{result['motif1_mismatch']}\t{result['fragment1']}\t{result['motif2_mismatch']}\t{result['fragment2']}\t{result['mismatch']}\t{result['gap_length']}\t{result['sequence']}\n")
+        if args.image:
+            plot_motifs_to_single_chart(output_file_path, output_file_path, args.display_both_directions, args.gff, args.motif_up, args.motif_down)
 
-def VisualMotif_function(args):
+def visualMotif_function(args):
     output_dir = args.output_dir    
     output_file_path = f"{output_dir}/visualization"
-    plot_motifs_to_single_chart(args.table_file, output_file_path, args.display_both_directions)
+    gff_file = args.gff
+    motif_up = args.motif_up
+    motif_down = args.motif_down
+    plot_motifs_to_single_chart(args.table_file, output_file_path, args.display_both_directions, gff_file, motif_up, motif_down)
+
+def extract_sequences_function(args):
+    if args.output is None:
+        raise ValueError("Output file path is required.")
+    sequences = SeqIO.to_dict(SeqIO.parse(args.fna, "fasta"))
+
+    output_handle = open(args.output, "w")
+
+    with open(args.gff, "r") as gff_handle:
+        for line in gff_handle:
+            line = line.strip()
+            if line.startswith("#"):
+                continue
+            fields = line.split("\t")
+            feature_type = fields[2]
+            strand = fields[6]
+            if feature_type == "CDS":
+                seq_name = fields[0]
+                seq_start = int(fields[3])
+                seq_end = int(fields[4])
+                attributes = fields[8].split(";")
+                cds_id = parent = gene = product = "None"
+
+                for attr in attributes:
+                    if attr.startswith("ID="):
+                        cds_id = attr[3:]
+                    elif attr.startswith("Parent="):
+                        parent = attr[7:]
+                    elif attr.startswith("gene="):
+                        gene = attr[5:]
+                    elif attr.startswith("product="):
+                        product = attr[8:]
+                if seq_name in sequences:
+                    sequence = sequences[seq_name].seq
+                    if args.promoter:
+                        if strand == "-":
+                            start = max(seq_end - args.downstream, 0)
+                            end = start + args.upstream + args.downstream
+                            seq_fragment = sequence[start:end].reverse_complement()
+                        else:
+                            start = max(seq_start - args.upstream, 0)
+                            end = start + args.upstream + args.downstream
+                            seq_fragment = sequence[start:end]
+                    elif args.orf:
+                        if strand == "-":
+                            seq_fragment = sequence[seq_start - 1:seq_end].reverse_complement()
+                        else:
+                            seq_fragment = sequence[seq_start - 1:seq_end]
+                    else:
+                        continue
+                    seq_record = SeqRecord(seq_fragment, id=f"{seq_name}|{cds_id}|{parent}|{gene}|{seq_start}|{seq_end}|{strand}|{product}",description="")
+                    SeqIO.write(seq_record, output_handle, "fasta")
+    # Close output file
+    output_handle.close()
 
 def generate_motif_variants(motif):
     variant_bases = []
     ambiguous_bases = {
         'W': 'AT',
         'S': 'GC',
         'M': 'AC',
@@ -549,15 +536,14 @@
     return mismatches
 
 
 def search_motif(record, motif, max_mismatches, motif_length):
     variants = generate_motif_variants(motif)
     sequence = str(record.seq)
     sequence_length = len(sequence)
-
     results = []
 
     for i in range(sequence_length - motif_length + 1):
         fragment = sequence[i:i+motif_length]
         mismatches = calculate_mismatches(fragment, variants)
         
         if mismatches <= max_mismatches:
@@ -596,14 +582,15 @@
                 'mismatches': mismatches,
                 'fragment': fragment,
                 'strand': '-',
             }
             results.append(result)
 
     return results
+
 def reverse_search_fix(record, motif, max_mismatches, motif_length):
     variants = generate_motif_variants(motif)
     sequence = str(record.seq.reverse_complement())
     motif_length = len(motif)
     sequence_length = len(sequence)
     results = []
 
@@ -622,19 +609,18 @@
                 'fragment': fragment,
                 'strand': '-',
             }
             results.append(result)
 
     return results	
 
-#protein
 def calculate_mismatche_protein(fragment, motif):
     mismatches = 0
     for aa, motif_aa in zip(fragment, motif):
-        if motif_aa == '-':  # Wildcard symbol, any amino acid is allowed
+        if motif_aa == '-':
             continue
         if motif_aa != aa:
             mismatches += 1
     return mismatches
 
 def search_motif_protein(record, motif, max_mismatches, motif_length):
     sequence = str(record.seq)
@@ -699,43 +685,38 @@
                 'mismatches':mismatches,
                 'fragment':fragment,
                 'strand':'-',
             }
             results.append(result)
     return results
 
-
 def process_genome_file_forward(fasta_file_path, motif, max_mismatches):
     window_size = len(motif)
     split_size = 500000
     all_results = []
     futures = []
     with ProcessPoolExecutor() as executor:
         for record in SeqIO.parse(fasta_file_path, "fasta"):
             sequence_id = record.id
             genome_sequence = str(record.seq)
             len_genome = len(genome_sequence)
             if len_genome <= split_size:
-                # 如果序列长度小于等于split_size，直接滑窗
                 sequence_chunk = genome_sequence
                 start = 0
                 future = executor.submit(process_window_forward, sequence_chunk, start, window_size, sequence_id, motif, max_mismatches,len_genome)
-                futures.append(future)
-                
+                futures.append(future)                
             else:
                 num_splits = math.ceil(len_genome / split_size)
                 for i in range(num_splits):
                     start = i * split_size
                     end = start + split_size + window_size - 1
                     sequence_chunk = genome_sequence[start:end]
                     if i == num_splits - 1 and len(sequence_chunk) < split_size:
-                        # 如果是最后一个片段且长度小于split_size，传递实际长度
                         future = executor.submit(process_window_forward, sequence_chunk, start, window_size, sequence_id, motif, max_mismatches,len_genome)
                     else:
-                        # 否则传递split_size
                         future = executor.submit(process_window_forward, sequence_chunk, start, window_size, sequence_id, motif, max_mismatches,len_genome)
                     futures.append(future)
                     
         for future in as_completed(futures):
             results = future.result()
             all_results.extend(results)
     return all_results
@@ -747,39 +728,35 @@
     futures = []
     with ProcessPoolExecutor() as executor:
         for record in SeqIO.parse(fasta_file_path, "fasta"):
             sequence_id = record.id
             genome_sequence = str(record.seq.reverse_complement())
             len_genome = len(genome_sequence)
             if len_genome <= split_size:
-                # 如果序列长度小于等于split_size，直接滑窗
                 sequence_chunk = genome_sequence
                 start = 0
                 future = executor.submit(process_window_reverse, sequence_chunk, start, window_size, sequence_id, motif, max_mismatches,len_genome)
                 futures.append(future)
             else:
                 num_splits = math.ceil(len_genome / split_size)
                 for i in range(num_splits):
                     start = i * split_size
                     end = start + split_size + window_size - 1
                     sequence_chunk = genome_sequence[start:end]
                     if i == num_splits - 1 and len(sequence_chunk) < split_size:
-                        # 如果是最后一个片段且长度小于split_size，传递实际长度
                         future = executor.submit(process_window_reverse, sequence_chunk, start, window_size, sequence_id, motif, max_mismatches,len_genome)
                     else:
-                        # 否则传递split_size
                         future = executor.submit(process_window_reverse, sequence_chunk, start, window_size, sequence_id, motif, max_mismatches,len_genome)
                     futures.append(future)
                     
         for future in as_completed(futures):
             results = future.result()
             all_results.extend(results)			  
     return all_results
 
-#combine	
 def combine_results_forward(record, motif1_results_chunk, motif2_results,max_mismatches, min_gap, max_gap):
     sequence = str(record.seq)
     sequence_length = len(sequence)
     sequence_id = record.id
     combined_results = []
     
     for motif1_result in motif1_results_chunk:
@@ -834,110 +811,14 @@
                     'gap_length': gap_length,
                     'sequence': sequence[motif1_result['start']:motif2_result['end'] + 1]
                 }
                 combined_results.append(combined_result)
     
     return combined_results
 
-
-
-
-def plot_motifs_to_single_chart(file_path, output_file, display_both_directions=False):
-    df = pd.read_csv(file_path, sep='\t', header=None, dtype={0: str, 1: int, 2: str, 3: int, 4: int, 5: str}, usecols=[0, 1, 2, 3, 4, 5], skiprows=1, names=["Sequence ID", "Length", "Motif", "Start", "End", "Strand"])
-    grouped_df = df.groupby("Sequence ID")
-    num_sequences = len(grouped_df)
-    height_interval = 0.5
-    max_length = df["Length"].max()
-    line_length = 15
-    multiplier = line_length / max_length
-
-    fig, ax = plt.subplots(figsize=(line_length, num_sequences * 0.5))
-    ax.axis('off')
-
-    color_list = ['#008000','#FF0000', '#0000FF', '#FF00FF', '#00FFFF', '#FFFF00', '#800000', '#00FF00', '#000080', '#808000', '#800080', '#008080', '#808080', '#C0C0C0', '#FFA500']
-    color_map = {}
-
-    first_line_position = None
-    first_seq_id = None
-    for idx, (seq_id, seq_group) in enumerate(grouped_df):
-        y_position = idx * 2
-        seq_length = seq_group.iloc[0]["Length"]
-        line = seq_length * multiplier
-        ax.plot([0, line], [y_position, y_position], color='black')
-        ax.text(-0.5, y_position, seq_id, ha='right', va='center', fontsize=10)
-
-        first_sequence_y = y_position
-        first_seq_id = seq_id
-  
-        for _, row in seq_group.iterrows():
-            start = row["Start"]
-            end = row["End"]
-            direction = row["Strand"]
-            motif = row["Motif"]
-            arrow_length = (end-start)*line_length/max_length*0.2
-            shift_amount = arrow_length
-
-            if not display_both_directions and direction == '-':
-                continue
-
-            motif_length = end - start
-
-            if motif not in color_map:
-                color_map[motif] = color_list[len(color_map) % 15]
-
-            color = color_map[motif]
-
-            if direction == '+':
-                rectangle = plt.Rectangle((start / seq_length * line, y_position), (end - start) / seq_length * line, height_interval, facecolor=color, edgecolor='none')
-            else:  # direction == '-'
-                rectangle = plt.Rectangle(((start - shift_amount) / seq_length * line, y_position), (end - start) / seq_length * line, height_interval, facecolor=color, edgecolor='none')
-
-            ax.add_patch(rectangle)
-
-            if direction == '+':
-                arrow_tail_x = (start + motif_length - shift_amount) / seq_length * line
-                arrow_head_x = arrow_tail_x + arrow_length
-            else:  # direction == '-'
-                arrow_tail_x = (start + shift_amount) / seq_length * line
-                arrow_head_x = arrow_tail_x - arrow_length
-
-            arrow_polygon = np.array([[arrow_head_x, y_position + height_interval / 2], [arrow_tail_x, y_position], [arrow_tail_x, y_position + height_interval]])
-            arrow = plt.Polygon(arrow_polygon, closed=True, edgecolor=color, facecolor=color)
-            ax.add_patch(arrow)
-    #
-    y_pos = first_sequence_y + 2
-    ax.plot([0, line_length], [y_pos, y_pos], color='black')
-
-    tick_positions = np.linspace(0, line_length, num=11)
-    tick_labels = np.linspace(0, max_length, num=11, dtype=int)
-    for tick_pos in tick_positions:
-        ax.plot([tick_pos, tick_pos], [y_pos, y_pos - 0.2], color='black')
-    for tick_pos, tick_label in zip(tick_positions, tick_labels):
-        ax.text(tick_pos, y_pos - 1.2 , str(tick_label), ha='center', va='bottom', fontsize=10)
-
-
-    ax.set_xlim(0, line_length) 
-    ax.set_ylim(-1, num_sequences * 2)
-    ax.set_xticks(np.arange(0, line_length + 1))
-    ax.set_xlabel('Position (cm)')
-    ax.set_title('Motif Search Results', fontweight='bold')
-    ax.set_yticks([])
-
-    legend_elements = [Patch(facecolor=color, edgecolor='black', label=motif) for motif, color in color_map.items()]
-    ax.legend(handles=legend_elements, title='Motif', bbox_to_anchor=(1.05, 1), loc='upper left')
-
-    plt.subplots_adjust(left=0.05, right=0.95, top=0.95, bottom=0.05)
-    #Save as PDF 
-    output_file_pdf = f'{output_file}.pdf'
-    plt.savefig(output_file_pdf, bbox_inches='tight',format='pdf')
-
-    #Save as PNG
-    output_file_png = f'{output_file}.png'
-    plt.savefig(output_file_png, bbox_inches='tight',format='png')
-
 def process_record_protein(record, motif1, motif2,max_mismatch1, max_mismatch2, max_mismatches, min_gap, max_gap):
     motif1_results = search_motif_protein(record, motif1, max_mismatch1, len(motif1))
     motif2_results_pre = search_motif_protein(record, motif2, max_mismatch2, len(motif2))
     motif2_results = sorted(motif2_results_pre, key=lambda x: x['start'])
     combined_results = combine_results_forward(record, motif1_results, motif2_results, max_mismatches, min_gap, max_gap)
     return combined_results
 
@@ -956,108 +837,557 @@
     return combined_results
 
 def calculate_average_length(sequence_file):
     total_length = 0
 
     sequence_count = 0
     
-    for record in SeqIO.parse(sequence_file, "fasta"):  # 假设文件格式是fasta格式
+    for record in SeqIO.parse(sequence_file, "fasta"):
         total_length += len(record.seq)
         sequence_count += 1
     
     if sequence_count == 0:
-        return 0 # Handle the case of an empty file
+        return 0
     
     average_length = total_length / sequence_count
     return average_length
 
-def filter_rows(result_list,line_count):
-    if len(set(row['motif_type'] for row in result_list)) < line_count:
-        return
+def check_sequential_numbers(nums,sorted_nums, m):
+    count = 0
+    ordered_nums = []
+    processed_nums = set()
+    i = 0
+    while i < len(nums):
+        if nums[i] in processed_nums:
+            i += 1
+            continue
+        if nums[i] == sorted_nums[count]:
+            ordered_nums.append((nums[i], i))
+            processed_nums.add(nums[i])
+            count += 1
+            i+=1
+
+        elif nums[i] != sorted_nums[count]:
+            if sorted_nums[count] not in nums[i:]: 
+                count += 1
+            else:
+                for x in range(i, len(nums)):
+                    if nums[x] == sorted_nums[count]:
+                        if x-i >=m and len(ordered_nums)+len(sorted_nums)-1-count >=m:
+                            count+=1
+                        else:
+                            ordered_nums.append((nums[x], x))
+                            processed_nums.add(nums[x])
+                            count += 1
+                            i = x + 1
+                        break
+    
+    if len(ordered_nums) >= m:
+        return [[index for _, index in ordered_nums]]
+    else:
+        return None
+
+def filter_rows(result_list, motif_nums, line_count,necessary_file=None):
+    if len(set(row['motif_type'] for row in result_list)) < motif_nums:
+        return None
 
-    filtered_rows = []
-    motif_type = []
+    temp = []
+    lists = []
     i = 0
-    while i <= len(result_list) - 1:
-        current_row = result_list[i]
-        after_row = result_list[i + 1] if i + 1 < len(result_list) else None
-        before_row = result_list[i - 1] if i - 1 >= 0 else None
-        if current_row['strand'] == "+":
-            if i == 0 and int(current_row['motif_type']) == 1:
-                m=0
-                while int(result_list[m]['motif_type']) == 1:
-                    m += 1
-                i = m - 1
-                filtered_rows.append(result_list[i])
-                motif_type.append(result_list[m]['motif_type'])
-                i += 1
-
-            elif after_row is not None and before_row is not None and 'motif_type' in current_row and 'motif_type' in after_row and current_row['motif_type'] < after_row['motif_type'] and current_row['end'] < after_row['start'] and current_row['start'] > before_row['end']:
-                filtered_rows.append(current_row)
-                motif_type.append(current_row['motif_type'])
-                i += 1
-            elif after_row is not None and before_row is not None and current_row['motif_type'] > after_row['motif_type'] and current_row['motif_type'] > before_row['motif_type']:
-                if after_row['motif_type'] in motif_type and current_row['start'] > before_row['end']:
-                    filtered_rows.append(current_row)
-                    motif_type.append(current_row['motif_type'])
-                    i += 2
-                elif after_row['motif_type'] not in motif_type and after_row['start'] > before_row['end']:
-                    filtered_rows.append(after_row)
-                    motif_type.append(after_row['motif_type'])
-                    i += 2
+
+    filtered_rows = []
+    num_list = []
+    num_list_add=[]
+    nums=[]
+    sorted_nums =[]
+
+    count_positive_strand = 0
+    count_negative_strand = 0
+    for item in result_list:
+        if item['strand'] == '+':
+            count_positive_strand += 1  
+        else:
+            count_negative_strand += 1
+    if count_positive_strand > count_negative_strand:
+        while i < len(result_list) -1:
+            temp.append((result_list[i], i))
+            if result_list[i]['motif_type'] >= result_list[i + 1]['motif_type']:
+                lists.append(temp)
+                temp = []
+            i += 1
+
+        if i == len(result_list) - 1:
+            temp.append((result_list[i], i))
+            lists.append(temp)
+
+        for sublist in sorted(lists, key=len, reverse=True):
+            filtered_temp=[]
+            if any(all(item in sublist for item in sublist_item) for sublist_item in num_list_add):
+                continue
+
+            if sublist[0][0]['motif_type'] > 1:
+                up = ((sublist[0][0]['motif_type'] - 1) // 3 + 1) * 1000
+                up_value = sublist[0][0]['start'] - up
+                if up_value < result_list[0]['start']:
+                    f_start=1
                 else:
-                    i += 2
-            elif before_row is not None and current_row['motif_type'] == line_count and current_row['start'] > before_row['end']:
-                filtered_rows.append(current_row)
-                motif_type.append(current_row['motif_type'])
-                break
-            elif before_row is not None and i == len(result_list) -1 and current_row['start'] > before_row['end']:
-                filtered_rows.append(current_row)
-                motif_type.append(current_row['motif_type'])
+                    for sub_list in lists:
+                        if sub_list[0][0]["start"] <= up_value <= sub_list[-1][0]['end']:
+                            f_start=sub_list[0][1]
+                            break
+                        elif up_value < sub_list[0][0]["start"] and lists.index(sub_list) > 0 and up_value > lists[lists.index(sub_list)-1][-1][0]['end']:
+                            f_start=lists[lists.index(sub_list)-1][0][1]
+                            break
+            else:
+                f_start = sublist[0][1]
+            if sublist[-1][0]['motif_type'] < line_count:
+                down = ((int(line_count - sublist[-1][0]['motif_type'])) // 3 + 1) * 1000
+                down_value = sublist[-1][0]['end'] + down
+                if down_value > result_list[-1]['end']:
+                    g_end = len(result_list)-1
+                else:
+                    for sub_list in lists:
+                        if sub_list[0][0]["start"] <= down_value <= sub_list[-1][0]['end']:
+                            g_end =sub_list[-1][1]
+                            break
+                        elif down_value < sub_list[0][0]["start"] and lists.index(sub_list) > 0 and down_value > lists[lists.index(sub_list)-1][-1][0]['end']:
+                            g_end =sub_list[-1][1]
+                            break
+            else:
+                g_end = sublist[-1][1]
+
+            if g_end - f_start < motif_nums:
                 break
+
+            num_list = result_list[f_start:g_end + 1]
+            num_list_add.append(num_list)
+            nums = [row['motif_type'] for row in num_list]
+            sorted_nums = sorted(set(nums))
+            result_index = check_sequential_numbers(nums, sorted_nums, motif_nums)
+
+            if result_index is None:
+                if filtered_rows:
+                    return filtered_rows
+                else:
+                    return None
             else:
-                i += 1
+                result_index = [item for expand in result_index if expand is not None for item in expand]
+                for i in result_index:
+                    filtered_temp.append(num_list[i])
+
+                if necessary_file:
+                    with open('file1.txt', 'r') as file:
+                        motif_must = file.readline().strip().split(',')
+                    data_list = [row['motif_type'] for row in filtered_temp]
+                    all_in = all(item in data_list for item in motif_must)
+
+                    if all_in:
+                        filtered_rows.append(filtered_temp)
+                    else:
+                        return filtered_rows
 
-        else:
-            if i == 0 and int(current_row['motif_type']) == 1:
-                m=0
-                while int(result_list[m]['motif_type']) == 1:
-                    m += 1
-
-                i = m - 1
-                filtered_rows.append(result_list[i])
-                motif_type.append(result_list[m]['motif_type'])
-                i += 1
-
-            elif after_row is not None and before_row is not None and 'motif_type' in current_row and 'motif_type' in after_row and current_row['motif_type'] < after_row['motif_type'] and current_row['end'] > after_row['start'] and current_row['start'] < before_row['end']:
-                filtered_rows.append(current_row)
-                motif_type.append(current_row['motif_type'])
-                i += 1
-            elif after_row is not None and before_row is not None and current_row['motif_type'] > after_row['motif_type'] and current_row['motif_type'] > before_row['motif_type']:
-                if after_row['motif_type'] in motif_type and current_row['start'] < before_row['end']:
-                    filtered_rows.append(current_row)
-                    motif_type.append(current_row['motif_type'])
-                    i += 2
-                elif after_row['motif_type'] not in motif_type and after_row['start'] < before_row['end']:
-                    filtered_rows.append(after_row)
-                    motif_type.append(after_row['motif_type'])
-                    i += 2
                 else:
-                    i += 2
-            elif before_row is not None and current_row['motif_type'] == line_count and current_row['start'] < before_row['end']:
-                filtered_rows.append(current_row)
-                motif_type.append(current_row['motif_type'])
-                break
-            elif before_row is not None and i == len(result_list) -1 and current_row['start'] < before_row['end']:
-                filtered_rows.append(current_row)
-                motif_type.append(current_row['motif_type'])
+                    filtered_rows.append(filtered_temp)
+
+
+    else:
+        while i < len(result_list) -1:
+            temp.append((result_list[i], i))
+            if result_list[i]['motif_type'] <= result_list[i + 1]['motif_type']:
+                lists.append(temp)
+                temp = []
+            i += 1
+            
+        if i == len(result_list) - 1:
+            temp.append((result_list[i], i))
+            lists.append(temp)
+
+        for sublist in sorted(lists, key=len, reverse=True):
+            filtered_temp=[]
+            if all(item in num_list for item in sublist):
+                continue
+
+            if sublist[0][0]['motif_type'] < line_count:
+                up = ((line_count-sublist[0][0]['motif_type'] ) // 3 + 1) * 1000
+                up_value = sublist[0][0]['start'] - up
+                if up_value < result_list[0]['start']:
+                    f_start=1
+
+                else:
+                    for sub_list in lists:
+                        if sub_list[0][0]["start"] <= up_value <= sub_list[-1][0]['end']:
+                            f_start=sub_list[0][1]
+                            break
+                        elif up_value < sub_list[0][0]["start"] and lists.index(sub_list) > 0 and up_value > lists[lists.index(sub_list)-1][-1][0]['end']:
+                            f_start=lists[lists.index(sub_list)-1][0][1]
+                            break
+            else:
+                f_start = sublist[0][1]
+
+            if sublist[-1][0]['motif_type'] >1 :
+                down = ((sublist[-1][0]['motif_type']-1) // 3 + 1) * 1000
+                down_value = sublist[-1][0]['end'] + down
+                if down_value > result_list[-1]['end']:
+                    g_end = len(result_list)-1
+                else:
+                    for sub_list in lists:
+                        if sub_list[0][0]["start"] <= down_value <= sub_list[-1][0]['end']:
+                            g_end = sub_list[-1][1]
+                            break
+                        elif down_value < sub_list[0][0]["start"] and lists.index(sub_list) > 0 and down_value > lists[lists.index(sub_list)-1][-1][0]['end']:
+                            g_end =sub_list[-1][1]
+                            break
+            else:
+                g_end = sublist[-1][1]
+
+            if g_end - f_start < motif_nums:
                 break
+
+            num_list = result_list[f_start:g_end + 1]
+            nums = [row['motif_type'] for row in num_list]
+            sorted_nums = sorted(set(nums),reverse=True)
+
+            result_index = check_sequential_numbers(nums, sorted_nums, motif_nums)
+            if result_index is None:
+                if filtered_rows:
+                    return filtered_rows
+                else:
+                    return None
             else:
-                i += 1
+                result_index = [item for expand in result_index if expand is not None for item in expand]
+                for i in result_index:
+                    filtered_temp.append(num_list[i])
 
+
+                if necessary_file:
+                    with open('file1.txt', 'r') as file:
+                        motif_must = file.readline().strip().split(',')
+                    data_list = [row['motif_type'] for row in filtered_temp]
+                    all_in = all(item in data_list for item in motif_must)
+
+                    if all_in:
+                        filtered_rows.append(filtered_temp)
+                    else:
+                        return filtered_rows
+
+                else:
+                    filtered_rows.append(filtered_temp)
     return filtered_rows
 
+def draw_triangle(fig, point1, point2, point3, color='blue', row=None, col=None):
+    fig.add_trace(
+        go.Scatter(
+            x=[point1[0], point2[0], point3[0], point1[0]],
+            y=[point1[1], point2[1], point3[1], point1[1]],
+            mode='lines',
+            line=dict(color="black"),
+            fill='toself',
+            fillcolor=color,
+            showlegend=False
+        ),
+        row=row,
+        col=col
+    )      
+
+def collate_gff(gff_file):
+    gene_list=[]
+    with open(gff_file, "r") as gff_handle:
+        for line in gff_handle:
+            line = line.strip()
+            if line.startswith("#"):
+                continue
+            fields = line.split("\t")
+            feature_type = fields[2]
+            strand = fields[6]
+            if feature_type == "CDS":
+                seq_name = fields[0]
+                seq_start = int(fields[3])
+                seq_end = int(fields[4])
+                attributes = fields[8].split(";")
+                gene = ""
+
+                for attr in attributes:
+                    if attr.startswith("gene="):
+                        gene = attr[5:]
+                gene_list.append([seq_name,seq_start, seq_end,strand,gene])
+    return gene_list
+
+def collate_bed(correction_gff, seq_id, min_length,option=None, start=None,end=None):
+    gene_df = pd.DataFrame(correction_gff, columns=['seq_name', 'seq_start', 'seq_end', 'strand', 'gene'])
+    grouped_df = gene_df.groupby("seq_name")
+    filtered_rows = pd.DataFrame(columns=['seq_name', 'seq_start', 'seq_end', 'strand', 'gene'])
+    for seq_name, seq_group in grouped_df:
+        if seq_name == seq_id and option == "A":
+            for index, row in seq_group.iterrows():
+                row["seq_name"] = row["seq_name"] + '|' + str(math.floor(row["seq_end"]/min_length)*min_length)
+                row["seq_start"] = row["seq_start"] % min_length
+                if( row["seq_end"]%min_length < row["seq_start"] % min_length):
+                    row["seq_start"] = min_length
+                else:
+                    row["seq_end"] = row["seq_end"] % min_length
+                row_df = pd.DataFrame([row])
+                filtered_rows = pd.concat([filtered_rows, row_df], axis=0)
+            break
+
+        elif seq_name == seq_id and option == "B":
+            for index, row in seq_group.iterrows():
+                seq_start = row["seq_start"]
+                seq_end = row["seq_end"]
+                if seq_start > start and seq_end < end:
+                    row["seq_start"]=row["seq_start"]-start
+                    row["seq_end"]=row["seq_end"]-start
+
+                elif seq_start < start and seq_end < end and seq_end > start:
+                    row['seq_start'] = start
+                    row["seq_start"]=row["seq_start"]-start
+                    row["seq_end"]=row["seq_end"]-start              
+
+                elif seq_start > start and seq_start < end and seq_end > end:
+                    row['seq_end'] = end
+                    row["seq_start"]=row["seq_start"]-start
+                    row["seq_end"]=row["seq_end"]-start
+
+                elif seq_start < start and seq_end > end:
+                    row['seq_start'] = start
+                    row['seq_end'] = end
+                    row["seq_start"]=row["seq_start"]-start
+                    row["seq_end"]=row["seq_end"]-start
+                else:
+                    continue
+                row_df = pd.DataFrame([row])
+                filtered_rows = pd.concat([filtered_rows, row_df], axis=0)
+            break
+        else:
+            continue
+    modified_gene_list = filtered_rows.values.tolist()
+
+    return modified_gene_list
+
+def plot_motifs_to_single_chart(file_path, output_file, display_both_directions=False, gff_file=None, motif_up=2000, motif_down=2000):
+    df = pd.read_csv(file_path, sep='\t', header=None, dtype={0: str, 1: int, 2: str, 3: int, 4: int, 5: str}, usecols=[0, 1, 2, 3, 4, 5], skiprows=1, names=["Sequence ID", "Length", "Motif", "Start", "End", "Strand"])
+    grouped_df = df.groupby("Sequence ID")
+    if df["Length"].min()>50000:
+        min_length = min(50000,df["Length"].min())
+    else:
+        min_length = 50000
+
+    correction_gff=[]
+    if gff_file:
+        correction_gff = collate_gff(gff_file)
+
+    gene_lists=[]
+
+    for idx, (seq_id, seq_group) in enumerate(grouped_df):
+        min_start_end = pd.concat([seq_group["Start"], seq_group["End"]]).min()
+        max_start_end = pd.concat([seq_group["Start"], seq_group["End"]]).max()
+        if (max_start_end - min_start_end > min_length):
+            if gff_file:
+                gene_list=collate_bed(correction_gff, seq_id,min_length, option="A", start=None,end=None)
+                gene_lists.extend(gene_list)
+            for index, row in seq_group.iterrows():
+                df.loc[index, "Sequence ID"] = row["Sequence ID"] + '|' + str(math.floor(row["End"]/min_length)*min_length)
+                df.loc[index, "Length"] = min_length
+                if row['Strand'] == "+":
+                    df.loc[index, "Start"] = row["Start"] % min_length
+                    if( row["End"]%min_length < row["Start"] % min_length):
+                        df.loc[index, "End"] = min_length
+                    else:
+                        df.loc[index, "End"] = row["End"] % min_length
+                if row['Strand'] == "-":
+                    df.loc[index, "End"] = row["End"] % min_length
+                    if( row["Start"]%min_length < row["End"] % min_length):
+                        df.loc[index, "Start"] = min_length
+                    else:
+                        df.loc[index, "Start"] = row["Start"] % min_length
+                df.loc[index, "type"] = "A"
+                df.loc[index, "n"] = math.floor(row["End"]/min_length)*min_length
+
+        elif(max_start_end - min_start_end < min_length and seq_group.iloc[0]["Length"] >=min_length):
+            start_from = max(min_start_end - motif_up,0)
+            end_to = min(max_start_end + motif_down, seq_group.iloc[0]["Length"])
+            if gff_file:
+                gene_list=collate_bed(correction_gff, seq_id, min_length,option="B", start=start_from, end=end_to)
+                gene_lists.extend(gene_list)
+            for index, row in seq_group.iterrows():
+                df.loc[index, "Length"] = end_to - start_from
+                df.loc[index, "Start"] = row["Start"] - start_from
+                df.loc[index, "End"] = row["End"] - start_from
+                df.loc[index, "start_from"] = start_from
+                df.loc[index, "end_to"] = end_to
+                df.loc[index, "type"] = "B"
+        else:
+            if gff_file:
+                gene_lists.extend(correction_gff)
+            for index, row in seq_group.iterrows():
+                df.loc[index, "type"] = "C"
+
+    grouped_again_df = df.groupby("Sequence ID", sort=False)
+    num_sequences = len(grouped_again_df)
+    height_interval = 0.7
+    max_length = df["Length"].max()
+    min_height = 300
+    if num_sequences <= 2:
+        height = min_height
+    else:
+        height = 100 * num_sequences
+
+    screen_width = 1920
+    max_length_proportion = 0.7
+    line_length = screen_width * max_length_proportion
+    multiplier = line_length / max_length
+
+    color_list = ['#008000','#FF0000', '#0000FF', '#FF00FF', '#00FFFF', '#FFFF00', '#800000', '#00FF00', '#000080', '#808000', '#800080', '#008080', '#808080', '#C0C0C0', '#FFA500', '#E64B35','#4DBBD5','#3C5488','#F39B7F','#91D1C2','#925E9F','#84BD00','#8C564B','#5C88DA','#D6616B','#6B58EE','#FDD0A2','#E7BA52','#3F4041','#9632B8']
+    color_map = {}
+
+    if gff_file:
+
+        fig = make_subplots(rows=num_sequences, cols=1, shared_xaxes=True)
+
+        for idx, (seq_id, seq_group) in enumerate(grouped_again_df):
+            y_position = idx * 2
+            seq_length = seq_group.iloc[0]["Length"]
+            line = seq_length * multiplier
+
+            fig.add_trace(go.Scatter(x=[0, line], y=[y_position, y_position], mode='lines', line=dict(color='black'), showlegend=False),row=idx+1,col=1)
+            fig.add_annotation(x=-0.5, y=y_position, text=seq_id, showarrow=False, font=dict(size=15), xanchor='right', yanchor='middle',row=idx+1,col=1)
+            tick_positions = np.linspace(0, line, num=11)
+            if (seq_group.iloc[0]["type"]=="A"):
+                tick_labels = np.linspace(seq_group.iloc[0]["n"], seq_group.iloc[0]["n"]+min_length, num=11, dtype=int)
+            
+            elif(seq_group.iloc[0]["type"]=="B"):
+
+                tick_labels = np.linspace(seq_group.iloc[0]["start_from"],seq_group.iloc[0]["end_to"], num=11, dtype=int)           
+            
+            else:
+                tick_labels = np.linspace(0, seq_length, num=11, dtype=int)
+
+            for tick_pos, tick_label in zip(tick_positions, tick_labels):
+                fig.add_trace(go.Scatter(x=[tick_pos, tick_pos], y=[y_position, y_position-0.5], mode='lines', line=dict(color='black'),showlegend=False),row=idx+1,col=1)
+                fig.add_annotation(x=tick_pos, y=y_position-1.5, text=str(tick_label), showarrow=False, font=dict(size=15), xanchor='center', row=idx+1,col=1)
+         
+            motif_gene_lists = []
+            if (seq_group.iloc[0]["type"]=="A" or seq_group.iloc[0]["type"]=="B"):
+                for _, row in seq_group.iterrows():
+                    seq_start = max(row["Start"] - motif_up, 0)
+                    seq_end = min(row["End"] + motif_down, min_length)
+                    seq_id_list = [item for item in gene_lists if item[0] == seq_id and item[1] >= seq_start  and item[2] <= seq_end]
+                    if seq_id_list not in motif_gene_lists:
+                        motif_gene_lists.extend(seq_id_list)
+            else:
+                for _, row in seq_group.iterrows():
+                    seq_start = max(row["Start"] - motif_up, 0)
+                    seq_end = min(row["End"] + motif_down, seq_group.iloc[0]["Length"])
+                    seq_id_list = [item for item in gene_lists if item[0] == seq_id and item[1] >= seq_start  and item[2] <= seq_end]
+                    if seq_id_list not in motif_gene_lists:
+                        motif_gene_lists.extend(seq_id_list)
+
+            num_ber = len(motif_gene_lists)
+            for i in range(num_ber):
+                seq_id = motif_gene_lists[i][0]
+                start_position = motif_gene_lists[i][1] * multiplier
+                end_position = motif_gene_lists[i][2] * multiplier
+                strand = motif_gene_lists[i][3]
+                gene = motif_gene_lists[i][4]
+
+                if strand == '+':
+                    fig.add_shape(type='rect', x0=start_position, y0= y_position - height_interval, x1=end_position, y1=y_position, line=dict(color='black'), fillcolor='black', row=idx+1,col=1)
+                    fig.add_annotation(x=(start_position+end_position)/2, y=y_position-1, text=str(gene), showarrow=False, font=dict(size=15), xanchor='center',row=idx+1,col=1)
+                else:
+                    fig.add_shape(type='rect', x0=start_position, y0=y_position - height_interval, x1=end_position, y1=y_position, line=dict(color='gray'), fillcolor='gray',row=idx+1,col=1)
+                    fig.add_annotation(x=(start_position+end_position)/2, y=y_position-1, text=str(gene), showarrow=False, font=dict(size=15), xanchor='center',row=idx+1,col=1)
+
+            for _, row in seq_group.iterrows():
+                start = row["Start"]
+                end = row["End"]
+                direction = row["Strand"]
+                motif = row["Motif"]
+                arrow_length = (end-start) * multiplier * 0.3
+
+                if not display_both_directions and direction == '-':
+                    continue
+
+                if motif not in color_map:
+                    color_map[motif] = color_list[len(color_map) % 15]
+                    fig.add_trace(go.Scatter(x=[None],y=[None],mode='markers',marker=dict(color=color_map[motif], size=30),name=motif))
+
+                color = color_map[motif]
+
+                if direction == '+':
+                    fig.add_shape(type='rect', x0=start * multiplier, y0=y_position, x1=end * multiplier - arrow_length, y1=y_position + height_interval, line=dict(color=color), fillcolor=color, row=idx+1,col=1)
+                    draw_triangle(fig, [end * multiplier - arrow_length,y_position], [end * multiplier - arrow_length, y_position + height_interval], [end * multiplier, y_position + height_interval / 2], color=color,row=idx+1,col=1)
+                else:
+                    fig.add_shape(type='rect', x0=start * multiplier + arrow_length, y0=y_position, x1=end * multiplier, y1=y_position + height_interval, line=dict(color=color), fillcolor=color, row=idx+1,col=1)
+                    draw_triangle(fig, [start * multiplier, y_position + height_interval / 2], [start * multiplier + arrow_length, y_position], [start * multiplier + arrow_length, y_position + height_interval], color=color,row=idx+1,col=1)
+
+        fig.update_xaxes(visible=False)
+        fig.update_yaxes(visible=False)
+        fig.update_layout(height= height, width= screen_width, title=None, showlegend=True,margin=dict(t=20, l=20, r=20, b=20), plot_bgcolor='rgba(0,0,0,0)')
+
+        fig.update_yaxes(
+            fixedrange=True,
+            showgrid=True
+        )
+
+        fig.write_html(f"{output_file}.html", config={'displayModeBar': True, 'scrollZoom': True, 'editable': False, 'modeBarButtonsToRemove': ['zoomIn', 'zoomOut'], 'toImageButtonOptions': {'format': 'svg'}})
+        fig.write_image(f"{output_file}.pdf" , format="pdf")
+        fig.write_image(f"{output_file}.png")
+        fig.write_image(f"{output_file}.svg")
+    else:
+        fig = make_subplots(rows=1, cols=1)
+        for idx, (seq_id, seq_group) in enumerate(grouped_again_df):
+            y_position = idx * 2
+            seq_length = seq_group.iloc[0]["Length"]
+            line = seq_length * multiplier
+            first_sequence_y=y_position
+            fig.add_trace(go.Scatter(x=[0, line], y=[y_position, y_position], mode='lines', line=dict(color='black'), showlegend=False))
+            fig.add_annotation(x=-0.5, y=y_position, text=seq_id, showarrow=False, font=dict(size=15), xanchor='right', yanchor='middle')
+
+            for _, row in seq_group.iterrows():
+                start = row["Start"]
+                end = row["End"]
+                direction = row["Strand"]
+                motif = row["Motif"]
+                arrow_length = (end-start) * multiplier * 0.3
+
+                if not display_both_directions and direction == '-':
+                    continue
+
+                if motif not in color_map:
+                    color_map[motif] = color_list[len(color_map) % 15]
+                    fig.add_trace(go.Scatter(x=[None],y=[None],mode='markers',marker=dict(color=color_map[motif],size=30),name=motif))
+                color = color_map[motif]
+
+                if direction == '+':
+                    fig.add_shape(type='rect', x0=start * multiplier, y0=y_position, x1=end * multiplier - arrow_length, y1=y_position + height_interval, line=dict(color=color), fillcolor=color)
+                    draw_triangle(fig, [end * multiplier - arrow_length,y_position], [end * multiplier - arrow_length, y_position + height_interval], [end * multiplier, y_position + height_interval / 2], color=color,row=None, col=None)
+                else:
+                    fig.add_shape(type='rect', x0=start * multiplier + arrow_length, y0=y_position, x1=end * multiplier, y1=y_position + height_interval, line=dict(color=color), fillcolor=color)
+                    draw_triangle(fig, [start * multiplier, y_position + height_interval / 2], [start * multiplier + arrow_length, y_position], [start * multiplier + arrow_length, y_position + height_interval], color=color,row=None, col=None)
+
+        y_pos = first_sequence_y + 2
+        fig.add_trace(go.Scatter(x=[0, line_length], y=[y_pos, y_pos], mode='lines', line=dict(color='black'), showlegend=False))
+        tick_positions = np.linspace(0, line_length, num=11)
+        tick_labels = np.linspace(0, max_length, num=11, dtype=int)
+        for tick_pos, tick_label in zip(tick_positions, tick_labels):
+            fig.add_trace(go.Scatter(x=[tick_pos, tick_pos], y=[y_pos, y_pos-0.5], mode='lines', line=dict(color='black'),showlegend=False))
+            fig.add_annotation(x=tick_pos, y=y_pos-1, text=str(tick_label), showarrow=False, font=dict(size=15), xanchor='center')
+
+        fig.update_xaxes(visible=False)
+        fig.update_yaxes(visible=False)
+        fig.update_layout(autosize=True,height=height,width= screen_width, yaxis_range=[0, num_sequences*2 + 1],plot_bgcolor='rgba(0,0,0,0)',margin=dict(t=10, l=5, r=5, b=20), title=None, showlegend=True, xaxis_title=None,yaxis_title=None)
+
+
+        fig.update_yaxes(
+            fixedrange=True,
+            showgrid=True
+        )
+
+        fig.write_html(f"{output_file}.html", config={'displayModeBar': True, 'scrollZoom': True, 'editable': False, 'modeBarButtonsToRemove': ['zoomIn', 'zoomOut'], 'toImageButtonOptions': {'format': 'svg'}})
+        fig.write_image(f"{output_file}.pdf" , format="pdf")
+        fig.write_image(f"{output_file}.png")
+        fig.write_image(f"{output_file}.svg")
+
 def main():
     get_args()
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `multiMotif-1.1.0/multiMotif.egg-info/PKG-INFO` & `multiMotif-1.2.1/multiMotif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: multiMotif
-Version: 1.1.0
+Version: 1.2.1
 Summary: A Computational Tool for Variable Motif scanning and Sequence-based Relative Position Visualization of Search Results in Sequences.
-Home-page: https://github.com/Sienna-L/multiMotif
+Home-page: https://github.com/SainanLuo/multiMotif
 Author: Sainan Luo
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: biopython>=1.78
 Requires-Dist: matplotlib>=3.3
 Requires-Dist: numpy>=1.19
 Requires-Dist: pandas>=1.1
+Requires-Dist: plotly>=5.18.0
 
 # VariaMotif
  Scanning and visualization for variable gap motifs.
 
 ## Installation
 
 To install VariaMotif, you can use [pip](https://pip.pypa.io/en/stable/installation/):
```

### Comparing `multiMotif-1.1.0/setup.py` & `multiMotif-1.2.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='multiMotif',
-    version='1.1.0',
+    version='1.2.1',
     packages=find_packages(),
     install_requires=[
         'biopython>=1.78',
         'matplotlib>=3.3',
         'numpy>=1.19',
-        'pandas>=1.1'
+        'pandas>=1.1',
+        'plotly>=5.18.0'
     ],
     author='Sainan Luo',
     description='A Computational Tool for Variable Motif scanning and Sequence-based Relative Position Visualization of Search Results in Sequences.',
     long_description=long_description,  # The new line
     long_description_content_type='text/markdown',  # The new line
-    url='https://github.com/Sienna-L/multiMotif',
+    url='https://github.com/SainanLuo/multiMotif',
     entry_points={
         'console_scripts': [
             'multiMotif=multiMotif.main:main',
         ],
     },
 )
```

