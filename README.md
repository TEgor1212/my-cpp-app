# my-cpp-app

![CI](https://github.com/TEgor1212/my-cpp-app/actions/workflows/ci.yml/badge.svg)

C++ app with CI — CMake build + CTest on push and PR.

A C++ application built with CMake and Google Test. The CI pipeline enforces code formatting with clang-format, builds with CMake, and runs tests via CTest. A Docker image is built on success.

## Quick Start

```bash
cmake -B build -DBUILD_TESTS=ON
cmake --build build
cd build && ctest --output-on-failure
```