# Slant Gate

A separate area-question edition of the latest Algorithm Gate game, created 15 November 2026. Download **slant-gate.html**, then double-click the saved file to play offline in a modern laptop browser.

## Maths

All gate and recovery-well questions vary one of these two ideas:

1. Find a parallelogram’s area, then subtract the area of a triangle inside it. The triangle uses the same perpendicular height and a shorter base.
2. Find the new area of a triangular garden after both its base and perpendicular height are doubled. The new area is four times the original area.

The first gate in chapter 1 uses the supplied 11 cm / 6 cm parallelogram and 5 cm / 6 cm triangle: **51 cm²** remains. The first gate in chapter 2 uses the supplied 10 m / 7 m garden: its new area is **140 m²**.

Both question types occur throughout the ten chapters. Later chapters use larger measurements and half-unit dimensions. Diagrams identify perpendicular height; hints explain the relevant formulas. Worked solutions appear after a correct answer. Enter a number, a fraction or a number with the matching square unit (for example 51, 102/2, or 51 cm²). Incorrect units are rejected without losing hearts.

## Same adventure

Routes, platform lengths, timed obstacles, guardians, arena cover, heroes, animation, controls, physical puzzles, upgrades and Light systems are retained from the latest Algorithm Gate edition. Wrong answers and hints remain free. Each newly accepted recovery-well question restores exactly one heart, with duplicate-submission protection and independent co-op recovery. Existing save-key names are preserved.

Algorithm Gate remains a separate, unchanged file. The included algorithm-gate-source.html is the exact source used for this fork.

## Validation

- 10,000 seeded questions checked independently across all ten chapters, including geometry, answers, both families, deterministic output and question identity.
- 34 answer-parser cases, including correct units, wrong units, decimals and fractions.
- 117 scripted Chromium/browser-engine checks: examples 51/140, gate submissions, free hints and wrong answers, worked solutions, recovery, 450 fresh-well sips with the existing recent-20 identity rule, concurrent co-op questions, duplicate prevention, saved Light/upgrades, controls, bosses, cover and secret rooms. Gate and well panels checked at 1366×768 and 1024×768.
- 7 source-parity checks: bosses, routes, engine, physical puzzles and economy are byte-identical. Campaign differences are only the displayed maths skill labels; gameplay artwork is unchanged.
- Offline Chromium context runs the engine, renders the new question and accepts the correct area answer without network requests.

These are automated simulations and scripted browser tests, with screenshot inspection. No manual full-game playthrough was performed. The exact double-click file:// path was not tested in this managed browser; the game has no external runtime dependencies.

## Downloads

For the complete source ZIP, download **download-backup.html**, open that saved HTML on your laptop, then press **Download Slant Gate backup ZIP**. The ZIP includes Slant Gate, the unchanged Algorithm Gate source used for it, tests and validation reports.

Source baseline SHA-256: bc6dd8022edc9ef4a7803ec95d7f7dca8b10953b421353b2807b957f171db241
