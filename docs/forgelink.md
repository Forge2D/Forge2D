# ForgeLink

ForgeLink is Forge2D's build workflow.

It connects a Forge2D project to a supported C++ compiler and manages the build process.

## What ForgeLink does

ForgeLink:

1. Reads `project.forge`.
2. Validates the project configuration.
3. Collects the project's source files.
4. Selects the configured C++ standard.
5. Invokes the installed compiler.
6. Produces the configured game executable.
7. Reports the build result inside Forge2D.

## Compiler support

ForgeLink is designed to work with supported C++ compilers installed on the user's system.

Depending on the Windows development environment, this may include:

* Microsoft Visual C++
* GCC / MinGW
* LLVM / Clang

The exact compiler configuration may depend on the user's environment.

## Build errors

If ForgeLink reports `BUILD FAILED`, check the build output for the compiler's error message.

Common causes include:

* Missing compiler
* Invalid C++ code
* Missing source file
* Incorrect project configuration
* Missing dependency

## Security

ForgeLink only accepts source files that belong to the project directory.

Project names, output names, and C++ standards are validated before compiler commands are constructed.
