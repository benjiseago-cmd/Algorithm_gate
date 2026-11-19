# Foldbreak Arena

**A local two-player platform fighter with nets-of-shapes comeback questions.** Ten playable characters, ten arenas, five lives each, one laptop keyboard. Created19November2026.

## Download and play

Open **foldbreak-arena.html** on GitHub and click **Download raw file** (the downward arrow above the code). Find the saved HTML in your laptop’s Downloads folder and double-click it. The whole game works offline in a modern browser.

Choose a left player and a right player below the portraits, select an arena and press **Start the match**. Matching characters are allowed. The game saves your fighter and arena selections separately from Algorithm Gate and Lockstep.

For the editable source ZIP, download **download-backup.html**, open that saved page and click **Download source backup ZIP**. The archive includes the complete playable HTML, source modules, build script, curriculum notes and test evidence.

## How the fight works

Damage raises your percentage and increases the knockback of later hits. Launch a rival beyond an arena’s blast boundary to use one of their five lives. While they still have lives left, a four-choice question about nets of shapes appears. A correct answer returns them to a safe landing at0% damage; wrong answers and hints cost no lives. The other player can keep moving while the question is open. Both players can answer separate questions at the same time.

A fifth lost life means elimination. The last player with lives remaining wins; simultaneous final knockouts are a draw. Correct answers do not create extra lives. Comeback protection lasts briefly and ends if you attack. Confirmation keys must be released before attacking after a respawn, so answering does not accidentally waste that protection.

Triple jumps, a short grace period after leaving a ledge and forgiving spawn points help with recovery. Down drops through upper perches and speeds up a fall; stable main floors hold you safely. Moving and crumbling platforms use their real geometry, including blocking projectiles. Removed platforms stop being cover.

## Controls

| Action | Left keyboard / Player1 | Right keyboard / Player2 |
|---|---|---|
| Move | A / D | Left / Right arrows |
| Jump, up to three presses | W | Up arrow |
| Drop through an upper platform / fall faster | S | Down arrow |
| Normal attack | C | Comma (,) |
| Slower heavy or ranged attack | V | Full stop (.) |
| Charged special | B | Slash (/) |
| Choose a quiz answer | W/S or A/D | Arrow keys |
| Confirm quiz answer | C | Comma (,) |
| Free quiz hint | B | Slash (/) |
| Pause / resume | Esc | Esc |

You can click answers and hint buttons too. Normal and heavy attacks repeat while held. Specials use a fresh press with a full bar. Hitting or receiving actual hits fills the bar; waiting or striking protected opponents does not. Meter carries across a knockout for comeback opportunities. Read each character’s three moves in the selection screen.

## The roster and arenas

Returning characters are **Ram**, **Stag**, **Rook** and **Kit**. New fighters are **Mr Seago**, a friendly blonde teacher with a ruler/chalk moveset; **Nova**, a star navigator; **Bolt**, a brass golem; **Moss**, a woodland sprout; **Glint**, a crystal cat; and **Ember**, a phoenix spirit. Each has a different normal reach, movement/weight profile, heavy attack and special ability. See ROSTER.md in the source ZIP for the complete move list.

Arenas: Foundry Ring, Whispering Grove, Cogspire Rooftops, Mr Seago’s Classroom, Tidal Docks, Star Observatory, Skyrail Express, Crystal Cavern, Ember Crucible and Eclipse Summit. They have different physical layouts, with moving crossings, raised perches, open roof gaps and crumbling wings.

## Maths and verification

Questions cover seven solids, valid/invalid cube nets, and opposite faces after folding. An independent geometry review verifies the answers, including all35freehexominos and exactly11validcube nets. Hints and worked comeback explanations support learning. CURRICULUM.md in the ZIP explains the conventions for cuboids and curved solids.

The release passed automated engine, geometry, rendering and browser tests, including a scripted five-life match, real attack keys, free wrong answers, simultaneous questions and the winner screen. There was **no manual two-person playthrough or subjective balance assessment**. TESTING.md gives the exact scope and limits.

Algorithm Gate, Lockstep, Slant Gate and the original uploaded attachment remain unchanged. This is a separate offline game with independent settings.
