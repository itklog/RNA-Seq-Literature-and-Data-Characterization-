# RNA-Seq Data Characterization Report

**Student Name:** Eugene Kim Ansag  
**Group Number:** Group 1 – Heat Stress  
**Assigned RNA-seq Accession:** `SRR9257065`  
**Assigned Sample:** `Recovery_Rep2`

## Study Information and Citation
### Group Paper
**Title:** Heat stress-induced transposon activation correlates with 3D chromatin organization rearrangement in Arabidopsis

**Full Citation:**  
Sun, L., Jing, Y., Liu, X. et al. Heat stress-induced transposon activation correlates with 3D chromatin organization rearrangement in Arabidopsis. Nat Commun 11, 1886 (2020). https://doi.org/10.1038/s41467-020-15809-5

**Study Accession / BioProject:** PRJNA547995 (SRP200947)


**Organism:** *Arabidopsis thaliana* (Col-0 ecotype)

---

## Assigned RNA-seq Sample

| RNA-seq Information | Details |
|---|---|
| **Student Name** | Eugene Kim Ansag |
| **Group Number** | Group 1 – Heat Stress |
| **SRA Run Accession** | `SRR9257065` |
| **BioSample Accession** | `SAMN11997382` |
| **Sample** | `Recovery_Rep2` |
| **Experimental Condition** | Heat-stress recovery |
| **Organism** | *Arabidopsis thaliana* |
| **Ecotype** | Col-0 |
| **Sequencing Layout** | Paired-end |
| **Number of Reads / Sequences** | 26,237,461 |
| **Read Length** | 150 bp |
| **GC Content** | 46% |

---

## Biological Representation of the Sample

The assigned sample, `Recovery_Rep2`, represents *Arabidopsis thaliana* Col-0 seedlings collected during the recovery phase following heat-stress exposure. Therefore, the sample reflects the transcriptional state of the seedlings after heat treatment rather than the immediate response during acute heat exposure.

The recovery sample can provide information about gene-expression patterns that persist, decrease, or begin to return toward the normal state following heat stress. It is also relevant to the study's investigation of heat-associated changes in transposable-element activity.


---

## Galaxy and RNA-seq Data Documentation

### **Figure 1. Galaxy History**

<img width="2560" height="1600" alt="1000040804" src="https://github.com/user-attachments/assets/99815057-c378-4d93-a339-695ec2e52adf" />

**Figure 1.** Galaxy history showing the imported `Recovery_Rep2`
RNA-seq dataset and the analysis steps performed in Galaxy.


### **Figure 2. SRA Run Accession and Dataset Information**

<img width="2560" height="1600" alt="1000040808" src="https://github.com/user-attachments/assets/69f3d2ef-ef5f-4bb2-9bfa-f323343b29f1" />


**Figure 2.** SRA run information for the assigned RNA-seq dataset
`SRR9257065`, including the run accession and associated sequencing
information.

### **Figure 3. FastQC Raw Data Results**

FastQC was used to examine the basic characteristics and quality of the
raw paired-end RNA-seq reads. The results include important sequencing
metrics such as the number of sequences, read length, and GC content.

<img width="2560" height="1600" alt="1000040811" src="https://github.com/user-attachments/assets/770b7fff-f9c5-4edd-bcad-fe75990f1674" />


**Figure 3.** FastQC raw-data results for the `Recovery_Rep2` RNA-seq
sample showing the basic sequencing characteristics, including sequence
count, read length, and GC content.

**Interpretation:**  
The FastQC results showed passing results for Basic Statistics, Per Base
Sequence Quality, and Per Sequence GC Content. Warnings were observed for
Adapter Content and Overrepresented Sequences, while Per Base Sequence
Content and Sequence Duplication Levels were flagged as failures.

The dataset contained 26,237,461 reads for both R1 and R2, with a read
length of 150 bp and approximately 46% GC content. The Sequence Duplication
Levels result indicated relatively high duplication, with approximately
37.8% of R1 reads and 40.5% of R2 reads classified as deduplicated
(unique) sequences. These results indicate potential duplication and
adapter-related quality concerns in the raw RNA-seq data that should be
considered during subsequent quality-control and downstream processing.

## Interpretation Questions 

