Welcome to our Hur lab Foxp3 paper's repository! Here you'll find the custom scripts with descriptions, sample inputs & expected outputs, as well as demo runs for our Foxp3 manuscript. All of them are written in Jupyter Notebook. To install Jupyter Notebook, please refer to their official website:

https://jupyter.org/install

As these scripts runs on Python, you'll be able to use them on any platform (windows, mac, linux) as long as you have a python environment. There are three folders here with distinct purposes:

1. Deeptools_matrix_processing

This notebook processes the outputs of Deeptools computeMatrix, and then calculate the row means to get the average intensity of each peak region. This is used for comparing the intensities of same set of peaks (e.g. Cut & Run peaks) in different samples.

2. FIMO_to_bed

This notebook processes the outputs of FIMO tsv file, and turns it into a bed file that can be readily used as any other bed files (e.g. by bedtools). For instance, you can FIMO search the TnG motif in organism genomes, use this to convert the FIMO tsv files to bed file, and then use bedtools merge to combine the overlapping FIMO regions to get TnG distribution in whole genomes.

3. HiC_Cool

This notebook processes HiC/Cool files into Pandas datasheets for further operation. For instance, we can separate Cut & Run peaks into TnG-contaning and not-TnG-containing by FIMO search, and then convert them into TnG-containing and NTnG-containing bins for HiC/Cool file operation. Here it then calculates the TnG-TnG, TnG-NTnG and NTnG-NTnG contact frequencies with different cutoffs.
