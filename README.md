# DataPackage.jl

[![Travis](https://travis-ci.org/frictionlessdata/datapackage-jl.svg?branch=master)](https://travis-ci.org/frictionlessdata/datapackage-jl)
[![Coveralls](http://img.shields.io/coveralls/frictionlessdata/datapackage-jl.svg?branch=master)](https://coveralls.io/r/frictionlessdata/datapackage-jl?branch=master)
[![SemVer](https://img.shields.io/badge/versions-SemVer-brightgreen.svg)](http://semver.org/)
[![Gitter](https://img.shields.io/gitter/room/frictionlessdata/chat.svg)](https://gitter.im/frictionlessdata/chat)

[![Julia Pkg](http://pkg.julialang.org/badges/JSON_0.6.svg)](http://pkg.julialang.org/?pkg=datapackage&ver=0.6)

A library for working with [Data Packages](http://specs.frictionlessdata.io/data-package/) in Julia.

Initially this package is primarily targeted and depends on [TableSchema.jl](https://github.com/frictionlessdata/tableschema-jl), where you can find the common [Design Document](https://github.com/loleg/TableSchema.jl/blob/master/DESIGN.md) for these libraries. Support for other types of data packages is to follow.

## Features

 - `Package` class for working with data packages
 - `Resource` class for working with data resources
 - `Profile` class for working with profiles
 - `validate` function for validating data package descriptors
 - `infer` function for inferring data package descriptors

### Status

:construction: This package is pre-release and under heavy development. Please visit the [issues page](https://github.com/frictionlessdata/datapackage-jl/issues) to contribute and make suggestions. For questions that need to a real time response, reach out via [Gitter](https://gitter.im/frictionlessdata/chat). Thanks! :construction:

Please visit [our wiki](https://github.com/frictionlessdata/datapackage-jl/wiki) for a list of related projects that we are tracking, and suggest use cases there or as enhancement [issues](https://github.com/frictionlessdata/datapackage-jl/issues).

# Usage

Install *tableschema-jl* (temporarily obtained from GitHub until released):

`$ julia -e 'Pkg.clone("https://github.com/frictionlessdata/tableschema-jl")'`

You may also need to explicitly install *HTTP*:

`$ julia -e 'Pkg.add("HTTP")'`

Update to the latest version with:

`$ julia -e 'Pkg.update("TableSchema")'`

Clone this repository and enter it:

`$ git clone https://github.com/frictionlessdata/datapackage-jl && cd datapackage-jl`

See *examples* folder and unit tests in [runtests.jl](test/runtests.jl) for current usage, e.g.:

`$ julia examples/basic.jl`

Running tests:

`$ julia -L src/DataPackage.jl test/runtests.jl`
