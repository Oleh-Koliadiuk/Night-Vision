# Night Vision Resource Pack

A lightweight Minecraft: Java Edition resource pack that brightens dark areas without granting the Night Vision status effect.

## Compatibility

Drop this folder directly into Minecraft's `resourcepacks` directory. It is built for Java Edition 1.21.4 through 26.1. This range uses one shader override and version-aware pack metadata. Bedrock Edition and older Java versions are not supported.

Minecraft core shader overrides are an unsupported resource-pack feature and may change in future releases. The pack has not been tested with every Minecraft release or modded renderer.

## Installation

1. Copy the `night-vision` folder into `.minecraft/resourcepacks`.
2. Start Minecraft and open **Options → Resource Packs**.
3. Enable **Night Vision**.

## How it works

The pack replaces the lightmap fragment shader with a constant full-bright output. Minecraft uses its built-in vertex shader, so the pack avoids bundling a duplicate or version-sensitive vertex shader. The small `lightmap.json` file supplies the legacy shader program definition used by Java 1.21.4; newer releases use the built-in definition.

## License

Released under the MIT License. See [LICENSE](LICENSE).
