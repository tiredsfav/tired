<div align="center">

# Tired Engine

**A custom game engine built from the ground up in C.**

*You make the game. Tired Engine handles the rest.*

![Status](https://img.shields.io/badge/status-work--in--progress-orange)
![Language](https://img.shields.io/badge/language-C-blue)
![Platforms](https://img.shields.io/badge/platforms-Windows%20%7C%20Linux%20%7C%20macOS-informational)

</div>

---

## About

Tired Engine is a **work-in-progress game engine** built entirely from scratch by a
**single developer**.

The goal is to provide the systems needed to build an application or game while
leaving the actual game and its architecture in the developer's hands.

Tired Engine currently includes its own:

- Application & window system
- Renderer
- Input system
- Event system
- Logger
- Dynamic array (`darray`)
- String system (`kstring`)
- Memory system (`kmemory`)
- Math library
- Core engine systems
- DLL/shared library interface

---

## Platforms

Tired Engine currently supports:

| Platform | Support |
|----------|---------|
| Windows  | ✅ |
| Linux    | ✅ |
| macOS    | ✅ |

The goal is to allow applications and games built with Tired Engine to run
natively across these platforms.

---

## Rendering

The current renderer is built around **Vulkan**.

The renderer is designed to be expandable, with other graphics APIs such as
**OpenGL** potentially being added in the future.

---

## Building

The project uses **Makefiles** for its build system.

### Requirements

- [Clang](https://clang.llvm.org/)
- [GNU Make](https://www.gnu.org/software/make/)
- [Vulkan SDK](https://www.lunarg.com/vulkan-sdk/)

The current Vulkan renderer requires the Vulkan SDK.

Build the engine with:

```bash
make
