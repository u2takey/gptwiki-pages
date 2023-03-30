# mashtree 
## chatgpt 
As an AI language model, I do not have access to a specific system or software to explain the command "mashtree" in detail. 

However, in general, "mashtree" can refer to a command or a tool used in bioinformatics to generate a phylogenetic tree based on genomic distances between bacterial strains. It is part of the Mash software suite and requires a set of input genomes in FASTA format. 

The command often involves options for specifying input files and output directory, as well as selecting a distance metric and phylogenetic reconstruction method. It can also offer graphical visualization of the resulting tree for further analysis and interpretation. 

Overall, performing a mashtree command requires knowledge and skills in bioinformatics and genomics, including familiarity with relevant software and data processing techniques. 

## tldr 
 
> Makes a fast tree from genomes.
> Does not make a phylogeny.
> More information: <https://github.com/lskatz/mashtree>.

- Fastest method in mashtree to create a tree from fastq and/or fasta files using multiple threads, piping into a newick file:

`mashtree --numcpus {{12}} {{*.fastq.gz}} {{*.fasta}} > {{mashtree.dnd}}`

- Most accurate method in mashtree to create a tree from fastq and/or fasta files using multiple threads, piping into a newick file:

`mashtree --mindepth {{0}} --numcpus {{12}} {{*.fastq.gz}} {{*.fasta}} > {{mashtree.dnd}}`

- Most accurate method to create a tree with confidence values (note that any options for `mashtree` itself has to be on the right side of the `--`):

`mashtree_bootstrap.pl --reps {{100}} --numcpus {{12}} {{*.fastq.gz}} -- --min-depth {{0}} > {{mashtree.bootstrap.dnd}}`
