# OpenAPI transformer

[![Coverage Status](https://coveralls.io/repos/github/armand-janssen/openapi-transformer/badge.svg?branch=master)](https://coveralls.io/github/armand-janssen/openapi-transformer?branch=master)

[![Build Status](https://travis-ci.org/armand-janssen/openapi-transformer.svg?branch=master)](https://travis-ci.org/armand-janssen/openapi-transformer)

This tool creates a [PlantUML Class Diagram](http://plantuml.com/class-diagram) from a **OpenApi 3 Yaml** specification

# Requirements
- OpenAPI 3.0.2
- OpenAPI specification should be in **YAML**
- [NodeJS](http://nodejs.org)
- All yaml files should be in 1 directory

# Usage
Always run the script from the directory in which the yaml file are.
```
Usage: index [options] <inputfile>

Options:
  -V, --version                    Output the version number
  -p, --plantuml <plantuml file>   The plantuml file
  -m, --markdown <output file>     The output file for markdown
  -v, --verbose                    Show verbose debug output
  -h, --help                       Output usage information
```

## Example
**Generates to plantuml**
```
openapi-transformer vehicle.yaml --plantuml vehicle.plantuml
```
**Generates to plantuml with verbose debug info :)**
```
openapi-transformer vehicle.yaml --verbose --plantuml vehicle.plantuml
```

**Generates to plantuml file and markdown file**
```
openapi-transformer vehicle.yaml --plantuml ./example.plantuml --markdown ./example.md
```
# Example output plantuml

## No details
![Example no details](https://raw.githubusercontent.com/armand-janssen/openapi-transformer/master/example/example-no-details.png)

## Details
![Example with details](https://raw.githubusercontent.com/armand-janssen/openapi-transformer/master/example/example-details.png)

