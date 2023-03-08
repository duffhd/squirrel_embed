## Squirrel embed

This repository is a template project to embed the [Squirrel programming language](https://github.com/albertodemichelis/squirrel)
in C++ with CMake. Squirrel is pulled as a library using git submodules.

To correctly execute the Squirrel's `.nut` scripts inside `/scripts` you need to make sure your
working directory is the root of this folder, whoever, you can change it on `main.cpp`.

## Debugging error
In CLion when using the bundled GDB with `-gstabs` (or the default config) flag the debugging process will crash, use GDB with `-g` flag or use
LLDB.