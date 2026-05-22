![R](https://img.shields.io/badge/R-4.0+-blue)
![RNA-seq](https://img.shields.io/badge/RNA--seq-Transcriptomics-green)
![DESeq2](https://img.shields.io/badge/DESeq2-Differential%20Expression-orange)
![Salmon](https://img.shields.io/badge/Salmon-Quantification-red)

# Bulk RNA-seq Analysis Pipeline

A comprehensive bulk RNA-seq analysis workflow for transcriptomic data processing, quality assessment, differential expression analysis, data visualization, and biological pathway interpretation.

This repository contains scripts, processed datasets, quality control reports, statistical analyses, and visualization outputs generated during a complete RNA-seq analysis workflow.

---

## Project Overview

The pipeline integrates widely used bioinformatics tools and statistical approaches to process RNA-seq data from raw counts to biologically meaningful insights.

Major components of the workflow include:

- RNA-seq data acquisition
- Quality control and assessment
- Transcript quantification
- Differential expression analysis
- Principal Component Analysis (PCA)
- Data visualization
- Pathway enrichment analysis
- Generation of publication-ready outputs

---

## Workflow Overview

### 1. Data Acquisition

RNA-seq datasets are downloaded and organized for downstream transcriptomic analyses.

### 2. Quality Assessment

Sequencing quality is evaluated using:

- FastQC
- MultiQC

Quality reports are generated to assess sequencing performance and sample integrity.

### 3. Transcript Quantification

Transcript abundance estimation is performed using Salmon, providing rapid and accurate expression quantification.

### 4. Differential Expression Analysis

Differentially expressed genes are identified using statistical approaches implemented in DESeq2.

### 5. Exploratory Data Analysis

Data structure and sample relationships are assessed through:

- Principal Component Analysis (PCA)
- Sample clustering
- Expression distribution evaluation

### 6. Visualization

Publication-ready visualizations are generated, including:

- PCA plots
- Volcano plots
- Quality control summaries
- Expression-based visual outputs

### 7. Functional Interpretation

Differentially expressed genes are subjected to pathway enrichment analysis to identify significantly altered biological processes and molecular pathways.

---

## Repository Structure

```text
bulk-rna-seq-analysis/
│
├── data/
│ ├── ileum_raw_counts.csv
│ ├── metadata.csv
│ └── pc_gene.txt
│
├── scripts/
│ ├── bulk_rnaseq_analysis.Rmd
│ ├── download_sra.py
│ ├── qc_fastqc_multiqc.sh
│ └── salmon_quantification.sh
│
├── results/
│ │
│ ├── qc_reports/
│ │ └── multiqc_report.html
│ │
│ ├── workflow_screenshots/
│ │ ├── SRA download
│ │ ├── Salmon indexing
│ │ ├── Salmon quantification
│ │ ├── FastQC execution
│ │ └── MultiQC summary
│ │
│ ├── PCA visualizations
│ ├── Volcano plot outputs
│ ├── Differential expression results
│ ├── Pathway enrichment results
│ └── Additional statistical summaries
│
└── README.md
```

---

## Software Requirements

### Core Tools

- FastQC
- MultiQC
- Salmon
- Python 3
- R (version 4.0 or later)

### Major R Packages

- DESeq2
- ggplot2
- EnhancedVolcano
- pheatmap
- clusterProfiler

---

## Data

The repository includes processed count matrices, sample metadata, gene annotation files, statistical outputs, and visualization results used for downstream transcriptomic analyses.

---

## Output Files

The workflow generates:

- MultiQC quality reports
- Differential expression result tables
- PCA visualizations
- Volcano plots
- Pathway enrichment summaries
- Statistical output files
- Workflow execution screenshots

---

## Author

**Harshit Mishra**
