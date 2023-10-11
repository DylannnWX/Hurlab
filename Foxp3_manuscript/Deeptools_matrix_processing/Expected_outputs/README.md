The format of these outputs are .csv files, with all peak intensities of all bw files combined into the same datasheet for downstream plotting (e.g. violin plots).

Each row of the csv represents the average intensity of observed peak region with given up/downstream lenghts in computeMatrix (e.g. -a 500, -b 500). If you kept the original peak orders in computeMatrix (e.g. --sortRegions keep), then the order of this csv file will be the same as your input peak used for computeMatrix.
