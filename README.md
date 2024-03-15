# RNAseq-upstream
Workflow to generate count table from paired-read RNA-seq.

## Prerequisites
The main workflow uses the following software/packages\: \
1. QC, adapter and quality trimming - Fastp \
2. Alignment - STAR \
3. Count generation - HTSeq-count 

It's recommended to install the softwares with conda\: \
1. Create conda environment\: `conda create -n rna-seq` \
2. Configure package channels\: \
`conda config --add channels defaults` \
`conda config --add channels bioconda` \
`conda config --add channels conda-forge` \
`conda config --set channel_priority strict` \
For Apple Silicon Mac, `conda config --add subdirs osx-64` \
3. Install packages\: \
`conda install -n rna-seq -c bioconda star fastp htseq` 
