# Changelog

All notable changes to the DominoGue.

## v0.19.0-beta — 2026-07-16
### Changed
- **Official studio splash.** Boot now opens on the real Devious Developments logo art —
  the horned D/D mark with "DEVIOUS DEVELOPMENTS · PRESENTS" — replacing the earlier
  code-drawn wordmark. Same timing, still click-to-skip.

## v0.18.0-beta — 2026-07-15
### Added
- **Free browser demo.** The itch.io browser edition is now a **demo** — it plays through **Act 1**
  (up to and including the first Warden, the Tallyman) with the Warrior, Mage, and Gambler, then invites
  you to the full game. The **full game** is available to purchase on itch.io (Windows download, no key),
  or here on GitHub with a product key.

## v0.17.0-beta — 2026-07-14
### Added
- **Product-key activation (Windows).** The desktop build now activates with a **product key** on
  first launch — one online check, then the license verifies **offline** on every launch after.
  Boot flow is now splash → activation → game. The **browser edition on itch.io needs no key.**
- **Single self-contained `DominoGue.exe`.** The game data is now embedded in the exe (no loose
  `.pck` to keep alongside it) and its scripts are **encrypted** in the Windows build.
### Fixed
- **Blank grey screen after activation.** The license gate now defers the scene change to the next
  idle frame, so the game reliably loads past the activation/passthrough step instead of stalling
  on a blank screen (most visible on the browser build).
- **Emoji icons now render everywhere.** Bundled a colour emoji font as a global fallback so the
  in-game icons (♟ 🎯 🗺 ✨ 💎 …) display correctly on the browser build — which has no system
  emoji font to borrow — and consistently on Windows.

