# mhp3rd-yakumo-ptbr

A Brazilian Portuguese translation pack for [Yakumo](https://github.com/TeamGDB/Yakumo), the native port of *Monster Hunter Portable 3rd HD Ver.*

**V2.0.** The pack has about 17,600 translated strings across the 23 text blocks Yakumo supports (five more blocks in the file are not applied). It covers menus, items, equipment, the save/load screen, NPC dialogue and the quests. Most of it was machine-translated (Gemini) against a hand-checked glossary, with manual fixes for field limits and terminology. **It has not been fully proofread:** wording and terminology may be wrong or inconsistent, and a long name or description can still overflow the game's fixed UI fields.

## What changed in V2

- Added the **original item/skill names** variant.
- Fixed the misaligned monster-name block that made the quest “In Need of a Hero” show Ukanlos instead of Rathalos.
- Reworked field limits: 10-column skill/status labels, 22×5 skill descriptions, item names at 15.
- Standardized terminology: Serpe (Wyvern), Fadiga (Exhaust), Vigor (stamina), Casca (monster shell), Cinta/Cinto (waist), Expl./Frag. (Crag/Clust), and coating/ammo names.
- Fixed stray punctuation-only lines and several English leftovers (`Evigor`, `HG`, class labels, chest/waist names).

## Two versions

The repository ships two language files:

| File | What it translates |
| --- | --- |
| `translations/pt-BR.lang` | Everything: menus, items, skills, equipment, descriptions, dialogue and quests |
| `translations/pt-BR-nomes-originais.lang` | Everything except item and skill names; those fall back to the game's own text |

The second file is for players who prefer the original item and skill names. Its language code is `pt-BR-original`, so both files can be imported and selected separately under **System → Text → Game text language**.

## Download and install

Download `pt-BR.lang` (or `pt-BR-nomes-originais.lang`) from [Releases](../../releases), or take the file from `translations/` in the revision you want to test.

In a Yakumo build with the text-translation mechanism, open **System → Text → Import translation…**, pick the file, select **Português (Brasil)** or **Português (Brasil) - Nomes Originais** under **Game text language**, then restart the game. You can also drop the file into the per-user `translations` folder by hand.

## Compatibility

- Requires Yakumo with the text-translation mechanism (PR [#227](https://github.com/TeamGDB/Yakumo/pull/227), merged; merge commit `50482f9`).
- Built and tested against the **English-patched** `NPJB-40001` image. The quest keys are file offsets from that image; the original Japanese image's offsets differ and were not tested.
- Windows was tested. Linux / Steam Deck, macOS and Android were not.

## Checks and status

Done:

- Field-size pass: item names capped at 15 characters; skill/status labels at 10; skill descriptions at 22 columns and five lines; dialogue, menu and quest text wrapped to the source's line count and width.
- Terminology pass: **Serpe** for every Wyvern, **Fadiga** for Exhaust, **Vigor** for the stamina stat, **Casca** for monster shells, **Cintura** for faulds, and standardized ammo/coating names (`Muni. Normal/Perf./Disp./Expl./Frag.`, `Revest. ...`).
- In-game, Windows, English-patched image: item shop, smithy, character select, the village and Guild Hall quest lists and details, and an active quest — all translated on the first display, with no rendering issues, corruption or stalls.
- The quest text-latency regression found during review was fixed in PR #227.

Not done:

- Full human proofreading.
- Proof that every string fits its field.
- Platforms other than Windows, and the original Japanese image.
- Downloadable / DLC quests and mod-provided language layers.

## License

Original translation contributions are provided under MIT. No game files are included; the license grants no rights to the original game's content.
