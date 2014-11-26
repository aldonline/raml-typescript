# Typescript definition file for RAML

<img src="https://raw.githubusercontent.com/aldonline/raml-typescript/master/images/a.png" width="800"/>

**WORK IN PROGRESS**

The following Typescript file will serve multiple purposes ( in order of importance ):

1. Enable Typescript tools to consume the output of the [raml-js-parser](https://github.com/raml-org/raml-js-parser) in a type-safe manner
2. Provide an additional source of documentation for developers trying to get their heads around the [RAML spec](https://github.com/raml-org/raml-spec)
3. Move towards a canonical javascript/json representation for RAML that other Javascript based tools can support

Considering the above, some comments to keep in mind:

* The starting point for this definition is highly influenced by the output of the pre-existing JS parser ( remember goal N1 ). We will probably be able to influence its design in future iterations as we move towards goal N3.
* The official RAML Spec is the only authoritative source
* Not every possible clever refactoring or Typescript idiom will be used ( to achieve goal N 2 )

Challenges

* YAML and JSON are differnet. This will leak
* Even if we define one canonical RAML model for JSON, there will always be at least 3 different models in reality:
 * Complete/Strict model - ex: the output of parsing a valid RAML file
 * Incomplete model - ex: the output of parsing a RAML file which is being edited ( by a parser that supports this kind of use case )
 * Complete + Interpretation - The fully expanded model ( with resource types and traits interpreted )

# How can you use this?

* Read the source for now. Suggest edits, etc.
* RAML is complex enough to require some advanced Typescript concepts that didn't make it to 1.3 ( Type Aliases and Union Types )
 * If you are in a hurry, check out the pre-release of the [CATS IDE](https://github.com/jbaron/cats)
 
## Features

### Documentation references the official Spec

<img src="https://raw.githubusercontent.com/aldonline/raml-typescript/master/images/b.png" width="800"/>

### Everything is typed - autocomplete to the rescue ;)

<img src="https://raw.githubusercontent.com/aldonline/raml-typescript/master/images/c.png" width="800"/>

### Takes advantage of advanced Typescript features

### Union Types

<img src="https://raw.githubusercontent.com/aldonline/raml-typescript/master/images/d.png" width="800"/>

### And more!

<img src="https://raw.githubusercontent.com/aldonline/raml-typescript/master/images/e.png" width="800"/>
