# ctools.hpp - Lightweight C++ Utility Headers

<!--
====================================================================================
  ____ __  __      _
 / ___|  \/  | ___(_)
| |   | |\/| |/ _ \ |
| |___| |  | |  __/ |
 \____|_|  |_|\___|_|

  ____ __  __      _   ____            _           _
 / ___|  \/  | ___(_) |  _ \ _ __ ___ (_) ___  ___| |_ ___
| |   | |\/| |/ _ \ | | |_) | '__/ _ \| |/ _ \/ __| __/ __|
| |___| |  | |  __/ | |  __/| | | (_) | |  __/ (__| |_\__ \
 \____|_|  |_|\___|_| |_|   |_|  \___// |\___|\___|\__|___/
                                    |__/

  ____ _ _   _           _
 / ___(_) |_| |__  _   _| |__
| |  _| | __| '_ \| | | | '_ \
| |_| | | |_| | | | |_| | |_) |
 \____|_|\__|_| |_|\__,_|_.__/

  ____ _ _
 / ___(_) |_ ___  ___
| |  _| | __/ _ \/ _ \
| |_| | | ||  __/  __/
 \____|_|\__\___|\___|

  ____ _ _                _
 / ___(_) |_ ___ ___   __| | ___
| |  _| | __/ __/ _ \ / _` |/ _ \
| |_| | | || (_| (_) | (_| |  __/
 \____|_|\__\___\___/ \__,_|\___|

====================================================================================
-->
[![GitHub](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white)](https://github.com/CMei-Projects/ctools)
[![Gitee](https://img.shields.io/badge/Gitee-C71D23?logo=gitee&logoColor=white)](https://gitee.com/CMei111/ctools)
[![GitCode](https://img.shields.io/badge/GitCode-2C2C2C?logo=git&logoColor=white)](https://gitcode.com/cmei-projects/ctools)
[![CI](https://github.com/CMei-Projects/ctools/actions/workflows/ci.yml/badge.svg)](https://github.com/CMei-Projects/ctools/actions/workflows/ci.yml)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-Indev_26.10__04-blue)](CHANGELOG.md)
![Status](https://img.shields.io/badge/Status-Indev-yellow)  
**Status: 🚧 Experimental / Indev**  
A single-header, cross-platform C++ utility library for terminal manipulation, math constants, and basic algorithms.

## ✨ Features
- 🖥️ **Terminal Control**: Colored warnings/errors (ANSI/VT for Win/Linux) with automatic fallback.
- 🔢 **Math Helpers**: `is_prime`, `is_even`, `Max/Min`, and constants (PI, E).
- 🔄 **Efficient Swap**: Move-aware `Swap` implementation.
- 📦 **Header-only**: Just `#include "ctools.hpp"` and go.
- 📊 **Progress Bar**: Terminal progress bar for long-running loops.
- 🎲 **Random String**: random 100~1:$1\%$ to all numbers.
> 🚀 **G++ First!** For the best experience, we highly recommend using the GNU Compiler (GCC/G++).

## 📦 Version
**Current:** `Indev 26.10_04` (API subject to breaking changes).  
Check [CHANGELOG.md](./CHANGELOG.md) for details.

## 🚀 Quick Start
```cpp
#include "ctools.hpp"

int main() 
{
    std::cout << "ctools version: " << ctools::version_string() << std::endl;
    ctools::write_warning("Hello, this is a warning!");
    return 0;
}
```

## 📋 Requirements
### C++17 (or higher)
Cross-platform: Linux (bash/terminal) & Windows (PowerShell / Windows Terminal)
> ### Tips
> ctools always need C++ 17! Some old version\'s will show \"C++ 11\", but it a bug.

## 📜 License
Distributed under the [MIT License](https://www.opensource.org/license/mit).

## 👔 Owner
<a href="https://www/github.com/CMei111">
  <img src="https://github.com/CMei111.png" alt="CMei111's Avatar" width="100" height="100" style="border-radius: 50%;">
</a>

**CMei111** (CMei)

## ❤️ Collaborator
Not yet collaborator. Want join? visit [Collaboration Guide](./CONTRIBUTING.md).

## ℹ️ Tips
- 🔍 **Easter Eggs**: The source code contains some interesting tricks! 
- 🚀 **Future-Proof**: `ctools` is fully compatible with the upcoming **C++26** standard (`-std=c++2c`).

<details>
<summary>👉 Click to reveal one of the interesting tricks</summary>

Look at the bottom of `ctools.hpp`. We embedded a compiler message: 
`#pragma message("[OK] ctools load completed.")`
Every time you compile successfully, the compiler gives you a green (or blue) `[OK]`!

</details>
