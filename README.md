# go-module-tutorial

This is the code from Go's official [module tutorial](https://golang.org/doc/tutorial/create-module).

Please note that this was created in February 2021, and the tutorial at the
above website may have been updated since then.

## Overview

This project contains two directories. `greetings` is the module which is used
as a library. This means that it is designed to be used by other libraries or
applications. `hello` is also a module, but used as an application. The code
in the `hello` module imports the `greetings` module and calls its functions.

One thing to note is that the hierarchy is module > package > file. This repo
contains two modules, `greetings` and `hello`. The `greetings` module contains
a `greetings` package, and the `hello` module contains a `main` package.
Packages are often made up of multiple files grouped together in a directory,
so it's helpful to think of a package as a directory when first learning
about packages in Go.
