<div align="center">

# Zinc lang

The zinc programming language.

</div>

---

<!-- 
@TODO: Add a taste of the syntax to the front page
@TODO: Add a tour of the language README
@TODO: Migrate to a checklist showing what is and isn't functional
-->

## Goals

- AOT compiled binary(s)
- Control over allocator(s)
- Scope local context that is implicitly passed to zinc functions
- Support constructs to allow for multiple paradigms, such as:
  - Procedural
  - Declarative 
  - Functional
  - Data oriented, with ways to specify SOA or AOS
  - Object oriented, inheritance and polymorphism
- Powerful compile-time execution
  - Syntax clearly separate for runtime and compile constructs and operations
  - Generics / templates
  - Powerful meta-programming
  - Macros, code generation based on code
  - Be transparent about generated code
  - Attributes / annotations, part of the macro system
- Strongly typed
  - Concepts as the preferred means of dynamic dispatch, think c++20's concepts
  - First-class trait/interface system, like rust, but some oop thrown in
  - Concept / trait / interface, effectively all the same thing
  - [runtime polymorphism done right](https://github.com/ldionne/dyno)
- First-class c interop
  - Binding generation from c header source code
- First-class IDE support
- Powerful package and project manager
- Powerful async, also much like rust

## Building

``` sh
git clone https://github.com/tealsnow/zinc.git
cd zinc
git submodule update --init --recursive
cd zincc
cargo b
```

## Usage

``` sh
# within zincc
cargo r -- --help
# or
cargo r -- -T ../zinc_src/<pick a file>
```

## Things I want to make with this (Eventual goals)

- Programming language(s)
  - Self-hosted zinc compiler
  - Proof-Of-Concept managed VM language
- OOP UI library, like flutter
  - A file editor, like a good one
- Game Engine
  - A commercial game
- Proof-Of-Concept OS
  
## Contributing

Feel free to open any pull request, I'm open to any contributions.

## License

This software is distributed under the terms of both the MIT license and Apache license (Version 2.0) unless any portion is specified otherwise.

See `LICENSE-APACHE`, `LICENSE-MIT`, and `COPYRIGHT` for details.
