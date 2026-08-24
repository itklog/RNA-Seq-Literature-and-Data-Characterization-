# RNA-Seq Analysis: Heat Stress-Induced Transposon Activation in *Arabidopsis*

**Name:** Martinez, Jen Marie A.
**Group:** Group I
**Research Article:** *Heat stress-induced transposon activation correlates with 3D chromatin organization rearrangement in Arabidopsis*

## Citation

Sun, L., Jing, Y., Liu, X., Li, Q., Xue, Z., Cheng, Z., Wang, D., He, H., & Qian, W. (2020). Heat stress-induced transposon activation correlates with 3D chromatin organization rearrangement in *Arabidopsis*. *Nature Communications, 11*(1), 1886. https://doi.org/10.1038/s41467-020-15809-5 

## Assigned Accession: 

SRX6027532

## Control or Treatment Condition

RNA-Seq-Col-Recover-Rep1

## Biological Description

This sample represents a biological replicate of Arabidopsis thaliana (Columbia/Col) seedlings collected during the recovery phase following heat stress. It was analyzed by RNA sequencing to examine changes in gene expression associated with the plant's response and recovery from heat stress.

## Sequencing Layout

Paired-end

## Number of Reads

R1: 27037331
R2: 27037331

## Read Length

R1: 150 bp
R2: 150 bp

## GC Content

R1: 46 %
R2: 46 %

## Summary of FASTQC Report

Both forward and reverse reads showed high overall sequence quality and consistent GC content, with no poor-quality sequences. However, both showed failed per-base sequence content and duplication levels, as well as warnings for overrepresented sequences and adapter contamination.

## Screenshots

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/f5dbf48d-2414-4e1b-b6ea-b39a0070c52e" />
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/9820b7b5-42b1-4556-9cfd-dfa2af45c485" />
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/56c48bd2-459e-49a6-88d1-86120efeaaf8" />
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/495c7dea-4135-400d-aedb-ddfc9c8b21a4" />
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/7b9113e1-0e32-425c-ae84-717022d2f3be" />



## RNA-seq Interpretation

The study aimed to determine how acute heat stress and recovery influence gene expression and transposable element activity in Arabidopsis thaliana seedlings, allowing the authors to examine stress-induced transcriptional changes at a genome-wide scale. Genomic DNA serves as the permanent genetic blueprint, whereas RNA molecules are temporary transcripts produced when genes are expressed. Therefore, RNA-seq provides information about functional gene activity rather than simply the genetic potential of the organism. A biological replicate is an independent sample from the same experimental condition, such as separate seedlings exposed to heat stress, and is important because it accounts for natural biological variation and increases the reliability of differential gene expression results. Single-end sequencing reads one end of a DNA fragment, while paired-end sequencing reads both ends, providing greater alignment accuracy and additional structural information. A FASTQ file is a text-based format containing raw sequencing reads and their corresponding per-base quality scores, making it a standard input for downstream RNA-seq analysis. FastQC evaluates sequencing quality through metrics such as per-base sequence quality, GC content, adapter contamination, sequence duplication, and sequence composition. A high per-base sequence quality score indicates a low probability of sequencing errors, meaning the reads are generally reliable for downstream analysis. Adapter contamination occurs when artificial adapter sequences remain in the reads and may interfere with alignment and gene quantification, so they may need to be removed through trimming. In our group, all RNA-seq samples were similar in quality because they showed the same FastQC results, indicating consistently good sequencing quality across the different accessions. None of the samples showed a possible quality problem because all samples passed the quality checks. Before comparing gene expression between control and treatment samples, the researchers would need to trim adapters and low-quality reads if necessary, align the reads to a reference genome or quantify transcripts, obtain gene-level read counts, normalize the counts to account for differences in sequencing depth, and perform statistical differential gene expression analysis to identify significantly differentially expressed genes.

## Conclusion

The RNA-seq samples showed good and consistent sequencing quality based on the FastQC results. No major quality problems were observed, as all samples passed the quality checks. The results indicate that the data are suitable for further RNA-seq analysis. However, additional steps such as read alignment, gene quantification, normalization, and differential expression analysis are needed to compare gene expression between control and treatment samples.




