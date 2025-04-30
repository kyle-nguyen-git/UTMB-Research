# UTMB-Research
R-Studio Code for UTMB Research- Summer 2024

deseq_analysis.R

Differential expression analysis using DESeq2 on piRNA data from RSV vs. mock-treated samples. Includes:

Reading count and metadata from Excel

DESeq2 normalization and significance testing

Filtering for adjusted p-values (padj ≤ 0.05)

Export of significantly differentially expressed piRNAs

volcano_plot.R

Volcano plot visualization of DESeq2 output:

Log2 fold change vs. -log10 adjusted p-value

Highlights significantly differentially expressed piRNAs (padj ≤ 0.05)

Annotated with cutoff thresholds (log2FC ±1, padj = 0.05)

heatmap_plot.R

Generates a heatmap of significant piRNA expression:

Filters DESeq2 output for padj ≤ 0.05

Extracts expression data of significant genes

Z-score normalization

Visualized using ComplexHeatmap with clustering by gene and sample

significant_miRNAs_export.R

Exports a list of significant piRNAs:

Extracts gene names with padj ≤ 0.05

Saves to a CSV file (significant_miRNAs_padj_0.05.csv) in the working directory

Data was collected from Baylor College of Medicine
  -Next Generation Sequencing Data
  -RSV, HMPV, and Control Group Data

Data was cleaned and prepped at Baylor
