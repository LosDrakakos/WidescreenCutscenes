# Ultrawide Cutscenes

A [Dalamud](https://github.com/goatcorp/Dalamud) plugin for Final Fantasy XIV that removes the letterboxing bars displayed during cutscenes on ultrawide monitors, allowing cutscenes to fill your full screen.

> **Note:** Because this expands the rendered viewport beyond the game's intended cutscene boundaries, you may occasionally see things you aren't supposed to — NPCs popping in at the edges, T-poses, scene geometry loading, etc. This is expected behavior and not a bug.

## Requirements

- [Final Fantasy XIV](https://www.finalfantasyxiv.com/)
- [XIVLauncher](https://goatcorp.github.io/) with Dalamud enabled

## Installation

### Via Custom Plugin Repository *(recommended)*

1. Open the Dalamud Plugin Installer with `/xlplugins` in chat.
2. Go to **Settings → Experimental → Custom Plugin Repositories**.
3. Add the URL https://raw.githubusercontent.com/DukePantarei/Dalamud.FullscreenCutscenes/main/repo.json and click **Save**:
4. Search for **Ultrawide Cutscenes** in the Available Plugins tab and install it.

### Manual / Developer Install

1. Clone or download this repository and build the solution in Visual Studio 2022 or JetBrains Rider (Release or Debug).
2. Open Dalamud settings with `/xlsettings`, go to **Experimental**, and add the full path to `Dalamud.FullscreenCutscenes.dll` under **Dev Plugin Locations**.
3. Open `/xlplugins`, navigate to **Dev Tools → Installed Dev Plugins**, and enable **Ultrawide Cutscenes**.

## Usage

The plugin is active as soon as it's enabled — there's no configuration required. Letterboxing will be removed automatically whenever a cutscene plays.

## Known Limitations

- The expanded viewport may reveal unfinished scene elements at the edges of the screen (NPC pop-in, T-poses, etc.).
- The plugin requires updates when Dalamud's API version changes; if the plugin stops working after a game or Dalamud update, check here for an updated release.

## Credits

- **[goaaats](https://github.com/goaaats/Dalamud.FullscreenCutscenes)** — original plugin author
- **[MapleHinata](https://github.com/MapleHinata/Dalamud.FullscreenCutscenes)** — prior maintained fork
- **aers** — discovered the underlying technique that makes this possible

## License

This project is licensed under the [AGPL-3.0 License](LICENSE).
