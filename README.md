# Introduction
Homopolish is a Nanopore-specific polisher able to generate a high-quality genome (Q40-50) for virus, bacteria, and fungus.

# Installation
Homopolish is recommendated to install and run within a conda environment

	git clone https://github.com/ythuang0522/homopolish.git
	conda env create -f environment.yml
	conda activate homopolish

# Download virus, bacteria, or fungi sketches
Homopolish makes uses of compressed genomes (Mash sketches) for identifying most-similar genomic sequences. The pre-sketches (virus/bacteria/fungi) can be downloaded.

	Virus: wget http://bioinfo.cs.ccu.edu.tw/bioinfo/mash_sketches/virus.msh.gz
	Bacteria: wget http://bioinfo.cs.ccu.edu.tw/bioinfo/mash_sketches/bacteria.msh.gz
	Fungi: wget http://bioinfo.cs.ccu.edu.tw/bioinfo/mash_sketches/fungi.msh.gz

# Execution
Homopolish is reccomended to run in conjunction with one of the three sketches.

	python homopolish.py polish -

