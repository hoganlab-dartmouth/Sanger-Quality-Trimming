# Sanger-Quality-Trimming
Workflow for manual quality anlysis and trimming of phred-scored sequence reads.

## Background

This script was created as a medium-throughput sequence quality analysis, for manual investigation of sequence reads with phred quality scores. 

It is designed for the beginner coder more comfortable with interactive genome browser tools, but for cases in which Snapgene and similar program default thresholds may provide infavorable or inaccurate results (ie. sanger sequencing reads of low quality, or specialized cases such as accurate detection of random transposon insertions).

## Workflow Steps

This markdown document requires import of files that contain 

1. A DNA sequence
2. Associated phred quality scores

These can be generated using many bash tools and interactive genome browsers. Test cases for this script were performed on tsv files, originally as ab1 files imported into Snapgene, which were then exported as tsv files.
