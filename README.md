# RNA-Seq Differential Gene Expression Analysis

## 📌 Project Overview

This project involves the analysis of quantitated gene expression data from an RNA-seq experiment. The experiment compares a diseased cell line with diseased cell lines treated with **Compound X** to identify genes significantly affected by the treatment.

The data was explored and visualized using base R and the `ggplot2` package, focusing on identifying differentially expressed genes based on log₂ fold change and statistical significance (p-value). Genes were categorized as **Upregulated**, **Downregulated**, or **Not significant**.

## 🧬 Dataset Description

The dataset contains the following columns:

- `Gene`: Gene name  
- `log2FoldChange`: Log2-transformed fold change in gene expression  
- `pvalue`: Statistical significance of the expression change  
- `padj`: Adjusted p-value to correct for multiple testing  

A sample of the first 6 rows:

| Gene     | log2FoldChange | pvalue     | padj      |
|----------|----------------|------------|-----------|
| DOK6     | 0.5100         | 1.861e-08  | 0.0003053 |
| TBX5     | -2.1290        | 5.655e-08  | 0.0004191 |
| SLC32A1  | 0.9003         | 7.664e-08  | 0.0004191 |
| IFITM1   | -1.6870        | 3.735e-06  | 0.0068090 |
| NUP93    | 0.3659         | 3.373e-06  | 0.0068090 |
| EMILIN2  | 1.5340         | 2.976e-06  | 0.0068090 |

## 📊 Visualization

### Volcano Plot

A volcano plot was generated to visualize the differential expression:

- **X-axis:** Log2 Fold Change  
- **Y-axis:** -log10(p-value)  
- **Red:** Upregulated genes  
- **Blue:** Downregulated genes  
- **Grey:** Not significant  

Dashed lines indicate fold change cutoffs (±1) and p-value cutoff (0.01).

![1UXNxG7cVAAAAAElFTkSuQmCC](https://github.com/user-attachments/assets/5cfd6bc9-b06f-4ebd-ac72-19187338e43f)


### Differential Expression Summary

- **Number of upregulated genes:** 19  
- **Number of downregulated genes:** 91
---

## 🔬 Top Differentially Expressed Genes

### Downregulated Genes

1. **TBX5**  
   - A DNA-binding protein involved in transcription regulation, heart development, and limb formation.

2. **IFITM1**  
   - Antiviral protein that blocks virus entry and plays a role in immune signaling and cell cycle arrest.

3. **LAMA2**  
   - Mediates cell attachment and tissue organization during embryonic development via ECM interaction.

4. **CAV2**  
   - Regulates G-protein activity and participates in caveolae formation with CAV1.

5. **TNN**  
   - ECM protein involved in neurite outgrowth, cell migration, and angiogenesis in tumors.

### Upregulated Genes

1. **EMILIN2**  
   - ECM component possibly involved in vessel formation and cell adhesion.

2. **POU3F4**  
   - Transcription factor active in early neural development and brain-specific expression.

3. **LOC285954 (INHBA-AS1)**  
   - No functional data available.

4. **VEPH1**  
   - Modulates TGF-beta signaling and may affect multiple signaling pathways (FOXO, Hippo, WNT).

5. **DTHD1**  
   - No functional data available.
