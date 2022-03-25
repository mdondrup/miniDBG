# miniDBG
Example solution for the De Bruijn Graph assembly problem in BINF301. The code consists of a single Jupyter notebook with a single class: DBGraph

Dependencies:

 - Igraph for Python https://igraph.org/python/
 - Bio.SeqIO

The notebook contains example usage code and an example FASTA file. This code is a toy example that is not maent to assemble real short read sequencing data. It is meant  to experiment with different graph analysis, assebly and filtering strategies. It should also demonstrate the multitude of special cases a developer has to consider when attempting a real implementation as opposed to reading about algorithms in papers.  Thanks to the Igraph package, small graphs can be visualized which helps debugging and seeing the effects of different graph transformations. 

