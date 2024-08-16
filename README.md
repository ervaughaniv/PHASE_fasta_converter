I needed to phase some single-gene Sanger sequence alignments for a BEAST phylogeny, and I opted to use the program PHASE (Stephens et al. 2001). This program requires a specific input file format 
which would be tedious to generate by hand from a fasta file (which was my existing data format). It also produces an output that does not easily convert back to fasta. I thus created two functions, 
the first of which takes in a fasta file and creates a PHASE input file, and the second of which generates two new phased fastas from the original fasta file and the PHASE output file. There are 
easily conceivable situations that would break the script (eg, a triple ambiguity code in the same data column as genuine heterozygous sites), but I wrote this script for my own data, so I didn't 
build the script to reckon with these cases.
