This jupyter notebook aims to process the numbers in the deepTools computeMatrix outputs. For instance, to get the matrix of TnG peaks in sample.bw with up and downstream of 500bp, the computeMatrix would be:

computeMatrix reference-point --referencePoint center -S sample.bw -R TnG_peaks.bed -a 500 -b 500 -o sample_output -p 6 --sortRegions keep --outFileNameMatrix **sample_matrix**

The **sample_matrix** would be the input for this jupyter notebook. To read more about computeMatrix, please refer to the deepTools manual:

https://deeptools.readthedocs.io/en/2.1.0/content/tools/computeMatrix.html

The matrix **Inputs** of this jupyter notebook is in the Input directory. They are calculated by using refined TnG and NTnG peaks +/- 500bp in different bw files. These bw files were acquired by trimming and aligning the raw fastq files (SRA fasterq-dump of database DRP003376) to mm10 genome in this paper by Sakaguchi group:

Kitagawa, Yohko, et al. "Guidance of regulatory T cell development by Satb1-dependent super-enhancer establishment." Nature immunology 18.2 (2017): 173-183.

The expected outputs of this jupyter notebook is in the **Expected_output** folder. These would be the combined csv datasheets with peak intensities. You can simply download everything in the Deeptools_matrix_processing directory recursively, execute the jupyter notebook, and you would see the same two csv datasheets in the same folder as the .ipynb file. You can then compare your own outputs with the two outputs in the **Expected_output** folder. 





