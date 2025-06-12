# SLE_RNAi_LNP_Thesis
# Bioinformatics Pipeline for RNAi Therapeutic Design in Systemic Lupus Erythematosus (SLE)

This repository contains the full R code and resources used in the master's thesis:

**“Bioinformatics driven development of lipid nanoparticles formulations for RNAi therapeutics in systemic lupus erythematosus (SLE)”**

📚 Author: Ali Hamza Bilal  
🏛️ Institution: Sechenov University  
🧪 Degree: Master’s in Biotechnology

---

## 🔧 Contents

- `sle_analysis_pipeline.R`: Main R script for the entire workflow
- `plots/`: Folder to save PCA, UMAP, volcano, and dispersion plots
- `results/`: Processed DEG tables and gene lists
- `README.md`: Reproducibility guide

---

## 🧬 Workflow Overview

This project implements a fully in-silico pipeline including:

1. **Transcriptomic data acquisition** from GEO (GSE72509)
2. **DEG analysis** using DESeq2
3. **QC visualizations**: PCA, UMAP, volcano plots
4. **siRNA target identification**
5. **RNA secondary structure & thermodynamic analysis**
6. **Docking and LNP encapsulation simulation (conceptual)**

---

## 🔗 Dataset Used

- GSE72509 (RNA-seq dataset from SLE patients and healthy controls)  
- Source: [https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE72509](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE72509)

---

## 📦 Required R Packages

```r
# CRAN & Bioconductor
install.packages("BiocManager")
BiocManager::install(c("DESeq2", "limma", "GEOquery", "Biobase", "EnhancedVolcano"))
install.packages(c("data.table", "ggplot2", "umap"))
