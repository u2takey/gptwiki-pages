# picard 
## chatgpt 
Picard is a command-line file format converter and manipulation tool for sequence data such as FASTQ, SAM, and BAM files. It is part of the Broad Institute's suite of bioinformatics tools and is written in Java.

Picard has a wide range of functions, including:

- Sorting and merging BAM files
- Marking duplicates in BAM files
- Quality control on sequencing data
- Reordering SAM/BAM files
- Converting between different file formats

To use Picard, you need to install it first. You can download the latest version from the Picard website. 

Once you have installed the Picard software, you can use it through the command line. For example, to sort a BAM file, you would type:

```
java -jar picard.jar SortSam \
     INPUT=input.bam \
     OUTPUT=output.bam \
     SORT_ORDER=coordinate
```

This command sorts the input.bam file by coordinate order and outputs the sorted file to output.bam. The `-jar` option specifies the Picard software JAR file, and the `SortSam` argument specifies the particular Picard function to use.

There are many other Picard functions you can use, and each has its own set of required and optional arguments. You can find more information about these functions by visiting the Picard documentation website. 

## tldr 
 
> Next generation MusicBrainz tagging application.
> More information: <https://picard.musicbrainz.org/>.

- Start Picard:

`picard`

- Open a set of files:

`picard {{path/to/file1.mp3}} {{path/to/file2.mp3}}`

- Display the version of Picard installed:

`picard --long-version`
