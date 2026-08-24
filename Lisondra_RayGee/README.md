# RNA-Seq Data Characterization Report

* **Student Name:** Ray Gee J. Lisondra
* **Group Number:** Group 1 (Heat Stress)
* **Assigned Sample:** Heat Stress Replicate 2 (`Heat_Rep2`)

---

## 1. Study Information & Citation

* **Paper Title:** Heat stress triggers genome‑wide release of transposable elements in Arabidopsis
* **Full Citation:** Ma, Q., Tharwat, M., Alshanbari, F. A., Khan, M. Z., Zhang, X., Zhang, Y., Hu, Y., Li, X., & Hu, Y. (2020). Heat stress triggers genome‑wide release of transposable elements in Arabidopsis. *Plant Physiology*.
* **Organism:** *Arabidopsis thaliana* (Col‑0 ecotype)
* **Assigned RNA-seq Accession:** `SRR9257063`
* **Experimental Condition:** Acute Heat Stress (Treatment)
* **Biological Representation:** This sample represents whole *Arabidopsis thaliana* (Col-0 ecotype) seedlings exposed to acute heat stress (Replicate 2). Biologically, it captures the genome-wide transcriptional responses, heat-shock gene activation, and transposable element expression dynamics under elevated temperature conditions compared to thermoneutral control growth.

---

## 2. Dataset Characteristics & Summary

| RNA-Seq Metric | Value / Observation |
| :--- | :--- |
| **SRA Run Accession** | `SRR9257063` |
| **BioSample Accession** | `SAMN11997384` |
| **Sequencing Layout** | Paired-End |
| **Number of Reads / Sequences** | *[25,963,048]* |
| **Read Length** | 150 bp |
| **GC Content** | *[45%]* |
| **Approximate File Size** | 2.6 GB |

---

## 3. FastQC Analysis & Screenshots

### Screenshot 1: Galaxy Workspace & History Overview
Below is the Galaxy panel showing the active history containing the imported paired-end dataset collection.

![Galaxy History](screenshots/galaxy_history.png)

---

### Screenshot 2: Four-Line FASTQ Structure
Below is the four-line FASTQ preview of the reverse read (`Heat_Rep2_R2`), showing the sequence ID, raw base calls, separator, and ASCII quality scores.

![FASTQ Structure](screenshots/fastq_preview.png)

---

### Screenshot 3: FastQC Basic Statistics
Below is the FastQC Basic Statistics table generated for the forward read (`SRR9257063_1`).

![FastQC Basic Statistics](screenshots/fastqc_basic_statistics_R1.png)

---

### Screenshot 4: FastQC Per Base Sequence Quality
Below is the Phred quality score plot across read positions.

![FastQC Per Base Quality](screenshots/fastqc_per_base_quality_R1.png)

* **Summary:** Base call quality is high across all read positions, maintaining Phred $Q$-scores well above $28$ (green zone).

---

### Screenshot 5: FastQC Per Base Sequence Content (Quality Observation)
Below is the sequence content plot highlighting a positional bias at the start of the reads.

![FastQC Per Base Sequence Content](screenshots/fastqc_per_base_sequence_content_R1.png)

* **Summary:** Flagged as failed (**X**) due to non-uniform base ratios in the first 10–12 bp. This is an expected artifact of random hexamer priming during cDNA synthesis in standard Illumina RNA-seq library preparation and does not indicate poor sample quality.

---

## 4. Interpretation Questions


---

## 5. Conclusion

The raw sequencing dataset for `SRR9257063` (Heat Stress Replicate 2) was successfully downloaded, imported, and characterized within Galaxy. Quality control evaluation via FastQC demonstrated high overall base quality across reads, with Phred scores consistently remaining in the acceptable range. Observed warnings, such as 5' sequence content bias, represent standard technical artifacts inherent to RNA-seq library preparation rather than biological degradation. Overall, the data quality is sufficient and ready for downstream alignment, quantification, and differential expression analysis.
