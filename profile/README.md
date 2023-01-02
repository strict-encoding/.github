Strict types is a formal notation for defining and serializing 
[generalized algebraic data types (GADT)](gadt) in a deterministic
and confined way. It is developed with [type theory] in mind.

In simple terms, strict types are _**protocol buffers and gRPC for functional 
programming**_ (or, for rust devs, _**functional-style serde**_).

Strict Types are:
* __schema-based__ (with the schema being strict encoding notation),
* __semantic__, i.e. defines types not just as they are layed out in memory, 
  but also depending on their meaning,
* __deterministic__, i.e. produces the same result for a given type,
* __portabile__, i.e. can run on ahy hardware architecture and OS, including
  low-performant embedded systems,
* __confined__, i.e. provides guarantees and static analysis on a maximum size
  of the typed data,
* __formally verifiabile__.

Strict Types include:
- **Strict Encoding** - set of libraries for serializing / deserializing data 
  types in binary formats (a protobuf analog);
- **Strict RPC**, which is a gRPC analog based on strict encoding;
- **Strict REST**, which is an HTML REST JSON analog, based on Strict RPC
  (instead of HTML) and Strict Encoding (instead of JSON).

![strict-encoding-box](https://user-images.githubusercontent.com/372034/209443924-add45986-d90c-42f9-bfaa-2fd2b0d50506.png)

Strict Types is WIP. Currently it is used by a number of projects
including [RGB smart contracts](https://github.com/RGB-WG),
[Farcaster](https://github.com/farcaster-project),
[CypherNet](https://github.com/CypherNet-WG) and others.

**[Whitepaper](https://github.com/strict-types/spec) | 
Yellowpaper | 
[Compiler](https://github.com/strict-types/stenc) | 
Disassembler | 
Standard type library (STL) |
Utilities**<br>

[gadt]: https://en.wikipedia.org/wiki/Algebraic_data_type
[type theory]: https://en.wikipedia.org/wiki/Type_theory
