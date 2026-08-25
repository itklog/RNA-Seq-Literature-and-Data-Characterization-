#  RNA-Seq Data Characterization Report

**• Student Name: Jerson Lloyd T. Ortega**

**• Group Number: Group 1 (Heat Stress)**

**• Assigned Sample: RNA-Seq-Col-Control-Rep1**


#  Study Information & Citation

**Paper Title:** Heat stress triggers genome‑wide release of transposable elements in Arabidopsis

**Full Citation:** Ma, Q., Tharwat, M., Alshanbari, F. A., Khan, M. Z., Zhang, X., Zhang, Y., Hu, Y., Li, X., & Hu, Y. (2020). Heat stress triggers genome‑wide release of transposable elements in Arabidopsis. Plant Physiology.

**Organism:** Arabidopsis thaliana (Col‑0 ecotype)**Assigned RNA-seq Accession:** SRR9257060**Experimental Condition:** Acute Heat Stress (Treatment)

**Biological Representation:** This sample represents whole Arabidopsis thaliana (Col-0 ecotype) seedlings exposed to acute heat stress (Replicate 2). Biologically, it captures the genome-wide transcriptional responses, heat-shock gene activation, and transposable element expression dynamics under elevated temperature conditions compared to thermoneutral control growth.

#  Dataset Characteristics and Summary
| RNA - Seq Metric | Value / Observation |
| :--- | :--- |
| SRA Run Accession | `SRR9257060` |
| BioSample Accession | `SAMN11997387` |
| Sequencing Layout | Paired - End |
| Number of Reads / Sequences | `33,115,474` |
| Read Length | 150 bp |
| GC Content | `46%` |
| Approximate File Size | 3.4 GB |

**Summary of FastQC Results:** Passed basic statistics and quality scores, but failures were observed for per base sequence content and sequence duplication levels.


#  Screenshots and Visualizations

<img width="1080" height="2066" alt="20392" src="https://github.com/user-attachments/assets/7f31d645-1002-40df-96cd-effe2488dffc" />

**Figure 1:** Galaxy History - Galaxy history panel showing the imported RNA-seq dataset and completed FastQC outputs.

<img width="1080" height="560" alt="20401" src="https://github.com/user-attachments/assets/bb57c30f-c55b-4624-b026-183e7a9a194f" />

**Figure 2:** FastQC Basic Statistics - FastQC summary table displaying basic metrics including total sequences (33,578,171), length (150 bp), and GC content (45%).

<img width="1080" height="574" alt="20408" src="https://github.com/user-attachments/assets/3265a435-3844-4097-a410-03e2633a4605" />

**Figure 3:** Per Base Sequence Quality reads.

# RNA-seq Interpretation
 
 The primary goal of this study is to investigate how acute heat stress and recovery affect gene expression and transposable element dynamics in Arabidopsis thaliana seedlings, enabling a genome-wide evaluation of stress-responsive transcriptional dynamics. While genomic DNA represents the static inheritance blueprint of an organism, RNA molecules reflect active transcriptional responses; thus, RNA-seq specifically measures dynamic, functional gene activity. The sample SRX6027528 (RNA-Seq-Col-Control-Rep1) serves as a biological replicate, which is an independent biological sample treated under identical control conditions. Biological replicates are essential for capturing natural biological variance, ensuring that observed expression changes are statistically significant rather than random noise. 

# Conclusion

The RNA-seq dataset for sample SRX6027528 (RNA-Seq-Col-Control-Rep1) demonstrated strong overall sequencing metrics, yielding 33,115,474 paired-end reads with high per-base quality scores and no detectable adapter contamination. The observed flags in sequence content and duplication levels align with expected library preparation artifacts rather than technical failure. Consequently, the data are high-quality and fully suitable for downstream bioinformatics workflows. Proceeding to transcript alignment, gene-level quantification, library normalization, and differential expression analysis will allow for robust comparison against heat-treated and recovery conditions. 
