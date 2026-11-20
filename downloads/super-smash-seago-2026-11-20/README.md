# Super Smash Seago

Updated 20 November 2026. An original offline platform fighter for a laptop keyboard, with a solo unlock campaign and local two-player battles.

## Download and play

Open **super-smash-seago.html** on GitHub and choose **Download raw file** (the down-arrow button). Open that saved HTML in Chrome, Edge, Firefox or another current desktop browser. The game is self-contained and works offline. No account, installation, assets folder or internet connection is needed.

For the editable source ZIP, download **download-backup.html** using the same down-arrow button, open that downloaded page, and click **Download source backup ZIP**. This extra page embeds the entire backup; it also works offline.

## Solo adventure and unlocks

Start with **Mr Seago** — “Just a teacher.” — and his classroom. The solo adventure has nine computer rivals. Win a five-life match to unlock that rival and their arena for two-player mode. Cleared challenges can be replayed; unlocked fighters may also be used in solo challenges. Losses and draws keep existing unlocks but award no new ones.

Unlocks save locally in this browser, on this device and game copy. Clearing browser storage or opening a different file/browser/device can give a fresh save. There is no online account or shared class save. A message appears if storage is unavailable; progress then lasts only for the current visit.

## Controls

| Action | Player 1 / solo | Player 2 |
|---|---|---|
| Move | A / D | Left / Right |
| Jump | W | Up |
| Drop from upper ledge / fall faster | S | Down |
| Normal attack | C | Comma |
| Heavy attack | V | Full stop |
| Charged special | B | Slash |
| Question selection | W/S or A/D | Arrows |
| Submit selected answer | C | Comma |
| Free hint | B | Slash |

Solo players can use **either complete keyboard layout**, including arrows/comma/slash for comeback questions. Both layouts control the same solo fighter; the CPU stays independent. In two-player mode the layouts stay separate.

Mouse clicks also select answers and hints. Escape pauses. The button in the **bottom-right arena corner** toggles browser fullscreen; it remains available in fullscreen.

## Match rules

Every new match, retry and rematch opens with **3–2–1–FIGHT**. Fighters, CPU, platforms, match time and powerup timers stay frozen during the countdown. Pause and help also freeze it.

- Each fighter starts with five lives. Ring-outs cost one life.
- While lives remain, a correct multiple-choice question about nets of 3D shapes returns you safely, with zero damage and brief protection. Attacking ends that protection.
- **A wrong answer costs one additional remaining life** and gives a fresh question. The final lost life ends the match. Hints are free. Duplicate/stale question submissions cannot take another life.
- Damage increases knockback and reduces normal jumps between landings: **three below100%, two from100%, one from130%**. Land to reset the jump count. Direct special movement remains possible without refunding normal jumps.
- All ten specials are strong offensive attacks with visible wind-ups, distinct large effects and substantial damage/launch. Earn a full special bar through real hits, then use B or slash.
- Sky crystals first fall around ten seconds into an active fight, then every twenty seconds. Touch one to become a **dragon** or **war elephant** for twelve seconds. Normal, heavy and special attacks change. Specials still need full charge. The form ends on expiry or knockout.
- The computer uses the same physics and ordinary movement/attack inputs. Its own knockout comeback takes2.5seconds; it never answers a pupil's question.

## Worlds and artwork

Ten arenas use distinct permanent routes, vertical steps, moving crossings/lifts and unstable shortcuts. Each includes two moving and two crumbling platforms. Stable spawn landings cannot be dropped through. Crumbles disappear temporarily and stop blocking shots; moving surfaces use their actual collision geometry. Platforms block projectiles, including fast shots.

The bright original waterfall-adventure art includes different scenery for each arena, animated lava falls in the ember-themed world, and cyan dot eyes for Rook. Lava, water, plants and distant scenery are decorative, not hidden hazards. No Nintendo artwork or characters are included.

## Source and testing

The ZIP includes the current standalone HTML, editable source, tests and reports, plus untouched copies of Foldbreak Arena and Super Smash Seago before this UI polish. To rebuild, run `python source/build.py` (Python3); this writes `source/super-smash-seago.html`. The playable HTML needs no build tools.

Test scripts require Node.js and, for browser checks, Playwright plus Chromium. The scripts preserve their development paths (`work/seago`); arrange that path or adjust it when reproducing tests elsewhere. Reports identify the fixtures used. See **TESTING.md**, **ROSTER.md** and **WORLDS.md** for details.

Verification uses automated physics/combat simulations and scripted Chromium clicks, keys, fullscreen and offline-content checks. Scripted campaign outcome fixtures verify unlock integration; they are not manually won campaign matches. **No manual two-person playthrough or pupil balance assessment has been performed.**

Algorithm Gate, Slant Gate, Lockstep and the previous Foldbreak Arena release remain unchanged.
