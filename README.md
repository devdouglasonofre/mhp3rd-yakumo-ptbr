# mhp3rd-yakumo-ptbr

Tradução para português do Brasil do [Yakumo](https://github.com/TeamGDB/Yakumo), o port nativo de *Monster Hunter Portable 3rd HD Ver.*

---

## Português (Brasil)

**V2.0.** O pacote tem cerca de 17.600 textos traduzidos nos 23 blocos de texto que o Yakumo suporta (outros cinco blocos no arquivo não são aplicados). Ele cobre menus, itens, equipamentos, tela de salvar/carregar, diálogos de NPCs e missões. A maior parte foi traduzida automaticamente (Gemini) com um glossário revisado à mão, mais ajustes manuais de limite de campo e terminologia. **A tradução não passou por revisão humana completa:** pode haver erros de redação ou inconsistências, e um nome ou descrição longa ainda pode estourar o campo fixo da interface.

### O que mudou na V2

- Adicionada a variante que mantém **nomes de itens e skills no original**.
- Corrigido o bloco de nomes de monstros que fazia a missão “Precisa-se de Herói” mostrar Ukanlos em vez de Rathalos.
- Limites de campo refeitos: rótulos de skill/status em 10 colunas, descrições de skill em 22×5 e nomes de itens em 15.
- Terminologia padronizada: **Serpe** (Wyvern), **Fadiga** (Exhaust), **Vigor** (stamina), **Casca** (Shell de monstro), **Cinta/Cinto** (cintura), **Expl./Frag.** (Crag/Clust) e nomes de munições/revestimentos.
- Corrigidas linhas com pontuação sozinha e sobras de inglês (`Evigor`, `HG`, rótulos de classe, nomes de peitorais e peças de cintura).

### Duas versões

O repositório traz dois arquivos de idioma:

| Arquivo | O que traduz |
| --- | --- |
| `translations/pt-BR.lang` | Tudo: menus, itens, skills, equipamentos, descrições, diálogos e missões |
| `translations/pt-BR-nomes-originais.lang` | Tudo, exceto nomes de itens e skills; esses caem no texto original do jogo |

O segundo arquivo é para quem prefere os nomes originais de itens e skills. O código de idioma dele é `pt-BR-original`, então os dois podem ser importados e escolhidos separadamente em **System → Text → Game text language**.

### Download e instalação

Baixe `pt-BR.lang` (ou `pt-BR-nomes-originais.lang`) em [Releases](../../releases), ou pegue o arquivo em `translations/` na revisão que quiser testar.

Em um build do Yakumo com o mecanismo de tradução de texto, abra **System → Text → Import translation…**, escolha o arquivo, selecione **Português (Brasil)** ou **Português (Brasil) - Nomes Originais** em **Game text language** e reinicie o jogo. Você também pode colocar o arquivo manualmente na pasta `translations` do diretório de dados do usuário.

### Compatibilidade

- Requer um Yakumo com o mecanismo de tradução de texto (PR [#227](https://github.com/TeamGDB/Yakumo/pull/227), já mesclado; merge commit `50482f9`).
- Construído e testado com a imagem **NPJB-40001 com patch em inglês**. As chaves das missões são offsets daquela imagem; os offsets da imagem japonesa original são diferentes e não foram testados.
- Windows foi testado. Linux / Steam Deck, macOS e Android não foram.

### Verificações e status

Feito:

- Passe de limites de campo: nomes de itens em até 15 caracteres; rótulos de skill/status em 10; descrições de skill em 22 colunas e cinco linhas; diálogos, menus e missões quebrados conforme o número de linhas e a largura da fonte.
- Passe de terminologia: **Serpe** para todo Wyvern, **Fadiga** para Exhaust, **Vigor** para stamina, **Casca** para Shell de monstro, **Cinta** para faulds/coat, e nomes padronizados de munição/revestimento (`Muni. Normal/Perf./Disp./Expl./Frag.`, `Revest. ...`).
- No jogo, Windows, imagem com patch em inglês: loja de itens, ferreiro, seleção de personagem, listas e detalhes de missões da vila e do Salão da Guilda, e uma missão ativa — tudo traduzido na primeira exibição, sem problemas de renderização, corrupção ou travamentos.
- A regressão de latência do texto de missões encontrada na revisão foi corrigida na PR #227.

Não feito:

- Revisão humana completa.
- Prova de que todo texto cabe no campo.
- Plataformas além de Windows, e a imagem japonesa original.
- Missões baixáveis/DLC e camadas de idioma fornecidas por mods.

### Licença

As contribuições originais de tradução são fornecidas sob MIT. Nenhum arquivo do jogo está incluído; a licença não concede direitos sobre o conteúdo original do jogo.

---

## English

**V2.0.** The pack has about 17,600 translated strings across the 23 text blocks Yakumo supports (five more blocks in the file are not applied). It covers menus, items, equipment, the save/load screen, NPC dialogue and the quests. Most of it was machine-translated (Gemini) against a hand-checked glossary, with manual fixes for field limits and terminology. **It has not been fully proofread:** wording and terminology may be wrong or inconsistent, and a long name or description can still overflow the game's fixed UI fields.

### What changed in V2

- Added the **original item/skill names** variant.
- Fixed the misaligned monster-name block that made the quest “In Need of a Hero” show Ukanlos instead of Rathalos.
- Reworked field limits: 10-column skill/status labels, 22×5 skill descriptions, item names at 15.
- Standardized terminology: Serpe (Wyvern), Fadiga (Exhaust), Vigor (stamina), Casca (monster shell), Cinta/Cinto (waist), Expl./Frag. (Crag/Clust), and coating/ammo names.
- Fixed stray punctuation-only lines and several English leftovers (`Evigor`, `HG`, class labels, chest/waist names).

### Two versions

The repository ships two language files:

| File | What it translates |
| --- | --- |
| `translations/pt-BR.lang` | Everything: menus, items, skills, equipment, descriptions, dialogue and quests |
| `translations/pt-BR-nomes-originais.lang` | Everything except item and skill names; those fall back to the game's own text |

The second file is for players who prefer the original item and skill names. Its language code is `pt-BR-original`, so both files can be imported and selected separately under **System → Text → Game text language**.

### Download and install

Download `pt-BR.lang` (or `pt-BR-nomes-originais.lang`) from [Releases](../../releases), or take the file from `translations/` in the revision you want to test.

In a Yakumo build with the text-translation mechanism, open **System → Text → Import translation…**, pick the file, select **Português (Brasil)** or **Português (Brasil) - Nomes Originais** under **Game text language**, then restart the game. You can also drop the file into the per-user `translations` folder by hand.

### Compatibility

- Requires Yakumo with the text-translation mechanism (PR [#227](https://github.com/TeamGDB/Yakumo/pull/227), merged; merge commit `50482f9`).
- Built and tested against the **English-patched** `NPJB-40001` image. The quest keys are file offsets from that image; the original Japanese image's offsets differ and were not tested.
- Windows was tested. Linux / Steam Deck, macOS and Android were not.

### Checks and status

Done:

- Field-size pass: item names capped at 15 characters; skill/status labels at 10; skill descriptions at 22 columns and five lines; dialogue, menu and quest text wrapped to the source's line count and width.
- Terminology pass: **Serpe** for every Wyvern, **Fadiga** for Exhaust, **Vigor** for the stamina stat, **Casca** for monster shells, **Cinta** for faulds/coats, and standardized ammo/coating names (`Muni. Normal/Perf./Disp./Expl./Frag.`, `Revest. ...`).
- In-game, Windows, English-patched image: item shop, smithy, character select, the village and Guild Hall quest lists and details, and an active quest — all translated on the first display, with no rendering issues, corruption or stalls.
- The quest text-latency regression found during review was fixed in PR #227.

Not done:

- Full human proofreading.
- Proof that every string fits its field.
- Platforms other than Windows, and the original Japanese image.
- Downloadable / DLC quests and mod-provided language layers.

### License

Original translation contributions are provided under MIT. No game files are included; the license grants no rights to the original game's content.
