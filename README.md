# Spectral_Flow_Workflow

This script is an addition to doi: 10.3389/fimmu.2021.768113. We will walk through the described pipeline with two different spectral flow cytometry datasets. Case A will use the dataset described in the paper and available at: https://flowrepository.org/id/FR-FCM-Z4KT . Case B will use part of the files of a spectral flow cytometry dataset https://flowrepository.org/experiments/3675. Files to download from this dataset are the healthy controls. 

If there are difficulties adapting the script to your own dataset, please do not hestitate to contact us: h.denbraanker@erasmusmc.nl or github.


```{r Installing packages, message=FALSE, eval=FALSE}
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("flowCore")
BiocManager::install("flowViz")
BiocManager::install("flowVS")
BiocManager::install("flowAI")
BiocManager::install("flowAI")
BiocManager::install("PeacoQC")
BiocManager::install("CATALYST")
BiocManager::install("SingleCellExperiment")

if(!requireNamespace("devtools", quietly=TRUE))
  install.packages("devtools")

devtools::install_github('saeyslab/CytoNorm')
install.packages("uwot")
install.packages("knitr")
install.packages("xlsx")
```
