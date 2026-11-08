# Contributing to ctools

First off, thank you for considering contributing to `ctools`! It's people like you that make open source such a great community.

## 🚀 1. Environment Requirements

To maintain the quality and cross-platform compatibility of `ctools`, please ensure your development environment meets the following requirements:

-   **Compiler:** **G++ (GCC) is highly recommended** (Version 8.0 or higher). `ctools` has the best compatibility and is optimized for the GNU Compiler Collection.
-   **Standard:** **C++17** or higher is strictly required. (`-std=c++17` or `-std=c++2c`)
-   **OS:** Linux, macOS, or Windows (MinGW/WSL).

## 🛠️ 2. How to Contribute

### Reporting Bugs
-   Check the [Issues](https://github.com/CMei111/ctools/issues) to see if the bug has already been reported.
-   If not, open a new issue. Describe the bug clearly, provide your OS, compiler version, and a minimal reproducible code snippet.

### Suggesting Enhancements
-   Open an issue with the label `enhancement`. Explain why this feature is useful and how it fits the "lightweight and cross-platform" philosophy of `ctools`.

### Submitting Pull Requests (PRs)
1.  **Fork** the repository and create your branch from `main`.
    ```bash
    git checkout -b feature/your-feature-name
    ```
2.  Write your code. Follow the coding style guidelines below.
3.  Test your code. Ensure it compiles with zero warnings:
    ```bash
    g++ -std=c++17 -fsyntax-only -Wall -Wextra -Wno-pragma-once-outside-header ctools.hpp
    ```
4.  Commit your changes. Follow the commit message convention:
    ```bash
    git commit -m "feat: add support for xxx"
    ```
5.  Push and submit a PR to the `main` branch.

## 📏 3. Coding Style Guidelines
To keep the codebase clean and consistent, please adhere to the following rules:
- **Formatting**: Use 4 spaces for indentation. (No tabs).
- **Header Guards**: Use both `#pragma once` and the standard `#ifndef CMEI_CTOOLS_HPP` ... `#endif` macro.
- Naming Conventions:
    - **Functions and Variables**: `snake_case` (e.g., `get_keypress`, `random_string`).
    - **Classes/Structs/Enums**: `PascalCase` or `snake_case` (e.g., `auto_ptr`, `operation_system`).
    - **Macros/Constants**: `UPPER_SNAKE_CASE` (e.g., `CTOOLS_VERSION_STRING`).
- **Cross-Platform**: If you are using OS-specific APIs, you **must** use `#ifdef _WIN32 / #elif defined(__linux__) / #else` to ensure it works on other platforms.
- **Zero Warnings**: Code that generates compilation warnings (under `-Wall -Wextra`) will not be merged.
- **No third-party dependencies**: Keep it a pure header-only library. Do not introduce any external `.lib` or `.so` dependencies.

## 📝 4. Commit Message Convention
We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:
- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that do not affect the meaning of the code (white-space, formatting)
- `refactor`: A code change that neither fixes a bug nor adds a feature
- `chore`: Changes to the build process or auxiliary tools

## 📜 5. License
By contributing to ctools, you agree that your contributions will be licensed under its [MIT License](https://opensource.org/license/mit)