# Sound atlas

Interactive chords and scales in all 12 keys. Open `index.html` locally or visit https://jacpagan.github.io/modes/.

- 62 chord formulas, compact inversions, and arpeggio keyboard sweeps.
- 149 scale/mode rows from 21 photographed charts, shown consecutively by chapter.
- Click a row to listen; ↑/↓ browse, ←/→ change inversion, Space replays, Esc stops.
- Play/Stop supports loops, inversion cycling, keyboard sweeps, and automatic browsing. Options contains tone, volume, and sweep range.

No installation or external audio dependencies. Audio begins after user interaction. Chords use compact voicings with repeated pitch classes omitted; scale formulas preserve printed accidentals. Every mode is rooted on the selected key.

Source photo filenames and page numbers are recorded in `data/scale-chapters.json`; `js/scale-chapters.js` supplies the same data for offline use. Symmetric whole-tone and diminished rows are retained as printed. Original demonstration pages remain available.

Run `node test-scale-chapters.cjs` to check initialization, the continuous scale list, modal rotations, and the chord view.
