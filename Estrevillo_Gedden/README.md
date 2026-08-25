
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

## Screenshots and Visualizations
  
 <img width="1080" height="800" alt="1000101655" src="https://github.com/user-attachments/assets/698eb521-785d-43b6-9784-266cf0c77d01" />

 **Figure 1: Galaxy History** - Galaxy history panel showing the imported RNA-seq dataset and completed FastQC outputs.

 <img width="2048" height="986" alt="1000101657" src="https://github.com/user-attachments/assets/def1b9cf-1dc6-42b8-a4c2-1dafb06cf210" />

 **Figure 2: FastQC Basic Statistics** - FastQC summary table displaying basic metrics including total sequences (33,578,171), length (150 bp), and GC content (45%).

  <img width="2048" height="988" alt="1000101658" src="https://github.com/user-attachments/assets/cea674ff-f8f5-4acb-9f73-89a351bfecb8" />

 **Figure 3: Per Base Sequence Quality** - FastQC per base sequence quality plot illustrating high-quality base calls across the reads.

 ## RNA-seq Interpretation

The study aimed to determine how acute heat stress and recovery influence gene expression and transposable element activity in *Arabidopsis thaliana* seedlings, allowing the authors to examine stress-induced transcriptional changes at a genome-wide scale. Genomic DNA serves as the permanent genetic blueprint, whereas RNA molecules are temporary transcripts produced when genes are expressed. Therefore, RNA-seq provides information about functional gene activity rather than simply the genetic potential of the organism. A biological replicate is an independent sample from the same experimental condition, such as separate seedlings exposed to heat stress, and is important because it accounts for natural biological variation and increases the reliability of differential gene expression results. Single-end sequencing reads one end of a DNA fragment, while paired-end sequencing reads both ends, providing greater alignment accuracy and structural information. A FASTQ file is a text-based format containing raw sequencing reads along with their corresponding per-base quality scores, serving as the standard input for downstream RNA-seq analysis. FastQC provides a summary of sequencing quality, including per-base quality scores, GC content, adapter contamination, and sequence duplication. A high per-base quality score indicates low error probability, making the reads reliable for downstream alignment and quantification. Adapter contamination can cause misalignment, false mapping, and quantification bias, which is why trimming is required before analysis. The RNA-seq samples showed consistent quality, and while minor common warnings like adapter content or duplication levels appeared, the data is suitable for downstream processing. Before comparing gene expression between control and treatment samples, the researchers would need to trim adapters and low-quality reads if necessary, align the reads to a reference genome or quantify transcripts, obtain gene-level read counts, normalize the counts to account for differences in sequencing depth, and perform statistical differential gene expression analysis to identify significantly differentially expressed genes.

## Conclusion

The RNA-seq samples showed good and consistent sequencing quality based on the FastQC results. No major quality problems were observed, as all samples passed the quality checks. The results indicate that the data are suitable for further RNA-seq analysis. However, additional steps such as read alignment, gene quantification, normalization, and differential expression analysis are needed to compare gene expression between control and treatment samples.

