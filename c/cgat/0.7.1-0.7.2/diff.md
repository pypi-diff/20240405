# Comparing `tmp/cgat-0.7.1.tar.gz` & `tmp/cgat-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgat-0.7.1.tar", last modified: Thu Apr  4 14:46:03 2024, max compression
+gzip compressed data, was "cgat-0.7.2.tar", last modified: Fri Apr  5 10:27:47 2024, max compression
```

## Comparing `cgat-0.7.1.tar` & `cgat-0.7.2.tar`

### file list

```diff
@@ -1,168 +1,169 @@
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.272001 cgat-0.7.1/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1188 2024-04-01 08:10:13.000000 cgat-0.7.1/LICENSE
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      680 2024-04-01 08:10:13.000000 cgat-0.7.1/MANIFEST.in
--rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      761 2024-04-04 14:46:03.272001 cgat-0.7.1/PKG-INFO
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2721 2024-04-01 08:10:13.000000 cgat-0.7.1/README.md
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      734 2024-04-01 08:10:13.000000 cgat-0.7.1/THANKS.txt
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.260001 cgat-0.7.1/cgat/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2765 2024-04-04 14:37:59.000000 cgat-0.7.1/cgat/AGP.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2016 2024-04-04 08:06:46.000000 cgat-0.7.1/cgat/AString.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.260001 cgat-0.7.1/cgat/BamTools/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    84091 2024-04-04 08:06:46.000000 cgat-0.7.1/cgat/BamTools/bamtools.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    73647 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/BamTools/geneprofile.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    13457 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/BamTools/peakshape.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17233 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    29497 2024-04-04 12:43:35.000000 cgat-0.7.1/cgat/Blat.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.260001 cgat-0.7.1/cgat/Components/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4766 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Components/Components.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3847 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Components/connected_components.cpp
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1734 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Components/connected_components.h
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3878 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/FastaIterator.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12895 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Fastq.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.260001 cgat-0.7.1/cgat/FastqTools/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3528 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/FastqTools/fastqtools.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3108 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/GFF3.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    31953 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/GTF.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)   185318 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/GeneModelAnalysis.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    49913 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/Genomics.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1053 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Glam2.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1492 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Glam2Scan.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19547 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Histogram.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1395 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Histogram2D.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    41337 2024-04-04 12:43:35.000000 cgat-0.7.1/cgat/IndexedFasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/IndexedGenome.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11505 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Intervals.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1756 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Iterators.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5499 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/MEME.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7369 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Masker.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12153 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/MatrixTools.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2312 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Motifs.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.264001 cgat-0.7.1/cgat/NCL/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5656 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/__init__.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4148 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/_cnestedlist.pxd
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19606 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/cnestedlist.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3933 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/default.h
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    32028 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/intervaldb.c
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4921 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/intervaldb.h
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1563 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/RLE.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5705 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/RateEstimation.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40094 2024-04-04 12:43:35.000000 cgat-0.7.1/cgat/SequenceProperties.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6141 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/SetTools.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7596 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Sra.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    34513 2024-04-04 08:06:46.000000 cgat-0.7.1/cgat/Stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    20140 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Tree.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    44920 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/TreeTools.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3137 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/VCF.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.264001 cgat-0.7.1/cgat/VCFTools/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25310 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/VCFTools/vcftools.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19027 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Variants.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/__init__.py
--rwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)     3480 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/cgat.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    28781 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/dictzip.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7542 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/makeGeneset.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.272001 cgat-0.7.1/cgat/tools/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/__init__.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25343 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2bam.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1895 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2bam_split_reads.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6227 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3410 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2depth.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16746 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4895 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    38204 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2geneprofile.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    37840 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16966 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2wiggle.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2502 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2window_stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9672 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_compare_alignments.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9070 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_pileup2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3866 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_vs_bam.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8170 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_vs_bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9174 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_vs_gtf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8328 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bams2bam.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3208 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bcl2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    22414 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5688 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4029 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2gff.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2181 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2graph.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5363 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    24191 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4857 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed_vs_bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10208 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/beds2beds.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4295 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/beds2counts.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10672 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/cgat2dot.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5393 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/cgat_get_options.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2586 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/cgat_rebuild_extensions.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1033 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/cgat_script_template.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1470 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/csv2csv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10096 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/csvs2csv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9275 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/data2histogram.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7781 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/diff_bam.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11704 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/tools/diff_bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    15078 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/diff_chains.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9500 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/diff_fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14426 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/tools/diff_gtf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6238 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/extract_stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10207 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    21393 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/tools/fasta2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14562 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5500 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2kmercontent.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2682 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12477 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3771 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2variants.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2536 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2vcf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2281 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastas2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1884 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17342 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5343 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2summary.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6364 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12133 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2tpm.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1337 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5041 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastqs2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3534 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastqs2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9491 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastqs2fastqs.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2597 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/genome_bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5443 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11034 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2coverage.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14023 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    30644 2024-04-04 13:58:31.000000 cgat-0.7.1/cgat/tools/gff2gff.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9967 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2histogram.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4537 2024-04-04 12:43:35.000000 cgat-0.7.1/cgat/tools/gff2psl.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7200 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14982 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12848 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff32gtf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    18122 2024-04-04 08:06:46.000000 cgat-0.7.1/cgat/tools/gtf2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40355 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtf2gff.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    52205 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtf2gtf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    39563 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtf2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11698 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtf2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11190 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtfs2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4123 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/index2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12771 2024-04-01 13:26:07.000000 cgat-0.7.1/cgat/tools/index_fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6509 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/split_fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7956 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/split_file.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/split_gff.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3071 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/table2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2346 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/table2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9522 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/tables2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11183 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14736 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf2vcf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8970 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf_compare_phase.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6901 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf_stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3447 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf_vs_vcf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6581 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcfstats2db.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6204 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/wig2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       22 2024-04-04 14:21:30.000000 cgat-0.7.1/cgat/version.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.272001 cgat-0.7.1/cgat.egg-info/
--rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      761 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/PKG-INFO
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3604 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/SOURCES.txt
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/dependency_links.txt
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       40 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/entry_points.txt
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-04 14:30:05.000000 cgat-0.7.1/cgat.egg-info/not-zip-safe
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        5 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/top_level.txt
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       38 2024-04-04 14:46:03.272001 cgat-0.7.1/setup.cfg
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9667 2024-04-04 14:06:34.000000 cgat-0.7.1/setup.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.272001 cgat-0.7.1/tests/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      795 2024-04-01 08:10:14.000000 cgat-0.7.1/tests/testComponents.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6048 2024-04-04 14:15:54.000000 cgat-0.7.1/tests/test_commandline.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3267 2024-04-01 08:10:14.000000 cgat-0.7.1/tests/test_import.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11491 2024-04-04 12:43:35.000000 cgat-0.7.1/tests/test_scripts.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2277 2024-04-01 08:10:14.000000 cgat-0.7.1/tests/test_style.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.406953 cgat-0.7.2/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1188 2024-04-01 08:10:13.000000 cgat-0.7.2/LICENSE
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      680 2024-04-01 08:10:13.000000 cgat-0.7.2/MANIFEST.in
+-rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      761 2024-04-05 10:27:47.406953 cgat-0.7.2/PKG-INFO
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2721 2024-04-01 08:10:13.000000 cgat-0.7.2/README.md
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      734 2024-04-01 08:10:13.000000 cgat-0.7.2/THANKS.txt
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.394953 cgat-0.7.2/cgat/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2765 2024-04-04 16:06:53.000000 cgat-0.7.2/cgat/AGP.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2016 2024-04-04 08:06:46.000000 cgat-0.7.2/cgat/AString.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.394953 cgat-0.7.2/cgat/BamTools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    84091 2024-04-04 08:06:46.000000 cgat-0.7.2/cgat/BamTools/bamtools.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    73647 2024-04-01 12:48:18.000000 cgat-0.7.2/cgat/BamTools/geneprofile.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    13457 2024-04-01 12:48:18.000000 cgat-0.7.2/cgat/BamTools/peakshape.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17233 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    29497 2024-04-04 12:43:35.000000 cgat-0.7.2/cgat/Blat.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.398953 cgat-0.7.2/cgat/Components/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4766 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Components/Components.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3847 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Components/connected_components.cpp
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1734 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Components/connected_components.h
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3878 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/FastaIterator.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12895 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Fastq.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.398953 cgat-0.7.2/cgat/FastqTools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3528 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/FastqTools/fastqtools.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3108 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/GFF3.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    31953 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/GTF.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)   185318 2024-04-01 12:48:18.000000 cgat-0.7.2/cgat/GeneModelAnalysis.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    49913 2024-04-01 12:48:18.000000 cgat-0.7.2/cgat/Genomics.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1053 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Glam2.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1492 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Glam2Scan.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19547 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Histogram.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1395 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Histogram2D.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    41337 2024-04-04 12:43:35.000000 cgat-0.7.2/cgat/IndexedFasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/IndexedGenome.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11505 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Intervals.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1756 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Iterators.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5499 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/MEME.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7369 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Masker.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12153 2024-04-01 12:48:18.000000 cgat-0.7.2/cgat/MatrixTools.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2312 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Motifs.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.398953 cgat-0.7.2/cgat/NCL/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5656 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/NCL/__init__.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4148 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/NCL/_cnestedlist.pxd
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19606 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/NCL/cnestedlist.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3933 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/NCL/default.h
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    32028 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/NCL/intervaldb.c
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4921 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/NCL/intervaldb.h
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1563 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/RLE.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5705 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/RateEstimation.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40094 2024-04-04 12:43:35.000000 cgat-0.7.2/cgat/SequenceProperties.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6141 2024-04-01 12:48:18.000000 cgat-0.7.2/cgat/SetTools.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7596 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Sra.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    34513 2024-04-04 08:06:46.000000 cgat-0.7.2/cgat/Stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    20140 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Tree.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    44920 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/TreeTools.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3137 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/VCF.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.398953 cgat-0.7.2/cgat/VCFTools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25310 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/VCFTools/vcftools.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19027 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/Variants.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/__init__.py
+-rwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)     3480 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/cgat.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    28781 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/dictzip.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7542 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/makeGeneset.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.402953 cgat-0.7.2/cgat/tools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/__init__.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25343 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1895 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2bam_split_reads.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6227 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3410 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2depth.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16746 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4895 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    38204 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2geneprofile.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    37840 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16966 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2wiggle.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2502 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam2window_stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9672 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam_compare_alignments.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9070 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam_pileup2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3866 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam_vs_bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8170 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam_vs_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9174 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bam_vs_gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8328 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bams2bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3208 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bcl2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    22414 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bed2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5688 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bed2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4029 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bed2gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2181 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bed2graph.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5363 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bed2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    24191 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bed2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4857 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/bed_vs_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10208 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/beds2beds.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4295 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/beds2counts.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10672 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/cgat2dot.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5393 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/cgat_get_options.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2586 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/cgat_rebuild_extensions.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1033 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/cgat_script_template.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1470 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/csv2csv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10096 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/csvs2csv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9275 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/data2histogram.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7781 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/diff_bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11704 2024-04-01 12:48:18.000000 cgat-0.7.2/cgat/tools/diff_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    15078 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/diff_chains.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9500 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/diff_fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14426 2024-04-01 12:48:18.000000 cgat-0.7.2/cgat/tools/diff_gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6238 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/extract_stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10207 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fasta2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    21393 2024-04-01 12:48:18.000000 cgat-0.7.2/cgat/tools/fasta2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14562 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fasta2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5500 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fasta2kmercontent.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2682 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fasta2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12477 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fasta2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3771 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fasta2variants.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2536 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fasta2vcf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2281 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastas2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1884 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastq2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17342 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastq2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5343 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastq2summary.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6364 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastq2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12133 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastq2tpm.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1337 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastq2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5041 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastqs2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3534 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastqs2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9491 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/fastqs2fastqs.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2597 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/genome_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5443 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gff2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11034 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gff2coverage.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14023 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gff2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    30644 2024-04-04 16:06:53.000000 cgat-0.7.2/cgat/tools/gff2gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9967 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gff2histogram.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4537 2024-04-04 12:43:35.000000 cgat-0.7.2/cgat/tools/gff2psl.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7200 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gff2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14982 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gff2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12848 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gff32gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    18122 2024-04-04 08:06:46.000000 cgat-0.7.2/cgat/tools/gtf2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40355 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gtf2gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    52205 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gtf2gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    39563 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gtf2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11698 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gtf2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11190 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/gtfs2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4123 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/index2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12771 2024-04-01 13:26:07.000000 cgat-0.7.2/cgat/tools/index_fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6509 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/split_fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7956 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/split_file.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/split_gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3071 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/table2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2346 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/table2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9522 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/tables2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11183 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/vcf2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14736 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/vcf2vcf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8970 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/vcf_compare_phase.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6901 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/vcf_stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3447 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/vcf_vs_vcf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6581 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/vcfstats2db.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6204 2024-04-01 08:10:13.000000 cgat-0.7.2/cgat/tools/wig2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       22 2024-04-05 10:27:37.000000 cgat-0.7.2/cgat/version.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.394953 cgat-0.7.2/cgat.egg-info/
+-rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      761 2024-04-05 10:27:47.000000 cgat-0.7.2/cgat.egg-info/PKG-INFO
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3617 2024-04-05 10:27:47.000000 cgat-0.7.2/cgat.egg-info/SOURCES.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-05 10:27:47.000000 cgat-0.7.2/cgat.egg-info/dependency_links.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       40 2024-04-05 10:27:47.000000 cgat-0.7.2/cgat.egg-info/entry_points.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-04 14:30:05.000000 cgat-0.7.2/cgat.egg-info/not-zip-safe
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        5 2024-04-05 10:27:47.000000 cgat-0.7.2/cgat.egg-info/top_level.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:17:00.000000 cgat-0.7.2/requires.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       38 2024-04-05 10:27:47.406953 cgat-0.7.2/setup.cfg
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10750 2024-04-05 10:15:49.000000 cgat-0.7.2/setup.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-05 10:27:47.402953 cgat-0.7.2/tests/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      795 2024-04-01 08:10:14.000000 cgat-0.7.2/tests/testComponents.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6048 2024-04-04 16:06:53.000000 cgat-0.7.2/tests/test_commandline.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3267 2024-04-01 08:10:14.000000 cgat-0.7.2/tests/test_import.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11491 2024-04-04 12:43:35.000000 cgat-0.7.2/tests/test_scripts.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2277 2024-04-01 08:10:14.000000 cgat-0.7.2/tests/test_style.py
```

### Comparing `cgat-0.7.1/LICENSE` & `cgat-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/MANIFEST.in` & `cgat-0.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/PKG-INFO` & `cgat-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgat
-Version: 0.7.1
+Version: 0.7.2
 Summary: cgat : the Computational Genomics Analysis Toolkit
 Home-page: http://www.cgat.org/cgat/Tools/
 Author: Andreas Heger
 Author-email: andreas.heger@gmail.com
 License: MIT
 Keywords: computational genomics
 Platform: any
