# Glosario y reglas de estilo — es_es (España)

Documento de **ratificación previa** al repaso de calidad (QA) de las traducciones publicadas en
el resource pack (beta.1: 101 namespaces / ~12,5k claves, MT MiMo‑V2.5 sin revisar).

- **Alcance del QA**: solo las claves que este pack aporta (capa *overlay* sobre el `es_es` propio
  de cada mod). No se tocan claves que ya traduce el jar del mod.
- **Modelo QA**: OpenCode `opencode-go/omen-alpha` (elegido por el usuario).
- **Referencia vanilla**: `assets/minecraft/lang/es_es.json` de MC 1.21.1 (8557 claves), fijada
  aparte. Cualquier término que exista en vanilla **manda** sobre este glosario.

Estado: **BORRADOR — pendiente de que el usuario apruebe/corrija la columna "Propuesta".**

---

## 1. Reglas globales (se aplican a todos los namespaces)

| # | Regla | Antes (MT actual) | Después |
|---|---|---|---|
| G1 | **Capitalización española**: solo la primera letra de la frase y los nombres propios van en mayúscula. Nada de *Title Case* inglés. | `Techo de Ático de Roble` · `Trampilla de Piedra de Fuente Pulida` · `Libro de Hechizos` | `Techo de ático de roble` · `Trampilla de piedra de fuente pulida` · `Libro de hechizos` |
| G2 | **Términos vanilla obligatorios** (de `minecraft/lang/es_es.json`): `redstone`→«redstone» (el polvo = «polvo de redstone»), `Blackstone`→«piedra negra», `Nether`→«Nether», `The End`→«el End», `crafting table`→«mesa de trabajo», `trapdoor`→«trampilla», `Deepslate`→«pizarra profunda». | `Mojón de Negrita` · `Mojón del Inframundo` | `Waystone de piedra negra` · `Waystone del Nether` |
| G3 | **Illagers**: `Pillager`→«Saqueador», `Vindicator`→«Vindicador», `Evoker`→«Evocador», `Illusioner`→«Ilusionista», `Ravager`→«Devastador». El grupo genérico «illagers» se deja como «illagers» o se reformula; **nunca** «pillagers». | `Alfabeto de los Pillagers` · `Avanposto de Pillagers` | `Alfabeto de los illagers` · `Puesto de avanzada saqueador` |
| G4 | **No inventar palabras**. Errores MT detectados: `rejerada`→«enrejada» / «con barrotes», `avanposto`→«puesto de avanzada», `waffle`→«gofre», `Piedra de Tocar`→«piedra de toque». | `Trampilla rejerada de %s` | `Trampilla enrejada de %s` |
| G5 | **Nombres de mod y de marca no se traducen**: `Ars Nouveau`, `Iron's Spellbooks`, `Create`, `Farmer's Delight`, `Supplementaries`, `Quark`, `BetterEnd`, `Moog's…`. Sí se traducen las descripciones (`modmenu.descriptionTranslation.*`) y las etiquetas de pestaña genéricas («Building Blocks Tab»→«Pestaña de bloques de construcción»). | — | — |
| G6 | **Placeholders y códigos intactos y en su sitio**: `%s %d %1$s %%`, `§a §l §r`, `\n`, `$(…)` de Patchouli, `{valor}`, `<tag>`, el glifo `⌛`. | — | — |
| G7 | **Registro**: castellano de España, neutro de videojuego. Evitar americanismos (`computadora`, `celular`, `carro` = coche, `jugo`, `frijol`). Usar la 2ª persona de «tú» como hace vanilla. | — | — |
| G8 | **Consistencia interna**: un término se traduce igual en todo el namespace (p. ej. `Source`/`Sourceberry`/`Archwood` en Ars). | `Bosque de Archwood` vs `Bosque Arcano` en el mismo archivo | Elegir uno y unificar |
| V1 | **Varas mágicas — usar el término que corresponde al inglés**, no unificar a la fuerza: `Staff`→«báculo», `Wand`→«varita», `Rod`→«vara», `Scepter`→«cetro», `Cane`→«bastón». Si el inglés es ambiguo o genérico, **«báculo»** como comodín. | `Bastón de Magus de Hielo` (era `Rod`) | `Vara del magus de hielo` |
| V2 | **Género de nombres propios sin traducir**: si el término inglés que se mantiene representa un bloque/piedra (Waystone, Portstone, Sharestone, Warpstone), concuerda en **femenino** («la Waystone», «las Waystones activadas», «Portstone amarilla»). | `el Waystone` · `Portstone rojo` | `la Waystone` · `Portstone roja` |

