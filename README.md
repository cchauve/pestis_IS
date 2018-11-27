Cedric Chauve, november 27, 2018

This directory contains data about a group of *Yersinia pestis* and
*Yersinia pseudoituberculosis* genomes, studied in the paper
*Comparative scaffolding and gap filling of ancient bacterial genomes
applied to two ancient Yersinia pestis genomes*
(http://dx.doi.org/10.1099/mgen.0.000123). 

The goal of collecting these data is to study the use of Insertion
Sequences (IS )as repeats mediating inversions in bacterial genomes,
as discussed in
* https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5009759/
* https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6114881/
* http://www.asmscience.org/content/journal/microbiolspec/10.1128/microbiolspec.MDNA3-0030-2014
* https://www.sciencedirect.com/science/article/pii/S1369527406001275?via%3Dihub


The directory *genomes/* contains the DNA sequence of the chromosome of
all considered genomes. This implies that the plasmids, which qre
important in terms of virulence and pathogenecity, are not present in
the sequence data. All sequences are in a single FASTA file.

The directory *basys_hmm/* contains, for a set of IS families, a
FASTA file, per IS family, of the IS genes found in the genomes by the
automatic bacterial genomes annotation system Basys
(https://www.basys.ca/, accessed prior to the submission of the
paper), together with an HMM file encoding the sequence profile of the
family. These HMMs were computed by Daniel Doerr using the hmmer tool
(http://hmmer.org/) and the basys-annotated IS. Note that the FASTA
files contains annotations for the strain *Angola* that is not present
elsewhere in these data, as the genome is generally recognized as
being poorly assembled.

Finally, the directory *detected_IS/* contains the list of IS elements
detected by running the HMM on the considered genomes, again
considering only chromosomes and excluding plasmids.

Likely, these data need to be looked at carefully before being used;
they result from a fully automated pipeline.