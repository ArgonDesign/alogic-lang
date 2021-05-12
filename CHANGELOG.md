# Change Log

All notable changes to the "alogic-lang" extension will be documented in this
file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to
[Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 0.4.3 - 2021-05-06

### Changed

* Allow error message for unreachable
* Allow comments to contain semicolons

### Fixed

* Fix backtracking issues with ()
* Fix gen-for-case and case-arm-block

## 0.4.2 - 2021-04-28

Resolve a regression in v0.4.1 for do-while loops.

## 0.4.1 - 2021-04-28

Further quality of life upgrades.

### Added

* Add $display statement

### Changed

* Allow function return type of struct/uint with params/size
* DPI imports can appear more generally
* FSMs in a network don't have to be singleton

### Fixed

* Resolve issue with variables starting with 'do'
* Fix issues with parentheses and strings
* For loop end condition is an expr not expr-stmt

## 0.4.0 - 2021-04-06

Further major upgrade to better cope with complex syntax cases.

### Added

* Add DPI import highlighting
* Enhance dictionaries
* Add pipeline-decl
* Add gen-for-case
* Add sram-decl
* Highlight @ builtin functions properly
* Highlight $ built-in functions properly
* Add ++/-- statement types
* Add wait statement
* Add shorthand assignment statements
* Add unreachable and constants as statements
* Add bubble modifier highlighting
* Add file-scope functions and asserts in structs
* Add struct parameters

### Changed

* Name scopes of comments as per other languages
* Allow entity instantiations with no params
* Allow structs to be declared inside FSMs
* Allow comments in gen-for-case
* Asserts can appear in network bodies
* Add test for if-stmt that is now fixed by slice fixes
* Allow expressions in slices
* Typedefs can have parameters, e.g. for structs

### Fixed

* Fix up literal highlighting
* Fix up highlighting of parameter list for typedef
* Fix issues with dictionaries and array syntax
* Fix comments in case statement
* Fix up var/field/const decl for {u,}int(N)
* Fix vector types for fields, variables & constants
* Fix method highlighting
* Fix multidimensional dictionary highlighting
* Highlight distributed memory declaration properly
* Method invocation can appear in statement position
* Fix import * and typedef in outer fsm body

## 0.3.0 - 2021-02-02

Major upgrade to cope properly with new Alogic syntax.

### Added

* Add support for let statements
* Allow block comments within expressions
* Add support for assert statements
* Add support for parameterised entity instantiations
* Add support for do-while loops
* Add boolean literals
* Add support for for loops
* Add support for continue statement
* Add support for break statements
* Add support for return statement
* Add support for unbraced case arms
* Support function decls in struct decls
* Add support for function arguments
* Add support for non-void function return types
* Add support for static functions
* Add support for typedef decls
* Add support for gen blocks
* Add support for import statements
* Add support file level constants

### Changed

* Simplified port-decl
* Remove highlighting for #include directives
* Made lvalue pattern more selective

### Fixed

* Removed error prone expr patterns
* Stop erroneous variable-decl highlights
* Fix variable assignment highlighting
* Fix unsized literal number highlighting

## 0.2.0 - 2019-08-07

### Added

Support for verbatim verilog entities.
Better expression parsing.

### Changed

Statement parsing to remove ambiguity with specific statements vs. expressions
as statements.

## 0.1.0 - 2019-08-07

Initial release
