# Seagomon: The Trading Game — Illustrated Edition

The same times-table speed game, now with 100 original painted creature scenes, one-card foil packs, rarity reveals and unlockable animated worlds. Updated 23 November 2026.

## Play

Open the hosted game, or download `seagomon-trading-game.html` and open it in a current desktop browser. On GitHub choose **Download raw file**. The HTML contains all illustrations, scenes, sounds and game code; playing offline needs no installation or network connection.

Four editable display cases, all eleven tables and the pack shop remain on the laptop dashboard. It targets 1024×768 and 1366×768 at normal zoom; smaller screens use a scrolling fallback. Dialogs can scroll internally.

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

All100 identities remain:60 creatures from the attachment and40 additions. Their old grids remain as provenance data; visible cards now use100 distinct, smooth illustrated scenes with developed creatures and rich environments. Gold-edged frames identify rarity; shiny variants use alternate colour treatment and moving foil. Ten optimized image atlases are embedded once inside the offline HTML.

Aurora Studio is available immediately. Your first purchase in this edition additionally unlocks Waterfall Sanctuary. Later packs can unlock Firefly Grove, Coral Lagoon, Ember Highlands, Starfall Observatory and Storm Summit. Normal/Lucky/Shiny background bonus chances are20%/30%/50%, choosing equally among still-locked worlds. Bonuses never repeat and stop when all six are found. A world is an extra cosmetic reward, never a second monster card. The first Waterfall equips automatically if you use the default Studio; later discoveries preserve your choice.

Choose **Options → Animated backgrounds** to equip an owned world. The dashboard layout stays the same; scenes animate behind readable translucent panels. Reduced-motion preferences stop decorative motion.

## Collection and saves

The catalogue contains40 Common,30 Uncommon,18 Rare,9 Epic and3 Mega Rare species, each with a shiny variant. Pick any case to display an owned variant. Empty cases fill automatically as cards arrive; existing choices stay yours.

Sell spare cards individually or with **Sell extras**. Keep at least one of each normal/shiny variant. Sale values: Common2, Uncommon5, Rare12, Epic35, Mega Rare100; shinies sell for5× those amounts.

Existing saves migrate automatically, keeping coins, cards, records, cases and statistics. A previously purchased five-card pack still reveals all five paid-for cards; only new purchases change to one card. Saves remain under the original browser storage key. Hosted and downloaded versions have separate browser storage: use **Options → Download save backup / Restore a save file** to move progress. Saving unavailable warnings recommend a backup. The game has no real-money purchases or player-to-player exchange.

## Source and preservation

`seagomon-original.html` is the unchanged uploaded attachment, SHA-256 `28ef248159a27871b1990ee0c73840554528e8aa6a9e2ce44b33477237ca5248`.

`seagomon-trading-before-illustrated.html` preserves the last pixel-art trading edition unchanged, SHA-256 `b1e7f4f019a381349d2f3e5f56df450225d1cc6afdc6f5d9f6fdf55d4f1770f6`.

Download/open `download-backup.html` and click its ZIP button for the self-contained game, both preserved HTML files, editable modules, optimized illustration assets and test reports. In the extracted `source` folder, `python build.py` rebuilds the same HTML; `npm ci` then `npm test` runs the simulations. `python build-illustrations.py` regenerates the embedded image module from the included WebP atlases when ImageMagick is installed. Full-resolution generated masters remain in the development checkout; the editable source backup includes the optimized art used by the game.

## Verification

Core rules, probability sampling, save migration and DOM interaction simulations pass; all100 paintings were visually inspected as images. Browser-control tooling is unavailable in this session. No real-browser layout/animation inspection, native fullscreen/download test or manual pupil playthrough is claimed. See `TESTING.md` for scope and limits.
