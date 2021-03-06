<p align="center"><img width="450" src="./xgen.svg" alt="xgen logo"></p>

# xgen

[![Build Status](https://github.com/xuri/xgen/workflows/Go/badge.svg)](https://github.com/xuri/xgen/actions?workflow=Go)
[![Code Coverage](https://codecov.io/gh/xuri/xgen/branch/master/graph/badge.svg)](https://codecov.io/gh/xuri/xgen)
[![Go Report Card](https://goreportcard.com/badge/github.com/xuri/xgen)](https://goreportcard.com/report/github.com/xuri/xgen)
[![GoDoc](https://godoc.org/github.com/xuri/xgen?status.svg)](https://godoc.org/github.com/xuri/xgen)
[![Licenses](https://img.shields.io/badge/license-bsd-orange.svg)](https://opensource.org/licenses/BSD-3-Clause)

## Introduction

xgen is a library written in pure Go providing a set of functions that allow you to parse XSD (XML schema files). This library needs Go version 1.10 or later. The full API docs can be seen using go's built-in documentation tool, or online at [godoc.org](https://godoc.org/github.com/xuri/xgen).

`xgen` commands automatically compiles XML schema files into the multi-language type or class declarations code.

Install the command line tool first.

```text
go get github.com/xuri/xgen
```

The command below will walk on the `xsd` path and generate generate Go language struct code under the `output` directory.

```text
$ xgen -i /path/to/your/xsd -o /path/to/your/output -l Go
```

Usage:

```text
$ xgen [<flag> ...] <XSD file or directory> ...
   -i <path> Input file path or directory for the XML schema definition
   -o <path> Output file path or directory for the generated code
   -p        Specify the package name
   -l        Specify the language of generated code (Go/C/Java/Rust/TypeScript)
   -h        Output this help and exit
   -v        Output version and exit
```



## Contributing

Contributions are welcome! Open a pull request to fix a bug, or open an issue to discuss a new feature or change. XSD is compliant with [XML Schema Part 1: Structures Second Edition](https://www.w3.org/TR/xmlschema-1/).

## Licenses

This program is under the terms of the BSD 3-Clause License. See [https://opensource.org/licenses/BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause).

Logo is designed by [xuri](https://xuri.me). Licensed under the [Creative Commons 3.0 Attributions license](http://creativecommons.org/licenses/by/3.0/).
