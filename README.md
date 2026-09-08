# Lamplight Dungeons

![Lamplight Dungeons title artwork](assets/title_lamplight_dungeons.png)

**A modern furry dungeon expedition built around the room-to-room rhythm of DEC-era mainframe DND.**

Lamplight Dungeons is not a tile-walking roguelike. Each chamber is a complete location. Type **N**, **S**, **E**, or **W** to take an available passage; the screen changes to the next room, and any waiting enemy immediately opens a command-driven encounter.

Its main playfield follows the sparse rhythm of Daniel Lawrence's mainframe DND: compact statistics at the upper left, a persistent dungeon map beside them, and movement or round-by-round combat prompts directly underneath. Modern graphics support that layout instead of replacing it.

All code, characters, rooms, writing, graphics, and audio are original to the Lamplight project. Historical DND, Moria, and Angband files are not included.

## Features

- Original title artwork and a skippable three-part opening sequence
- Room-to-room navigation using typed compass commands
- Persistent DEC-inspired overhead map with tiled chambers, walls, corridors, and exploration fog
- Immediate DND-style enemy encounters
- Six species: Bunny, Fox, Ferret, Cat, Chicken, and Human
- Four classes: Knight, Archer, Priest, and Mage
- Every species/class combination has its own portrait
- Twenty procedural levels and four named guardians
- Treasure, traps, fountains, shrines, stairs, rations, and guild supplies
- Adventure recovery or Classic permanent-death modes
- Autosave, manual save, safe atomic writes, and encounter resuming
- Keyboard and mouse controls, resizable window, and F11 fullscreen
- Original ambient music and event sound effects

## Install on Linux

Extract the release ZIP, open a terminal inside the `Lamplight-Dungeons` folder, and run:

```bash
chmod +x INSTALL.sh run.sh
./INSTALL.sh
./run.sh
```

Ubuntu and Linux Mint may first require:

```bash
sudo apt install python3-venv
```

## Room commands

| Key | Action |
| --- | --- |
| N / S / E / W | Travel through an available passage |
| D | Descend when standing in the stair chamber |
| U | Return to the guild from the entrance chamber |
| R | Consume a ration to rest |
| L | Read the room description again |
| F5 | Save |
| Esc | Save and return to the title |
| F11 | Toggle fullscreen |
| M | Mute or unmute audio |

## Encounter commands

| Key | Action |
| --- | --- |
| F | Fight |
| C | Use the class skill |
| H | Drink a healing potion |
| E | Evade and retreat |
| S | Stay and watch |
| 1–5 | Choose an action directly |
| Arrows + Enter | Navigate the action list |

## The guild

Gold found below is carried and unsafe. Return to the entrance chamber and type **U** to bank it at the guild. The guild restores health and spirit, sells healing potions and rations, and remembers the deepest level reached.

Adventure mode rescues a defeated character but loses carried gold. Classic mode deletes the save when the character dies.

Progress is stored in `savegame.json` beside the game.

## License

The original Lamplight Dungeons code is available under the [MIT License](LICENSE.txt). Copyright © 2026 Kit Zoro.
