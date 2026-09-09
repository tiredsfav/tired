<div align="center">

Game Engine

A lightweight, low-level game engine written in C.

Build the game yourself.
The engine takes care of the underlying systems.

<br>







</div>

About

This is a work-in-progress game engine, developed entirely by one person.

The goal is to provide the low-level systems required to build a game while leaving the actual game architecture and gameplay entirely up to the developer.

The engine currently handles:

🪟 Application & window management
🎨 Vulkan rendering
⚙️ Engine core systems
🔗 DLL interface & exports
🔨 Makefile-based builds

You make the game. The engine handles the boring parts.

Architecture

The engine is built as a dynamic library and used by separate applications.

┌──────────────────────┐
│        Game          │
│                      │
│  Gameplay            │
│  Game Logic          │
│  Entities            │
│  Scenes              │
└──────────┬───────────┘
           │
           │ Engine API
           ▼
┌──────────────────────┐
│     engine.dll       │
│                      │
│  Application         │
│  Window              │
│  Renderer            │
│  Vulkan              │
│  Core Systems        │
└──────────────────────┘
Requirements

Currently supported build environment:

Requirement	Purpose
Clang	C compiler
GNU Make	Build system
Vulkan SDK	Vulkan development & libraries

Windows is currently the target platform.

The Vulkan SDK must be installed with the VULKAN_SDK environment variable configured.

Building

Build the engine with:

make

The engine will be generated as:

bin/
└── engine.dll

The testbed can be built using its Makefile:

make

which produces:

bin/
└── testbed.exe

To clean generated files:

make clean
Project Structure
.
├── engine/       # Engine source
├── testbed/      # Engine testbed
├── tests/        # Tests
├── bin/          # Compiled output
├── obj/          # Object files
└── README.md
Development

The engine is still in early development.

The architecture, renderer, API, build system, and project structure are expected to change as development continues.

Roadmap

Basic engine DLL

Application system

Window creation

Initial Vulkan setup

Renderer development

Input system

Resource management

Audio

Improved game API

Documentation

Example game

Philosophy

The engine isn't meant to tell you how to make your game.

Instead, it provides the foundation and lets you decide what happens on top of it.

The engine provides the tools.
You build the game.

<div align="center">

🚧 Work in Progress

Made with C, Vulkan, and a lot of time.

Developed by a solo developer.

</div>
