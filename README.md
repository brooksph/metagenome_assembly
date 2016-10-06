# Metagenomic assembly pipline 
I am testing a metagenomic assembly pipline on a small E. coli data set 
provided by Sherine Awad and avaiable
[here](https://s3.amazonaws.com/public.ged.msu.edu/ecoli_ref-5m.fastq.gz)

## Sequencing files 

All raw Fastq sequences are in 'data/seqs/':

	$Find data/seqs -name ".fq.gz"

## Quality control steps 

After the sequencing data was downloaded our first step of analysis was assuring 
that the sequences are of high quality. We ran the sequence through a quality 
diagnostic and control pipeline: 

1. Create base quality diagnostic graphs 

Fastqc v 

2. Check reads for adapter sequences

3. Trim adapter sequences 

4. Trim poor quality bases 

Trimmomatic or skewer 




