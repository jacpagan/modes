# Sound atlas

Interactive chords and scales in all 12 keys. Open `index.html` locally or visit https://jacpagan.github.io/modes/.

- 62 chord formulas, compact inversions, and arpeggio keyboard sweeps.
- 179 scale/mode rows from 26 photographed charts, shown consecutively by chapter.
- Click a row to listen; ↑/↓ browse, ←/→ change inversion, Space pauses/resumes, Esc stops.
- Play/Stop supports loops, inversion cycling, keyboard sweeps, and automatic browsing. Options contains tone, volume, and sweep range.

No installation or external audio dependencies. Audio begins after user interaction. Chords use compact voicings with repeated pitch classes omitted; scale formulas preserve printed accidentals. Every mode is rooted on the selected key.

Source photo filenames and page numbers are recorded in `data/scale-chapters.json`; `js/scale-chapters.js` supplies the same data for offline use. Symmetric whole-tone and diminished rows are retained as printed. Original demonstration pages remain available.

Run `node test-scale-chapters.cjs` to check initialization, the continuous scale list, modal rotations, and the chord view.

## Sing review
Call-and-response now supports scale, every-other-note, and 1–3–5 patterns, with optional live guidance. Per-note review reports detection coverage, sustained median signed and absolute errors, onset median error, and pitch spread. Sustained windows omit the initial 200 ms (or 25% of short notes) and final 60 ms. Fewer than three clear frames or less than 60% sustained coverage produces an uncertain result. These are engineering heuristics, not validated conservatory thresholds. Manual timing alignment shifts target windows; it does not calibrate microphone latency. Real-voice/device validation remains outstanding.
Run `node test-take-analysis.cjs`, `node test-call-response.cjs`, `node test-sing.cjs`, and `node test-exercise.cjs` for analysis and exercise checks.
