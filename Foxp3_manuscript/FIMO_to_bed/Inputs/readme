The goal of this notebook is to convert FIMO outputs to peak bed files. This allows further operation by a variety of softwares (e.g. bedtools).

For instance, the attached .tsv files are direct FIMO outputs by searching the TnG motif in all human, mouse or zebrafish genome. 

The bed files have some specific format requirements that this notebook will cover:

1. All must be tab-delimited.

2. The first column, chromosome, have a naming convention checks. 
  2a. If any row starts with "chr", then all other must start with "chr" as well.
  2b. If none of the rows start with "chr", you can then name your chromosome however you like.
  2c. Apparently, the authors of bedtools did this because some genome references have names like "chr1" while other just call it "1". This creates problems when you process any peak overlaps or whatnot.

3. The second and third column, start and end, must be integers. In addition, the start number must be smaller than the end number. This isn't always the case for FIMO, because for minus-stranded motifs, the start number is larger.

4. This notebook also includes motif length, strand and name. For minus-stranded motifs, the start/end numbers will be switched, while the strand will be marked as "-". 
