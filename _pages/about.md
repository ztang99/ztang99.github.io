---
permalink: /
title: "Zitian Tang"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
/* Styling for section headers */
.page__content h2 {
  padding-top: 80px;
  margin-top: -60px;
}

/* Optional: Add some visual separation between sections */
section {
  margin-bottom: 3em;
  padding-bottom: 2em;
  border-bottom: 1px solid #e0e0e0;
}

section:last-child {
  border-bottom: none;
}
</style>

<section id="about" markdown="1">

Hi there 👋 I'm Zitian. I'm a graduating Ph.D. in bioinformatics. 
I'm super interested in how computational genomics and biomedical informatics help translate research findings to clinical outcomes. 
I'm a strong problem-solver, communicator, and collaborator passionate about translating bioinformatics research into real-world solutions.
Happy to connect via LinkedIn!

**I am actively looking for full-time bioinformatics scientist position starting summer 2026. Feel free to reach out via email to discuss any potential opportunities.**


<section id="portfolio" markdown="1">

## Projects

### RFC1 STR Expansion Detection Pipeline (WGS)

[Code](https://github.com/ztang99/STR-detection-genotyping){: .btn .btn-code} 
[Manuscript](https://www.medrxiv.org/content/10.1101/2025.04.18.25325809v3){: .btn .btn-manuscript}

**Problem**: I developed a scalable, clinical-grade pipeline to detect **pathogenic RFC1 AAGGG repeat expansions** from short-read whole-genome sequencing, addressing the challenge that these intronic expansions far exceed read length and are not accurately captured/genotyped by existing tools.

**Method**: I built an end-to-end workflow combining **genome-wide STR discovery (ExpansionHunter Denovo)**, **targeted locus genotyping (ExpansionHunter)**, **sequence validation (BLAT)**, and a **custom unsupervised ML framework** to objectively classify samples as **biallelic, monoallelic, or non-carriers** without relying on arbitrary thresholds. The pipeline was fully containerized and optimized to scale across ~800 patients and ~850 controls.

**Result**: The method identified 22 biallelic (2.8%) and 118 monoallelic (15%) expansion carriers in patient cohort, with **>95% concordance to repeat-primed PCR**. Unsupervised clustering revealed distinct genotype signatures between biallelic and monoallelic RFC1 expansions.

**Impact**: This work improves diagnostic accuracy for RFC1-related neuropathies, provides a reproducible framework for STR genotyping from short-read WGS, and is **open-sourced and generalizable** to other repeat expansion disorders especially those with altered repeat motifs.

---

### Comprehensive Somatic Variant Benchmark (SMaHT Consortium)

[Code](https://github.com/ztang99/Graph-Based-Benchmark){: .btn .btn-code} 
[Benchmark Resource](https://github.com/jinlab-washu/HapMap-BenchmarkSet-Manuscript){: .btn .btn-benchmark} 
[Manuscript](https://www.biorxiv.org/content/10.1101/2025.09.29.679336v2){: .btn .btn-manuscript}

**Problem**: As part of the NIH **SMaHT Consortium**, I co-led development of a **technology-agnostic benchmarking resource** to evaluate somatic variant detection across variant classes and allele fractions—addressing a major gap in the field where existing benchmarks were limited to autosomal SNVs and based on caller consensus.

**Method**: I played major roles in designing and validating a benchmark spanning **SNVs, indels, structural variants, and mobile element insertions** across **autosomes, sex chromosomes, and mitochondrial DNA**, using controlled mixtures of six HapMap cell lines to generate variants at** 0.25–16.5% allele fractions**. I contributed to implementing a **pangenome-based truth set (Minigraph-Cactus)** derived from de novo assemblies, developed **statistical validation and coverage models** using ultra-deep sequencing, and led analyses of **caller performance in difficult genomic regions**.

**Result**: The final resource includes **>6M SNVs, 1.8M indels, 49K structural variants, and 10K mobile element insertions**, making it the most comprehensive somatic benchmarking dataset to date. It provides gene-level coverage recommendations for **6,600+ clinically relevant genes**, reveals systematic detection biases, and is now actively used to benchmark **research and clinical somatic variant detection pipelines**.

**Impact**: This benchmark enables rigorous, future-proof evaluation of somatic variant callers and supports more reliable detection of low-frequency mosaic variants across technologies.

---

### Bulk RNA-seq Analysis Pipeline

[Code](){: .btn .btn-code}
[Blog](../_posts/bulk_RNAseq_analysis_minimal.html){: .btn .btn-manuscript}

**Problem**: Comprehensive analysis pipeline for bulk RNA-sequencing data from differential expression to pathway analysis.

**Method**: Integrated quality control, alignment, quantification, and statistical analysis using R/Bioconductor tools.

**Result**: Reproducible pipeline with automated reporting and visualization capabilities.

---

### Single-cell RNA-seq Analysis Framework

[Code](){: .btn .btn-code}
[Blog](){: .btn .btn-manuscript}

**Problem**: Analysis framework for single-cell RNA-sequencing data including cell type identification and trajectory analysis.

**Method**: Implemented Seurat-based pipeline with custom clustering and annotation methods.

**Result**: Scalable framework for single-cell analysis with interactive visualizations.

---

### Graph Neural Network Classifying Glioblastoma Patient Phases 
[Code](https://github.com/JiaruiFeng/KP-GNN){: .btn .btn-code} (Code adapted from original KP-GNN implementation)

---

### Graph Attention-Based Neural Network to Identify Pathogenic Biomarkers from MRI Images 
[Code](https://github.com/ztang99/nnUNet_neuroimaging){: .btn .btn-code} (Code forked and adapted from https://github.com/MIC-DKFZ/nnUNet)




<section id="publications-talks" markdown="1">

## Publications / Talks
* Kong N\*, **Tang Z**\*, et al. “A Comprehensive Benchmarking Resource for Somatic Variant Detection using HapMap Mixtures and Human Pangenome Graphs”. Available on bioRxiv: https://doi.org/10.1101/2025.09.29.679336. (2025)
* **Tang Z**\*, Ovunc S\*, et al. “Heterozygous and Homozygous RFC1 AAGGG Repeat Expansions are Common in Idiopathic Peripheral Neuropathy”. Available on medRxiv: https://doi.org/10.1101/2025.04.18.25325809. (2025)
* Fu Q, Xin Z, Miao B, Zhang W, Kong N, Tang Z, et al. “Leveraging Human Pangenome for Improved Somatic Variant Detection.” Under review at Cell Genomics. Available on bioRxiv: https://doi.org/10.64898/2026.01.04.697580. (2025)
* **Somatic Mosaicism across Human Tissues Network**, Alexej Abyzov. "Comprehensive benchmarking of somatic mutation detection by the SMaHT Network". Available on bioRxiv. (2025)
* Choi J\*, **Tang Z**\*, et al. “Unleashing the Power of Multi-Omics: Unraveling the Molecular Landscape of Peripheral Neuropathy”. Ann Clin Transl Neurol. 2025 Apr;12(4):674-685. doi: 10.1002/acn3.70019. Epub 2025 Mar 24. PMID: 40126913; PMCID: PMC12040521.
* •	Coorens THH, ...; The Somatic Mosaicism across Human Tissues Network†. “The somatic Mosaicism across Human Tissues Network”. Nature. 2025 Jul;643(8070):47-59. doi: 10.1038/s41586-025-09096-7. Epub 2025 Jul 2. PMID: 40604182. 
**†Member of consortium**

#### Talks
* Invited Talk at Hope Center for Neurological Disorders Monday Noon Seminars. Nominated by HOPE center. November 2025.
* Invited Talk at Genetics department WIP (work-in-progress). Nominated by Dr. Sheng-Chih Jin (PI). April 2025.
* Invited Talk at Program Showcase for Immersion at Washington University School of Medicine. Nominated by graduate program faculty members. Aug 2024.



<section id="education" markdown="1">

## Education

#### Ph.D. in Biomedical Informatics and Data Science

Washington University School of Medicine • St. Louis, MO • 2026.06 • 4.00 GPA

#### Bachelor of Science in Biomedical Engineering

Minor in Computer Science (AI track) • Georgia Institute of Technology • Atlanta, GA • 2021.12 • 4.00 GPA


<section id="work-experience" markdown="1">

## Work Experiences

Engineering Intern • Motus Nova LLC • 2022.01 - 2022.06 • Atlanta, GA
* Contributed to the manufacturing process of FDA-listed medical devices for stroke tele-rehabilitation by following established assembly protocols and utilizing precision tooling skills.
* Issue, manage, maintain, and revise device quality control systems.
* Perform clinical demonstrations to stroke survivors and redesign linkage structures to smooth device’s donning process.

Research & Development Team Intern • Huahui Health Ltd. • 2020.05 - 2021.01 • Beijing, China 
* Constructed three antibody libraries with 10 billion+ high-affinity functional antibody fragments.
* Increased antibody expression level by 10,000% using recombinant DNA technique.


<section id="awards" markdown="1">

## Awards

* Precision Medicine Pathway Fellow, Washington University School of Medicine [2023 - 2025]
* Jackson Laboratory's Human Genetics and Genomics: The McKusick Short Course Travel Reward [2023]
* Outstanding Academic Achievements Award (Nomination), Georgia Institute of Technology [2021]
* Faculty Honors and Dean's List recipient, Georgia Institute of Technology [2018 - 2021]



