Strict encoding is a formal notation for defining and serializing 
[generalized algebraic data types (GADT)](gadt) in a deterministic
and confined way. It is developed with [type theory] in mind.

In simple terms, strict encoding is _**protocol buffers for functional 
programming**_ (or, for rust devs, _**functional-style serde**_).

Strict encoding is:
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

Alongside strict encoding this organization hosts related projects:
- **Strict RPC**, which is a gRPC analog based on strict encoding;
- **Strict REST**, which is an HTML REST JSON analog, based on Strict RPC
  (instead of HTML) and Strict Encoding (instead of JSON).

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
[type theory]: https://en.wikipedia.org/wiki/Type_theory
