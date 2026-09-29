# SiSimple
A Python based tool for the analysis of siRNA designed based on the works of Fakhr and associates


This tool is designed to perform 17 checks on siRNA design:
- Blast of Sense and antisense strand (>78% coverage)
- Not being located at SNP site
- Not being located within the first 75 base pairs
- Not being in the intron 
- Having GC content between 36-52%
- Antisense G/C content 2nd-7th N=19% and 8th to 18th N=52%
- Assymetrical base pairing in the duplex
- GC and AT repeats less than 3 and 4 respectively 
- Not having any internal secondary structures
- Having 3' overhanging -TT's
- Weak base pairing of the 5' end of antisense 
- Strong base pairing at the 5' end of the sense strand 
- Presence of A at the 6th position of the antisense strand
- Presence of A at the 3rd, 19th position of the sense strand
- Absence of G at 13th nucleotide of the sense strand 
- Absence of GC at the 19th position of the sense strand
- Presence of U at the 10th nucleotide  of the sense strand

**In order to use this tool, 3 main pieces of information need to be provided:**
- siRNA Guide Strand
- NCBI gene name
- Ensembl ID
With the option to provide the target sequence as well

**You must also have installed Biopython and ViennaRNA, the method for doing which will depend where you intend to run the code**

**Troubleshooting**
Since this programme uses online databases for many of the criteria, it is unfortunately subject to the whims of uptime and maintenance. Ensembl especially seems to enjoy being inaccessible at the time of writing. The three main error codes to be aware of are:
Code 500: Ensembl server error
Code 429: Rate limited

These codes should be reported to you, and the code will bypass the checks and continue the rest of the scoring. 

DISCLAIMER: I do not have a programming background, please inform me of any errors or ways to improve this code, as I would like it to remain open source and "upgradable" as my skills and knowledge improve. One such example is my ongoing crusade to understand Molecular Mechanics Poisson–Boltzmann Surface Area computations, which will hopefully be included soon. Thank you for using Sam's Simple siRNA.
