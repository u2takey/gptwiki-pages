# semver 
## chatgpt 
Semver is not a command, but a concept and a set of guidelines for versioning software. 

Semver stands for "Semantic Versioning" and it is a standard way to assign version numbers to software releases. It provides a clear and simple set of rules for determining when to release a new version and what changes to apply to the version number.

The version number is divided into three segments: MAJOR.MINOR.PATCH. Each segment has a specific meaning:

- MAJOR: Increment this number when making incompatible changes to the software API, i.e., when it breaks backwards compatibility.
- MINOR: Increment this number when adding new functionality that is backward compatible with the previous version.
- PATCH: Increment this number when fixing bugs or making minor changes that do not affect the API.

Semver also defines pre-release and build metadata versions, which are optional and allow for even more granularity in versioning.

Using Semver can help developers communicate changes and compatibility issues with their users, and can also help automate software releases and dependency resolution. 

## tldr 
 
> Semantic version string parser.
> More information: <https://github.com/npm/node-semver>.

- Check if a version string respects the semantic versioning format (prints an empty string if it does not match):

`semver {{1.2}}`

- Convert a version string to the semantic versioning format:

`semver --coerce {{1.2}}`

- Test if `1.2.3` matches the `^1.0` range (prints an empty string if it does not match):

`semver {{1.2.3}} --range "{{^1.0}}"`

- Test with multiple ranges:

`semver {{1.2.3}} --range {{">=1.0"}} {{"<2.0"}}`

- Test multiple version strings and return only the ones that match:

`semver {{1.2.3}} {{2.0.0}} --range "{{^1.0}}"`
