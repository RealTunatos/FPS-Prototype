# AimTrainingPrototype

A simple first-person aim training prototype developed with Unreal Engine 5.6.1.

The project started as an FPS prototype and evolved into a small aim-training experience. The main goal of the project was to practice Unreal Engine gameplay systems, Blueprint scripting, UI, weapons, damage systems, target spawning and Behavior Tree.

## Features

- First-person character movement
- Functional firearm system
- Line Trace based shooting
- Weapon recoil
- Ammo system
- Reload system
- Crosshair
- Damage system using a Blueprint Interface
- Target dummies
- Random target spawning within a defined area
- Targets automatically disappear after a certain time
- Target hit counter
- Hit impact Niagara effect
- Pause menu
- Main menu
- Exit game functionality
- Packaged Windows build

## Gameplay

The player spawns in an enclosed shooting range and attempts to hit as many target dummies as possible.

Target dummies spawn at random locations within the designated area. Each target can be damaged by shooting it and disappears when destroyed or after a short amount of time.

The game is intentionally simple and focuses on the core FPS mechanics rather than complex gameplay systems.

## Controls

| Key | Action |
| --- | --- |
| `WASD` | Move |
| `Mouse` | Look |
| `Left Mouse Button` | Shoot |
| `R` | Reload |
| `ESC` | Pause Menu |

## Technical Details

### Engine

- Unreal Engine 5.6.1
- Blueprint Visual Scripting
- Niagara
- Unreal Engine First Person Template

### Gameplay Systems

The weapon uses a **Line Trace** based shooting system rather than physical projectile actors.

Damage communication between the weapon and target dummies is handled using a **Blueprint Interface**, allowing the weapon to interact with damageable actors without tightly coupling the two Blueprints.

Target spawning is handled by a dedicated target spawner Blueprint. Targets are spawned at random valid locations inside the designated area and are removed after a set amount of time or when destroyed.

### What I Learned

This project was mainly created as a learning and portfolio project. During development I practiced:

-Blueprint communication
-Blueprint Interfaces
-Line Trace based weapon systems
-Damage handling
-Weapon recoil
-Ammo and reload systems
-Niagara effects
-UMG UI
-Level and GameMode management
-Main menu and pause menu implementation
-Actor spawning and destruction
-Randomized target placement
-Packaging an Unreal Engine project
-Git and GitHub workflow for Unreal Engine projects

## AI Experiment

An AI system using Behavior Trees was initially planned for the project.

The original idea was to create an enemy that would patrol between points, detect the player, follow them and attack.

I eventually decided not to include the AI system in the final version. Although the system was not completed, experimenting with Behavior Trees helped me understand the basic structure of Unreal Engine's AI framework and how AI Controllers, Blackboards and Behavior Trees interact.

## Status

**Completed**

This project is considered a completed prototype. It is not intended to be a full commercial aim-training game.

The main purpose of the project was to gain practical experience with Unreal Engine gameplay programming and complete a small playable FPS project.