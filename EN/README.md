# English guide

This is a practical, paired-end short-read RNA-seq walkthrough. It covers the core path from raw FASTQ files to expression count matrices and functional annotation.

## Chapters

1. [Quality control](1.quality_control.md): clean paired-end reads with fastp and generate QC reports
2. [Alignment](2.alignment.md): prepare the reference, align reads with HISAT2, then sort and index BAM files with samtools
3. [Quantification and annotation](3.quantification.md): quantify with StringTie and continue with gffread, TransDecoder, and eggNOG-mapper

The original Chinese notes are indexed in the [Chinese guide](../CN/README.md).

## Before you start

- This repository is a learning guide and command template, not a production-ready automated workflow.
- The examples assume paired-end data named `<sample>_1.fq.gz` and `<sample>_2.fq.gz`.
- Replace every example path, sample name, thread count, and reference filename before running a command.
- The reference FASTA and GTF/GFF must use the same assembly and matching chromosome/contig names.
- Record tool versions, commands, and logs, and test the workflow on a small subset first.
