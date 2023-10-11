This Jupyter Notebook documents the steps for converting HiC/Cool data to pandas dataframes, and calculating the contact intensities between bins containing TnG vs NTnG Cut & Run peaks.
The HiC/Cool datasets were directly downloaded from these two papers and their associated GSE datasets:

1. GSE190057; Ramirez, Ricardo N., et al. "FoxP3 associates with enhancer-promoter loops to regulate Treg-specific gene expression." Science immunology 7.67 (2022): eabj9836.
2. GSE217147; Liu, Zhi, et al. "Foxp3 Orchestrates Reorganization of Chromatin Architecture to Establish Regulatory T Cell Identity." bioRxiv (2023): 2023-02.

To process the .hic or .cool datasets, two packages were needed in Jupyter Notebook: 
1. hic2cool; this can be readily installed by "pip install hic2cool"
2. cooler; similarly, this can be readily installed by ""pip install cooler"

In the Jupyter Notebook example, the GSE samples used were:
1. GSM5702000, Foxp3 Treg HiChip repeat1, cool format
2. GSM5702001, Foxp3 Treg HiChip repeat2, cool format
3. GSM6705677, Foxp3 PLACseq, HiC format

As the raw HiC and cool files are too big to upload for GitHub, please download them directly from GSE database and put them in the same folder as the Jupyter Notebook.

The two bed files are the bins containing TnG-CnR peaks and NTnG-CnR peaks; they were used as additional inputs for dataframe operations
