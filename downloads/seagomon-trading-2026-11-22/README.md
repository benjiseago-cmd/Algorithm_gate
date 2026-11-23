# Seagomon: The Trading Game — Illustrated Edition

The same times-table speed game, now with 200 original illustrated creature scenes, one-card foil packs, rarity reveals and unlockable animated worlds. Updated 23 November 2026.

## Play

Direct hosted downloads: `seagomon-200-offline.zip` contains the ready-to-play HTML; `seagomon-trading-source-backup.zip` contains the complete game and editable source. Extract either ZIP before opening its HTML.

Open the hosted game, or download `seagomon-trading-game.html` and open it in a current desktop browser. On GitHub choose **Download raw file**. The HTML contains all illustrations, scenes, sounds and game code; playing offline needs no installation or network connection.

Four editable display cases, all eleven tables and the pack shop remain on the laptop dashboard. It targets 1024×768 and 1366×768 at normal zoom; smaller screens use a scrolling fallback. Dialogs can scroll internally.

## The 200-card collection

This expansion adds 100 new monsters with individual illustrated scenes, lore and assigned rarities: 40 Common, 30 Uncommon, 18 Rare,9 Epic and 3 Megarare. The original 100 identities, rarities and illustrations remain unchanged. Every creature also has a shiny variant, for 400 normal/shiny variants in total. The new cards join all three existing pack pools; prices, rarity weights, shiny chances, maths rewards and selling values are unchanged. Species within each rarity are equally likely, so each individual species now has half its previous chance within the larger pool.

The four display cards stand straight in matching glass cases with dark velvet backings, fine brass trim and a clean shelf. Cases keep their upright alignment on hover and on smaller screens. Existing display choices stay selected.

## Times tables and coins

Complete twelve facts, ×1 through ×12. Type an answer and press Enter. Mistakes keep the stopwatch running until corrected; there is no deadline.

| Tables | Coin multiplier |
|---|---:|
| 2, 5, 10 | 1× |
| 3, 4, 9, 11 | 2× |
| 6, 7, 8, 12 | 3× |

Ordered runs use 1×; shuffled runs use 2×. Base reward is `30 × table multiplier × order multiplier`. First clears add one base reward; beating an existing personal best adds three base rewards. An easy ordered first clear earns60 coins; improving23.00s to22.00s earns120 coins. Each of the22 table/order combinations keeps its own record. Official times round upward to hundredths; displayed ties cannot award a bonus. Closing unfinished runs gives no coins; repeated submissions cannot duplicate rewards.

## One-card packs

| Pack | Coins | Cards | Common | Uncommon | Rare | Epic | Mega Rare | Shiny |
|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Normal | 60 | 1 | 60% | 25% | 11% | 3.5% | 0.5% | 2% |
| Lucky | 120 | 1 | 35% | 32% | 24% | 8% | 1% | 4% |
| Shiny | 900 | 1 | 45% | 30% | 18% | 6% | 1% | 100% |

Every new pack contains exactly one monster card. Species within a rarity are equally likely. Shiny is independent of rarity, and a Shiny pack guarantees its single card is shiny. Duplicates remain possible. The shop and individual card pages show exact odds.

Rip the top foil strip, then watch the card gather energy. Higher rarities take longer to emerge, with stronger rings, particles and arrival effects; shinies add a prismatic effect. **Skip animation** reveals the already-drawn card immediately. Reduced-motion preferences bypass the opening animation. Purchases save coins, card, cosmetic bonus and pending reveal together before animation, so reloads never charge or grant twice.

## Illustrated cards and animated worlds

All 200 identities include 60 creatures from the attachment, 40 earlier additions and 100 new discoveries. The original 100 pixel grids remain as provenance data; visible cards now use 200 distinct, smooth illustrated scenes with developed creatures and rich environments. Gold-edged frames identify rarity; shiny variants use alternate colour treatment and moving foil. Twenty optimized image atlases are embedded once inside the offline HTML.

Aurora Studio is available immediately. Your first purchase in this edition additionally unlocks Waterfall Sanctuary. Later packs can unlock Firefly Grove, Coral Lagoon, Ember Highlands, Starfall Observatory and Storm Summit. Normal/Lucky/Shiny background bonus chances are20%/30%/50%, choosing equally among still-locked worlds. Bonuses never repeat and stop when all six are found. A world is an extra cosmetic reward, never a second monster card. The first Waterfall equips automatically if you use the default Studio; later discoveries preserve your choice.

Choose **Options → Animated backgrounds** to equip an owned world. The dashboard layout stays the same; scenes animate behind readable translucent panels. Reduced-motion preferences stop decorative motion.

## Collection and saves

The catalogue contains 80 Common, 60 Uncommon, 36 Rare, 18 Epic and 6 Mega Rare species, each with a shiny variant. Pick any case to display an owned variant. Empty cases fill automatically as cards arrive; existing choices stay yours.

Sell spare cards individually or with **Sell extras**. Keep at least one of each normal/shiny variant. Sale values: Common 2, Uncommon 5, Rare 12, Epic 35, Mega Rare 100; shinies sell for 5× those amounts.

Existing saves migrate automatically, keeping coins, cards, records, cases and statistics. A previously purchased five-card pack still reveals all five paid-for cards; only new purchases change to one card. Saves remain under the original browser storage key. Hosted and downloaded versions have separate browser storage: use **Options → Download save backup / Restore a save file** to move progress. Saving unavailable warnings recommend a backup. The game has no real-money purchases or player-to-player exchange.

## Source and preservation

`seagomon-original.html` is the unchanged uploaded attachment, SHA-256 `28ef248159a27871b1990ee0c73840554528e8aa6a9e2ce44b33477237ca5248`.

`seagomon-trading-before-200.html` preserves the unchanged first illustrated 100-card edition, SHA-256 `724cf8634b401bd28452d3a3afb7fa92393e0a247524319e9d2c988052753ff2`.

`seagomon-trading-before-illustrated.html` preserves the last pixel-art trading edition unchanged, SHA-256 `b1e7f4f019a381349d2f3e5f56df450225d1cc6afdc6f5d9f6fdf55d4f1770f6`.

Download/open `download-backup.html` and click its ZIP button for the self-contained game, all three preserved HTML files, editable modules, all artwork and test reports. In the extracted `source` folder, `python build.py` rebuilds the same HTML; `npm ci` then `npm test` runs the simulations. The Python build regenerates the embedded image module from the included WebP atlases using only the Python standard library; no image editor is needed. Artwork is stored once inside the supplied offline HTML. The first source build extracts all20 editable WebP atlases from that HTML and recreates `illustrations.js` automatically. Keep the extracted `source` folder beside the included game HTML. `node build-catalog.mjs` regenerates the 200-card catalogue from the original catalogue data and all three new-monster data files. Full-resolution generated masters remain in the development checkout; the editable source backup contains every optimized artwork atlas inside the self-contained game, with automatic extraction for editing.

## Verification

Core rules, probability sampling, save migration and DOM interaction simulations pass; all 200 paintings were visually inspected as images. Browser-control tooling is unavailable in this session. No real-browser layout/animation inspection, native fullscreen/download test or manual pupil playthrough is claimed. See `TESTING.md` for scope and limits.