---

## 2. Decisiones de término — **RATIFICADO 2026-09-07**

`opencode-go/omen-alpha` aplica la columna **Decisión**.

### 2.1 Waystones (mod entero — el pack aporta las 263 claves «gap»)

**Regla de familia**: los nombres propios acabados en `-stone`/`Waystone` **NO se traducen** (se
tratan como marca del mod). Lo descriptivo (placas, portales, pergaminos, GUI) sí se traduce, en
minúscula estilo español.

| EN | MT actual | Decisión | Motivo |
|---|---|---|---|
| Waystone | «Mojón» | **«Waystone»** (sin traducir) | decisión del usuario; «mojón» además era vulgar en España |
| Black / Ender / Nether / Muddy / … Waystone | Mojón de Negrita / del Fin / … | **«Waystone de piedra negra / del End / del Nether / de barro / …»** (adjetivo en minúscula, término vanilla; «Waystone» fijo) | |
| Portstone | Piedra de Puerto | **«Portstone»** (sin traducir) | familia `-stone` |
| Sharestone / Warp Stone | Piedra Compartida / de Salto | **«Sharestone» / «Warpstone»** (sin traducir) | familia `-stone` |
| Warp Plate | Placa de Salto | Placa de traslado | descriptivo |
| Warp Portal | Portal de Salto | Portal de traslado | descriptivo |
| Warp Scroll / Return Scroll / Bound Scroll | Pergamino de Salto / Regreso / Vinculado | Pergamino de traslado / de regreso / vinculado | descriptivo, minúscula |
| Fleeting Memorial | Memorial Efímero | Monolito efímero | «memorial» es anglicismo |

### 2.2 Ars Nouveau / Ars Additions / Ars Elemental / Ars Creo

| EN | MT actual | Propuesta | Motivo |
|---|---|---|---|
| Source (energía mágica) | Fuente / Maná (mezclado) | **Fuente** | término del mod; no es «maná» |
| Sourcestone | Piedra de Fuente | Piedra de fuente | mantener, solo casing |
| Sourceberry / Source Berry Bush | Baya de Fuente / Arbusto de Bayas de Fuente | Baya de fuente / Arbusto de bayas de fuente | casing |
| Archwood | Archwood (a veces «Arcano») | **Archwood** (sin traducir) | nombre propio de madera del mod |
| Spell Parchment | Pergamino de Hechizo | Pergamino de hechizo | casing |
| Starbuncle / Wilden / Drygmy | (se dejan) | se dejan sin traducir | criaturas del mod |
| Mana | Maná | Maná | ok |
| Glyph / Form / Effect / Augment | Glifo / Forma / Efecto / Aumento | igual, casing | |

### 2.3 Iron's Spells 'n Spellbooks

| EN | MT actual | Propuesta |
|---|---|---|
| Spellbook | Libro de Hechizos | Libro de hechizos |
| Scroll | Pergamino | Pergamino |
| Rune / Runestone | Runa / Piedra rúnica | Runa / Piedra rúnica |
| Upgrade Orb | Orbe de Mejora | Orbe de mejora |
| Arcane Essence | Esencia Arcana | Esencia arcana |
| Ancient Knowledge Fragment | Fragmento de Conocimiento Antiguo | Fragmento de conocimiento antiguo |
| School (Fire, Ice, Lightning, Holy, Ender, Blood, Evocation, Nature) | Escuela… | Escuela de fuego / hielo / rayo / sagrada / ender / sangre / evocación / naturaleza |

