# ts-node 
## chatgpt 
`ts-node` is a command used to execute TypeScript files directly without the need to first compile it to JavaScript. It is a package that allows users to run TypeScript files without the extra steps of configuring a build process, as is typically required when using TypeScript.

When the `ts-node` command is executed, it first transpiles the TypeScript code into JavaScript in-memory using the TypeScript compiler, then executes the resulting JavaScript code directly in Node.js. This allows for a faster and more streamlined development process that eliminates the need for an extra build step.

To use the `ts-node` command, you must first install it globally on your system:

```bash
npm install -g ts-node
```

Once `ts-node` is installed, you can run a TypeScript file directly using the following syntax:

```bash
ts-node path/to/file.ts
```

This command will transpile the TypeScript code in `file.ts` into JavaScript and run the resulting code directly in Node.js. Additionally, `ts-node` supports a variety of command-line options that can be used to customize its behavior, such as specifying compiler options and setting environment variables. 

## tldr 
 
> Run TypeScript code directly, without any compiling.
> More information: <https://typestrong.org/ts-node>.

- Execute a TypeScript file without compiling (`node` + `tsc`):

`ts-node {{path/to/file.ts}}`

- Execute a TypeScript file without loading `tsconfig.json`:

`ts-node --skip-project {{path/to/file.ts}}`

- Evaluate TypeScript code passed as a literal on the command-line:

`ts-node --eval '{{console.log("Hello World")}}'`

- Execute a TypeScript file in script mode:

`ts-node --script-mode {{path/to/file.ts}}`

- Transpile a TypeScript file to JavaScript without executing it:

`ts-node --transpile-only {{path/to/file.ts}}`

- Display TS-Node help:

`ts-node --help`
