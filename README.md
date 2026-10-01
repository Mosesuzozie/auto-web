# Ghost Client (Fabric, Minecraft 1.21.11)

Client-side mod. Auto Web, Pressure Plate Web and Auto Obby, all configurable in Mod Menu, with smooth camera aim.

## Build
Needs JDK 21 and Gradle 9.2+ (or copy `gradlew`, `gradlew.bat` and `gradle/` from a Fabric template for 1.21.11).

    gradle build        (or ./gradlew build)

The jar ends up in `build/libs/ghostclient-1.0.0.jar`.

## Install
Put the jar in `.minecraft/mods` together with: Fabric Loader, Fabric API, Mod Menu, Cloth Config API.

## Use
- `G` toggles Auto Web, `H` toggles Auto Obby (rebind in Controls). Both start OFF.
- Everything else: Mod Menu -> Ghost Client -> config.
- Auto Web fires every N seconds (default 5) at the nearest player you can see.
- Auto Obby fires every N seconds (default 20): walls -> lava -> water -> seal. Needs blocks, a lava bucket and a water bucket in the hotbar. It never places lava unless a water bucket is also in the hotbar.
- Turn on "Debug messages in chat" to see why a step was skipped.

If the build fails with a version not found, copy the current 1.21.11 versions from https://fabricmc.net/develop into gradle.properties.
