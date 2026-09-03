# Changelog

Todos los cambios notables de Mystical Realms Translation & Fixes se documentan en este archivo.

El formato sigue [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)
y el proyecto adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.0-beta.3] - 2026-09-03

### Añadido

- **Traducciones al español (`es_es`) para 3 namespaces más** (~520 claves), tomando como origen el
  `en_us.json` de cada mod. Cierra los huecos de traducción reales detectados en el snapshot del
  modpack v5.134.4 (`docs/SNAPSHOT_MODPACK_5.134.4.md`):
  - `apothic_enchanting` (Apothic Enchanting 1.6.2) — 425 claves. Nombres de bloques (estanterías
    Hellshelf/Seashelf/Deepshelf/Endshelf…), GUI de la mesa de encantamientos, tooltips y descripciones.
    Los nombres propios del sistema de Apotheosis (`Eterna`, `Quanta`, `Arcana`) y los numerales
    romanos de nivel se mantienen sin traducir.
  - `apothic_spawners` (Apothic Spawners 1.4.0) — 89 claves. Estadísticas de generador, tooltips y el
    encantamiento *Capturing*.
  - `placebo` (Placebo 9.9.2) — 6 claves (comandos y toggles cosméticos de mecenas).
- Total del pack: **104 namespaces**, ~13k claves.

### Notas

- El snapshot `docs/SNAPSHOT_MODPACK_5.134.4.md` marcaba como huecos otros mods que tras verificación
  jar a jar **no lo son**: `embeddium_extra` empaqueta su texto bajo el namespace `sodium-extra` (ya
  traducido); `integrated_cataclysm`, `integrated_villages` y `waystone_towers` traen `en_us.json`
  vacío o ningún `lang/`; `attributefix` y `utility_nexus_fixes` no tienen archivos de idioma. Sin
  cadenas que traducir en ninguno.

## [0.1.0-beta.2] - 2026-09-03

### Añadido

- **Fixes de guías Patchouli** — sobrescribe 3 entradas de libro de mods incluidos que
  referencian recetas inexistentes (spam `Recipe X not found` en el log del cliente, la
  página del libro salía sin la receta):
  - `butchery` · `butchers_guide/blocks/butchers_table` — `butchery:crimnsonbutcherstablerecipe`
    → `butchery:crimsonbutcherstablerecipe` (errata en el propio libro); `jungle:acaciabutcherstablerecipe`
    → `butchery:junglebutcherstablerecipe` (namespace y nombre erróneos).
  - `butchery` · `butchers_guide/resources/dragon_scale` — la página era `patchouli:smithing`
    pero `dragonscaleingotrecipe` / `dragonscaleblockrecipe` son `minecraft:crafting_shaped`;
    cambiada a `patchouli:crafting`.
  - `irons_spellbooks` · `iss_guide_book/progression/late_game` — `irons_spellbooks:cryomancer_helmet`
    / `pyromancer_helmet` → `..._helmet_crafting` (los ids reales llevan sufijo `_crafting`).
- `apotheosis` · `apoth_chronicle` referencia `minecraft:bookshelf` (receta vanilla válida y
  crafteable in-game): **no se toca**, es ruido de orden de carga de Patchouli, no un fallo del libro.

## [0.1.0-beta.1] - 2026-09-03

### Cambiado

- **Proyecto renombrado** de *Mystical Realms Resource Pack* a **Mystical Realms Translation & Fixes**
  (slug `mystical-realms-translation-fixes`) por políticas de CurseForge. El `project_id` de CurseForge
  no cambia. Remote GitLab nuevo:
  `https://gitlab.com/stalking-dragons/minecraft/mystical-realms-translation-fixes.git`.
- Nombre del ZIP: `MysticalRealms_ResourcePack-*.zip` → `MysticalRealms_TranslationFixes-*.zip`.
- `pack.mcmeta`, `README.md` y la descripción de CurseForge actualizados para reflejar el nuevo alcance
  (traducciones + fixes).

### Añadido

- **Traducciones al español (`es_es`)** para **101 namespaces de mods** (~12.515 claves), tomando como
  origen el `en_us.json` de cada mod. Minecraft fusiona estos ficheros `lang` sobre lo que cada mod ya
  trae, así que en los mods con `es_es` parcial solo se añaden las claves que faltaban.
  - **59 mods sin ninguna traducción española previa**: everycomp, butchery, mcwroofs, reliquary,
    sodium-extra (rubidium-extra), xaeroworldmap, ars_additions, toms_storage, bookshelf, modernfix,
    spell_power, bclib, caravans, farmers_sandwiches, aces_spell_utils, morevillagers, irons_lib,
    inventoryessentials, mysticalautomation, notenoughcrashes, craftingtweaks, arssophisticatedcompat,
    balm, aquaculturedelight, player_activity_view, wishfulrecipes, carry_mechanics, teleport_animation,
    worldweaver (wover / wover-generator / wover-ui), horde_hoard, justenoughbreeding, info_tab,
    better_party_x_xaeros_world_map, farmer_delight_pizza_lovers, ars_creo, cucumber, just_in_nether,
    better-villager-animations, moogs_structures, betterendisland, zeta, idas, integrated_stronghold,
    skd_menu, fusion, mes, mns, data_miner, mowzies_cataclysm, lionfishapi, common_toolkit,
    irons_patreon_lib, terrablender, dangerous, justenoughprofessions, supermartijn642corelib,
    visualworkbench.
  - **42 mods con `es_es` incompleto, completados** (nº de claves añadidas): supplementaries (+1055),
    ars_nouveau (+921), xaerominimap (+522), irons_spellbooks (+475), betterend (+367), quark (+324),
    dawnoftimebuilder (+275), waystones (+263), moonlight (+239), farmersdelight (+193), jei (+188),
    create (+178), armoroftheages (+161), enchdesc (+151), sophisticatedbackpacks (+149),
    deeperdarker (+136), biomesoplenty (+119), jade (+105), tombstone (+72), embeddium (+71),
    L_Ender's Cataclysm + integrated_cataclysm (+61), guardvillagers (+59), obscure_tooltips (+41),
    mowziesmobs (+36), aquamirae (+31), aquaculture (+30), bettercombat (+20), xaerobetterpvp (+17),
    relics (+15), sophisticatedcore (+15), vellumli (+13), regalia_slots_api (+12), iris (neoculus) (+11),
    configured (+10), mcwbridges (+6), workhand_tools (+3), ascendant_spawners (+2), ars_elemental (+1),
    jeresources (+1), mysticalagriculture (+1), naturescompass (+1), villagertradingplus (+1).

## [0.0.0-beta.1] - 2026-09-02

### Añadido

- Primera versión versionada del resource pack para el modpack **Mystical Realms** (MC 1.21.1).
- Icono del pack (`resourcepack/pack.png`, 256x256).
- **Fix Butchery `ravager_carcass`**: `assets/butchery/models/custom/ravager_carcass.json`.
  Butchery 5.2 incluye un archivo de modelo huérfano (`custom/ravager_carcass.json`, doble `s`) con una
  rotación de elemento ilegal (`angle: -90`; solo se admiten ±45/±22.5/0). No lo referencia nada, pero
  MC 1.21 carga en bloque todos los `models/**/*.json` al arrancar y registra un `ERROR` de parseo por él.
  Se sustituye por el modelo hermano ya corregido del propio mod (`custom/ravager_carcas.json`, una `s`),
  de modo que la carga tiene éxito y el log queda limpio. Sin cambios visuales in-game
  (la carcasa en el mundo usa un modelo Java por código; el ítem usa `custom/ravager_carcas`).
