# SolVessel

A Hollow Knight mod that lets you play as Yi from Nine Sols. Swap between the Knight and Yi at any bench.

Yi brings his Nine Sols moveset: the roll, parries and Unbounded Counter, talismans (Qi Blast, Water Flow, Full Control), the bow with all three arrows, the charged strike, the pipe, and his skill tree with XP and levels. He grows through Hallownest:

- **Pipe uses:** 2 to start, +1 for every 2 vessel fragments, and 2 more from Sly.
- **Pipe healing:** upgraded at the nailsmith (press down near him).
- **Bow:** each nail upgrade improves Azure Sand and the arrows.
- **Tao Fruits:** bosses drop them, for skill points and damage.
- **Charged strike:** learned from your first Nailmaster.
- **Charms:** many of the Knight's charms work for Yi too.

If something doesn't work for you, hold dash in the skill tree (at a bench) for a second: it unlocks everything Yi has for free, including full masks. Hold it again to go back to normal.

## Requirements

- Hollow Knight (1.5) with the [Hollow Knight Modding API](https://github.com/hk-modding/api)
- **Nine Sols installed on the same PC.** The mod includes no Nine Sols files: on first launch its converter builds Yi from your own copy of Nine Sols (it takes about half a minute).

## Install

Download `SolVessel-v0.1.0.zip` from the Releases page and extract it into
`Hollow Knight/hollow_knight_Data/Managed/Mods/SolVessel/`, so that folder contains `SolVessel.dll` and the `prep` folder.

## Building from source

Requires the .NET SDK. Build `src/Mod/Mod.csproj` (the mod) and `src/Prep/Prep.csproj` (the converter) in Release; copy the mod's dll into the Mods folder and the converter's output into its `prep` subfolder. `sheets/` holds the design data; `tools/gen.ps1` regenerates `Generated/Sheets.cs` from it and `tools/preflight.ps1` checks it.
