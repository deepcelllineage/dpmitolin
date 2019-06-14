# dpmitolin
Use mitochondrial sequence from single cells to determine cell lineage relationships with deep learning techniques. 
The questions to be answered are 

1. How do basal (B), luminal progenitor (P), and luminal terminal (T) cells relate using mitochondrial sequence data.  In traditional bioinformatics relationships between cells established by using hierarchical clustering over gene expression data. Gene expression data is derived from raw sequences using alignment with a reference genome. This process involves several steps using state of the art library Seurat available in R. Can we do as good of a job in figuring out relationships among cells directly from raw FASTA data bypassing the gene expression and Seurat using power of Deep Neural Networks?

The methods that we would create should be able to 
- overcome technical noise created by sequencing equipment so that our technique would reliable pull valid  mutation signal from the error noise introduced by sequencing process.
- be as good as Seurat in detection of relationships 
- be computationally cheaper, faster or simpler than the current state of the art practice

2. Given all features, with what accuracy can a DNN assign cells to their mtLT-defined cluster? All features: 
- For ATAC: all DNA sequence data, i.e. mtDNA sequences & uncoiled nuclear DNA sequences 
- For C1 and 10x: all mRNA sequences (including mtRNA) and expression levels of each sequence
More features can be added to both...


## More Info

For more information on the deepcelllineage (DCL) project and background for dpmitolin, please see our overview repo and especially the [overview wiki](https://github.com/deepcelllineage/overview/wiki)