```

### Comparing `cgat-0.7.1/README.md` & `cgat-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/THANKS.txt` & `cgat-0.7.2/THANKS.txt`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/AGP.py` & `cgat-0.7.2/cgat/AGP.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/AString.py` & `cgat-0.7.2/cgat/AString.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/BamTools/bamtools.pyx` & `cgat-0.7.2/cgat/BamTools/bamtools.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/BamTools/geneprofile.pyx` & `cgat-0.7.2/cgat/BamTools/geneprofile.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/BamTools/peakshape.pyx` & `cgat-0.7.2/cgat/BamTools/peakshape.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Bed.py` & `cgat-0.7.2/cgat/Bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Blat.py` & `cgat-0.7.2/cgat/Blat.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Components/Components.pyx` & `cgat-0.7.2/cgat/Components/Components.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Components/connected_components.cpp` & `cgat-0.7.2/cgat/Components/connected_components.cpp`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Components/connected_components.h` & `cgat-0.7.2/cgat/Components/connected_components.h`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/FastaIterator.py` & `cgat-0.7.2/cgat/FastaIterator.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Fastq.py` & `cgat-0.7.2/cgat/Fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/FastqTools/fastqtools.pyx` & `cgat-0.7.2/cgat/FastqTools/fastqtools.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/GFF3.py` & `cgat-0.7.2/cgat/GFF3.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/GTF.py` & `cgat-0.7.2/cgat/GTF.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/GeneModelAnalysis.pyx` & `cgat-0.7.2/cgat/GeneModelAnalysis.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Genomics.py` & `cgat-0.7.2/cgat/Genomics.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Glam2.py` & `cgat-0.7.2/cgat/Glam2.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Glam2Scan.py` & `cgat-0.7.2/cgat/Glam2Scan.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Histogram.py` & `cgat-0.7.2/cgat/Histogram.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Histogram2D.py` & `cgat-0.7.2/cgat/Histogram2D.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/IndexedFasta.py` & `cgat-0.7.2/cgat/IndexedFasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/IndexedGenome.py` & `cgat-0.7.2/cgat/IndexedGenome.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Intervals.py` & `cgat-0.7.2/cgat/Intervals.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Iterators.py` & `cgat-0.7.2/cgat/Iterators.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/MEME.py` & `cgat-0.7.2/cgat/MEME.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Masker.py` & `cgat-0.7.2/cgat/Masker.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/MatrixTools.py` & `cgat-0.7.2/cgat/MatrixTools.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Motifs.py` & `cgat-0.7.2/cgat/Motifs.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/NCL/__init__.py` & `cgat-0.7.2/cgat/NCL/__init__.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/NCL/_cnestedlist.pxd` & `cgat-0.7.2/cgat/NCL/_cnestedlist.pxd`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/NCL/cnestedlist.pyx` & `cgat-0.7.2/cgat/NCL/cnestedlist.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/NCL/default.h` & `cgat-0.7.2/cgat/NCL/default.h`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/NCL/intervaldb.c` & `cgat-0.7.2/cgat/NCL/intervaldb.c`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/NCL/intervaldb.h` & `cgat-0.7.2/cgat/NCL/intervaldb.h`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/RLE.py` & `cgat-0.7.2/cgat/RLE.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/RateEstimation.py` & `cgat-0.7.2/cgat/RateEstimation.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/SequenceProperties.py` & `cgat-0.7.2/cgat/SequenceProperties.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/SetTools.py` & `cgat-0.7.2/cgat/SetTools.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Sra.py` & `cgat-0.7.2/cgat/Sra.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Stats.py` & `cgat-0.7.2/cgat/Stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Tree.py` & `cgat-0.7.2/cgat/Tree.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/TreeTools.py` & `cgat-0.7.2/cgat/TreeTools.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/VCF.py` & `cgat-0.7.2/cgat/VCF.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/VCFTools/vcftools.pyx` & `cgat-0.7.2/cgat/VCFTools/vcftools.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/Variants.py` & `cgat-0.7.2/cgat/Variants.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/cgat.py` & `cgat-0.7.2/cgat/cgat.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/dictzip.py` & `cgat-0.7.2/cgat/dictzip.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/makeGeneset.py` & `cgat-0.7.2/cgat/makeGeneset.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2bam.py` & `cgat-0.7.2/cgat/tools/bam2bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2bam_split_reads.py` & `cgat-0.7.2/cgat/tools/bam2bam_split_reads.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2bed.py` & `cgat-0.7.2/cgat/tools/bam2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2depth.py` & `cgat-0.7.2/cgat/tools/bam2depth.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2fasta.py` & `cgat-0.7.2/cgat/tools/bam2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2fastq.py` & `cgat-0.7.2/cgat/tools/bam2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2geneprofile.py` & `cgat-0.7.2/cgat/tools/bam2geneprofile.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2stats.py` & `cgat-0.7.2/cgat/tools/bam2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2wiggle.py` & `cgat-0.7.2/cgat/tools/bam2wiggle.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam2window_stats.py` & `cgat-0.7.2/cgat/tools/bam2window_stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam_compare_alignments.py` & `cgat-0.7.2/cgat/tools/bam_compare_alignments.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam_pileup2tsv.py` & `cgat-0.7.2/cgat/tools/bam_pileup2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam_vs_bam.py` & `cgat-0.7.2/cgat/tools/bam_vs_bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam_vs_bed.py` & `cgat-0.7.2/cgat/tools/bam_vs_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bam_vs_gtf.py` & `cgat-0.7.2/cgat/tools/bam_vs_gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bams2bam.py` & `cgat-0.7.2/cgat/tools/bams2bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bcl2fastq.py` & `cgat-0.7.2/cgat/tools/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bed2bed.py` & `cgat-0.7.2/cgat/tools/bed2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bed2fasta.py` & `cgat-0.7.2/cgat/tools/bed2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bed2gff.py` & `cgat-0.7.2/cgat/tools/bed2gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bed2graph.py` & `cgat-0.7.2/cgat/tools/bed2graph.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bed2stats.py` & `cgat-0.7.2/cgat/tools/bed2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bed2table.py` & `cgat-0.7.2/cgat/tools/bed2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/bed_vs_bed.py` & `cgat-0.7.2/cgat/tools/bed_vs_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/beds2beds.py` & `cgat-0.7.2/cgat/tools/beds2beds.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/beds2counts.py` & `cgat-0.7.2/cgat/tools/beds2counts.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/cgat2dot.py` & `cgat-0.7.2/cgat/tools/cgat2dot.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/cgat_get_options.py` & `cgat-0.7.2/cgat/tools/cgat_get_options.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/cgat_rebuild_extensions.py` & `cgat-0.7.2/cgat/tools/cgat_rebuild_extensions.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/cgat_script_template.py` & `cgat-0.7.2/cgat/tools/cgat_script_template.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/csv2csv.py` & `cgat-0.7.2/cgat/tools/csv2csv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/csvs2csv.py` & `cgat-0.7.2/cgat/tools/csvs2csv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/data2histogram.py` & `cgat-0.7.2/cgat/tools/data2histogram.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/diff_bam.py` & `cgat-0.7.2/cgat/tools/diff_bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/diff_bed.py` & `cgat-0.7.2/cgat/tools/diff_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/diff_chains.py` & `cgat-0.7.2/cgat/tools/diff_chains.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/diff_fasta.py` & `cgat-0.7.2/cgat/tools/diff_fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/diff_gtf.py` & `cgat-0.7.2/cgat/tools/diff_gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/extract_stats.py` & `cgat-0.7.2/cgat/tools/extract_stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fasta2bed.py` & `cgat-0.7.2/cgat/tools/fasta2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fasta2fasta.py` & `cgat-0.7.2/cgat/tools/fasta2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fasta2fastq.py` & `cgat-0.7.2/cgat/tools/fasta2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fasta2kmercontent.py` & `cgat-0.7.2/cgat/tools/fasta2kmercontent.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fasta2stats.py` & `cgat-0.7.2/cgat/tools/fasta2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fasta2table.py` & `cgat-0.7.2/cgat/tools/fasta2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fasta2variants.py` & `cgat-0.7.2/cgat/tools/fasta2variants.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fasta2vcf.py` & `cgat-0.7.2/cgat/tools/fasta2vcf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastas2fasta.py` & `cgat-0.7.2/cgat/tools/fastas2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastq2fasta.py` & `cgat-0.7.2/cgat/tools/fastq2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastq2fastq.py` & `cgat-0.7.2/cgat/tools/fastq2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastq2summary.py` & `cgat-0.7.2/cgat/tools/fastq2summary.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastq2table.py` & `cgat-0.7.2/cgat/tools/fastq2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastq2tpm.py` & `cgat-0.7.2/cgat/tools/fastq2tpm.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastq2tsv.py` & `cgat-0.7.2/cgat/tools/fastq2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastqs2fasta.py` & `cgat-0.7.2/cgat/tools/fastqs2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastqs2fastq.py` & `cgat-0.7.2/cgat/tools/fastqs2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/fastqs2fastqs.py` & `cgat-0.7.2/cgat/tools/fastqs2fastqs.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/genome_bed.py` & `cgat-0.7.2/cgat/tools/genome_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gff2bed.py` & `cgat-0.7.2/cgat/tools/gff2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gff2coverage.py` & `cgat-0.7.2/cgat/tools/gff2coverage.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gff2fasta.py` & `cgat-0.7.2/cgat/tools/gff2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gff2gff.py` & `cgat-0.7.2/cgat/tools/gff2gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gff2histogram.py` & `cgat-0.7.2/cgat/tools/gff2histogram.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gff2psl.py` & `cgat-0.7.2/cgat/tools/gff2psl.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gff2stats.py` & `cgat-0.7.2/cgat/tools/gff2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gff2table.py` & `cgat-0.7.2/cgat/tools/gff2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gff32gtf.py` & `cgat-0.7.2/cgat/tools/gff32gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gtf2fasta.py` & `cgat-0.7.2/cgat/tools/gtf2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gtf2gff.py` & `cgat-0.7.2/cgat/tools/gtf2gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gtf2gtf.py` & `cgat-0.7.2/cgat/tools/gtf2gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gtf2table.py` & `cgat-0.7.2/cgat/tools/gtf2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gtf2tsv.py` & `cgat-0.7.2/cgat/tools/gtf2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/gtfs2tsv.py` & `cgat-0.7.2/cgat/tools/gtfs2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/index2bed.py` & `cgat-0.7.2/cgat/tools/index2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/index_fasta.py` & `cgat-0.7.2/cgat/tools/index_fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/split_fasta.py` & `cgat-0.7.2/cgat/tools/split_fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/split_file.py` & `cgat-0.7.2/cgat/tools/split_file.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/split_gff.py` & `cgat-0.7.2/cgat/tools/split_gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/table2stats.py` & `cgat-0.7.2/cgat/tools/table2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/table2table.py` & `cgat-0.7.2/cgat/tools/table2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/tables2table.py` & `cgat-0.7.2/cgat/tools/tables2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/vcf2tsv.py` & `cgat-0.7.2/cgat/tools/vcf2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/vcf2vcf.py` & `cgat-0.7.2/cgat/tools/vcf2vcf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/vcf_compare_phase.py` & `cgat-0.7.2/cgat/tools/vcf_compare_phase.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/vcf_stats.py` & `cgat-0.7.2/cgat/tools/vcf_stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/vcf_vs_vcf.py` & `cgat-0.7.2/cgat/tools/vcf_vs_vcf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/vcfstats2db.py` & `cgat-0.7.2/cgat/tools/vcfstats2db.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat/tools/wig2bed.py` & `cgat-0.7.2/cgat/tools/wig2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/cgat.egg-info/PKG-INFO` & `cgat-0.7.2/cgat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgat
-Version: 0.7.1
+Version: 0.7.2
 Summary: cgat : the Computational Genomics Analysis Toolkit
 Home-page: http://www.cgat.org/cgat/Tools/
 Author: Andreas Heger
 Author-email: andreas.heger@gmail.com
 License: MIT
 Keywords: computational genomics
 Platform: any
```

