# F1Lab
This is an internship emulator by Dean Lee: F1L on Linkedin
# **Week 1**
**The KSQ:** Using available scRNA-seq data from cancer cell lines, can the following cancer therapies, Trastuzumab and Bevacizumab, help/target additional cancers?

**What is scRNA-seq?** 
scRNA stands for single-cell RNA sequencing. This methodology allows for the collection of gene expression of individual cells by measuring the abundance of mRNA molecules. The data gathered can help you understand gene expression since it can provide information on which genes are expressed and the expression level.  

ScRNA-seq data can be used to group cells with similar gene expression profiles. The data can also identify if gene expression is different groups of cells, such as those of healthy vs. cancerous cell lines. The data can also be collected as cells undergo dynamic changes, such as differentiation, development, and response to stimuli (treatment), to understand which genes may be necessary in driving these transitions. 

**What are the best practices when dealing with this data?**
Best practices begin in the data collection, where low-quality cells (doublets) are filtered out. People then normalize the data to reduce the variability across cells and dimensionality reduction (PCA or UMAP) to simplify the data while retaining key bio information. We can cluster cells based on similar gene expression profiles. Still, before that, it is good to do batch effect corrections (minimize or remove the variability that occurs when collecting data in multiple or different batches while retaining meaningful differences). Differential gene expression can be used to understand the difference between clusters. Trajectory inferring can be used to understand the dynamics of cells (e.g., gene expression as cells progress through development). 

**What are the most commonly used cell lines in cancer?**
HEK293 (Human Embryonic Kidney 293): A widely used cell line derived from human embryonic kidney cells. HEK293 cells are often used in studies related to gene expression, signaling pathways, and for validating scRNA-seq methods.

A549 (Lung Cancer Cell Line): A human lung adenocarcinoma cell line frequently used in cancer research. A549 cells are particularly useful in studies involving drug sensitivity and cancer cell biology.

K562 (Chronic Myeloid Leukemia): This human leukemia cell line is used extensively in studies of blood cancer, hematopoiesis, and gene regulation. It's also a popular choice for scRNA-seq studies involving immune cells.

MCF-7 (Breast Cancer Cell Line): Derived from human breast cancer, MCF-7 cells are frequently used to study cancer biology, especially breast cancer, and to test responses to therapeutic agents.

Jurkat (T Cell Leukemia): This human T cell leukemia cell line is widely used in immunology research, particularly for studying T cell signaling, immunotherapy, and T cell receptor (TCR) biology.

HCT116 (Colon Cancer): A commonly used human colon cancer cell line in cancer research, particularly in studies of colorectal cancer biology and drug testing.

iPSCs (Induced Pluripotent Stem Cells): These are cells generated by reprogramming adult cells to a pluripotent state. They are frequently used in developmental biology, regenerative medicine, and studies on differentiation and cell lineage tracing using scRNA-seq.

**What is the molecular mechanism of action for Trastuzumab?**
Trastuzumab is a monoclonal antibody that primarily treats HER2-positive breast cancer. HER2 receptor is a tyrosine kinase that, when it's overexpressed, leads to uncontrollable cell growth and cancer. Trastuzumab binds to the HER2 receptor, blocking the receptor from growth signal and preventing its activation, which reduces cell proliferation. It also promotes the internalization and degradation of the HER2 receptor.  

*According to information online, HER2 is in the same receptor family as EGFR. 

**What is the molecular mechanism of action for Bevacizumab?**
Bevacizymab is a monoclonal antibody that targets vascular endothelial growth factor A (VEGF-A). VEGT-A is a protein that helps promote the growth of new blood vessels. It's involved in developing a few cancers like colorectal, lung, kidney, and other cancers. This drug binds to the VEGT-A protein, inhibiting the expression of VEGFR-1 and VEGFR-2 receptors found in the surface of endothelial cells. 

**Unanswered Questions** 
How does this data look like when it's reported? What variables should I expect to see in this dataset?

#**References**
Haque, A., Engel, J., Teichmann, S. A., & Lönnberg, T. (2017). A practical guide to single-cell RNA-sequencing for biomedical research and clinical applications. Genome Medicine, 9(1). https://doi.org/10.1186/s13073-017-0467-4

Swain, S.M., Shastry, M. & Hamilton, E. Targeting HER2-positive breast cancer: advances and future directions. Nat Rev Drug Discov 22, 101–126 (2023). https://doi.org/10.1038/s41573-022-00579-0

