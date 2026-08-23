# Student README

* **Student Name:** Estrevillo, Gedden
* **Group Number:** Group 1

---

## Project & Sample Information
* **Title and citation of the group paper:** 
  * Title: Heat stress-induced transposon activation correlates with 3D chromatin organization rearrangement in Arabidopsis
  * Citation: Sun, L., Jing, Y., Liu, X., Li, Q., Xue, Z., Cheng, Z., Wang, D., He, H., Qian, W. (2020). Heat stress-induced transposon activation correlates with 3D chromatin organization rearrangement in Arabidopsis. *Nat Commun*, 11(1), 1886. https://doi.org/10.1038/s41467-020-15809-5
* **Assigned RNA-seq accession number:** SRX6027530
* **Control or treatment condition:** Heat Stress (RNA-Seq-Col-Heat-Rep 1)
* **Short explanation of what the sample represents biologically:** This sample represents *Arabidopsis thaliana* seedlings subjected to heat stress treatment to evaluate transcriptional responses and chromatin changes.

---

## Sequencing & FastQC Dataset Metrics
* **Sequencing layout:** Paired-end
* **Number of reads:** 
  * R1: 33,578,171 
  * R2: 33,578,171
* **Read length:** 
  * R1: 150 bp 
  * R2: 150 bp
* **GC content:** 
  * R1: 45% 
  * R2: 45%
* **Summary of FastQC results:** Passed basic statistics and quality scores; failed sequence content due to positional nucleotide bias and adapter/primer content at the beginning of reads.

---

## Required Screenshots
* Galaxy history showing imported RNA-seq dataset (`screenshots/galaxy_history.png`)
* FASTQ preview showing four-line structure (`screenshots/fastq_preview.png`)
* FastQC Basic Statistics & Per Base Quality (`screenshots/fastqc_quality.png`)

---

## Interpretation Questions & Answers
1. **How is a FASTQ file different from the FASTA genome file used in previous assignments?**
   * A FASTQ file contains raw sequencing reads alongside quality scores, whereas a FASTA file contains only nucleotide sequences without quality data.
2. **What information is present in FASTQ that is not present in FASTA?**
   * Per-base quality scores.
3. **Why are quality scores important in RNA-seq?**
   * They allow identification and filtering of unreliable base calls to prevent downstream mapping errors.
4. **What is a biological replicate and why is it important?**
   * Biological replicates are independent biological samples treated identically, crucial for accounting for biological variation and ensuring statistical reliability.
5. **What is the difference between single-end and paired-end sequencing?**
   * Single-end sequencing sequences one end of a fragment, while paired-end sequencing sequences both ends for improved alignment and structural resolution.

---

## Conclusion
The analysis of our assigned *Arabidopsis thaliana* heat stress dataset (`SRX6027530`) confirmed high sequencing depth and generally strong base quality. Although minor adapter and sequence content warnings were flagged by FastQC near the start of the reads, the dataset met benchmarks for quality. Overall, the data is reliable and well-suited for downstream alignment and differential expression profiling.

