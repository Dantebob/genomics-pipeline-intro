# Genomics Pipeline Introduction Worksheet

<!--- Write name below --->
## Name: Dante Celani 

<!--- For this worksheet, answer the following questions --->

## Q1: What is a bioinformatics pipeline?
Answer: a bioinformatics pipeline is an algorithm that processes sequences. If the program already exists you don't need to write it. 


## Q2: What are the three basic filetypes discussed in this repository? What information do they contain?
Answer: Fata/fastq, SAM/BAM, and VCF (variant call format)

## Q2: What does a general bioinformatics pipeline look like? Draw a schematic of a pipeline (using boxes and arrows) and add the image file name to the <insert-file-name-here> text below (png or jpg will work). Your schematic should include file types, program types (e.g., mapping program), and arrows between file types.
![Raw Read FastQC Quality](./images/general_bioinformatics_pipeline.png)

## Q3: Using information from the genomics-pipeline-intro.sh script and [Farkas et al., 2021](https://doi.org/10.3389/fmicb.2021.665041), draw another schematic specific to their study showing file types, program types (use specific program names in this schematic), and arrows between file types. Add the image file name to the <insert-file-name-here> text below.
![Raw Read FastQC Quality](./images/more_specific_bioinformatics_pipeline.png)

## Q4: After running the genomics-pipeline-intro.sh script, how many variants are in merged.vcf?
Answer: 1640

## Q5: What is the alternate allele depth of sample SRR11621811|unknown at site 25350 in contig NC_045512.2?
Answer:  DPRA = 0
" grep 'NC_045512.2' SRR11621811.bam.freebayes.vcf "
##INFO=<ID=DPRA,Number=A,Type=Float,Description="Alternate allele depth ratio

## Q6: In what ways would you consider filtering the VCF? In other words, what criteria would you use to remove variants / genotypes from the dataset?
Answer: If a variant had a really low quality score I'd remove it.
