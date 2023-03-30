# texliveonfly 
## chatgpt 
TeXLiveOnFly is a package of TeXLive that allows users to download and automatically input the required packages, classes, and fonts for typesetting LaTeX documents. In other words, it is a tool to automatically download missing dependencies during typesetting from CTAN (Comprehensive TeX Archive Network) repository.

To use TexLiveOnFly, you can run a command in the terminal:

```
texliveonfly <filename.tex>
```

This will compile the LaTeX document with its necessary packages that are not installed on your local computer. If a package is not available online, the process will halt, and you will see an error message.

When you run this command, the TexLiveOnFly package will fetch the missing files from CTAN and stores them in the working directory. It then re-runs LaTeX and compiles the document using the downloaded packages. After compilation, the temporary files created during the process will be deleted.

TexLiveOnFly can be especially useful for beginners, who might not know which packages are required to compile their code. By automatically downloading missing packages, TexLiveOnFly saves time and eliminates errors caused by missing dependencies. 

## tldr 
 
> Downloads missing TeX Live packages while compiling `.tex` files.
> More information: <https://ctan.org/pkg/texliveonfly>.

- Download missing packages while compiling:

`texliveonfly {{source.tex}}`

- Use a specific compiler (defaults to `pdflatex`):

`texliveonfly --compiler={{compiler}} {{source.tex}}`

- Use a custom TeX Live `bin` folder:

`texliveonfly --texlive_bin={{path/to/texlive_bin}} {{source.tex}}`
