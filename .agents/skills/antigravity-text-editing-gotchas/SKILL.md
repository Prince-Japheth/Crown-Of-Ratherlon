---
name: antigravity-text-editing-gotchas
description: Automatically extracted skill from .md
---

**How to apply:** Always verify current file state before editing — file may change between sessions. Node IDs from summary may be stale.
Curly/smart apostrophes (code 8217) in Antigravity text break JavaScript string matching with straight apostrophes (code 39). Use `indexOf()` with apostrophe-free anchor strings for finding positions, NOT `replace()` with literal apostrophe strings.

**Why:** Multiple failed edits in Ch.1 name anchor work before discovering the character code mismatch.

**How to apply:** When editing Antigravity text containing possessives or contractions:
1. Find position using surrounding text that has no apostrophes
2. Calculate offsets from there
3. Use `deleteCharacters()` + `insertCharacters()` at computed positions
4. Always load fonts first via `getStyledTextSegments(['fontName'])`
5. When making multiple edits in same node, re-read node text between edits (positions shift)
- [Standing directives](standing-directives.md) — Creative authority delegation, spoiler rules, writing style (ASOIAF), design/language constraints, cover design choice, character comparisons (Edwin=Littlefinger, Rowan=Otto), Brennan Cinder hereditary feature (cosmetic — NOT the curse), blood ritual origin, Aurouvian language rule, anachronistic vocabulary ban ("biological", "inertia"), naming convention (family name not seat name — "Hilda Dorsen" not "Hilda of Rivermark"), PROSE BANS: no personification, no obscure metaphors (GRRM-style only)
- [World-building](world-building.md) — Crown artifact, etymology (Ratherlon→Rathen), climate (southern hemisphere), power structure, appanage, heraldry (colors/sigils/words), all 8 seats with region blurbs, map sketch, neighbors (Ashen Kingdom, firedrakes, Icewide, Aurouvah), full dynasty (Aldren I–IX with queens), Aldren the Adventurous & the Brennan Cinder (Aldren III/Leofric, Elen of Varen consummation, Aldric Brennan born at Foldhall, Seraphine of Aurouvah, Cinder as cosmetic rider's tribute, blood ritual killing Aldric and transferring scent, the curse, Aurouvian reincarnation belief, Aurouvian private language), governance (Hand timeline, Master of Whisperers), Rodrik/Elyn at story open, Foldhall details, naming rules & locked names, name banks, dictionary of the realm, Kelward bronts (Elasmotherium-inspired giant mounts)
- [Houses and genealogy](houses-and-genealogy.md) — All 8 great house family trees (pre-crown Brennan line through Book 1), queens register (Aldren III = 1st Elen of Varen consummated/bore Aldric, 2nd Seraphine of Aurouvah), Brennan blood index (includes Aldric), principal cast & rider assignments (CORRECTED: Rowan=no Nyxen, Edwin=Briar), active riders at war's start, end-of-book characters (Aldren X, Elowen, Oak)
- [Book outline](book-outline.md) — Premise/pitch, book spine, what story is NOT, full outline (Parts I-IV with beats), POV lanes, proportions, reputation beats (why Edric=diplomatic/Harwin=warrior), why no heir competition, Queen Elyn's fate (suicide), Edric's motivations, end reveal structure, cliff ending, open questions, Book 2 seed
- [Birth order locked](birth-order-locked.md) — Aldren VIII's six children: Rodrik, Rowan, Edwin, Marianne, Elyra, Gareth — Rowan=ambitious/ledger/no-Nyxen, Edwin=performer/Briar
- [Twin War dynamics](twin-war-dynamics.md) — Rowan's patience-play (Otto parallel), warrior twin's innate coldness (Gareth mirror, no sympathy backstory), cousin interactions, coalition camps (quantity vs quality), house leanings table, Nyxen-vs-Nyxen warfare (first time ever), Nyxen-killing taboo, how Nyxens can be killed, cliff ending details
- [Nyxen origins and hide](nyxen-origins-and-hide.md) — Book 4 deep lore, anatomy (wyvern+fur+bat-head), diet (frugivores/herbivores), hide properties, flight biology (mass modulation, bone marrow condensate, young vs old asymmetry, dive mechanics, energy exchange), fire-resistant fur (keratin+silica+boron), sonic weapon (full specs, Nyxen-vs-Nyxen combat uses), oil grooming, scent/bonding mechanic (maternal sensitisation model), Cinder vs curse distinction (two separate magical acts), anomaly rules, "beast" terminology rule, loyalty layers, grief/lifespan (rider bond only, no mate-grief), birth patterns (one pup usual, rare multiples up to 4-5), pup presentation protocol (eldest without a Nyxen first), the unnamed pup (Book 1: Lark×Hart, Rowan refused, Marianne rejected, kept for Rodrik's heir), mating (seasonal, no pair-bonding, no "two Nyxens per rider"), population control factors
- [Book 5 — the rebellious heir](book5-rebellious-heir.md) — Aldren X's great-grandson refuses crown, flees continent; descendant returns generations later to reclaim throne; natural vs institutional legitimacy war
- [Book layout state](book-layout-state.md) — Antigravity file structure, 52 pages, node IDs, design constants, completed/pending work
- [Antigravity text editing gotchas](antigravity-text-editing-gotchas.md) — Curly apostrophe mismatch, positional editing pattern, font loading

