# alogic-lang

Language support for alogic in Visual Studio Code.

## Features

* Syntax Highlighting for _.alogic_ files.

## Requirements

No third-party requirements.

## Extension Settings

No configuration.

## Known Issues

* Some `gen` constructs aren't highlighted correctly.
* Line-breaks or atypical lack thereof in various constructs aren't presently
  supported. (Highlighting breaks.)
* The highlighter is sometimes overly permissive; some illegal constructs
  highlight as if they are legal.
* Brace enclosed lvalues (e.g. concatenations) aren't highlighted correctly.
* Highlighting of function arguments of types with parameters, e.g. `uint(5)`.
* Slice highlighting is sometimes incorrect.

## Further information

* [Alogic language](https://github.com/ArgonDesign/alogic)
* [License](LICENSE)
