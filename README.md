# SpecialCourse-TCRpMHC
Large Scale Modelling and Analysis of TCR-pMHC

To get the input file:

wget -O "new_name.tar.gz" "https://www.dropbox.com/s/7qwe0a277nlulap/SearchTable-2020-02-06%2014_18_56.611.tsv?dl=0"

Content:

Infiles are SearchTable, Vgenes File, Jgenes File.

Search Table in a dataframe each TCR (complex.id) with:
  - TRA/TRB
  - CDR3
  - V gene
  - J gene
  - Specie
  - MHC A
  - MHC class
  - Epitope
  
Drop N/A and unpaired entries

### Heatmaps with the data normalized by KL divergence
-How often V genes are seen together with J genes per germline (Alpha and Beta) --> Alpha(Vgene vs Jgene)
-How often V genes in alpha are together with V genes in beta (VgeneAlpha vs VgeneBeta) Plot Clustermap
(Do same for Beta)

### Sequences are put together and the alignment is performed with HMM

### Calculate seq_id from CDR3

### Calculate seq_id from peptides after Pairwised alignment

### Calculate seq_id from MHC after alignment with HMM
Get the sequences, for some of them the name must be processed in order to be found (4 digits MHC nomenclature)

