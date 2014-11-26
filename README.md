# Typescript definition file for RAML

**WORK IN PROGRESS**

The following Typescript file will serve multiple purposes ( in order of importance ):

1. Enable Typescript tools to consume the output of the raml-js-parser in a type-safe manner
2. Provide an additional source of documentation Javascript developers trying to get their heads around the RAML spec
3. Formalize a canonical javascript/json representation for RAML ( as much as possible )

Considering the above, some comments to keep in mind:

* The shape of this particular JS model for RAML was influenced by the output of the pre-existing JS parser
* The official RAML Spec is the only authoritative source
* Not every possible clever refactoring or Typescript idiom will be used ( remember goal N 2 )

# How can you use this?

* Read the source for now. Suggest edits, etc.
* RAML is complex enough to require some advanced Typescript concepts that didn't make it to 1.3 ( Type Aliases and Union Types )
 * ( Check out the pre-release of the [CATS IDE](https://github.com/jbaron/cats) )