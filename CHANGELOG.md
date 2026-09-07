# Changelog

Todos los cambios notables de Mystical Realms Translation & Fixes se documentan en este archivo.

El formato sigue [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)
y el proyecto adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.0-beta.7] - 2026-09-07

### Corregido

- **Repaso de calidad del `es_es` de beta.1 — lote 2: Macaw's Roofs** (`mcwroofs`, 606 de 610
  cadenas reescritas).
  - **Eliminado el *Title Case* inglés** de todos los nombres de bloque y objeto («Techo de Ático
    de Roble» → «Techo de ático de roble»). Era el defecto dominante de este namespace: casi todo
    el archivo.
  - **Nombres de madera y material alineados con el `es_es` vanilla**: *spruce* «picea» → «abeto»;
    *warped* «retorcido» → «distorsionado»; *Blackstone* «Negroita» → «piedra negra»; *cobblestone*
    «adoquín» → «roca»; además *cherry*, *bamboo*, *crimson*, *dark oak*, *deepslate*.
  - **Vocabulario de tejado consistente** en todo el archivo: *attic* → «de ático», *top* →
    «superior», *lower* → «inferior», *steep* → «empinado», *Roofing Hammer* → «Martillo de tejador».
  - Correcciones menores de concordancia de género en las losas de techo de color.

### Notas

- Claves y placeholders intactos; solo valores. 4 cadenas ya estaban bien. `itemGroup.mcwroofs`
  se mantiene «Macaw's Roofs» (marca).
- Pasada con OpenCode (MiMo-V2.5) contra `docs/GLOSARIO_ES.md` y el `es_es` vanilla 1.21.1;
  integridad de claves, placeholders y Title Case residual verificados con script.

## [0.1.0-beta.6] - 2026-09-07

### Corregido

- **Repaso de calidad del `es_es` de beta.1 — lote 1: Waystones** (190 de 263 cadenas reescritas).
  La traducción automática original tenía errores de criterio; este es el primer lote de una pasada
  por tandas contra un glosario ratificado (`docs/GLOSARIO_ES.md`).
  - **«Mojón» eliminado.** La MT traducía *Waystone* como «mojón» (vulgar en España). Por decisión
    del proyecto, *Waystone* se mantiene sin traducir, igual que la familia `-stone` (*Portstone*,
    *Sharestone*, *Warpstone*). Lo descriptivo sí se traduce: *Warp Plate* → «Placa de traslado»,
    *Warp Portal* → «Portal de traslado», *Bound / Return Scroll* → «Pergamino vinculado / de regreso».
  - **Terminología vanilla.** *Blackstone* «Negrita» → «piedra negra»; *Nether* «Inframundo» →
    «Nether»; *Ender* «del Fin» → «del End»; nombres de color alineados con el `es_es` vanilla
    (light blue → «azul claro», etc.).
  - **Capitalización española.** Eliminado el *Title Case* inglés de todos los nombres de bloque,
    objeto y GUI («Piedra de Puerto Azul Claro» → «Portstone azul claro»).
  - **Concordancia de género.** Toda la familia `-stone` concuerda ahora en femenino («la Waystone»,
    «las Waystones activadas», «Portstone amarilla»).

### Notas

- Claves, placeholders (`%s`, `%d`, `%1$s`) y códigos de formato intactos; solo se tocaron valores.
  73 cadenas ya estaban correctas y se dejaron igual.
- Pasada con OpenCode (MiMo-V2.5) contra el glosario, con el `es_es` vanilla 1.21.1 como referencia;
  integridad de claves, placeholders y concordancia verificados con script.

## [0.1.0-beta.5] - 2026-09-07

### Añadido

