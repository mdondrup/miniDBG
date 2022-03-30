# miniDBG
Example solution for the De Bruijn Graph assembly problem in BINF301. The code consists of a single Jupyter notebook with a single class: DBGraph

------

Try it right in your browser! No installs necessary. Ready to 'Run All' upon notebook appearing.   
Press the launch button below to launch a session served via MyBinder:  
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mdondrup/miniDBG/HEAD?labpath=DBG-miniassembler.ipynb)


------------


Dependencies:

 - Igraph for Python https://igraph.org/python/
 - Bio.SeqIO

The notebook contains example usage code and an example FASTA file. This code is a toy example that is not maent to assemble real short read sequencing data. It is meant  to experiment with different graph analysis, assebly and filtering strategies on toy examples and for teaching. It should also demonstrate the multitude of special cases a developer has to consider when attempting a real implementation as opposed to reading about algorithms in papers.  Thanks to the Igraph package, small graphs can be visualized which helps debugging and seeing the effects of different graph transformations. 

What is supported:

 - create graphs with user defined k-mer size
 - alphabet is not restricted to ACGT, can be any unicode characters
 - add nodes or k-mers directly, or parse a FASTA file
 - compact the graph by joining linear nodes into one
 - simple bubble detection and removal
 - greedy assembly into contigs
 - visualization of graphs

What is lacking:

 - DBGraph does only support forward strand
 - no paired end support
 - no support for FASTQ and sequence quality 
 - will likely not work with larger datasets with millions of reads
 - no multithreading

-------------

Launch a session in your browser with everything installed and ready to run:  
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mdondrup/miniDBG/HEAD?labpath=DBG-miniassembler.ipynb)
