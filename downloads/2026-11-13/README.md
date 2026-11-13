# Algorithm Gate downloads

## Updated game — platform lengths, timing and arena revision

1. Open **algorithm-gate-updated.html** and choose **Download raw file** (the down-arrow button above the code).
2. Find it in your laptop’s Downloads folder, then double-click it to play offline.
3. For the complete ZIP, download **download-backup.html**, open that saved HTML on your laptop, and press **Download backup ZIP**.

This revision varies platform lengths, adds 33 timed crossings, removes starting-floor enemies, anchors tips to real stone, and reworks each guardian’s attacks and arena together. Warden’s floor brambles now have a clear lane; warned roots make stationary perch camping unsafe. Real projectile cover remains.

The untouched original is **algorithm-gate-original.html**. The ZIP contains that original, this update, the previous update, test scripts and detailed results.

Algorithm Gate — platform lengths, timed crossings and guardian arena revision
13 November 2026

Download algorithm-gate-updated.html and open it in Chrome, Edge or Firefox on a laptop. The game remains a self-contained offline HTML: no library, image, audio or network dependency is required. Both heroes, ten algorithm chapters, solo/co-op, puzzle stages, upgrades, Light and recovery rules are retained.

What changed in this revision
- 28–31 distinct main platform lengths per chapter (excluding the broad ground floors); individual stepping stones/run-ups span 108–242px, with narrow shaft shelves kept 118–138px. Optional branch ledges vary too. Puzzle chambers and the final refuge keep broad permanent floors.
- 33 authored timed crossings: moving blades and spectral plumes positioned between selected route stones. Each has a permanent waiting stone and visible stone-edge rune anchors. Plumes show an amber warning before activation; warning and damage use the same timing state. Off windows are deliberately forgiving. Other edge vents/blades add variety, with the well approaches kept clear.
- Ten arenas now work with their guardians' attacks. Warden/Prism/Cinder/Crown have open floor-wave lanes. Warden uses 1.05-second warned roots from the occupied floor or ledge. Tideclaw's refuges remain reachable, with slow arcing bubbles aimed at a locked position to discourage camping. Dives/leaps mark the actual occupied ledge height. Prism casts from above and its 3.2-second barrage lasts long enough for distant shots to arrive. Weaver casts from two heights and uses 1.1-second warned web markers, keeping its 4.2-second clean opening.
- Corrected several projectile origins that were inside their own arena platforms. Stone still physically blocks shots; no attack is made to phase through cover. Falling ice/lightning still clip against real cover. Roots/webs grow from the marked support rather than falling through a roof.
- Removed the enemy on every chapter's starting floor, after assigning stable Light IDs to the remaining monsters. No start-of-level heart loss while reading the controls.
- World tips use posts anchored to actual stone, or plaques inset into arena floors. Start controls are combined, shaft/gallery/drop advice is repositioned, timing clues identify their launch stones, and text wraps without squeezing.

Validation on the merged game
- 86/86 scripted Chromium integration checks, covering ordered algorithms, all ten solo/co-op recovery systems, duplicate heart prevention, retries, outside-arena protection, actual keyboard controls including focused-well co-op input, saved upgrades/Light, projectile cover and secret-room isolation.
- 112 focused engine assertions for safe starts in every chapter/mode, no hazards in the well approach, warning-versus-live damage state, and ballistic cover collision.
- All ten chapters pass continuous traversal simulations in solo and co-op: 39 accepted transitions per chapter, no teleports between accepted transitions. The solver searches/replays input timings from saved states. Combat, puzzle mechanisms, barriers and hazards are excluded here; actual stone, roofs, walls, crumble, moving platforms and shared-camera physics remain.
- 66/66 live timed-crossing solutions (33 crossings in each mode) take no damage; waiting is safe.58 cases also demonstrate that mistimed launches can hurt. These tests isolate one timed crossing at a time.
- 60/60 optional branch transitions pass exact contact tests in solo/co-op.
- Every arena shelf is reachable without upgrades in jump-physics graph tests.34/34 guardian/arena checks pass, including actual shot paths, open bramble lanes, warned escape input, Tideclaw refuge/bubble paths, locked-height dive warnings and clear exposure windows. Stationary camping probes sample floor and ledge positions over three cycles, repeatedly pinning the hero to that position to test whether the real attack can threaten it; they are not difficulty ratings or natural player behavior.
- 70 world signs pass geometry clearance checks; browser text measurements fit their plaques and use no max-width text squeezing. Scripted route/arena screenshots were visually reviewed. New root/web/bubble/plume states render without browser errors.
- All 76 puzzle-stage physics solutions and local resets remain valid from the prior mechanism suite; the mechanism implementation is unchanged in this revision.
- Offline Chromium context successfully loads HTML directly and makes no network requests. Managed Chrome blocks file:// navigation in this environment, so exact double-click file navigation was not tested here.

Limits
No manual human playthrough was performed. No complete run combines all live route hazards, puzzle solving and guardian combat end to end. Overall difficulty, pacing and real two-person keyboard comfort still need player/classroom feedback. Automated traversal, isolated timed crossings, mechanisms and guardian attack paths are tested separately. No known failing automated checks remain.

Archive contents
algorithm-gate-updated.html: this revision.
algorithm-gate-original.html: byte-for-byte original uploaded algorithm edition.
algorithm-gate-before-round2.html: the previous delivered update.
reports/: automated results.
tests/: test scripts. These use Node.js; browser tests use Playwright/Chromium. Some retain work/ output paths from the development checkout.

Original SHA-256
0c22f65182fe43da471ce43720a00828bbd470d927c7527636d5e3370792f1d9
