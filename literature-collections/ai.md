---
description: 'Literature, Course and Book Recommendations'
---

# Machine learning & AI

## 1. **Startup of Literature Reading**

* **Deep Learning**: 2015 _Nature Biotech._ - DeepBind: Predicting the sequence specificities of DNA- and RNA-binding proteins by deep learning
* **Cancer Locator**:  2017 _Genome Biology_ - CancerLocator: non-invasive cancer diagnosis and tissue-of-origin prediction using methylation profiles of cell-free DNA
* **Batch correction**: 2018 _Nature Biotech._ - Batch effects in single-cell RNA-sequencing data are corrected by matching mutual nearest neighbors

[PDFs](https://cloud.tsinghua.edu.cn/d/928f3f4a8c8d4ab8b8ad/?p=/Literature%20shared%20by%20John/Recommendation%20for%20Startup/AI%20%26%20Machine%20Learning&mode=list)

## 2. Deep Learning on RNA

> * **Course:**  Machine Learning \(CS229\) -- Andrew Ng : [coursera](https://www.coursera.org/learn/machine-learning)\*\*\*\*
> * **Book:    《**机器学习》-- 周志华 \([link](https://book.douban.com/subject/26708119/)\)  \([更多书籍课程推荐](https://lulab1.gitbook.io/training/appendix/appendix-i.keep-learning)\)

* **AS of RNA**: 2019 _Cell_ - Predicting Splicing from Primary Sequence with Deep Learning
* **AS of RNA \(DARTS**\): 2019 _Nature Methods_ - Deep-learning augmented RNA-seq analysis of transcript splicing
* **APA of RNA**: 2019 _Cell_ - A Deep Neural Network for Predicting and Engineering Alternative Polyadenylation
* **RNA/DNA-Protein Binding \(DeepBind\)**: 2015 _Nature Biotech._ - DeepBind: Predicting the sequence specificities of DNA- and RNA-binding proteins by deep learning
* **RNA secondary structure**: see [below](ai.md#3-1-rna-secondary-structure-prediction)
* **Cancer prediction using exRNA-seq**: see [below](ai.md#4-5-transfer-learning)

[PDFs](https://cloud.tsinghua.edu.cn/d/9553a9a553304ff7b311/?p=%2FDeep%20Learning%20on%20RNA&mode=list)

## 3. RNA Structure

> * **Course**: [生物物理学（清华大学）](https://www.ncrnalab.org/courses/#biophysics) 
> * **Book**:   《Biological Sequence Analysis: **Probabilistic Models** of Proteins and Nucleic Acids》by _Richard Durbin, Sean R. Eddy, Anders Krogh, Graeme Mitchison_  \([English](http://www.amazon.com/Biological-Sequence-Analysis-Probabilistic-Proteins/dp/0521629713) \| [中文](http://www.amazon.cn/dp/B003ZUIRZ2)\)

### 3.1 RNA Secondary Structure Prediction

* **Energy Model** 
  * **RNAstructure/Mfold**  and **RNAfold** 
    * How do RNA folding algorithms work? \(Sean R Eddy\) [2004 _Nature Biotech_](https://www.nature.com/articles/nbt1104-1457) 
    * What is dynamic programming? \(Sean R Eddy\) [2004 _Nature Biotech_](http://dx.doi.org/10.1038/nbt0704-909)\_\_
  * **SuperFold** for long distance base pairs \(folding\)  [2014 _Nature Methods_](https://www.ncbi.nlm.nih.gov/pubmed/25028896)\_\_

> **RNAstructure**/**Mfold**  and **RNAfold** perform good for sequence less than 200nt.
>
> **SuperFold** uses partition in RNAstructure package to predict partition functions for subsequences of long RNA, then merge the results. Therefore, it claims to perform better on long distance base pairs.

* **SCFG Model** \(Rfam/Infernal\)
  * What is a hidden Markov model? \(Sean R Eddy\) [2004 _Nature Biotech_](http://dx.doi.org/10.1038/nbt1004-1315) 
  * _You can read the SCFG section in the book_ [_above_](ai.md#3-1-rna-secondary-structure-prediction)_. \(Need a short tutorial for SCFG.\)_
* **Deep Learning Method**
  * \*\*\*\*[2020 ICLR](https://openreview.net/forum?id=S1eALyrYDH) - RNA Secondary Structure Prediction By Learning Unrolled Algorithms \([Chinese comments](https://mp.weixin.qq.com/s/SSFOJfljhRZuOOTErNefig)\)
  * \(**Transfer learning**\) 2019 _Nature Commn._ - SPOT-RNA: RNA secondary structure prediction using an ensemble of two-dimensional deep neural networks and transfer learning

[PDFs & PPTs](https://cloud.tsinghua.edu.cn/d/9553a9a553304ff7b311/?p=%2FRNA%20secondary%20structure%20prediction&mode=list)

### 3.2 Structural Motif Finder

* **SCFG \( Rfam/Infernal** [https://rfam.xfam.org/](https://rfam.xfam.org/) \)
  * **SCFG**: CMfinder - [2006 _Bioinformatics_](https://www.ncbi.nlm.nih.gov/pubmed/16357030) 
  * **SCFG**: RNApromo - [2008 _PNAS_ ](https://www.ncbi.nlm.nih.gov/pubmed/18815376)
  * **CFG:** TEISER - [2012 _Nature_](https://www.ncbi.nlm.nih.gov/pubmed/22495308)  
* **Graph Kernel:** GraphProt - [2014 _Genome Biology_ ](https://www.ncbi.nlm.nih.gov/pubmed/24451197)
* **SHAPE+HMM**:  PATTERNA - [2018 _Genome Biology_ ](https://www.ncbi.nlm.nih.gov/pubmed/29495968)

[PDFs & PPTs](https://cloud.tsinghua.edu.cn/d/9553a9a553304ff7b311/?p=%2FRNA%20Structural%20Motif&mode=list) 

## 4. Comp. Methods for Liquid Biopsy

### 4.1 Normalization and Batch Correction

* **Methods for Single Cell RNA-seq**: imputation, normalization, clustering, etc
  * Dropout and Sparseness
  * Heterogeneity and Normalization
  * Batch effect and Confounder
* **Recommendations**:
  * 2020 _Nature COMMN_ - Embracing the **dropouts** in single-cell RNA-seq analysis
  * 2019 - _Nature Methods_ - A discriminative learning approach to differential expression analysis for single-cell RNA-seq
  * 2017 - _Nature Methods_ - Normalizing single-cell RNA sequencing data: challenges and opportunities

> [PDFs](https://cloud.tsinghua.edu.cn/d/9553a9a553304ff7b311/?p=%2Fmethod%20-%20single%20cell&mode=list)
>
> [Tutorial](https://lulab1.gitbook.io/training/part-iii.-case-studies/case-study-1.exrna-seq/1.4.normalization-issues)

### 4.2  Feature Selection Method

[PDFs](https://cloud.tsinghua.edu.cn/d/9553a9a553304ff7b311/?p=%2Fmethod%20-%20Feature%20Selection&mode=list)

### 4.3 Network Approach

* 2018 _Nature COMMN._ - Pathway based subnetworks enable cross-disease biomarker discovery

[PDFs](https://cloud.tsinghua.edu.cn/d/9553a9a553304ff7b311/?p=%2Fmethod%20-%20Feature%20Selection&mode=list)

### 4.4 Tumor Location Method

* [Methods for Metagenomics](https://cloud.tsinghua.edu.cn/d/9553a9a553304ff7b311/?p=%2Fmethod%20-%20metagenomics&mode=list): tumor locator \(tissue match\), ranking, etc
* [Methods for Tumor Location](https://cloud.tsinghua.edu.cn/d/9553a9a553304ff7b311/?p=%2Fmethod%20-%20locator&mode=list): tumor locator \(tissue match\), etc

### 4.5 Transfer Learning

* 2020 _Bioinformatics_ - Exploiting transfer learning for the reconstruction of the human gene regulatory network
* \(see another example of transfer learning in SPOT-RNA [above](ai.md#3-1-rna-secondary-structure-prediction)\)

[PDFs](https://cloud.tsinghua.edu.cn/d/9553a9a553304ff7b311/?p=%2FTransfer%20Learning&mode=list)



