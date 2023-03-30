# latexdiff 
## chatgpt 
Latexdiff is a software program used to highlight the differences between two LaTeX files. It is particularly useful when reviewing changes made to a document, or for comparing two versions of a manuscript. Here are the various components of the latexdiff command:

- The command: The command for running latexdiff is simply "latexdiff" followed by the two file names you want to compare. For example:

latexdiff old_file.tex new_file.tex

- Input files: The first argument to the latexdiff command is the original file (often the old version) that you want to compare with the second argument, which is the revised file (the new version). Both files should be in LaTeX format, typically with the .tex extension. The two files should contain similar content, but with some modifications, deletions, or additions.

- Output format: By default, latexdiff outputs an annotated (colored) LaTeX code that highlights the differences between the two input files. This output file can be compiled with LaTeX to produce a PDF or DVI document.

- Options: Latexdiff has many options that allow you to customize the output. For example, you can modify the colors and styles used to highlight the changes, or specify which parts of the documents should be compared. You can also generate a standalone document with the changes highlighted, or include the changes in the main manuscript.

Some of the most common options include:

--flatten: Combines the changes into a single document, instead of showing them side-by-side.

--math-markup: Shows changes to equations and other math environments.

--exclude-textcmd: Ignores certain types of text commands (such as \cite, \ref, etc.).

--graphics-markup: Shows changes to graphics files.

Overall, latexdiff is a versatile tool that can help streamline the process of editing and revising LaTeX documents. 

## tldr 
 
> Determine differences between two LaTeX files.
> More information: <https://ctan.org/pkg/latexdiff>.

- Determine changes between different versions of a LaTeX file (the resulting LaTeX file can be compiled to show differences underlined):

`latexdiff {{old.tex}} {{new.tex}} > {{diff.tex}}`

- Determine changes between different versions of a LaTeX file by highlighting differences in boldface:

`latexdiff --type=BOLD {{old.tex}} {{new.tex}} > {{diff.tex}}`

- Determine changes between different versions of a LaTeX file, and display minor changes in equations with both added and deleted graphics:

`latexdiff --math-markup=fine --graphics-markup=both {{old.tex}} {{new.tex}} > {{diff.tex}}`