1. What biological question was the original RNA-seq study trying to answer?
- The study investigated how acute heat stress and subsequent recovery alter genome-wide gene expression and transposable     element (TE) activity in Arabidopsis thaliana seedlings, providing insight into transcriptional responses to thermal stress.
2. Why did the authors use RNA-seq instead of only examining the genome?
- RNA-seq was used to characterize the transcriptome, allowing the researchers to measure actively expressed genes and TEs. In contrast, genomic DNA primarily represents the organism's genetic potential rather than its condition-specific transcriptional activity.
3. What is the difference between genomic DNA and the RNA molecules measured by RNA-seq?
- Genomic DNA is the relatively stable hereditary genetic material, whereas RNA molecules are transient transcripts generated through gene expression. RNA-seq therefore provides a molecular profile of active transcription under specific physiological conditions.
4. What is a biological replicate and why is it important?
- A biological replicate is an independently derived sample subjected to the same experimental condition. Replicates capture natural biological variability, improve statistical power, and increase the reliability of differential gene-expression analysis.
5. What is the difference between single-end and paired-end sequencing?
- Single-end sequencing determines the sequence from one end of a nucleic-acid fragment, whereas paired-end sequencing sequences both ends. Paired-end reads generally provide greater mapping confidence and structural information, particularly across repetitive or complex genomic regions.
6. What is a FASTQ file?
- A FASTQ file is a text-based format containing raw nucleotide sequences and their corresponding per-base Phred quality scores. It serves as a primary input for RNA-seq quality control and downstream computational analysis.
7. What information does FastQC provide?
- FastQC evaluates sequencing quality using metrics including per-base sequence quality, GC-content distribution, adapter contamination, sequence duplication, and nucleotide composition bias. These metrics help identify technical artifacts before downstream analysis.
8. What does a high per-base quality score indicate?
- A high Phred quality score indicates a low probability of base-calling error, reflecting accurate sequencing and increasing confidence in subsequent read alignment and transcript quantification.
9. Why can adapter contamination be a problem?
- Adapter contamination occurs when artificial library-preparation sequences remain within sequencing reads. These sequences can interfere with read alignment and transcript quantification, potentially producing spurious mappings and biased expression estimates; therefore, adapter trimming is required.
10. Were all RNA-seq samples in your group similar in quality? Explain.
- The samples were generally comparable in overall sequencing quality, with all exhibiting 150-bp reads, approximately 45–46% GC content, and acceptable per-base quality scores. However, variation was observed in adapter contamination, nucleotide-composition bias, and sequence duplication, indicating differences in library-level quality.
11. Did any sample show a possible quality problem? What was it?
- Yes. SRX6027532 (Recovery Rep1) exhibited the most notable QC concerns, including adapter contamination, overrepresented sequences, nucleotide-composition bias, and sequence duplication. SRX6027530 also showed adapter/primer bias, whereas SRX6027531 and SRX6027528 exhibited sequence-composition and duplication-related issues.
12. What additional steps would be needed before the researchers could compare gene expression between control and treatment samples?
- The datasets should undergo adapter/primer trimming, quality filtering, and removal of low-quality or contaminant reads. The cleaned reads should then be aligned to the reference genome and subjected to transcript quantification and normalization. Finally, biological replicates should be incorporated into appropriate statistical differential-expression analyses to reliably compare control and heat-stressed samples.





## Conclusion
  The examination of the `SRR9257065` (`Recovery_Rep2`) RNA-seq dataset
provided an understanding of how raw sequencing data can be characterized
in the context of a heat-stress study in *Arabidopsis thaliana*. The dataset
contained 26,237,461 paired-end reads of 150 bp with approximately 46% GC
content, while FastQC revealed generally acceptable basic sequencing
characteristics but also identified concerns involving adapter content,
overrepresented sequences, per-base sequence composition, and sequence
duplication. These findings demonstrate that raw RNA-seq data must be
carefully assessed for quality and sequence characteristics before being
used for downstream analyses, since technical features of the reads can
influence subsequent interpretation. Overall, tracing the sample from its
public SRA accession through FASTQ inspection and FastQC analysis helped
establish how raw sequencing data are connected to the biological question
of understanding transcriptional responses associated with heat stress and
recovery.
