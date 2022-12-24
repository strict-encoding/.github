Strict encoding is a formal notation and implementation of a 
serialization for [generalized algebraic data types (GADT)](gadt).

In simple terms, strict encoding is _**protocol buffers for functional programming**_ (or, for rust devs, _**functional-style serde**_).

Strict encoding is both a language for defining GADT and libraries for their
serialization. It is:
* __schema-based__ (with the schema being strict encoding notation),
* __semantic__, i.e. defines types not just as they are layed out in memory, 
  but also depending on their meaning,
* __deterministic__, i.e. produces the same result for a given type,
* __portabile__, i.e. can run on ahy hardware architecture and OS, including
  low-performant embedded systems,
* __confined__, i.e. provides guarantees and static analysis on a maximum size
  of the typed data,
* __formally verifiabile__.

![strict-encoding-box](https://user-images.githubusercontent.com/372034/209443924-add45986-d90c-42f9-bfaa-2fd2b0d50506.png)

Strict encoding is WIP. Currently it is used by a number of projects
including [RGB smart contracts](https://github.com/RGB-WG),
[Farcaster](https://github.com/farcaster-project),
[CypherNet](https://github.com/CypherNet-WG) and others.

In this organization we plan to provide:<br>
**[Whitepaper](https://github.com/strict-encoding/spec) | 
Yellowpaper | 
[Compiler](https://github.com/strict-encoding/stenc) | 
Disassembler | 
Standard type library (STL) |
Utilities**<br>
**Language-specific libs: 
[Rust](https://github.com/strict-encoding/strict_encoding/tree/master/rust) | 
Swift | 
Kotlin | 
TypeScript**

[gadt]: https://en.wikipedia.org/wiki/Algebraic_data_type
