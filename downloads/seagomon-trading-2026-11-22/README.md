# Seagomon: The Trading Game

A times-table speed game with Seago Coins, five-card packs, 100 collectible monsters and a shiny variant of every card. Built on 22 November 2026 from the supplied Seagomon HTML.

## Play

Use the hosted game, or download `seagomon-trading-game.html` and open it in a current desktop browser. On GitHub, choose **Download raw file**. The new game is self-contained and works offline; it makes no image, font, Firebase or other game-data requests.

The main screen puts four editable display cases, all eleven tables and the pack shop on one dashboard. It is designed for 1024×768 and 1366×768 laptop viewports at normal zoom, with a scrolling fallback for smaller screens. Collection and shop dialogs may scroll internally.

## Speed runs and records

Choose a table from 2 to 12, then Start clock. Complete all twelve facts, multiplying by 1 through 12. Type each answer and press Enter. A mistake does not advance the question; time keeps running until corrected. There is no fixed time limit.

| Tables | Table coin multiplier |
|---|---:|
| 2,5,10 | 1× |
| 3,4,9,11 | 2× |
| 6,7,8,12 | 3× |

In order adds 1×; shuffled adds 2×. A completed run earns `30 × table multiplier × order multiplier` coins. The first clear of each table/order adds one base reward. Beating an existing personal best adds three base rewards. Thus an easy ordered first clear pays 60 coins, and a later 23.00s→22.00s record pays 120 coins (30 base + 90 bonus).

There are 22 independent saved records. Times are rounded upward to the next hundredth of a second for both display and comparison, so a displayed tie cannot secretly earn a record bonus. Closing/reloading an unfinished run gives no reward; repeated final submissions cannot duplicate a payment.

## Pack shop and odds

| Pack | Cost | Cards | Common | Uncommon | Rare | Epic | Mega Rare |
|---|---:|---:|---:|---:|---:|---:|---:|
| Normal | 60 | 5 | 60% | 25% | 11% | 3.5% | 0.5% |
| Lucky | 120 | 5 | 35% | 32% | 24% | 8% | 1% |
| Shiny | 900 | 5 | 45% | 30% | 18% | 6% | 1% |

These are rarity chances **per card**, with replacement. Each species within a rarity is equally likely. Normal cards have a 2% shiny roll; Lucky cards 4%. A Shiny pack guarantees one randomly chosen shiny slot, with 4% shiny rolls for the other four. The guaranteed shiny can be any rarity; it does not guarantee a Mega Rare.

The shop shows rarity odds and at-least-one-in-pack probabilities. Individual collection pages show each normal/shiny variant's exact pack chances. A purchase saves its coin charge, all five cards and pending reveal together before the animation. Reloading resumes that pack without charging or awarding again. Finish a pending pack before another purchase or sale.

## Collection and display cases

The catalogue has 40 Common, 30 Uncommon, 18 Rare, 9 Epic and 3 Mega Rare cards. There are 100 base species and 100 shiny variants. All 60 monsters from the attachment are retained, plus 40 new designs. Four original elite monsters shared an identical sprite; each gained distinct features while preserving original pixels. Some other original palette variants retain related silhouettes. All 100 full-color card artworks are distinct; all 40 new monster silhouettes are distinct.

Choose any case to pick an owned normal or shiny card. The first pack fills empty cases with its best finds; your later choices are not overwritten. A card can also be assigned to any case from its detail page.

Sell extra copies individually or use **Sell extras**. One copy of each normal/shiny variant is always kept. Values per spare copy: Common 2, Uncommon 5, Rare 12, Epic 35, Mega Rare 100; shiny copies are worth five times that. Displayed cards remain owned after sales.

## Saved progress

Coins, records, cards, display choices and pending packs save in this browser on this device. The hosted game and a downloaded file have different browser storage. Use **Options → Download save backup**, then Restore a save file in the other copy to move your collection. If storage is unavailable, the game continues in memory and clearly recommends a backup.

Sound and fullscreen are optional under Options. Reduced-motion preferences disable decorative animations. The game has no account, multiplayer exchange or real-money purchases.

## Source and untouched original

`seagomon-original.html` is the supplied attachment, byte-for-byte unchanged (SHA-256`28ef248159a27871b1990ee0c73840554528e8aa6a9e2ce44b33477237ca5248`). Its external services are separate from this new game.

Download/open `download-backup.html`, then click **Download source backup ZIP** for the current game, original attachment, editable modules and test reports. Rebuild with `python build.py` in the extracted `source` folder. Playing needs no installation. In that same `source` folder, `npm ci` installs the DOM-test dependency and `npm test` runs the suites after rebuilding.

## Verification limits

Core and independent probability/economy simulations pass, as do DOM integration simulations using jsdom. Artwork was XML-checked and its contact sheets visually inspected. The supported cloud browser-control tool was unavailable, so **no real browser interaction, rendered dashboard layout, native fullscreen/download flow or manual pupil playtest was completed**. Main-screen fit is a design target rather than a browser-measured result. See TESTING.md and reports for exact scope.
