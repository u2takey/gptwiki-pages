# svgr 
## chatgpt 
SVGR is a Node.js-based tool that converts SVG files to React components. It can be used to optimize and stylize SVG files by converting them to reusable React components which can be easily integrated into React applications.

To use the SVGR command, you will need to install it globally using the Node.js package manager (npm):
```
npm install -g svgr
```
Once installed, you can use the SVGR command to convert SVG files to React components from the command line:
```
svgr myicon.svg
```
This will create a new file named `Myicon.js` in the same directory as the original SVG file. The new file will contain a React component that renders the original SVG graphic.

The SVGR command also supports a number of options that can be used to customize the output, such as specifying a custom component name, setting default props for the component, and adding custom CSS styling.

For example, the following command will create a new React component named `MyIcon` with a default fill color of `#F00`:
```
svgr myicon.svg --icon --replace-attr-values "#F00=currentColor" --out-dir=src/ --ext=js
```
This will create a new file named `MyIcon.js` in the `src/` directory with the specified options. The `--icon` option tells SVGR to format the output as a React component, while the `--replace-attr-values` option sets the default fill color for the component to `currentColor`. The `--out-dir` and `--ext` options specify the output directory and file extension, respectively.

In summary, the SVGR command is a useful tool for converting SVG files to reusable React components, and it provides a number of options for customizing the output to suit your needs. 

## tldr 
 
> Transform SVGs into React components.
> More information: <https://react-svgr.com>.

- Transform a SVG file into a React component to `stdout`:

`svgr -- {{path/to/file.svg}}`

- Transform a SVG file into a React component using TypeScript to `stdout`:

`svgr --typescript -- {{path/to/file.svg}}`

- Transform a SVG file into a React component using JSX transform to `stdout`:

`svgr --jsx-runtime automatic -- {{path/to/file.svg}}`

- Transform all SVG files from a directory to React components into a specific directory:

`svgr --out-dir {{path/to/output_directory}} {{path/to/input_directory}}`

- Transform all SVG files from a directory to React components into a specific directory skipping already transformed files:

`svgr --out-dir {{path/to/output_directory}} --ignore-existing {{path/to/input_directory}}`

- Transform all SVG files from a directory to React components into a specific directory using a specific case for filenames:

`svgr --out-dir {{path/to/output_directory}} --filename-case {{camel|kebab|pascal}} {{path/to/input_directory}}`

- Transform all SVG files from a directory to React components into a specific directory without generating an index file:

`svgr --out-dir {{path/to/output_directory}} --no-index {{path/to/input_directory}}`
