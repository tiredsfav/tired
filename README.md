Game Engine

> A work-in-progress game engine written in C, providing the underlying systems needed to build a game.

*> This project is developed entirely by one person.

Overview

The engine is designed to handle the low-level parts of a game application while leaving the actual game implementation to the developer.

Currently, the engine provides:

Application
Window management
Vulkan renderer
Engine core
DLL interface

The engine is compiled into a DLL and linked by separate applications such as the testbed.

> Note: The engine is currently a work in progress and its API may change.

Requirements

The current build system requires:

Clang
GNU Make
Vulkan SDK

The Vulkan SDK must be installed and its VULKAN_SDK environment variable configured.

> The current Makefiles target Windows and use .dll and .exe outputs.

Building

The engine can be built using:

make

This produces:

bin/
└── engine.dll

The testbed can be built separately using its Makefile:

bin/
└── testbed.exe

To remove generated files:

make clean
Project Structure
.
├── engine          # Engine source code
├── testbed         # Engine testbed
├── tests           # Tests
├── bin             # Compiled DLLs and executables
├── obj             # Compiled object files
└── README.md
Philosophy

*> You make the game. The engine handles the underlying systems.

The engine is intended to provide the foundation for building a game without dictating how the game itself should be structured.

Status

*> Work in progress

The engine, renderer, API, and build system are still actively being developed.

Author

This engine is developed entirely by one person — me.
