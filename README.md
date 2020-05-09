# Comp_Genomics
Repository for the final Computational Genomics project, analyzing gliomas.

The data for this project can be found on the Chinese Glioma Genome Atlas (http://www.cgga.org.cn/download.jsp - Part C). It consists of a matrix of RNA-seq gene expression counts for 24000+ genes and a separate matrix of clinical information of each of the 325 patients/samples. The clinical data as well as the processed train and test data are included in this repository.

To replicate this project, download the raw expression and clinical data sets from the Chinese Glioma Genome Atlas. Load this into the same directory as the downloaded repository. First, run the data_processing script to create test and train data and labels. Save those data in the directory as well. The remaining code can be run in any order.

The code can be run on any RNA-seq expression count data as long as each sample is given a pre-determined label, and the format follows that of the original data.

Requirements: Python with the following packages:
- numpy
- sklearn
- seaborn
- matplotlib
- scipy
- pandas
- pygmnormalize (git+https://github.com/ficusss/PyGMNormalize.git)
- skfuzzy (-U scikit-fuzzy)
- umap (only for the umap code)
- collections (only for supervised)
- torch (only for supervised)
- mord (only for supervised)

All of the above can be installed using the `pip` command. 
