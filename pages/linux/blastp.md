# blastp 
## chatgpt 
The command "blastp" is a bioinformatics program that is used for comparing protein sequences with each other. The 'blast' is an acronym for Basic Local Alignment Search Tool. The 'p' in 'blastp' stands for protein, since it is used for protein to protein alignments. 

Blastp compares the query protein sequence to a protein database and identifies regions of similarity that may indicate functional, structural, or evolutionary relationships between the sequences. The output of the blastp program provides information about the similarities and differences in sequence among the query and the database proteomes.

The blastp command takes several arguments to carry out the protein sequence comparison. The arguments include the input query sequence, the protein database to search, and the search parameters such as gap penalties, word size, e-value threshold, and matrix to be used for scoring the alignments.

Overall, the blastp command is a powerful tool used by bioinformaticians, molecular biologists, and computational biologists for identifying and studying protein sequences and their functions. 

## tldr 
 
> Protein-Protein BLAST.
> More information: <https://www.ncbi.nlm.nih.gov/books/NBK279684/table/appendices.T.blastp_application_options/>.

- Align two or more sequences using blastp, with the e-value threshold of 1e-9, pairwise output format, output to screen:

`blastp -query {{query.fa}} -subject {{subject.fa}} -evalue {{1e-9}}`

- Align two or more sequences using blastp-fast:

`blastp -task blastp-fast -query {{query.fa}} -subject {{subject.fa}}`

- Align two or more sequences, custom tabular output format, output to file:

`blastp -query {{query.fa}} -subject {{subject.fa}} -outfmt '{{6 qseqid qlen qstart qend sseqid slen sstart send bitscore evalue pident}}' -out {{output.tsv}}`

- Search protein databases using a protein query, 16 threads to use in the BLAST search, with a maximum number of 10 aligned sequences to keep:

`blastp -query {{query.fa}} -db {{blast_database_name}} -num_threads {{16}} -max_target_seqs {{10}}`

- Search the remote non-redundant protein database using a protein query:

`blastp -query {{query.fa}} -db {{nr}} -remote`

- Display help (use `-help` for detailed help):

`blastp -h`
