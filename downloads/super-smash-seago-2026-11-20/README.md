# Super Smash Seago

Updated 20 November 2026. A self-contained laptop platform fighter with fifteen fighters, fifteen arenas, a fourteen-rival solo campaign, local two-player battles and nets-of-shapes comeback questions.

## Download and play

Open **super-smash-seago.html** on GitHub and choose **Download raw file** (the down-arrow button). Open the saved HTML in a current desktop browser. It works offline with no installation, account, assets folder or server.

For the editable source ZIP, download **download-backup.html** with the same down-arrow button, open that saved page, and click **Download source backup ZIP**. That downloader embeds the complete backup and also works offline.

## New fighters and worlds

- **Girly Girl / Makeup Box** — cheerleading, dancing and makeup; the second campaign fight. Every platform crumbles, including three travelling trays. There is no permanent floor. Platforms return after2.5seconds; a respawn drawer gets1.8seconds of grace before it can start crumbling. Keep moving.
- **Napoleon / Waterloo Waterline** — bicorne, baton, cannonball and cannon salute, with forts, pontoons and mechanical lifts.
- **Edmund / Lanternwood Wardrobe** — ginger hair, freckles, a nervous hunched pose, wintry delight attacks and snowy wardrobe/lamppost scenery.
- **007 / Secret Service Hangar** — tuxedo, pistol shots, ricochets and a charged gadget barrage, with moving vaults and gantries.
- **Harry Kane / Golden Boot Stadium** — football kicks, ball shots and a hat-trick special, with a split pitch, stands and moving sporting platforms.

These rivals are interleaved with the earlier fighters rather than appended as a separate block. The original ten fighters and ten arenas retain their earlier combat statistics and map geometry.

## Campaign and saved unlocks

Only **Mr Seago** — “Just a teacher.” — and his classroom start unlocked. Win against a rival to unlock that fighter and arena for two-player mode. Defeat, a draw or multiplayer cannot unlock campaign content. Cleared fights can be replayed with any already unlocked fighter.

Earlier version1 saves are migrated automatically: old wins and their fighter/map unlocks remain. The campaign offers the earliest undefeated challenge, including new rivals inserted among old ones. The save format is now version2, using the existing browser storage key. Replays do not duplicate unlocks.

Saves belong to the browser, device and game-copy location. Keep the same file location when replacing an older download. Clearing storage or opening a different copy/browser/device can start a fresh save. If browser storage is unavailable, progress lasts only for that visit.

## Controls

| Action | Player 1 / solo | Player 2 |
|---|---|---|
| Move | A / D | Left / Right |
| Jump | W | Up |
| Drop / fast-fall | S | Down |
| Normal attack | C | Comma |
| Heavy attack | V | Full stop |
| Charged special | B | Slash |
| Choose quiz answer | W/S or A/D | Arrows |
| Confirm quiz answer | C | Comma |
| Free hint | B | Slash |

Solo accepts either complete layout, including questions. The computer remains independent. In two-player mode the layouts control separate fighters. Mouse answers and hints also work. Escape pauses.

Use **Full screen** in the menu or the arena’s bottom-right corner. Fullscreen now covers the whole page: after a match you can return to the menu, scroll through fighters/arenas, and start again without pressing Escape. Both fullscreen buttons show the current state.

## Rules and visual reminders

Every new match, retry and rematch starts **3–2–1–FIGHT**. Fighters, CPU, moving platforms, clock and powerup timers freeze during the countdown; pause/help also freeze it.

Each fighter has five lives. Ring-outs cost one life. If lives remain, a correct four-choice question about nets of3Dshapes returns you at zero damage with brief protection. Attacking ends protection. Each wrong answer costs another life and gives a fresh question; hints are free. Stale or duplicate submissions cannot consume another life. The final lost life ends the match.

Normal jumps between landings: three below100%, two from100%, one from130%. Damage also increases knockback. The damage number grows at100%, grows again and pulses at130%. A full special bar shakes and glows until used. Reduced-motion preferences disable those animations while keeping static emphasis.

All fifteen specials are offensive charged attacks with readable wind-ups, substantial damage/launch and distinct effects. Full charge is earned from real hits, not waiting. Platforms block projectiles using actual swept collision geometry; removed crumbles stop covering.

Sky crystals first fall at roughly ten active seconds, then every twenty. Three twelve-second forms cycle fairly: fire-breathing **Dragon**, charging **War elephant**, and a very fast armored **Gladiator lion**. Each replaces normal/heavy/special moves; charged specials still need a full bar. A form ends on expiry or knockout. The lion runs at480units/second before other status effects. Crystals wait for a returning support if Makeup Box is temporarily entirely gone.

The computer uses ordinary movement/attack inputs and the same physics. Its own quiz comeback takes2.5seconds; it never answers a pupil’s question. It is a deterministic heuristic rather than a human or trained opponent.

## Source and verification

The ZIP contains the current offline HTML, editable modules/build script, tests/reports and untouched previous HTML releases. Rebuild with `python source/build.py` (Python3); the output is `source/super-smash-seago.html`. No build tools are needed to play.

Node.js tests use Playwright and Chromium for browser checks. Some scripts retain development paths such as `work/seago`; arrange that path or adjust it to reproduce them elsewhere. Companion `.cjs` fixtures are included.

Reports distinguish automated physics/combat simulations, prepared knockout/attack fixtures and actual browser clicks/keys/wheel/fullscreen events. Unlock fixtures are not manually won campaigns. Offline HTML contents were tested with networking disabled; the managed browser blocks direct file-URL navigation. **No manual two-person playthrough, class trial or human balance assessment has been performed.** See TESTING.md, ROSTER.md, WORLDS.md and source validation notes.

Algorithm Gate, Slant Gate, Lockstep and the earlier Foldbreak Arena release remain unchanged. All rendering is procedural with no external image assets.
