# Althing Hall: Historical Source of Truth (SOT) Data
This repository contains a standardized, high-integrity collection of Old Norse historical and ritual data in JSON format. The primary goal of this project is to provide a "metal-up" foundation for developers and practitioners, strictly anchored in primary manuscript evidence.

## 🏛️ Primary Sources
Every data point in these files has been cross-referenced and pulled from the following authoritative manuscripts:

- The Prose Edda (Gylfaginning and Skáldskaparmál).

- The Poetic Edda (specifically the Völuspá, Hávamál, and Þrymskviða).

- Heimskringla (Ynglinga Saga).

- The Rune Poems (Old Icelandic, Old Norwegian, and Anglo-Saxon).

## 🛡️ File Synopses
`aesir-gods.json`

A standardized registry of the `30 Æsir` figures explicitly categorized in the `Gylfaginning`. Each entry includes the original Old Norse manuscript text, three scholarly English translations, and verified ritual associations.

`vanir-gods.json`

A strict registry of the 4 primary Vanir figures named in the SOT manuscripts: `Njörðr`, `Freyr`, `Freyja`, and `Kvasir`. This file maintains the same schema as the `Æsir` registry for seamless data mapping.

`artifacts_master_v1.json`

Contains entries for the 6 major mythic artifacts (e.g., `Mjölnir`, `Gungnir`, `Draupnir`). Unlike clinical dictionaries, this file includes `usage_roadmaps` and `practitioner_guidance` to bridge the gap between mythic lore and ritual utility.

`calendar-v3.json`

A registry of 5 historical holidays grounded in seasonal and lunisolar timing. It provides a `ceremony_roadmap` for each holiday, mapping ancient sacrificial logic to modern adaptations like "apartment-safe" or "sober-friendly" alternatives.

`elder-futhark-v3.json` & `younger-futhark-v3.json`

Separated registries for the 24 `Elder Futhark` and 16 `Younger Futhark` runes. Both includeera-appropriate Rune Poems and standardized phonetic guides.

`havamal_api_v1_gold.json`

The full text of the 164 `Hávamál` stanzas. It preserves the original alliterative meter alongside three verified translations (Bellows, Bray, and Petit).

## ⚙️ Architectural Decisions
1. Exclusion of Modern "Fixed-Date" Holidays

Most modern resources list holidays on static Gregorian dates. This registry rejects that model, instead using Lunisolar Logic (e.g., "Full Moon of the fourth winter month") to align with the historical timing described in the `Ynglinga Saga` and `Orkneyinga Saga`.

2. Strict Pantheon Counts

To maintain academic integrity, figures were only included if the SOT manuscripts explicitly defined them as part of a specific pantheon.

- The Æsir (30): Includes the full list of goddesses from the Gylfaginning often omitted by other resources.

- The Vanir (4): Limited to the core family and the emissary Kvasir. Figures like Gerðr (a Jötunn) were excluded to prevent "lore bloat".

3. Inclusion of Practitioner Guidance

Artifact entries include a practitioner_guidance object to solve common "bottlenecks" in modern practice. This allows users to access the Logic of the Tool (e.g., using the Hammer Sign to hallow a space) even if they do not possess physical, museum-quality replicas.

## 🏺 Developer Note
The total footprint of these registries is approximately ***262 KB***, optimized for local-first storage and high-performance rendering on the end-user's device.

