- **Locale español (`es_es`) para Apothic Attributes** — 161 claves, tomando como origen el
  `en_us.json` del mod (Apothic Attributes 2.10.1). El mod trae un `es_es.json`, pero está
  **obsoleto**: se escribió para una versión anterior y sus claves ya no coinciden con las que
  busca la versión actual. Las 161 claves vivas caían a inglés en la partida: nombres de atributos
  en el equipo, sus tooltips con Shift, los efectos de estado propios con sus pociones, y los
  mensajes de muerte de combate. El pack aporta ahora esas 161 claves, fusionadas sobre el archivo
  (desactualizado) del propio mod.
  - **Atributos** — nombre + descripción de Perforación/Trituración de armadura y de protección,
    Probabilidad/Daño de crítico, Daño de frío/fuego/HP actual/flecha/proyectil, Robo de vida,
    Sobrecuración, Salud fantasma, Velocidad de tensado/minado, Velocidad de flecha, Probabilidad
    de esquiva, Experiencia/Curación recibida, Reducción de enfriamiento, Vuelo con élitros/creativo.
  - **Descripciones de atributos vanilla y de NeoForge** — las líneas `.desc` de Armadura, Daño/
    Velocidad/Empuje de ataque, Suerte, Salud máxima, Velocidad de movimiento, Alcance de bloques/
    entidades, Altura de escalón, Velocidad de nado, Gravedad, y los efectos de poción vanilla.
  - **Efectos de estado propios** — Sangrado, Vitalidad desbordante, Conocimiento antiguo, Heridas
    graves, Resquebrajadura, Detonación, Vuelo: nombre, tooltip y descripción del efecto, más los
    nombres de poción / poción arrojadiza / poción persistente / flecha con punta de cada uno.
  - **Mensajes de muerte** — fuentes de daño por Sangrado, Detonación, HP actual, Fuego y Frío
    (variantes con objeto y con jugador).
  - **Pantalla de atributos** — cadenas de la GUI (Mantén Shift, base, mín, máx, modificadores,
    fórmula).

### Notas

- La terminología se alineó, donde el archivo obsoleto del mod aún tenía español utilizable, con
  sus decisiones previas (*Sundering* → «Resquebrajadura», *Knowledge* → «Sabiduría», *Bleeding*
  → «Sangrado»).
- Se conservan literalmente el glifo de enfriamiento `⌛`, todos los especificadores de formato
  `%s` / `%1$s` y los nombres propios del estilo *Eterna / Quanta / Arcana*.
- Traducción hecha con OpenCode (MiMo-V2.5); integridad de claves, placeholders y validez JSON
  verificados con script.

## [0.1.0-beta.4] - 2026-09-04

### Añadido

- **Traducción al español (`es_es`) de las guías Patchouli con texto incrustado** — 188 ficheros
  JSON, ~779 cadenas. Estos libros no usan claves de idioma (`i18n`), así que la capa `lang` del
  pack no los cubría y salían en inglés en la partida aunque el mod trajera `es_es`. Se inyectan
  como carpeta `es_es/` paralela a la `en_us/` del mod (Patchouli la prioriza; *fallback* a inglés
  fichero a fichero). Todos los códigos de formato de Patchouli (`$(br)`, `$(l:...)`, colores
  `$(#...)`, `$(playername)`…) se conservan literalmente; no se tocan `type`/`icon`/`recipe` ni
  las *resource locations*.
  - `butchery` · `butchers_guide` — 52 ficheros (47 entradas + 5 categorías). Terminología alineada
    con `assets/butchery/lang/es_es.json` (p. ej. *cleaver* → «Cuchillo de forjar», *skinning knife*
    → «Cuchillo de despiece», *blood grate* → «Rejilla de sangre»).
  - `apotheosis` · `apoth_chronicle` — 126 ficheros (107 entradas + 19 categorías).
  - `irons_spellbooks` · `iss_guide_book` — 10 ficheros (9 entradas + 1 categoría).

### Notas

- **No traducible desde un resource pack**: el título del libro y el `landing_text` (página de
  bienvenida) de `butchery` e `irons_spellbooks` viven en `book.json` (zona de *data pack*) y no
  usan `i18n`; quedan en inglés. El de `apotheosis` sí sale en español (usa clave de idioma, ya
  traducida en el `es_es` oficial del mod).
- `BetterEnd` (`guidebook`), `ars_nouveau`/`ars_elemental` (`worn_notebook`) y
  `mysticalagriculture` (`guide`) **no** se incluyen: el primero trae carpeta `es_es/` propia en
  el jar; los otros dos usan claves `i18n` ya traducidas en sus locales oficiales.
- Traducción hecha con OpenCode (MiMo-V2.5); revisión de estructura, tokens y cadenas restantes
  con script propio.

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
