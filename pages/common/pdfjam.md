# pdfjam 
## chatgpt 
Pdfjam is a command-line tool in Ubuntu Linux that is used to manipulate and rearrange pdf files. It provides a collection of scripts that allow you to join, split, rotate, crop, watermark, and rearrange pages in a pdf file.

Here are some of the options that you can use with the pdfjam command:

1. Join pdf files: `pdfjoin file1.pdf file2.pdf output.pdf`

2. Split pdf files: `pdfsplit input.pdf`

3. Rotate pdf files: `pdf90 input.pdf`

4. Arrange pdf files: `pdfnup input.pdf`

5. Add watermark to pdf files: `pdfjam input.pdf -o output.pdf --background water.pdf`

Overall, the pdfjam command provides powerful tools for working with pdf files and can save you a lot of time and effort when manipulating them. 

## tldr 
 
> Shell frontend for the LaTeX pdfpages package for mingling PDFs.
> More information: <https://github.com/rrthomas/pdfjam>.

- Merge two (or more) PDFs:

`pdfjam {{path/to/file1.pdf}} {{path/to/file2.pdf}} --outfile {{path/to/output_file.pdf}}`

- Merge the first page of each file together:

`pdfjam {{files...}} 1 --outfile {{path/to/output_file.pdf}}`

- Merge subranges from two PDFs:

`pdfjam {{path/to/file1.pdf 3-5,1}} {{path/to/file2.pdf 4-6}} --outfile {{path/to/output_file.pdf}}`

- Sign an A4 page (adjust delta to height for other formats) with a scanned signature by overlaying them:

`pdfjam {{path/to/file.pdf}} {{path/to/signature}} --fitpaper true --outfile {{path/to/signed.pdf}} --nup "{{1x2}}" --delta "{{0 -842pt}}"`

- Arrange the pages from the input file into a fancy 2x2 grid:

`pdfjam {{path/to/file.pdf}} --nup {{2x2}} --suffix {{4up}} --preamble '{{\usepackage{fancyhdr} \pagestyle{fancy}}}'`

- Reverse the order of pages within each given file and concatenate them:

`pdfjam {{files...}} {{last-1}} --suffix {{reversed}}`
