# Ghidra, batteries included

A distribution of Ghidra 9.2<sup>[1]</sup> with several extensions and data archives included to simplify reversing of game code.
 
[1] - Ghidra 9.2 is not yet available, the distribution available here is created by building against `master`.
See the git submodule in [ghidra/upstream](ghidra/upstream) for more information.

## What's included?

### Extensions

- [C++ Class Analyzer](https://github.com/astrelsky/Ghidra-Cpp-Class-Analyzer) - Simplifies analysis of executables with C++ RTTI or vtables present.

### Ghidra patches

- [Shifted pointers](https://github.com/NationalSecurityAgency/ghidra/pull/2189/files) - Support for shifted pointers that begin in the middle of a structure, rather than the base of it. 