# Predict_IAV_Host
Machine Learning Predicts Human-adaptative Influenza A Viruses Based on Viral Nucleotide Composition

## Overview

This project aims to calculate and analyze the composition of mono-nucleotides and dinucleotides in the coding region of influenza genomic sequences. The project includes sequence editing, the counting of mono-nucleotides and dinucleotides and the machine learning analysis. The scripts for all figures and supplementary figures were also provided.

## Installation Dependencies:
Python 3.6
Sklearn 0.18.1
Pandas 0.20.1
Numpy 1.12.1
Scipy 0.19.0
Seaborn 0.7.1
Biopython 1.74 

## Description
Script-1 was utilized to extract ID, strain name, sequence length, and other labels. It consists of the following scripts:
A_dropout_repeat_seqs.py
B_dropout_out_of_seq_len_range.py
C_batch_CDS_Seq_ID_isolation.py

Script-2 was utilized to count and calculate nts and dnts respectively at each of the three types of nucleotide position within a trinucleotide code. It consists of the following scripts:
D_batch_CDS_nt_count_DF.py
E_batch_CDS_dnt_count_DF.py

All following sequence counting, statistical analysis, the analysis with machine learning methods were performed based on data (in the format of csv), which were produced by above-mentioned methods. Some items in the csv file was edited manually with excel software.

The resampling to keep approximately 1:1 of USA to China for each segment was performed with “Script-3, df_all_usa_resampled.py”.

The data split was performed with “Script-4, data_split.py”
fasta sequence files:
IAV_avian.fasta
IAV_human.fasta
IAV_swine.fasta,
Above-mentioned three fasta sequence files were downloaded from IRD website.

gisaid_epiflu_sequence.fasta
Above-mentioned fasta sequence file was downloaded from GISAID website.

