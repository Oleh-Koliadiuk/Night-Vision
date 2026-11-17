# Night Vision Resource Pack

A lightweight Minecraft: Java Edition resource pack that replaces the core lightmap shader with a constant full-bright output. The world remains visible in dark areas without changing block or entity textures.

## Supported versions

Choose the folder that matches your Minecraft Java Edition version:

| Minecraft version | Pack to install |
| --- | --- |
| 1.21.9–1.21.11 | The files in the repository root |
| 1.21.5–1.21.8 | `versions/java-1.21.5-1.21.8/` |

The two releases use different `pack.mcmeta` formats. Do not combine their metadata or shader files. Minecraft core shader overrides are an unsupported resource-pack feature, so a future game update can change or break this pack. Versions before 1.21.5, snapshots, Bedrock Edition, and modded renderers are not supported by these releases.

## Installation

1. Select the pack folder for your game version.
2. Copy that folder's `assets` directory and `pack.mcmeta` into a new folder in Minecraft's `resourcepacks` directory. For the root release, use the repository root as the source.
3. Start Minecraft, open **Options → Resource Packs**, and enable **Night Vision**.

You can also zip the contents of the selected pack folder. Make sure `pack.mcmeta` and `assets/` are at the top level of the ZIP, not inside an extra nested directory.

## How it works

The pack overrides `assets/minecraft/shaders/core/lightmap.fsh` and outputs white for every lightmap pixel. The matching vertex shader passes the lightmap geometry through. This affects the game's lightmap rendering; it does not grant the Night Vision status effect or change gameplay.

## License

This project is released under the MIT License. See [LICENSE](LICENSE).
