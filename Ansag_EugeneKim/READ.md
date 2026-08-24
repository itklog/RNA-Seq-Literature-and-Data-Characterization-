# RNA-Seq Data Characterization Report

**Student Name:** Eugene Kim Ansag  
**Group Number:** Group 1 – Heat Stress  
**Assigned RNA-seq Accession:** `SRR9257065`  
**Assigned Sample:** `Recovery_Rep2`

## Study Information and Citation
### Group Paper
**Title:** Heat stress-induced transposon activation correlates with 3D chromatin organization rearrangement in Arabidopsis

**Full Citation:**  
Ma, Q., Tharwat, M., Alshanbari, F. A., Khan, M. Z., Zhang, X., Zhang, Y., Hu, Y., Li, X., & Hu, Y. (2020). *Heat stress triggers genome-wide release of transposable elements in Arabidopsis*. *Plant Physiology*.

**DOI:** https://doi.org/10.1038/s41467-020-15809-5

**Study Accession / BioProject:** SRX6027533

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