### 2.4 Reliquary

| EN | MT actual | Propuesta | Motivo |
|---|---|---|---|
| Touchstone of Midas | Piedra de Tocar de Midas | Piedra de toque de Midas | «piedra de toque» es el término real |
| Tome of Alkahestry / Alkahest | Tomo de Alkahestry | **«Tomo de Alkahestry»** (Alkahestry sin traducir) | decisión del usuario |
| Ice Magus Rod | Bastón de Magus de Hielo | **Vara del magus de hielo** | `Rod` = vara (ver regla V1); «Magus» se mantiene |
| Rending Gale | Viento Desgarrador | Vendaval desgarrador | |
| Fortune Coin | Moneda de la Fortuna | Moneda de la fortuna | casing |
| Pyromancer's Staff | Bastón del Piromante | **Báculo del piromante** | `Staff` = báculo (ver regla V1) |
| Handgun / Magazine | Pistola / Cargador | Pistola / Cargador | |

### 2.5 Create

| EN | MT actual | Propuesta |
|---|---|---|
| Andesite Alloy | Aleación de Andesita | Aleación de andesita |
| Brass | Latón | Latón |
| Cogwheel / Shaft / Belt | Rueda dentada / Eje / Cinta | Rueda dentada / Eje / Cinta transportadora |
| Contraption | Artilugio | Artilugio |
| Schematic | Esquema / Plano | Esquema |
| Kinetic / Stress / SU | Cinético / Tensión | Cinético / Esfuerzo (SU) |

### 2.6 Otros recurrentes

| EN | Propuesta | Nota |
|---|---|---|
| Trapdoor | Trampilla | vanilla |
| Barred / Windowed / Meshed Trapdoor | Trampilla con barrotes / con ventana / de malla | corrige «rejerada» |
| Rich Soil (Farmer's Delight) | Tierra fértil | |
| Skillet / Cooking Pot / Cutting Board | Sartén / Olla / Tabla de cortar | si están en nuestras claves |
| Backpack (Quark/Sophisticated) | Mochila | |
| Ancient Tome | Tomo antiguo | |
| Waystone/rune «attunement» | sintonización | |
| Scavenger (encantamiento) | Carroñero | ya correcto |

---

## 3. Plan de ejecución — **por tandas** (decisión del usuario)

1. Referencia vanilla `minecraft/lang/es_es.json` 1.21.1 ya extraída (scratchpad).
2. Lotes por tamaño/afinidad, peor primero. **Cada lote validado = su propia beta** (beta.6, beta.7…),
   workflow completo por cada una (`build_pack.py`, `docs/curseforge/versions/*`, `CHANGELOG.md`,
   commit, tag, subida CurseForge, instancia).
   - Orden previsto: `waystones` (piloto) → `mcwroofs` → `everycomp` → `supplementaries` →
     `ars_*` → `reliquary`+`irons_spellbooks` → `quark`+`create`+`farmersdelight` → `xaero*` → resto.
3. Por lote: `omen-alpha` reescribe cada `es_es.json` aplicando reglas G1–V1 + tabla §2, con el
   `en_us` del mod y el vanilla `es_es` como contexto. Permisos edit‑only sin shell.
4. Verificación por script (claves idénticas, placeholders, JSON, % de cambios) + muestreo manual
   por Claude antes de publicar cada beta.

---

## 4. Preguntas — **RESUELTAS 2026-09-07**

1. **Waystone** → se mantiene **«Waystone»** sin traducir (y la familia `-stone`: Portstone, Sharestone, Warpstone).
2. **Alkahestry** → se mantiene **«Alkahestry»** sin traducir.
3. **Varas mágicas** → usar el término que corresponde al inglés (`Staff`=báculo, `Wand`=varita,
   `Rod`=vara, `Scepter`=cetro, `Cane`=bastón); **«báculo»** solo como comodín si el inglés es genérico. Ver regla V1.
4. **Publicación** → **por tandas**, una beta por lote validado.
