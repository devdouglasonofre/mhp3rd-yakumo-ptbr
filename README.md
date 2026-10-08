# mhp3rd-yakumo-ptbr

A Brazilian Portuguese translation pack for [Yakumo](https://github.com/TeamGDB/Yakumo), the native port of *Monster Hunter Portable 3rd HD Ver.*

**V1.0.** The pack has 17,639 translated strings across the 23 text blocks Yakumo supports (five more blocks in the file are not applied). It covers menus, items, equipment, the save/load screen, NPC dialogue and the quests. Most of it was machine-translated (Gemini) against a hand-checked glossary, with manual fixes for field limits and terminology. **It has not been fully proofread:** wording and terminology may be wrong or inconsistent, and a long name or description can still overflow the game's fixed UI fields.

## Download and install

Download `pt-BR.lang` from [Releases](../../releases), or take `translations/pt-BR.lang` from the revision you want to test.

In a Yakumo build with the text-translation mechanism, open **System → Text → Import translation…**, pick the file, select **Português (Brasil)** under **Game text language**, then restart the game. You can also drop the file into the per-user `translations` folder by hand.

## Compatibility

- Requires Yakumo with the text-translation mechanism (PR [#227](https://github.com/TeamGDB/Yakumo/pull/227), merged; merge commit `50482f9`).
- Built and tested against the **English-patched** `NPJB-40001` image. The quest keys are file offsets from that image; the original Japanese image's offsets differ and were not tested.
- Windows was tested. Linux / Steam Deck, macOS and Android were not.

## Checks and status

Done:

- Field-size pass: item names capped at 15 characters; dialogue, menu and quest text wrapped to the source's line count and width.
- In-game, Windows, English-patched image: item shop, smithy, character select, the village and Guild Hall quest lists and details, and an active quest — all translated on the first display, with no rendering issues, corruption or stalls.
- The quest text-latency regression found during review was fixed in PR #227.

Not done:

- Full human proofreading.
- Proof that every string fits its field.
- Platforms other than Windows, and the original Japanese image.
- Downloadable / DLC quests and mod-provided language layers.

## License

Original translation contributions are provided under MIT. No game files are included; the license grants no rights to the original game's content.
