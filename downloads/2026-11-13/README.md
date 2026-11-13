# Algorithm Gate — 13 November 2026 backup

The uploaded `algorithm-gate (3).html` was used as the source of truth. The original algorithm edition is preserved byte for byte in `algorithm-gate-original.html`.

## Download and play

1. Open `algorithm-gate-updated.html` in GitHub and choose **Download raw file** (the down-arrow button above the code).
2. Find the saved file in your laptop's Downloads folder.
3. Double-click it to play offline in Chrome, Edge or Firefox.

For the complete source backup, download `download-backup.html`, open that saved HTML on your laptop and press **Download backup ZIP**. The ZIP contains both game versions, testing notes and test scripts.

Algorithm Gate — updated algorithm edition

Open algorithm-gate-updated.html in a modern desktop browser. It contains all CSS, JavaScript, art and audio generation, with no external dependencies. The original attachment is preserved separately, byte for byte. No game modules were extracted.

Changes
- Ten authored routes with different starting/gate/arena elevations, climbs, drop passages, four wall-jump shafts, covered galleries, moving crossings and reconnecting branches. Lantern secret entrances and shelf layouts vary by chapter.
- Counterweight targets 2–6, varied lift positions, reordered reusable rune sequences, 1–3 reflected mirrors with either emitter direction, and left/right sliding ice with movable stoppers. Later optical ice combines mechanisms. R resets only the nearby unfinished stage for free.
- Ten arena layouts with low solid cover and aerial stone. Swept shot collision includes current/moving platforms, active crumble, walls, crates and closed barriers. Cover wins ties before hero damage; removed crumble stops covering. Shockwaves spawn above the floor. Falling ice/lightning warning and damage regions use the same cover clipping. Flood remains a floor hazard.
- Articulated walking, separate rising/apex/falling/landing poses, breathing, cloak and head movement, true side skull profiles with ram horns/stag antlers, and quill sweep/follow-through. Longreach remains exactly 20% for both hitbox width and visible horizontal swing reach.
- Original ten guardians, ordered algorithm questions, solo/co-op, keyboard bindings, well recovery, Light/save/purchases, eight upgrades and small monsters remain.

Validation performed
- 86/86 automated Chromium integration checks, including 1,000 ordered algorithm examples; all ten solo/co-op well/retry scenarios; zero-heart return; one heart per accepted fresh answer; duplicate rejection; free wrong answers; one partner recovering while combat continues; full retreat reset; ordinary one-heart gate revival; outside-arena protection; actual keyboard and focused-well co-op input; save/reload; secret dimension isolation.
- 76 solo/co-op puzzle stage solutions and 76 local reset scenarios, using actual crate/ice/lift/beam engine methods (11,904 crate push operations). Stage solver sets up heroes and mirror orientations directly and mounts the finished lift directly; it is not a complete player walkthrough of each chamber.
- Continuous traversal solver passes all 10 chapters solo and co-op, 39 accepted transitions each, from the actual spawn without teleports between accepted transitions. Solver searches/replays input timings from previous valid states. Hazards, enemies, puzzle mechanisms/blocks and barriers are excluded; gates are pre-solved. Actual platforms, roofs, walls, moving/crumbling stone and shared-camera constraints remain. Three redundant buried waypoints map to the permanent ground surface above them.
- Forced wall-jump physics tests pass all four shafts. All ten secret-room treasure graphs are reachable using jump/ceiling physics.
- 26 animation/render checks for both heroes, including visible reach 69 → 82.8. Ten arena renders inspected; Tideclaw first refuge reached by an actual no-upgrade single-jump simulation. Mirror Weaver keeps its 4.2-second recovery opening.
- Offline Chromium context loaded HTML directly, ran 120 engine frames, and made zero network requests. Managed Chromium administrator policy blocks file:// navigation here, so the exact double-click-from-disk path was not tested in this environment.

Limits / remaining playtesting
No manual human playthrough was performed. No end-to-end run with every puzzle and live hazard/combat enabled together was completed. Route and puzzle correctness were checked separately; difficulty, pacing, sustained guardian fights and real two-person keyboard comfort still warrant classroom playtesting. No known failing automated checks remain. No claim is made about why the previous workspace went pending/offline.

Untouched original SHA-256
0c22f65182fe43da471ce43720a00828bbd470d927c7527636d5e3370792f1d9
