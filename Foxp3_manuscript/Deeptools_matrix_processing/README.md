This jupyter notebook aims to process the numbers in the deepTools computeMatrix outputs. For instance, to get the matrix of TnG peaks in sample.bw with up and downstream of 500bp, the computeMatrix would be:

computeMatrix reference-point --referencePoint center -S sample.bw -R TnG_peaks.bed -a 500 -b 500 -o sample_output -p 6 --sortRegions keep --outFileNameMatrix **sample_matrix**

The **sample_matrix** would be the input for this jupyter notebook. To read more about computeMatrix, please refer to the deepTools manual:

https://deeptools.readthedocs.io/en/2.1.0/content/tools/computeMatrix.html

