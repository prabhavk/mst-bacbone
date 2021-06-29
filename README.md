# About mst-backbone

mst-backbone is a phylogeny inference program that performs constrained search through tree-space. The main features of mst-backbone are

1) The use of a minimum spanning tree framework for constraining search through phylogenetic tree-space.

2) Performing tree search under the general Markov model (GMM) using structural EM. We plan on extending the tree search operations to include NNI and SPR.

Here is the link to the preprint describing the performance of mst-backbone. 

https://www.biorxiv.org/content/10.1101/2020.06.30.180315v1

# Instructions for compilation

Please download all the files in the repository and run make. The binary file for conducting tree search is **mst-backbone**

# Usage: 

mst-backbone  multiple_sequence_alignment_file  size_of_subtree

Parameters:

A multiple sequence alignment file either in FASTA format or PHYLIP format

size_of_subtree: the size of the vertex sets that induce a subtree and a connected graph in the MST; The sequences of the selected vertices (taxa) are used to infer local phylogenetic trees that are subsequently combined to construct a global phylogenetic tree. Default value of 10 seems adeqate and was tested on multiple empirical and simulated datasets.
