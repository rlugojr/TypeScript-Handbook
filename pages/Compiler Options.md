## Compiler Options

Option                                  | Shorthand | Description
----------------------------------------|-----------|----------------------------------------------------------------------
`--declaration`                         | `-d`      | Generates corresponding '.d.ts' file.
`--help`                                | `-h`      | Print help message.
`--version`                             | `-v`      | Print the compiler's version.
`--module`                              | `-m`      | Specify module code generation: 'commonjs', 'amd', 'system', 'umd', or 'es2015'. Only 'amd' and 'system' can be used in conjunction with `--outFile`. The 'es2015' value may not be used when targeting ES5 or lower.
`--project`                             | `-p`      | Compile the project in the given directory. The directory needs to contain a `tsconfig.json` file to direct compilation. See [tsconfig.json](./tsconfig.json.md) documentation for more details.
`--target`                              | `-t`      | Specify ECMAScript target version: 'ES3' (default), 'ES5', or 'ES6'<sup>[1]</sup>
`--watch`                               | `-w`      | Run the compiler in watch mode. Watch input files and trigger recompilation on changes.
`--charset`                             |           | The character set of the input files.
`--diagnostics`                         |           |  Show diagnostic information.
`--emitBOM`                             |           |  Emit a UTF-8 Byte Order Mark (BOM) in the beginning of output files.
`--emitDecoratorMetadata`<sup>[1]</sup> |           |  Emit design-type metadata for decorated declarations in source. See [issue #2577](https://github.com/Microsoft/TypeScript/issues/2577) for details.
`--experimentalDecorators` | | Enables experimental support for ES7 decorators.
`--inlineSourceMap`                     |           |  Emit a single file with source maps instead of having a separate file.
`--inlineSources`                       |           |  Emit the source alongside the sourcemaps within a single file; requires `--inlineSourceMap` or `--sourceMap` to be set.
`--isolatedModules`                     |           |  Unconditionally emit imports for unresolved files.
`--jsx`                                 |           |  Support JSX in '.tsx' files: 'React' or 'Preserve'. See [JSX](./JSX.md).
`--reactNamespace`                      |           | Specifies the object invoked for `createElement` and `__spread` when targeting 'react' JSX emit.
`--listFiles`                           |           |  Print names of files part of the compilation.
`--locale`                              |           |  The locale to use to show error messages, e.g. en-us.
`--mapRoot`                             |           |  Specifies the location where debugger should locate map files instead of generated locations. Use this flag if the .map files will be located at run-time in a different location than than the .js files. The location specified will be embedded in the sourceMap to direct the debugger where the map files where be located.
`--moduleResolution`                    |           |  Determine how modules get resolved. Either 'node' for Node.js/io.js style resolution, or 'classic' (default).
`--newLine`                             |           |  Use the specified end of line sequence to be used when emitting files: 'CRLF' (dos) or 'LF' (unix)."
`--noEmit`                              |           |  Do not emit outputs.
`--noEmitOnError`                       |           |  Do not emit outputs if any errors were reported.
`--noEmitHelpers`                       |           |  Do not generate custom helper functions like `__extends` in compiled output.
`--noImplicitAny`                       |           |  Raise error on expressions and declarations with an implied 'any' type.
`--noLib`                               |           |  Do not include the default library file (lib.d.ts).
`--noResolve`                           |           |  Do not add triple-slash references or module import targets to the list of compiled files.
`--skipDefaultLibCheck`                 |           |
`--out`                                 |           |  DEPRECATED. Use `--outFile` instead.
`--outDir`                              |           |  Redirect output structure to the directory.
`--outFile`                             |           |  Concatenate and emit output to single file. The order of concatenation is determined by the list of files passed to the compiler on the command line along with triple-slash references and imports. See output file order documentation for more details.
`--preserveConstEnums`                  |           |  Do not erase const enum declarations in generated code. See [const enums documentation](https://github.com/Microsoft/TypeScript/blob/master/doc/spec.md#94-constant-enum-declarations) for more details.
`--pretty`<sup>[1]</sup>                |           | Stylize errors and messages using color and context.
`--removeComments`                      |           | Remove all comments except copy-right header comments beginning with `/*!`
`--rootDir`                             |           |  Specifies the root directory of input files. Only use to control the output directory structure with `--outDir`.
`--sourceMap`                           |           |  Generates corresponding '.map' file.
`--sourceRoot`                          |           |  Specifies the location where debugger should locate TypeScript files instead of source locations. Use this flag if the sources will be located at run-time in a different location than that at design-time. The location specified will be embedded in the sourceMap to direct the debugger where the source files where be located.
`--stripInternal`<sup>[1]</sup>         |           |  Do not emit declarations for code that has an `/** @internal */` JSDoc annotation.
`--suppressExcessPropertyErrors`<sup>[1]</sup> | | Suppress excess property checks for object literals.
`--suppressImplicitAnyIndexErrors`      |           |  Suppress `--noImplicitAny` errors for indexing objects lacking index signatures. See [issue #1232](https://github.com/Microsoft/TypeScript/issues/1232#issuecomment-64510362) for more details.
`--allowUnusedLabels`                   |           |  Do not report errors on unused labels.
`--noImplicitReturns`                   |           |  Report error when not all code paths in function return a value.
`--noFallthroughCasesInSwitch`          |           |  Report errors for fallthrough cases in switch statement.
`--allowUnreachableCode`                |           |  Do not report errors on unreachable code.
`--forceConsistentCasingInFileNames`    |           |  Disallow inconsistently-cased references to the same file.
`--allowSyntheticDefaultImports`        |           |  Allow default imports from modules with no default export. This does not affect code emit, just typechecking.
`--allowJs`                             |           |  Allow JavaScript files to be compiled.
`--noImplicitUseStrict`                 |           |  Do not emit `"use strict"` directives in module output.

<sup>[1]</sup> These options are experimental.

## Related

* Setting compiler options in [`tsconfig.json`](./tsconfig.json.md) files.
* Setting compiler options in [MSBuild projects](./Compiler Options in MSBuild.md).
