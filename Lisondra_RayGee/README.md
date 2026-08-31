# RNA-Seq Data Characterization Report

* **Student Name:** Ray Gee J. Lisondra
* **Group Number:** Group 1 (Heat Stress)
* **Assigned Sample:** Heat Stress Replicate 2 (`Heat_Rep2`)
---

## 1. Study Information & Citation

* **Paper Title:** Heat stress-induced transposon activation correlates with 3D chromatin organization rearrangement in Arabidopsis
* **Full Citation:** Ma, Q., Tharwat, M., Alshanbari, F. A., Khan, M. Z., Zhang, X., Zhang, Y., Hu, Y., Li, X., & Hu, Y. (2020). Heat stress triggers genome‑wide release of transposable elements in Arabidopsis. *Plant Physiology*.
* **Organism:** *Arabidopsis thaliana* (Col‑0 ecotype)
* **Assigned RNA-seq Accession:** `SRR9257063`
* **Experimental Condition:** Acute Heat Stress (Treatment)
* **Biological Representation:** This sample represents whole *Arabidopsis thaliana* (Col-0 ecotype) seedlings exposed to acute heat stress (Replicate 2). Biologically, it captures the genome-wide transcriptional responses, heat-shock gene activation, and transposable element expression dynamics under elevated temperature conditions compared to thermoneutral control growth.
* **DOI:** https://doi.org/10.1038/s41467-020-15809-5
---

## 2. Dataset Characteristics & Summary

| RNA-Seq Metric | Value / Observation |
| :--- | :--- |
| **SRA Run Accession** | `SRR9257063` |
| **BioSample Accession** | `SAMN11997384` |
| **Sequencing Layout** | Paired-End |
| **Number of Reads / Sequences** | *25,963,048* |
| **Read Length** | 150 bp |
| **GC Content** | *45%* |
| **Approximate File Size** | 2.6 GB |

---

## 3. FastQC Analysis & Screenshots

### Figure 1: Galaxy Workspace & History Overview
Below is the Galaxy panel showing the active history containing the imported paired-end dataset collection.

![Galaxy History](screenshots/galaxy_history.png)

---

### Figure 2: Four-Line FASTQ Structure
Below is the four-line FASTQ preview of the reverse read (`Heat_Rep2_R2`), showing the sequence ID, raw base calls, separator, and ASCII quality scores.

![FASTQ Structure](screenshots/fastq_preview.png)

---

### Figure 3: FastQC Basic Statistics
Below is the FastQC Basic Statistics table generated for the forward read (`SRR9257063_1`).

![FastQC Basic Statistics](screenshots/fastqc_basic_statistics_R1.png)

---

### Figure 4: FastQC Per Base Sequence Quality
Below is the Phred quality score plot across read positions.

![FastQC Per Base Quality](screenshots/fastqc_per_base_quality_R1.png)

* **Summary:** Base call quality is high across all read positions, maintaining Phred $Q$-scores well above $28$ (green zone).

---

### Figure 5: FastQC Per Base Sequence Content (Quality Observation)
Below is the sequence content plot highlighting a positional bias at the start of the reads.

![FastQC Per Base Sequence Content](screenshots/fastqc_per_base_sequence_content_R1.png)

* **Summary:** Flagged as failed (**X**) due to non-uniform base ratios in the first 10–12 bp. This is an expected artifact of random hexamer priming during cDNA synthesis in standard Illumina RNA-seq library preparation and does not indicate poor sample quality.

---

## 4. Interpretation Questions
The original RNA-seq study aimed to determine how acute heat stress and recovery influence gene expression and transposable element activity in *Arabidopsis thaliana* seedlings to explore stress-induced transcriptional changes at a genome-wide scale. Unlike genomic DNA—which is the static, permanent genetic blueprint—RNA-seq measures temporary RNA transcripts to capture real-time, functional gene activity rather than just static genetic potential. To ensure reliable results, the experimental design utilized biological replicates (independent samples from the same condition) to account for natural biological variation and strengthen statistical confidence in differential expression analysis. Sequencing was performed to output standard text-based FASTQ files containing raw sequencing reads along with per-base quality scores, where high quality scores indicate low error probability and high read reliability. Depending on design, sequencing can be single-end (reading one end of a DNA fragment) or paired-end (reading both ends), with paired-end offering superior alignment accuracy and structural information in complex genomes. Sample quality was evaluated using FastQC to summarize metrics such as per-base quality, GC content, adapter contamination, sequence duplication, and composition bias. While all group samples demonstrated similar overall quality with 150-bp reads, ~45–46% GC content, and acceptable base quality, noticeable quality variations emerged: SRX6027532 (Recovery Rep1) exhibited the most severe QC concerns—including adapter contamination, overrepresented sequences, sequence-content bias, and high duplication—while SRX6027530 showed adapter/primer bias, and SRX6027531 and SRX6027528 displayed sequence-content and duplication issues. Because unaddressed adapter contamination causes misalignment and biased quantification, the dataset requires preprocessing (adapter/primer trimming, quality filtering, and removal of contaminants) prior to comparing expression levels. Finally, to compare gene expression between control and treatment samples, these cleaned reads must be aligned to the reference genome, quantified, normalized, and analyzed using appropriate statistical methods across biological replicates.


---

## 5. Conclusion

The raw sequencing dataset for `SRR9257063` (Heat Stress Replicate 2) was successfully processed and evaluated in Galaxy. FastQC confirmed high overall read quality, with Phred scores remaining within acceptable thresholds. Minor warnings, including 5' sequence content bias, reflect typical RNA-seq library preparation artifacts rather than sample degradation. Consequently, the dataset meets quality standards for downstream alignment, quantification, and differential expression analysis.
