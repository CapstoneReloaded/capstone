
## Capstone Engine (Reloaded)

```diff
-▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂
```
> :exclamation: This is an *independent community* development fork of the original [Capstone](https://github.com/aquynh/capstone) project that was made in order to secure the future existence of that great, but slowly dying project. Unfortunately the original project is badly suffering from an extreme lack of maintenace and very slow response to any community involvement, if at all. This is an attempt to remedy the situation, but **is not meant to replace that project**, and rather complement it in such a way that *issues*, project *milestones* and *pull requests* can be handled more rapidly to push the project forward. :exclamation: 

<sub> For questions regarding the original project and its status, please contact the original *Capstone* owner and repository maintainer:\
[Nguyen Anh Quynh](https://github.com/aquynh/) at aquynh@gmail.com.</sub>

```diff
-▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂▂
```

[![Capstone](https://img.shields.io/badge/capstone-3.0.5-lightgray.svg)](https://github.com/aquynh/capstone)
[![GitHub last commit](https://img.shields.io/github/last-commit/CapstoneReloaded/capstone.svg)](https://github.com/CapstoneReloaded/capstone)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/CapstoneReloaded/capstone/graphs/commit-activity)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/CapstoneReloaded/capstone.svg)](http://isitmaintained.com/project/CapstoneReloaded/capstone "Average time to resolve an issue")




#### Capstone Reloaded:

| STATUS: | Version | Date | Maintained? |
|:------- |:------- |:---- |:----------- |
| Working | `3.0.5` | 2018-11-02 | YES |

#### Original Capstone:

| STATUS: | Version | Date | Maintained? |
|:------- |:------- |:---- |:----------- |
| Working | `3.0.5` | 2018-07-18 | ? |

[![GitHub last commit](https://img.shields.io/github/last-commit/aquynh/capstone.svg)](https://github.com/aquynh/capstone)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-low-orange.svg)](https://GitHub.com/aquynh/capstone/graphs/commit-activity)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/aquynh/capstone.svg)](http://isitmaintained.com/project/aquynh/capstone "Average time to resolve an issue")

[![Build Status](https://travis-ci.org/aquynh/capstone.svg?branch=next)](https://travis-ci.org/aquynh/capstone)
[![Build status](https://ci.appveyor.com/api/projects/status/a4wvbn89wu3pinas/branch/next?svg=true)](https://ci.appveyor.com/project/aquynh/capstone/branch/next)

---

### What is Capstone?

Capstone is the *disassembly* engine which is part of the *Reverse Engineering* (RE) framework known as the "Reversing Trilogy", consisting of:
- [Capstone](https://capstone-engine.org)
- [Unicorn](https://unicorn-engine.org)
- [Keystone](https://keystone-engine.org) 

The framwork has as target to become the ultimate tool for binary analysis in the security community, and has already established itself as an important part in a long list of [related projects](http://www.capstone-engine.org/showcase.html) using its engine to various degrees.

As such, *Capstone* offers some unparalleled features:

- Support multiple hardware architectures: \
  *ARM, ARM64 (ARMv8), Ethereum VM, M68K, Mips, PPC, Sparc, SystemZ, TMS320C64X, M680X, XCore and X86/X86_64*

- Having clean/simple/lightweight/intuitive architecture-neutral API.

- Provide details on disassembled instruction (called “decomposer” by others).

- Provide semantics of the disassembled instruction, such as list of implicit
  registers read & written.

- Implemented in pure C language, with lightweight bindings for:\
  Clojure, F#, Common Lisp, Visual Basic, PHP, PowerShell, Emacs, Haskell, Perl, Python,
  Ruby, C#, NodeJS, Java, GO, C++, OCaml, Lua, Rust, Delphi, Free Pascal & Vala \
  (Available either in main code or provided externally by the community.)

- Native support for all popular platforms:\
  Windows/Cygwin, Mac OSX, iOS, Android, Linux, \*BSD, Solaris, etc.

- Thread-safe by design.

- Special support for embedding into firmware or OS kernel.

- High performance & suitable for malware analysis (capable of handling various
  X86 malware tricks).

- Distributed under the open source BSD license.

Further information is available at http://www.capstone-engine.org

---

#### Compile

See [COMPILE.md](COMPILE.md) file for how to compile and install Capstone.


#### Documentation

See [docs/README] for how to customize & program your own tools with Capstone.


#### Hack

See [HACK.TXT](HACK.TXT) file for the structure of the source code.


#### License

This project is released under the BSD license. If you redistribute the binary
or source code of Capstone, please attach file LICENSE.TXT with your products.
