<p align="center">
  <img src="https://img.shields.io/badge/status-superseded-red" alt="Superseded">
  <a href="https://www.fab.com/listings/c84e5b41-ad2b-45cf-ac8c-dc84e0a690ce"><img src="https://img.shields.io/badge/replaced%20by-Watabou%20Bridge-1A1A1A" alt="Replaced by Watabou Bridge"></a>
</p>

<p align="center">
  <img src="Resources/Watabou_Logo.png" alt="PCGEx + Watabou Logo" width="180">
</p>

<h1 align="center">PCGEx + Watabou</h1>

<p align="center">
  <strong>This early prototype has been superseded.</strong><br>
  It now lives on as <strong>Watabou Bridge</strong> -- a free, standalone Unreal Engine plugin on FAB.
</p>

---

## ⚠️ This repository is deprecated

**PCGEx + Watabou** was an early, open-source prototype for importing Watabou's procedural maps into Unreal Engine's PCG framework. It has been replaced by **Watabou Bridge**, a dedicated, free plugin distributed on FAB.

This repository is **no longer maintained**. No further updates, features, or fixes will land here. Please switch to Watabou Bridge.

<p align="center">
  <a href="https://www.fab.com/listings/c84e5b41-ad2b-45cf-ac8c-dc84e0a690ce"><strong>>> Get Watabou Bridge on FAB (free) <<</strong></a>
  <br><br>
  <a href="https://pcgex.gitbook.io/pcgex/watabou-bridge">Documentation</a> •
  <a href="https://discord.gg/3SGPbEc5tv">Discord</a>
</p>

---

## What changed?

Watabou Bridge is a ground-up rework of this prototype:

- **Standalone** - it no longer depends on PCGEx (or anything else).
- **Generators run in-editor** - instead of exporting JSON from the website and re-importing it, the generators are embedded directly in an editor window. What you see in the preview is exactly what gets imported (bundles included with Watabou's permission).
- **More generators** - Perilous Shores, City, Village, Dwellings, One Page Dungeon, Urban Places and Neighbourhood.
- **A cleaner PCG workflow** - two nodes, **Generate** (geometry) and **Load Properties** (metadata as attributes).
- **Free, on FAB** - distributed as a free, closed-source plugin.

---

## What this means for you

- Existing clones still build against their respective versions, but won't receive updates or fixes.
- Issues and pull requests opened here won't be actioned - please use the **[Discord](https://discord.gg/3SGPbEc5tv)** or the new **[documentation](https://pcgex.gitbook.io/pcgex/watabou-bridge)**.
- There's no automatic migration - just re-generate your maps in Watabou Bridge's import window. It's quicker than the old JSON round-trip.

---

<details>
<summary><strong>&#128230; Original prototype README (archived for reference)</strong></summary>

<br>

<p align="center">
  <img src="https://github.com/Nebukam/PCGExElementsWatabou/blob/main/Resources/Watabou_Logo.png" alt="PCGEx Logo">
</p>
<h1 align="center">PCGEx + Watabou</h1>
<p align="center">
  <strong>Import procedural maps from Watabou's generators into Unreal Engine's PCG framework</strong><br>
  Cities, villages, neighborhoods, and dungeons - from JSON to PCG data in seconds.
</p>
<p align="center">
  <a href="https://pcgex.gitbook.io/pcgex/watabou">Documentation</a> •
  <a href="https://discord.gg/mde2vC5gbE">Discord</a> •
  <a href="https://www.fab.com/listings/ac5c54f5-1a92-4e96-99c6-ff8fd9a37b4c">FAB</a>
</p>

### What is PCGEx + Watabou?

This is a **companion plugin for [PCGEx](https://github.com/Nebukam/PCGExtendedToolkit)** that converts JSON exports from [Watabou's procedural generators](https://watabou.itch.io/) into PCG & PCGEx data you can use directly in Unreal Engine.

![Image](https://github.com/user-attachments/assets/b9cd1aa8-9f61-49b6-8428-5082f60bc295)

#### Supported Generators

- [Medieval Fantasy City Generator](https://watabou.itch.io/medieval-fantasy-city-generator)
- [Neighborhood Generator](https://watabou.itch.io/neighbourhood)
- [Village Generator](https://watabou.itch.io/village-generator)
- [One Page Dungeon](https://watabou.itch.io/one-page-dungeon)

#### Experimental Status

This plugin is **experimental**. Watabou's JSON data structures may change over time. The code is designed to support multiple data versions, but if something breaks, [open an issue](https://github.com/Nebukam/PCGExElementsWatabou/issues) and I'll look into it.

### Requirements

- **Unreal Engine 5.6+**
- **[PCGExtendedToolkit](https://github.com/Nebukam/PCGExtendedToolkit)** - Core PCGEx plugin (free, MIT licensed)

### Installation

#### From FAB

Get the latest release from the **[FAB Marketplace](https://www.fab.com/listings/ac5c54f5-1a92-4e96-99c6-ff8fd9a37b4c)**.

#### From Source

1. Clone this repository into your project's `Plugins/` folder
2. Ensure **PCGExtendedToolkit** is also installed
3. Regenerate project files and build

### Getting Started

1. Go to any of the supported Watabou generators listed above
2. Right-click and export to JSON
3. Rename the file extension from `.json` to `.wataboujson` - this is key for the auto-import to kick in
4. Drag and drop the file into Unreal - this generates a new Data Asset. Save it.
5. In a PCG Graph, use the `Load Watabou Data` node and pick your data asset

> The content of the JSON export depends on what is displayed in the generator. Some generators expose different data types such as districts — play around with them!

### License

**MIT License** -- Free for personal and commercial use. See [LICENSE](LICENSE) for full terms.

</details>

---

## Support

- **[Watabou Bridge on FAB](https://www.fab.com/listings/c84e5b41-ad2b-45cf-ac8c-dc84e0a690ce)** - the current, maintained plugin
- **[Documentation](https://pcgex.gitbook.io/pcgex/watabou-bridge)** - guides and node reference
- **[Discord](https://discord.gg/3SGPbEc5tv)** - community support and discussion
- **[Patreon](https://www.patreon.com/c/pcgex)** - support PCGEx development
