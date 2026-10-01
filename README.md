# AutoTrap Client — Fabric 1.21.11

Client-side PvP automation for Minecraft 1.21.11.

## Features

- **Normal Web** — configurable feet/head cobweb placement.
- **Pressure-Plate Web** — pressure plate on the block under the target, then cobweb at head level.
- **Auto Obby** — looks for a nearby wall, places configurable obsidian blocks in front of the player, then lava and water in sequence.
- **Smooth Rotation** — rotates toward the exact placement spot instead of snapping directly to it.
- **Visible-target filter** — by default it only targets players the client can currently see.
- **Mod Menu configuration** — General, Web, and Obby tabs.
- **Persistent JSON config** — stored at `.minecraft/config/autotrap-client.json`.

## Requirements

- Minecraft **1.21.11**
- Fabric Loader **0.19.5+**
- Fabric API **0.141.3+1.21.11**
- Mod Menu **17.0.0-beta.2** (required for the settings button)
- Java **21**

The project does not use MixinExtras.

## Build

Use Java 21 and a Gradle 9.x installation.

```text
gradle build
```

The mod JAR is written to `build/libs/`.

Fabric's 1.21.11 documentation also places built JARs in `build/libs` when using the Gradle build task.

## GitHub Actions

The included workflow installs Java 21 and Gradle 9.4.0, builds the project, and uploads both the normal and sources JARs as workflow artifacts.

## Notes

The automation is client-side and still obeys normal Minecraft item/inventory requirements: the required item must be present in the hotbar, and the server must allow the placement. It does not bypass server permissions or placement checks.
