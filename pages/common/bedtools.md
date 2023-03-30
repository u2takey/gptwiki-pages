# bedtools 
## chatgpt 
Bedtools is a powerful and widely used command-line tool that is designed to help bioinformaticians perform complex operations on genomic data. This tool offers several functions to manipulate genomic data things such as genomic intervals like BED, GFF, and VCF files (as well as other generic interval formats), and to compare, merge, intersect, and subtract them. Here are some of the main command-line tools that fall under the bedtools package:

1. `bedtools intersect`: This tool identifies the regions of overlap between two or more BED files.

2. `bedtools merge`: This tool merges overlapping or adjacent BED files into a single, non-redundant set of genomic intervals.

3. `bedtools subtract`: This tool computes the regions in one BED or GFF file that are not covered by another.

4. `bedtools coverage`: This command-line tool calculates the coverage of features in a BAM file compared to a set of genomic intervals.

5. `bedtools window`: This tool extracts the genomic features within a defined distance (upstream or downstream) from a set of reference intervals.

6. `bedtools shuffle`: This command is used to shuffle the intervals within a BED file or between two BED files.

Bedtools is used extensively in the field of genomics and bioinformatics to perform advanced analysis of genomic data. The tool is fast, accurate, and easy to use, and it can handle large datasets with ease, which makes it a valuable resource for researchers and scientists working on genomics projects. 

## tldr 
 
> A swiss-army knife of tools for genomic-analysis tasks.
> Used to intersect, group, convert and count data in BAM, BED, GFF/GTF, VCF format.
> More information: <https://bedtools.readthedocs.io>.

- Intersect two files regarding the sequences' strand and save the result to the specified file:

`bedtools intersect -a {{path/to/file_1}} -b {{path/to/file_2}} -s > {{path/to/output_file}}`

- Intersect two files with a left outer join, i.e. report each feature from {{file_1}} and NULL if no overlap with {{file_2}}:

`bedtools intersect -a {{path/to/file_1}} -b {{path/to/file_2}} -lof > {{path/to/output_file}}`

- Using more efficient algorithm to intersect two pre-sorted files:

`bedtools intersect -a {{path/to/file_1}} -b {{path/to/file_2}} -sorted > {{path/to/output_file}}`

- Group file {{`path/to/file`}} based on the first three and the fifth column and summarize the sixth column by summing it up:

`bedtools groupby -i {{path/to/file}} -c 1-3,5 -g 6 -o sum`

- Convert bam-formatted file to a bed-formatted one:

`bedtools bamtobed -i {{path/to/file}}.bam > {{path/to/file}}.bed`

- Find for all features in {{file_1}}.bed the closest one in {{file_2}}.bed and write their distance in an extra column (input files must be sorted):

`bedtools closest -a {{path/to/file_1}}.bed -b {{path/to/file_2}}.bed -d`
