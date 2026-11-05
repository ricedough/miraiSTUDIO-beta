# Changelog

## v0.2

LOLOLOL heres a beta update that i got pushed out pretty fast, honestly i was hoping the last version of the beta wouldnt have been as buggy as it was. i apologize for that. i was originally planning to just release that and fix small bugs along the way, v0.2 was supposed to be released WAYYYYY later and was supposed to include all features for testers. though i changed my mind as i realized the current beta needed an update ASAP (mostly due to minimizing FREEZING :sob:) i still plan for the next release to hopefully have all features, though if needed i will update miraiSTUDIO as soon as i can for bug fixes. 

### New

- **Chart takes**: keep copies of a chart (Chart panel > Takes) and switch between them. Only the chart changes.
- **Song versions**: File > Save a version... keeps a named copy of the whole song; File > Versions... brings one back. They're kept in `My Files\Song versions`.
- **Line tool** (Note lines): draw straight lines, bend them into curves, and add or remove corners, like Adobe Animate's line tool.
- **Screen camera keys** (Note lines) work like the line's points: click or box-pick them, drag to move, double-click to add, Del to remove. Shift-drag moves the screen.
- **Snapping and handles** (Note lines): hold Ctrl while dragging to snap to the grid. Turn on Handles to bend the path with Bezier handles.
- The timeline shows the snap's divisions between beats.
- **Rides** in the Inspector shows which line a note is on, and lets you choose it.
- **Put notes on the lines** puts every note on the line it belongs to (under Warnings, or Sections in Note lines).

### Changed

- Snap sizes are named as note values: 1/4 is a beat, then 1/8, 1/16 and so on.
- "Extreme" is now **Super Hard**, as in the game.
- Edits to the game's songs are saved in `My Files\Songs`, like your own songs.

### Fixed

- The beat grid was a few beats off on some songs.
- Scrolling the timeline while box-picking moved the box.
- Notes stayed on no line (and didn't show in the game) when their line was made before them. New, pasted and moved notes now go onto their line.
- Saving failed with "no LINE layer to copy" after all of a song's lines were deleted.
- The hold sound kept playing after a hold ended, and cut out on long holds.
- Super Hard levels didn't show in Song Info or the Library.
- Importing a song mod also copied game songs it didn't change.
- Long holds were drawn past the end of the blue line in the game view.
- The application window "froze" or went white after minimizing the window. (technically was still working but would kinda just softlock and freeze the screen so it was just unusable)
- The dancer's shadow slid around under the feet.

### For testers

- If the app freezes, the `crash logs` folder gets a freeze report. Please attach it to your issue.
- To transfer your data and work to the new version, move **miraiSTUDIO_settings.txt** , **miraiSTUDIO_layout.ini** , **miraiSTUDIO_last_song.txt**, your **work** folder, and optionally the **crash logs** folder if theres still crashes you need to report.
