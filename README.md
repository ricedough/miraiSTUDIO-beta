# miraiSTUDIO beta

A chart editor for **Hatsune Miku: Project Mirai DX** (3DS). Use it to:
- make and change a song's notes
- shape the lines the notes fly along, and the screen camera
- build the song into the game and play it in Azahar or on a 3DS

This beta is the charter part of miraiSTUDIO, released for testing. Bug reports and feedback are very welcome.

**[Download the latest beta](../../releases/latest)**: get `miraiSTUDIO-beta-v0.1.zip` under Assets.

## What you need

- Windows 10 or 11, 64-bit. Nothing else to install.
- **Your own Project Mirai DX game files.** These are the romfs, the folder with `pv`, `nwbin`, `aet_en` and `sound` in it. Dump them from your own copy of the game. miraiSTUDIO does not include any of the game's files.
- To play what you make: the [Azahar](https://azahar-emu.org/) emulator with your game, or a 3DS with Luma3DS.

## Getting started

1. Unzip the download anywhere and run `miraiSTUDIO beta.exe`.
   Windows may say it "protected your PC", because the exe isn't signed. Click **More info**, then **Run anyway**.
2. The first time, it asks where things are. Anything it finds by itself is filled in already, and you can change these later in **Settings > Folders**.
   - your game files
   - Azahar's mod folder for the game (`...\Azahar\load\mods\0004000000148C00`)
   - My Files, where your songs are kept
3. **Home** shows what you can do: open a song, make a new one, or import a song mod.

Everything the beta saves stays in its own folder (settings, your work, crash logs). The only exceptions are your songs (My Files) and the mod it builds into the game.

## What to try

**Chart (Song > Chart)**
- Place notes at the cursor with `W` `D` `S` `A` (X / A / B / Y) and `Q` (star).
- Drag notes on the timeline.
- Pick several notes and use the **Edit** menu: mirror, change buttons, snap to the grid, fewer notes.
- `P` plays the chart yourself. `F1` lists every key.

**Note lines and camera (Song > Note lines)**
- Draw a line, or build one from track pieces.
- Set the screen camera: pick a style and how closely it follows.
- The corner of the view shows what the player sees.
- **Properties** checks each line against what the game can handle.

**Songs (Library)**
- Make a new song from one of the game's, or import a downloaded song mod.
- Give a song your own music (a WAV) and pictures.
- **Build and test** (top right) plays it in Azahar, or builds the files for a 3DS.

**Sound offset (Settings > Sound > Measure it by tapping)**
- Matches the timing to your speakers or headphones.

## Reporting a problem

Open an issue on the [Issues](../../issues) tab and say:
- what you did
- what you expected
- what happened instead

A screenshot helps.

If the beta closes because of an error, it writes a crash log to the `crash logs` folder next to the exe (a `.txt` and a `.dmp`) and tells you the next time you start it. Zip both files and attach them to the issue.

## About the mod it builds

The mod includes a small code patch (`code.ips` and `exheader.bin`) that lets the game hold more songs (up to 999) and keeps custom songs' progress in their own save file. It goes into the mod folder only. Your game and your saves are left as they are.

## Not in the beta

The full miraiSTUDIO also edits:
- 3D stages and PV effects
- 2D animations
- costumes and room items
- saves

The beta keeps to charting. A song's dance and stage stay as they were in the song it started from.

## Legal

miraiSTUDIO is a fan-made tool. It is not affiliated with or endorsed by SEGA or Crypton Future Media. Hatsune Miku: Project Mirai DX and its characters belong to their owners.

Copyright (c) 2026 ricedough. All rights reserved. You may download and use the beta to test it, but not share changed copies of it. The third-party libraries and fonts it uses keep their own licenses; see `Third-party notices.txt` in the download.
