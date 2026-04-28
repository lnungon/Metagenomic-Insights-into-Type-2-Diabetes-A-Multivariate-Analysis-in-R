# Metagenomic-Insights-into-Type-2-Diabetes-A-Multivariate-Analysis-in-R
This repository contains a multivariate statistical analysis of the human gut microbiome associated with Type 2 Diabetes (T2-D). 

## Project Summary and goal
The primary objective of this analysis is to acquired already proccessed relative abundances of bacteria present in the gut microbiota of control subjects and patients with T2-D. Multiple ecological analyses will be conducted, including the Shannon index. Particular emphasis is placed on the application of various multivariate analyses, including principal component analysis (PCA), non-metric multidimensional scaling (nMDS), and correspondence analysis (CA). 

**Dataset Highlights**: Analysis of a subset of 30 healthy controls and 30 patients from the original study. This study uses fecal samples to investigate the gut microbiome.
**Conditions:** Comparison between Healthy Controls and T2-D patients
**Technology:** Metagenome-Wide Association Study(MGWAS) based on deep shotgun sequencing of the gut microbial DNA (Illumina GAIIx and HiSeq 2000). 

## Key Steps
* **Data Preprocessing:** acquisition with Bioconductor 
* **Ecological parameters:** Visualizing Species Richness and Shannon index within each group
* **Outlier detection**: using Euclidean and Mahalanabois distances
* **Data normalization**: Centering, scaling, and logarithmic transformation
* **Exploratory Data Analysis:** PCA, nMDS (Kruskal method with Bray-Curtis distance) and CA.
* **Comparison with the original article** : possible differences, advantages and limitations of our study

## Analysis overview
The following visualizations demonstrate the robust biological signal captured from the 195 blood samples in the GSE161731 dataset.

## Software & Libraries
This pipeline is built on the Bioconductor ecosystem for genomic data science and the primary frameworks used are: 
* **Language:** R
* **Bioinformatics:** Bioconductor:
  * curatedMetagonicData, SummarizedExperiment: for data acquisition and object manipulation
  * vegan: central study of ecological parameters like Shannon index
  * robusbase: for Mahalanabois distance calculation
  * FactoMineR, factoextra: calculations and visualizations of CA
* **Data manipulation & Visualization:** `tidiverse`(`ggplot2` and `tdyr`)
  
Reproducibility Note: A comprehensive list of all loaded packages, versions, and the computational environment is provided in the Session Information section at the end of the final report.

## Repository Structure
* This data comes from a published study: Qin J., *Nat.*, 2012. ** and complete data is available in GigaDB under accesion number [100036]([https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE161731](https://gigadb.org/dataset/100036))**.  
* [Main Analysis Script (R)](): Clean and commented code. 
* [Full Research Report (HTML)](): Interactive report with all visualizations and statistical tables.
* [Executive Summary (PDF)](): High-level summary of findings for clinical stakeholders with minimal code requirements.
* [Plots](): Folder with all the individual images and figures inside the project.
* [Session Info (txt)](t): Complete information about the used environment. 

---
*Developed as part of my technical portfolio in Biostatistics and Genomic Data Science.*
