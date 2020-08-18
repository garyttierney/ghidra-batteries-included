# Ghidra, batteries included

A distribution of Ghidra 9.2 (as of now unreleased) with several extensions and data archives included to simplify reversing of game code.

## What's included?

### Extensions

- [C++ Class Analyzer](https://github.com/astrelsky/Ghidra-Cpp-Class-Analyzer) - Simplifies analysis of executables with C++ RTTI or vtables present.

### Ghidra patches

- [Shifted pointers](https://github.com/NationalSecurityAgency/ghidra/pull/2189/files) - Support for shifted pointers that begin in the middle of a structure, rather than the base of it.

## Where do I get it?

Builds can be downloaded straight from GitHub action runs, like [here](https://github.com/garyttierney/ghidra-batteries-included/actions/runs/212796178).
Note: you'll need to be authenticated with a GitHub account to download archives listed here.

Alternatively, builds of the latest version in this repository can be downloaded at the following locations:

- [Windows](https://ghidradistribution.z35.web.core.windows.net/builds/ghidra-windows-latest.zip)
- [Linux](https://ghidradistribution.z35.web.core.windows.net/builds/ghidra-ubuntu-latest.zip)