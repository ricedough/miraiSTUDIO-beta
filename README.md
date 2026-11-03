# miraiSTUDIO beta

A chart editor for **Hatsune Miku: Project Mirai DX** (3DS), made by ricedough and documentable.
- edit existing charts, or make your own
- edit or create the chart's blue lines
- build the song into the game and play/test it in Azahar or on a 3DS

This is a beta build of miraiSTUDIO made for testing. Please report bugs and give feedback while using it.

**[Download the latest beta](../../releases/latest)**: get `miraiSTUDIO-beta-v0.1.zip` under Assets.

## Dependencies

- Windows 10 or 11, 64-bit
- **Your own romfs dump of Hatsune Miku: Project Mirai DX.** miraiSTUDIO does not include any of the game's files and requires a dump for any assets used.
- The [Azahar](https://azahar-emu.org/) emulator isn't required, but it will make testing easier and faster. Or you can use a 3DS with Luma3DS (which I recommend).

## Getting started

1. Unzip the download anywhere and run `miraiSTUDIO beta.exe`.
   Windows may say it "protected your PC", because the exe isn't signed. Click **More info**, then **Run anyway**.
2. The first time it boots, it asks for file locations. Anything it finds by itself is filled in already, and you can change these later in **Settings > Folders**.
   - your game files
   - Azahar's mod folder for the game (`...\Azahar\load\mods\0004000000148C00`). **PLEASE BACK UP YOUR CURRENT MODS AND SAVE FILE BEFORE USING MIRAISTUDIO.**
   - My Files (can be any folder), where your songs are kept
3. **Home** shows what you can do: open a song, make a new one, or import a song mod.

Everything the beta saves stays in its own folder (settings, your work, crash logs). The only exceptions are your songs (My Files) and the mod it builds into the game.

## What to try

**Chart (Song > Chart)**
- Place notes at the cursor with `W` `A` `S` `D` (X / Y / B / A) and `Q` (star).
- Drag notes on the timeline.
- Pick several notes and use the **Edit** menu: mirror, change buttons, snap to the grid, fewer notes.
- `P` plays the chart yourself. `F1` lists every key.

**Note lines and camera (Song > Note lines)**
- Draw a line, or build one from track pieces.
- Set the screen camera: pick a style and how closely it follows.
- The corner of the view shows what the player sees.
- **Properties** checks each line against what the game can handle.

**Songs (Library)**
- Make a new song from one of the game's, or import a modded chart.
- Give a song your own music (a WAV) and pictures.
- **Build and test** (top right) plays it in Azahar, or builds the files for a 3DS.

**Sound offset (Settings > Sound > Measure it by tapping)**
- Matches the timing to your speakers or headphones.

## Reporting a problem

Open an issue on the [Issues](../../issues) tab and say:
- what you did
- what you expected
- what happened instead

A screenshot helps. (Or please DM me on Discord: @ricedough.)

If the beta closes because of an error, it writes a crash log to the `crash logs` folder next to the exe (a `.txt` and a `.dmp`) and tells you the next time you start it. Zip both files and attach them to the issue.

## About the mod it builds

The mod includes a small code patch (`code.ips` and `exheader.bin`) that lets the game hold more songs (up to 999) and keeps custom songs' progress in their own save file. It goes into the mod folder only. Your game and your saves are left as they are.

**THESE CODE PATCHES ARE EXPERIMENTAL AND MAY NOT BE STABLE.** Please report any problems that come with them, so I know what I need to fix.

## Not in the beta

The full miraiSTUDIO also edits:
- 3D stages and PV effects
- 2D animations
- costumes and room items
- saves

All of these aren't ready for release yet and need work, which is why they aren't included.

## Legal

miraiSTUDIO is a fan-made tool. It is not affiliated with or endorsed by SEGA or Crypton Future Media. Hatsune Miku: Project Mirai DX and its characters belong to their owners.

Copyright (c) 2026 ricedough and documentable. All rights reserved. You may download and use the beta to test it, but not share changed copies of it. The third-party libraries and fonts it uses keep their own licenses; see `Third-party notices.txt` in the download.
