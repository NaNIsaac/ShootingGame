# ShootingGame

A small slingshot shooting game written in C++ with raylib, running on a hand-written 2D physics engine.

Hobby project from 2023. It continues the game prototype
from [FlatPhysics](https://github.com/NaNIsaac/FlatPhysics): launch a limited number of shots to bring
the enemy's HP to zero; damage depends on how hard it is hit.

## Requirements

- Windows, Visual Studio 2022 with "Desktop development with C++" (toolset v143)
- raylib 4.2, bundled as 32-bit headers and libraries in `include/` and `lib/`

## Run

1. Open `FlatPhysics.sln` (the project kept the engine's name).
2. Select the `Debug` / `x86` configuration and run (F5).

Textures, music and sounds are loaded from `asset/`, so the game must start with `FlatPhysics/`
as the working directory (the Visual Studio default).

## Controls

- Start / Exit buttons on the title screen
- Drag and release the projectile with the left mouse button to launch it
- Mouse wheel: zoom, arrow keys: pan the camera, `T`: reset the camera
- `||` button: pause menu, `Music` button: switch or mute background music
- `C` / `G`: jump to the game-clear / game-over screen (debug shortcuts)

## Structure

- `FlatPhysics/src/Engine/` - physics engine and raylib helpers
- `FlatPhysics/src/Game/` - entry point (`Application.cpp`) and game logic
- `FlatPhysics/asset/` - textures, music and sound effects
