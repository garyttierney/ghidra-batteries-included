# Ghidra, batteries included

## **🛈 ATTENTION: Ghidra 9.2 is now [generally availlable](https://ghidra-sre.org/releaseNotes_9.2.html)! However, I will continue to provide binaries of the latest changes to both Ghidra core and extensions**  


A distribution of Ghidra 9.2 with extensions and patches included to simplify reversing code patterns commonly found in games.

## **⚠ WARNING: Unstable patches and features included.**  

Before using this Ghidra distribution, you should be aware of the risks of using a version of Ghidra that is not yet considered stable.

### What does _stable_ mean in the context of this distribution?

There are 3 main components to consider when we think about what is _stable_ here:

- Ghidra patches (typically from in-progress pull requests)
- Ghidra extensions (3rd party plugins like cpp-class-analyzer)
- Ghidra core

Since we build from the latest versions of these components, we run the risk of introducing non backwards compatible changes when Ghidra, a patch, or an extension changes its schema.
On the other side of this, when we include a Ghidra pull request that has not yet been merged we run the risk of introducing changes that are not _forward compatible_ if the pull request is never accepted.

Some care is taken to ensure that only pull requests providing good value or with existing reviews are included with the assumption that they are likely to be merged, but the risk is always there.

### What does this mean for me?

Until an official Ghidra release is published with all the corresponding components included (or available), you should rely on this build only for working with programs.
There may be a scenario where a program has been upgraded due to a change in Ghidra that later has to be reverted, leaving you stuck on a single version of Ghidra until a remedy can be found.

These problems will obviously happen on a case-by-case basis, however, I would endeavor to fix them if they should ever occur.
If you do run into this please open an issue on the issue tracker.

## What's included?

### Extensions

- [C++ Class Analyzer](https://github.com/astrelsky/Ghidra-Cpp-Class-Analyzer) - Simplifies analysis of executables with C++ RTTI or vtables present.
- [ret-sync](https://github.com/bootleg/ret-sync) - Synchronize the Ghidra listing with a debugger.
- [Better GoTo](https://github.com/NationalSecurityAgency/ghidra/pull/2004) - Support complex expressions in the GoTo dialog.

### Ghidra patches

- [Shifted pointers](https://github.com/NationalSecurityAgency/ghidra/pull/2189/files) - Support for shifted pointers that begin in the middle of a structure, rather than the base of it.

## Where do I get it?

Builds can be downloaded straight from GitHub action runs [here](https://github.com/garyttierney/ghidra-batteries-included/actions/).
Note: you'll need to be authenticated with a GitHub account to download archives listed here.

Alternatively, builds of the latest version in this repository can be downloaded at the following locations:

- [Windows](https://ghidradistribution.z35.web.core.windows.net/builds/ghidra-windows-latest.zip)
- [Linux](https://ghidradistribution.z35.web.core.windows.net/builds/ghidra-ubuntu-latest.zip)

## Future additions and contributions

See the [issues](https://github.com/garyttierney/ghidra-batteries-included/issues) for planned additions that are not yet present in the builds above.
