# ChordKeys
Setup: upload these files to the root of a GitHub repo, then Settings > Pages > Deploy from branch (main, / root).
Release an update: edit index.html as needed, change VERSION in sw.js (e.g. '3.9'), commit and push.
Installed copies check on launch, every 30 minutes and when the app returns to the foreground, then show an "Update now" banner.
The current version shows next to the title and at the bottom, where "Check for updates" also lives.
Everything the app saves (progress, recent songs, settings) stays on the device. Use Help > Back up progress to keep a copy.

## Opening scores and chords (v4.0)
- **Open file** accepts MIDI (.mid), MusicXML (.musicxml, .xml, .mxl) and chord text (.txt, .cho).
- **Type chords** builds a two-hand score from typed or pasted chords (Ultimate Guitar charts, ChordPro, or `| C | Am7 | Dm7 G7 | C |`). The result can be downloaded as a MIDI file.
- Guitar Pro (Songsterr), MuseScore project files and PDFs cannot be read directly. Export MIDI or MusicXML from MuseScore Studio instead.
- To release: bump `VERSION` in `sw.js`, upload, and installed copies show the update prompt.