### Comparing `cgat-0.7.1/cgat.egg-info/SOURCES.txt` & `cgat-0.7.2/cgat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 THANKS.txt
+requires.txt
 setup.py
 cgat/AGP.py
 cgat/AString.py
 cgat/Bed.py
 cgat/Blat.py
 cgat/FastaIterator.py
 cgat/Fastq.py
```

### Comparing `cgat-0.7.1/setup.py` & `cgat-0.7.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,14 +133,45 @@
     return None
 
 REPO_REQUIREMENT = re.compile(
     r'^-e (?P<link>(?P<vcs>git|svn|hg|bzr).+#egg=(?P<package>.+)-(?P<version>\d(?:\.\d)*))$')
 HTTPS_REQUIREMENT = re.compile(
     r'^-e (?P<link>.*).+#(?P<package>.+)-(?P<version>\d(?:\.\d)*)$')
 install_requires = []
+dependency_links = []
+
+for requirement in (
+        l.strip() for l in open('requires.txt') if not l.startswith("#")):
+    match = REPO_REQUIREMENT.match(requirement)
+    if match:
+        assert which(match.group('vcs')) is not None, \
+            ("VCS '%(vcs)s' must be installed in order to "
+             "install %(link)s" % match.groupdict())
+        install_requires.append("%(package)s==%(version)s" % match.groupdict())
+        dependency_links.append(match.group('link'))
+        continue
+
+    if requirement.startswith("https"):
+        install_requires.append(requirement)
+        continue
+
+    match = HTTPS_REQUIREMENT.match(requirement)
+    if match:
+        install_requires.append("%(package)s>=%(version)s" % match.groupdict())
+        dependency_links.append(match.group('link'))
+        continue
+
+    install_requires.append(requirement)
+
+if major == 2:
+    install_requires.extend(['web.py>=0.37',
+                             'xlwt>=0.7.4',
+                             'matplotlib-venn>=0.5'])
+elif major == 3:
+    pass
 
 cgat_packages = find_packages()
 cgat_package_dirs = {'cgat': 'cgat'}
 
 ##########################################################
 ##########################################################
 # classifiers
@@ -282,14 +313,15 @@
     package_dir=cgat_package_dirs,
     include_package_data=True,
     entry_points={
         'console_scripts': ['cgat = cgat.cgat:main']
     },
     # dependencies
     install_requires=install_requires,
+    dependency_links=dependency_links,
     # extension modules
     ext_modules=extensions,
     cmdclass={'build_ext': build_ext},
     # other options
     zip_safe=False,
     test_suite="tests",
 )
```

### Comparing `cgat-0.7.1/tests/testComponents.py` & `cgat-0.7.2/tests/testComponents.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/tests/test_commandline.py` & `cgat-0.7.2/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/tests/test_import.py` & `cgat-0.7.2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/tests/test_scripts.py` & `cgat-0.7.2/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.1/tests/test_style.py` & `cgat-0.7.2/tests/test_style.py`

 * *Files identical despite different names*

