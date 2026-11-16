# Algorithm Gate downloads

## Latest original edition — 16 November 2026

1. Open **algorithm-gate-updated.html** and choose **Download raw file** (the downward arrow above the code).
2. Find the saved HTML in your laptop's Downloads folder and double-click it to play offline.
3. For the complete ZIP, download **download-backup.html**, open that saved HTML, and click **Download backup ZIP**.

This revision fixes legs showing through the cloaks, smooths the branch attack, consolidates redundant lanterns and shares route checkpoints between both heroes. The first boss's behavior is unchanged; the Crown's casting position is corrected after reviewing every guardian.

Slant Gate is a separate edition and has not been changed by this update.

Algorithm Gate — cloak, branch attacks and shared lanterns
16 November 2026

Open algorithm-gate-updated.html in a modern laptop browser. It is a self-contained offline HTML. This update is for the original algorithm-maths edition. Slant Gate remains unchanged.

Changes
- Both articulated legs use the same moving cloak silhouette as an occlusion mask. They no longer paint over the cloth, including damage-blink frames. Walking, rising, apex, falling and landing poses remain.
- Both heroes hold forked branches. A continuous eased pose moves from rest through a wind-up, sweep, follow-through and return. The branch has fixed geometry and turns into/out of the picture plane instead of abruptly changing length. Trails are short and restrained. The ram horns, stag antlers and skull artwork are retained.
- Damage still resolves when an attack is triggered. The existing 0.23-second attack timer and 0.38-second normal / 0.30-second Quicksilver cooldowns are unchanged. The visual return ends at 0.30 seconds. Longreach still increases both hitbox width and peak visible horizontal reach by exactly 20% (69 to 82.8 world pixels). A hero at zero hearts or reading the well rests the branch.
- Redundant checkpoint nodes on the same real landing are consolidated. Route lanterns sit on actual stable stone, including the low ledges above two gate-approach floors. Each chapter now has 10–14 useful route lanterns, with no adjacent duplicates on the same landing.
- When either living co-op hero touches a new route lantern, both heroes receive its route respawn anchor. Nobody is teleported, healed or revived just by touching it. A dead partner keeps the future anchor but still needs the existing gate-revival rule. A repeated touch of the latest lamp also resynchronizes a teammate after a gate revival. Older lamps cannot move the party's checkpoint backwards.
- Shared respawn positions fit both heroes on the support and stay on the lantern's side of unopened gates/seals. Falls recheck current crate and obstacle geometry. Boss-well recovery keeps its separate safe refuge and one-heart-per-fresh-answer rules.
- Reviewed every guardian against its arena, including warnings, safe escape choices, usable attack openings and real projectile cover. One defect was found in the final guardian: part of its barrage could spawn inside the middle shelf. The Crown now casts from a higher actual position; projectiles still collide with cover. Boss HP, speeds, timings and arena geometry are otherwise unchanged.
- The first guardian's attack pattern and arena are unchanged. Four deterministic solo/co-op normal/enraged traces match the previous build exactly.

Validation on the final integrated HTML
- 169/169 automated browser/engine checks: algorithm progression, controls, purchases/saves, co-op recovery, projectile cover, secrets and the new checkpoint behavior across all ten chapters.
- 21 focused checkpoint checks: re-touch after gate revival, no teleport/heal, safe return from the secret collision dimension, and unchanged Slant Gate checksum.
- 41 animation checks, including 224 pixel-mask comparisons across both heroes, both directions, walking/air/landing and translucent damage frames. Branch phase boundaries and Longreach geometry are checked. Pose and locomotion sheets were visually inspected.
- 87 guardian quality checks: normal/enraged fights and the Crown's three stages in both modes; explicit warnings, bounded phases, clean exposure windows, 216 no-upgrade approaches to a strike opportunity and tested rush/dive/leap/marker escape choices. Some deliberately wrong-direction attempts take damage; passing means an intended safe choice exists, not that every choice is safe.
- 34 guardian cover/camping checks remain passing.
- 460 natural-cycle emitter scenarios cover sampled floor/perch positions and both modes. 28,200 projectiles were observed, with zero births inside collision cover.
- Four Warden trace comparisons are identical over 30 simulated seconds each.
- Offline Chromium content test runs without external requests.

Limits
These are automated engine simulations, scripted Chromium tests and screenshot inspections. No manual full-game playthrough or subjective fun rating was performed. Simulations sample positions and input timings; they do not prove every possible action or real two-person keyboard experience. Overall feel still benefits from player feedback.

Archive
algorithm-gate-updated.html is this revision.
algorithm-gate-before-round3.html is the previous delivered algorithm edition.
algorithm-gate-original.html is the byte-for-byte initial uploaded attachment.
reports/ and tests/ contain the validation evidence and test scripts. Some test scripts retain work/ paths from the development checkout. The game itself needs only the HTML file.

Original attachment SHA-256
0c22f65182fe43da471ce43720a00828bbd470d927c7527636d5e3370792f1d9
