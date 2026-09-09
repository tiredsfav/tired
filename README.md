<div align="center">

# K Engine

### A work-in-progress game engine written in C

Build the game yourself.  
K Engine provides the systems underneath it.

![Status](https://img.shields.io/badge/status-work--in--progress-orange)
![Language](https://img.shields.io/badge/language-C-blue)
![Renderer](https://img.shields.io/badge/renderer-Vulkan-red)
![Build System](https://img.shields.io/badge/build-Make-informational)

</div>

---

## About

K Engine is a low-level game engine focused on providing the fundamental systems needed to create a game, while leaving the actual game architecture and gameplay up to the developer.

The engine currently provides:

- Application and window management
- Vulkan rendering
- Core engine systems
- DLL exports
- Makefile-based builds

> **You make the game. The engine handles the underlying systems.**

---

## Architecture

The engine is built as a DLL and is used by applications built on top of it.

```text
Game
 │
 ├── Gameplay
 ├── Game Logic
 ├── Entities
 └── Scenes
       │
       ▼
  Engine API
       │
       ▼
engine.dll
 │
 ├── Application
 ├── Window
 ├── Renderer
 ├── Vulkan
 └── Core Systems
