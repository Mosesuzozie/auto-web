# Easy Web

**Automatic cobwebs, pressure plates and obsidian traps for Fabric 1.21.11, with smooth, human-looking aim and a full Mod Menu config.**

![Fabric](https://img.shields.io/badge/loader-Fabric-dbd0b4) ![Minecraft](https://img.shields.io/badge/minecraft-1.21.11-62b47a) ![Environment](https://img.shields.io/badge/environment-client-blue)

---

## Features

### 🕸️ Auto Web
Every few seconds (default **5s**) Easy Web picks the nearest player you can see, smoothly turns your camera to a spot you can actually reach, and places:

1. a **pressure plate**, then
2. a **cobweb**

You choose where each one goes: **Feet**, **Head** or **Front** of the target.

### 🧱 Auto Obby
Every few seconds (default **20s**) it traps a target who is up against a wall:

1. **Blocks** them in
2. **Lava**
3. **Water** (turns the lava into obsidian)
4. **Seals** the open side

Every step can be switched on or off. Lava is never placed unless a water bucket is also in your hotbar.

### 🎯 Smooth aim
No snapping. The camera eases in and out, slows down near the spot, adds a little natural wobble, and only places once your crosshair is really on the block face.

- Max turn speed
- Smoothing
- Aim randomness
- Delay between placements

### ✅ Won't act without the right items
If an enabled step is missing its item in your hotbar (pressure plate, cobweb, blocks, lava bucket, water bucket), Easy Web simply does nothing.

---

## Controls

Three keybinds, all **unbound by default**. Set your own in **Options → Controls → Easy Web**:

| Keybind | What it does |
|---|---|
| Toggle Auto Web | Turns Auto Web on or off |
| Toggle Auto Obby | Turns Auto Obby on or off |
| Toggle Easy Web (master switch) | Pauses or resumes everything |

Both modules start **off**.

## Configuration

Open **Mod Menu → Easy Web → Config**. Tabs:

- **General**: master switch, target range, line-of-sight, never-target list, debug messages
- **Smooth Aim**: speed, smoothing, randomness, delays
- **Auto Web**: interval, pressure plate, cobweb, spots
- **Auto Obby**: interval, wall requirement, each step, which blocks to use

## Requirements

| Mod | Needed |
|---|---|
| [Fabric API](https://modrinth.com/mod/fabric-api) | Yes |
| [Cloth Config API](https://modrinth.com/mod/cloth-config) | Yes |
| [Mod Menu](https://modrinth.com/mod/modmenu) | Yes, for the config screen |

Needs **Fabric Loader 0.18+** and **Java 21**. Client-side only; don't install it on a server.

## FAQ

**It does nothing when I turn it on.**
Check your hotbar has the items for every enabled step, that a player is within range and in view, and turn on *Debug messages* in the General tab to see why a step was skipped.

**Is it safe to use on servers?**
Automating placements against other players breaks the rules on most public servers and can get you banned. Only use it where it's allowed, like your own server or with friends who agree.

**Which versions are supported?**
Minecraft 1.21.11 on Fabric only.

---

*Early release. Tell me what breaks.*
