# Sanger Quality Trimming
Workflow for manual quality anlysis and trimming of phred-scored sequence reads.

## Background

This script was created as a medium-throughput sequence quality analysis, for manual investigation of sequence reads with phred quality scores, and bulk alignment of said assessed reads against the genome of your choice. 

It is designed for the beginner coder more comfortable with interactive genome browser tools, but for cases in which Snapgene and similar program default thresholds may provide infavorable or inaccurate results (ie. sanger sequencing reads of low quality, or specialized cases such as accurate detection of random transposon insertions).

## Workflow Steps

This markdown document requires import of files that contain 

1. A DNA sequence
2. Associated phred quality scores

These can be generated using many bash tools and interactive genome browsers. Test cases for this script were performed on tsv files, originally as ab1 files imported into Snapgene, which were then exported as tsv files.

The Rmd template has four sections:

1. Background/Objective

2. Function Modules (3), to be run before data import/analysis. These code modules will create three functions that can each be run as a single command on imported data.

3. Worfklow Section, where data will be imported and analyses/subsequent multi-fasta export are completed. This is also contained in a code chunk, but the chunk should not be run all at once. Instead, import your data, run through the manual process of evaluating each of your spectra files, and gather those results sample by sample into a single dataframe (template code provides all necessary steps).

4. Next Steps. Once your dataframe of trimmed reads is complete and exported as a multi-fasta file, it can be aligned to the relevant genome using any alignment tool you are comfrotable with (command line or interactive software).