## v0.16.0-beta — 2026-07-14
### Added
- **Studio splash screen.** Launch now opens with a two-stage intro — the hand-drawn
  **Devious Developments** wordmark (devil-horned D's, drawn entirely in code) fading into the
  **DominoGue** title, then straight into the game. Click or press any key to skip.
- **Web build.** DominoGue now has an **HTML5 / browser** edition on **itch.io** — playable in any
  modern desktop browser, no download.

## v0.15.0-beta — 2026-07-13
### Added
- **Full audio.** The House of Bones has a voice — a complete music & sound pass across the game.
- **Music** — a dark-fantasy **main-menu / hub theme**, **five battle tracks** (one picked at random
  each match), and a dedicated **shop theme** that fades in behind the door-bell. Tracks crossfade on
  every scene change.
- **Sound effects** — a looping bonfire crackle, the Blacksmith's anvil on each upgrade, a shop door
  chime, **victory** & **defeat** stings, **trophy-unlock** and **level-up** chimes, a **treasure**
  reveal, and a game-feel layer on button clicks, domino placement, purchases, and damage.
- **Volume settings** — separate **Music** and **Sound-effects** sliders in Settings, saved to your profile.

## v0.14.0-beta — 2026-07-13
### Added
- **Achievements & the Trophy Room.** 25 trophies across five categories (Combat · Mastery ·
  Collection · Story · Challenge), each with a reward that **persists across every future run**.
  19 give small permanent buffs — collect them all for **+4 STR / +3 WIS / +3 LUCK / +2 FOR /
  +3 VIT / +8 max HP / +25 starting gold**. Track everything in the new **Trophy Room** off the
  main menu.
- **6 content unlocks** behind marquee trophies: **Heirloom** (start every run with a free Common
  relic), a secret **Mythic relic**, a golden **Gilded Bones** domino skin, an **Obsidian** table
  theme, a secret **Legendary boon**, and **Ascension Mode**.
- **Ascension Mode** — an unlockable harder run: tougher foes and bosses for **+50% coins and bonus
  XP**. Toggle it on the class screen once you've earned it.
- **Unlock toasts** — a 🏆 pops on-screen the moment you earn a trophy.
- **Cosmetics** — the Gilded Bones domino skin and the Obsidian table theme, switchable in the Trophy Room.

## v0.13.1-beta — 2026-07-12
### Fixed
- **Battle screen** — reverted the player's HP bar and character info to their original
  top-of-screen layout (the lower-left placement from v0.13.0 looked off).

## v0.13.0-beta — 2026-07-12
### Added
- **Story mode — *The House of Bones*.** Climb the Stack while the Dealer narrates every stair.
  Each act ends with a **Warden**; beating one drops a **Memory Shard** of your past — five per
  class, each a different soul's arc. The **Vault** at floor 50 is the final hand and a **choice
  of two endings**.
- **Pre-battle cutscenes** — every opponent gets an intro (portrait, name, taunt); Wardens get a
  heavier framing from the Dealer.
- **Mythic rarity** — a new top tier above Legendary, with Mythic gear and relics in every slot.
- **Starting gear** — each class now begins a run wearing a themed set of Common armor across all
  six slots.
- **Boss armor** — bosses wear their own armor sets that scale with your depth (opening ward pool,
  ward each turn, and bonus damage).
- **Shop services** — **Mystery Box** (random reward), **Tome of Power** (raise a stat), and
  **Reforge** / **Cleanse** (reroll or wipe a domino's enchants).
- **Treasure variety** — chests can now heal you, grant a stat, or bind a free enchant to one of
  your dominoes, alongside relics, coins, and the occasional trap.
- **Quit a run** — abandon back to the menu from a battle's pause overlay or the path fork.
### Changed
- **Powerups replaced by a Boon / Doom system.** Every domino can carry a **boon** (helps you when
  you play it) and a **doom** (hurts the AI when it plays it); both fire on any play and **double
  when that play scores**. Tiles show both badges.
- **Rarities renamed** Normal → **Common** — the ladder is now Common → Rare → Epic → Legendary →
  **Mythic**.
- **Character panel** moved to a clean lower-left column (portrait, HP, stats, relics, gear).
- **Wardens are consistent** — each act's boss face now matches its story (the Tallyman, the
  Duchess, the Iron Matron, Grandmaster Six, and the Bonelord in the Vault).
### Fixed
- **Fixed a hard soft-lock** — enchanting a domino can no longer strand a run; every tile is a
  valid target and you can always skip.

## v0.12.0-beta — 2026-07-12
### Added
- **Persistent progression** — characters keep their **levels and stat points between runs**,
  saved to your PC. Two new souls unlock as your combined level climbs: the **Oracle** at 100 and
  the **Spy** at 250.
- **Respec** — reallocate a character's stat points anytime from the class-select screen.
- **Settings menu** — including a **Reset Progress** option.
- **LUCK stat + critical hits** — LUCK raises crit chance *and* loot rarity; Strength sharpens how
  hard crits land. New luck/crit relics and gear.
- **The Blacksmith** — a room dedicated to upgrading equipment (moved out of the shop).
### Improved
- **Character portraits** for every class and enemy, on class-select and in battle.
- **Themed art** on every non-battle screen (forge, bonfire, shop, treasure vault, stairwell…).
- **Shop** organised into categories with item icons; you can now sell relics, and sold items
  leave the list.
- **Board** — doubles (including on spinner arms) sit sideways correctly, long boards stay readable
  with a camera that follows your play, and drop zones sit on the actual open ends.

## v0.11.1-beta — 2026-07-11
### Fixed
- **Shop now scrolls** — a stocked shop (with upgrade/sell rows) no longer overflows the screen.

## v0.11-beta — 2026-07-11
### Added
- **Equipment & inventory** — armor now lives in six slots (helmet, necklace, chest, gloves,
  ring, boots) on a paper-doll. Click a slot to open your inventory and swap gear; only the
  piece equipped in a slot counts toward your stats.
- **Icons + tooltips** — relics and armor show as icons; hover any of them for the full name,
  rarity, level, and effect.
- **Sell gear in shops** — offload duplicate, old, or downgraded items for coins.
- **Prettified stat panel** — STR / VIT / FOR / WIS (and MAG when magic is active) as clean,
  colour-coded chips.
### Changed
- **Armor pool reorganised by slot**, with magic and offensive pieces to build around.

## v0.10-beta — 2026-07-11
### Added
- **Character stats** — STR / VIT / FOR / WIS. Strength adds damage, Vitality adds max HP,
  Fortitude reduces incoming damage, Wisdom powers magic. Each class starts with its own spread.
- **XP & leveling** — win battles to earn XP; every level lets you raise a stat of your choice.
- **Magic** — Wisdom fuels a *separate extra attack* on every scoring play, but only while you're
  carrying magic items — a genuine build path rather than a flat bonus.
- **Upgradable armor** — spend coins in the shop to level up the armor pieces you own.
- **Bigger item pool** — 25 relics & armor sets, including stat relics, three magic relics, and a
  legendary that boosts every level-up.
- **Battle loadout panel** — your live stats, relics, and armor (with levels) shown beside the table.
- **Drag-and-drop placement** — drag a tile from your hand onto the board; each open end lights up
  **green** (playable) or **red** (not). Clicking still works too.
- **Shop reroll** — reroll the stock for a coin cost that climbs with each reroll.
### Changed
- **Bosses are now scheduled** — a forced boss every 10 rooms instead of appearing at random.
- **Rooms don't repeat** — leaving a treasure, bonfire, or shop locks it until your next battle.
- **New main menu** — the two O's in DOMINOGUE are rocking domino tiles.

## v0.9.1-beta — 2026-07-11
### Added
- **In-game "How to Play"** tutorial on the main menu (goal, All-Fives scoring, doubles & the
  spinner, going out, the path fork, relics & rarity, classes).
### Fixed
- **Wards now build every turn and stack all match** (Mage + armor sets were only granting once
  per hand, so shields never accumulated).

## v0.9.0-beta — 2026-07-11
### Added
- **Roguelike run structure** — class → battle → reward → **pick 1 of 2 paths**
  (Battle · Shop · Treasure · Bonfire · Boss).
- **Persistent HP** between battles; **Bonfires** fully restore it.
- **Relics & armor sets** across four rarities (Normal / Rare / Epic / Legendary) with
  tier-scaled bonuses and rarity-weighted drops.
- **Shop** (powerups, relics, armor, heals), **Treasure** events (boon or bane), and **Boss**
  fights with enemy boons + a free relic reward.
- **Named opponents** with pre-battle taunts and per-enemy table colours.
- **Scoring HUD** ("Board ends: N → scores M"), live enemy tile count, and a domino-out reveal
  of the loser's remaining tiles.
- **Branding** — app icon, boot splash, and window/exe icon; standalone Windows build.
### Changed
- **Spinner scoring** reworked: a double counts both pips while open and **zero once closed**;
  the spinner's side branches open only after both of its line ends are filled.
