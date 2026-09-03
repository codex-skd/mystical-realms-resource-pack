# Snapshot de mods y traducciones - Mystical Realms modpack v5.134.4

> Snapshot generado el 2026-09-03. Fuente: instancia CurseForge '(Translations) Mystical Realms - A Modded Server'.

- Modpack: Mystical Realms - A Modded Server v5.134.4 (autor: LlaGuiT0)
- Minecraft: 1.21.1
- Cargador: NeoForge 21.1.249
- Jars en mods/: 170
- Resource pack de traducciones: MysticalRealms_TranslationFixes 0.1.0-beta.3 - 104 namespaces con carpeta lang/

Locale objetivo: es_es. Se listan tambien el resto de locales que cada mod empaqueta, para dar contexto del alcance de i18n de cada mod.

---

## 0. Verificacion jar a jar y cierre de huecos (2026-09-03)

Tras el snapshot inicial se verificaron uno a uno los "huecos". Resultado:

**Traducidos e integrados en el RP 0.1.0-beta.3** (~520 claves, origen `en_us.json` de cada mod, delegado a OpenCode `mimo-v2.5`):

| Namespace | Mod | Claves |
|---|---|---|
| `apothic_enchanting` | Apothic Enchanting 1.6.2 | 425 |
| `apothic_spawners` | Apothic Spawners 1.4.0 | 89 |
| `placebo` | Placebo 9.9.2 | 6 |

`Eterna` / `Quanta` / `Arcana` (nombres propios del sistema de Apotheosis) y los numerales romanos de nivel se dejan sin traducir a proposito.

**Falsos positivos del snapshot** (no habia nada que traducir):

| Marcado como | Realidad |
|---|---|
| `embeddium_extra` "solo dependencia" (fila 131 y seccion 4) | Empaqueta TODO su texto bajo el namespace `sodium-extra`, que el RP ya traduce. Cubierto al 100%. |
| `integrated_cataclysm` "solo dependencia" (fila 79) | `assets/integrated_cataclysm/lang/en_us.json` tiene **0 claves** (archivo vacio). |
| `integrated_villages` "solo dependencia" (fila 81) | Sin ningun archivo `lang/` propio. |
| `waystone_towers` (seccion 5a) | `assets/waystone_towers/lang/en_us.json` tiene **0 claves**. Ademas es un mod propio. |
| `attributefix`, `utility_nexus_fixes` (seccion 4) | Sin archivos `lang/`. |

Las secciones 1-7 de abajo se regeneraron con el RP ya a 104 namespaces: `apothic_enchanting`, `apothic_spawners` y `placebo` aparecen ahora como `RP` / `propio`. Las notas "solo dependencia" de la seccion 4 sobre `embeddium_extra` / `integrated_cataclysm` / `integrated_villages` deben leerse con la tabla de arriba: no son huecos.

---

## 1. Resumen ejecutivo

| Categoria | Num |
|---|---|
| Jars totales | 170 |
| Ya traen es_es empaquetado | 66 |
| Sin es_es pero con algun lang/ | 60 |
| Sin ningun archivo lang/ | 44 |
| Sin es_es y CUBIERTOS por nuestro resource pack | 62 |
| Sin es_es y NO cubiertos (huecos) | 42 |

---

## 2. Tabla completa de mods (v5.134.4)

Columna es_es: 'mod' = lo trae el propio mod; 'RP' = lo aporta nuestro resource pack (total o parcial via namespaces de dependencia, ver seccion 4); '-' = no existe en ningun sitio.

| # | Mod | modid | Version | Locales empaquetados por el mod | es_es |
|---|---|---|---|---|---|
| 1 | Ace's Spell Utils | `aces_spell_utils, neoforge, minecraft` | `1.2.7.2-1.21.1` | en_us | RP |
| 2 | Apotheosis | `apotheosis, minecraft, neoforge, placebo, apothic_attributes, apothic_spawners, apothic_enchanting, curios, gateways` | `8.7.0` | en_us es_es fr_fr ja_jp ko_kr lzh pl_pl pt_br ru_ru tr_tr uk_ua zh_cn | mod |
| 3 | Apothic Attributes | `apothic_attributes, minecraft, neoforge, placebo` | `2.10.1` | en_us es_es ja_jp ko_kr pl_pl pt_br ru_ru tr_tr uk_ua vi_vn zh_cn | mod |
| 4 | Apothic Enchanting | `apothic_enchanting, minecraft, neoforge, placebo, apothic_attributes` | `1.6.2` | en_us fr_fr ja_jp ko_kr pt_br ru_ru tr_tr vi_vn zh_cn | RP |
| 5 | Apothic Spawners | `apothic_spawners, minecraft, neoforge, placebo` | `1.4.0` | en_us pt_br ru_ru tr_tr uk_ua zh_cn | RP |
| 6 | AppleSkin | `appleskin, neoforge` | `3.0.9+mc1.21` | cs_cz de_de en_us es_ar es_cl es_ec es_es es_mx es_uy es_ve fr_fr hy_am ja_jp ko_kr pl_pl pt_br ru_ru tr_tr uk_ua zh_cn zh_tw | mod |
| 7 | Aquaculture 2 | `aquaculture, neoforge` | `2.7.21` | de_de en_pt en_us es_ar es_es es_mx fr_fr he_il it_it ja_jp ko_kr pt_br ru_ru tr_tr uk_ua zh_cn zh_tw | mod |
| 8 | Aquaculture Delight (A Farmer's Delight Add-on) | `aquaculturedelight, minecraft` | `1.1.0` | en_us ru_ru | RP |
| 9 | Aquamirae [Neo/Forge Edition] | `aquamirae, minecraft, neoforge, fragmentum, geckolib` | `7.2.4` | de_de en_us es_es fr_fr id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru th_th tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 10 | Architectury API | `architectury, minecraft, neoforge` | `13.0.11` | (ninguno) | - |
| 11 | Armor Cosmetic | `armor_cosmetic, neoforge` | `1.0.0` | cs_cz de_de en_us es_es fr_fr it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se tr_tr zh_cn | mod |
| 12 | Armor Model API | `armor_model_api, neoforge, minecraft` | `1.1.0+1.21.1` | (ninguno) | - |
| 13 | Armor of the Ages | `armoroftheages, neoforge, minecraft, yet_another_config_lib_v3` | `1.5.10` | af_za ar_sa ca_es cs_cz da_dk de_de el_gr en_us es_es fi_fi fr_fr he_il hu_hu id_id it_it ja_jp jv_id ko_kr nl_nl no_no pl_pl pt_br pt_pt ro_ro ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 14 | Ars Additions | `ars_additions, neoforge, minecraft, curios, ars_nouveau` | `1.21.1-21.3.0` | en_us zh_cn | RP |
| 15 | Ars Creo | `ars_creo, neoforge, minecraft, ars_nouveau, create` | `5.4.0` | en_us pt_br zh_cn | RP |
| 16 | Ars Elemental | `ars_elemental, minecraft, ars_nouveau, ars_creo` | `0.7.10.1` | de_de el_gr en_us es_es fr_fr it_it ja_jp ko_kr pt_br pt_pt ru_ru tr_tr uk_ua zh_cn zh_tw | mod |
| 17 | Ars Nouveau | `ars_nouveau, neoforge, curios, geckolib` | `5.13.1` | af_za ar_sa ca_es cs_cz da_dk de_de el_gr en_us es_es fi_fi fr_fr he_il hu_hu it_it ja_jp ko_kr nl_nl no_no pl_pl pt_br pt_pt ro_ro ru_ru sr_sp sv_se tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 18 | Arsenal (RPG Series) | `arsenal, neoforge, minecraft, spell_engine, ranged_weapon_api` | `1.5.0` | cs_cz de_de en_us es_ar es_es fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn | mod |
| 19 | Sophisticated Backpacks: Ars Compat / Sophisticated Backpacks Ars-Nouveau Compatibility | `arssophisticatedcompat, neoforge, minecraft, sophisticatedcore, sophisticatedbackpacks, ars_nouveau` | `0.3.0` | en_us | RP |
| 20 | AttributeFix | `attributefix, neoforge, minecraft, bookshelf, prickle` | `21.1.3` | (ninguno) | RP |
| 21 | AttributeFix-Sync | `attributefixsync, neoforge, minecraft, attributefix` | `0.0.2` | (ninguno) | - |
| 22 | AzureLib | `azurelib, neoforge, minecraft` | `3.1.11` | en_us es_es fr_fr ru_ru zh_cn | mod |
| 23 | Balm | `balm, neoforge, minecraft` | `21.0.65` | en_us es_ar es_mx it_it pt_br tr_tr | RP |
| 24 | BCLib: New Dawn | `bclib, neoforge, minecraft, wunderlib, wover` | `21.0.26` | de_de en_us ko_kr pt_br ru_ru tr_tr uk_ua zh_cn | RP |
| 25 | Better Combat [Fabric & Forge] | `bettercombat, neoforge, minecraft, playeranimator, cloth_config` | `2.4.0+1.21.1` | de_de en_us es_ar es_es es_mx fr_fr it_it ja_jp ko_kr pt_br ru_ru uk_ua vi_vn zh_cn | mod |
| 26 | BetterEnd: New Dawn | `betterend, neoforge, minecraft, bclib, wover, wunderlib` | `21.0.34` | de_de en_gb en_us es_es ko_kr pt_br ru_ru thai_th tr_tr zh_cn | mod |
| 27 | Better End Cities Better End | `(sin toml)` | `?` | (ninguno) | - |
| 28 | Better Party | `better_party, neoforge, minecraft` | `1.1.5` | de_de en_us es_es fr_fr pt_br ru_ru | mod |
| 29 | Better Party X Xaero's World Map | `better_party_x_xaeros_world_map, neoforge, minecraft, better_party, xaeroworldmap` | `1.0.0` | de_de en_us | RP |
| 30 | Better Villager Animations | `bettervillageranimations, neoforge, minecraft` | `1.0.0` | ar_sa en_us | RP |
| 31 | Biomes O' Plenty | `biomesoplenty, neoforge, glitchcore, terrablender` | `21.1.0.14` | cs_cz de_de en_us es_ar es_cl es_es es_mx fr_fr it_it ja_jp kk_kz ko_kr nl_nl nn_no pl_pl pt_br ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 32 | Bookshelf | `bookshelf, neoforge, minecraft` | `21.1.81` | en_us es_ar ja_jp pt_br zh_cn | RP |
| 33 | Bundle API | `bundleapi, neoforge, minecraft` | `1.1.0` | (ninguno) | - |
| 34 | Butchery | `butchery, neoforge, minecraft, jei` | `5.2` | en_us | RP |
| 35 | Pillager Caravans | `caravans, minecraft, neoforge, fragmentum` | `3.0.0` | en_us pt_br | RP |
| 36 | Carry Mechanics | `carry_mechanics, neoforge, minecraft` | `0.0.0-beta.2` | en_us | RP |
| 37 | Cataclysm & BetterCombat - Compatibility | `(sin toml)` | `?` | (ninguno) | - |
| 38 | Cataclysmic Combat | `cataclysmiccombat, neoforge, minecraft` | `1.4.1` | (ninguno) | - |
| 39 | Clean Swing Through Grass | `cleanswing, neoforge, minecraft` | `1.9` | (ninguno) | - |
| 40 | Cloth Config API (Fabric/Forge/NeoForge) | `cloth_config, neoforge` | `15.0.140` | bg_bg de_de en_ud en_us es_es es_mx et_ee fr_fr hu_hu it_it ja_jp kk_kz ko_kr lol_us lzh pt_br ru_ru sv_se tt_ru uk_ua zh_cn zh_hk zh_tw | mod |
| 41 | Configured | `configured, neoforge, minecraft, framework, jei` | `2.6.3` | de_de en_us es_es it_it ru_ru | mod |
| 42 | Connected Glass | `connectedglass, neoforge, minecraft, supermartijn642corelib, fusion` | `1.1.14` | de_at de_ch de_de en_us es_ar es_cl es_es es_mx es_uy es_ve fr_fr it_it ja_jp ko_kr nl_be nl_nl ru_ru tr_tr uk_ua vi_vn | mod |
| 43 | Connectivity | `connectivity, neoforge, minecraft, cupboard` | `7.6` | (ninguno) | - |
| 44 | Crafting Tweaks | `craftingtweaks, neoforge, minecraft, balm` | `21.1.11` | en_us es_mx fr_fr pl_pl pt_br pt_pt ru_ru sv_se uk_ua zh_cn | RP |
| 45 | Create | `create, neoforge, minecraft, flywheel, ponder, sodium, lithium, journeymap, xaeroworldmap, radium, palladium` | `6.0.10` | af_za ar_sa be_by bel_tr bg_bg ca_es cs_cz cy_gb da_dk de_de el_gr en_gb en_pt en_ud en_us enws eo_uy es_cl es_es es_mx et_ee eu_es fa_ir fi_fi fr_ca fr_fr he_il hr_hr hu_hu hy_am id_id is_is it_it ja_jp kk_kz ko_kr ksh lol_us lt_lt lt_lv lzh nl_nl no_no pl_pl pt_br pt_pt qep ro_ro rpr ru_ru sv_se th_th tok tr_tr uk_ua vi_vn vp_vl zh_cn zh_tw | mod |
| 46 | Cucumber Library | `cucumber, neoforge, minecraft` | `8.0.16` | en_us fr_fr ja_jp ko_kr pt_br ru_ru uk_ua zh_cn | RP |
| 47 | Cupboard | `cupboard, minecraft` | `4.1` | (ninguno) | - |
| 48 | CustomSkinLoader | `customskinloader-bootstrap` | `15.0.1` | (ninguno) | - |
| 49 | Dangerous - Just A Difficulty Mod | `dangerous, neoforge, minecraft` | `1.5.2` | en_us | RP |
| 50 | Data Miner | `data_miner, neoforge, minecraft` | `0.0.0-beta.2` | en_us | RP |
| 51 | Dawn Of Time | `dawnoftimebuilder, neoforge, minecraft, fusion` | `1.6.6` | af_za ar_sa ca_es cs_cz da_dk de_de el_gr en_us es_es fi_fi fr_fr he_il hu_hu id_id it_it ja_jp jv_id ko_kr la_la lo_la nl_nl no_no pl_pl pt_br pt_pt ro_ro ru_ru sr_sp sv_se tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 52 | Deeper and Darker | `deeperdarker, minecraft, neoforge` | `1.4.1` | ca_es de_de en_au en_ca en_gb en_nz en_pt en_us es_es fr_ca fr_fr he_il it_it ja_jp ko_kr la_la lol_us nl_be nl_nl pl_pl pt_br pt_pt ro_ro ru_ru sl_si sv_se tr_tr uk_ua vi_vn zh_cn zh_hk zh_tw | mod |
| 53 | Deimos Lib | `deimos, neoforge, minecraft` | `2.7` | (ninguno) | - |
| 54 | Embeddium | `embeddium, neoforge, sodium` | `1.0.15+mc1.21.1` | de_de en_us es_es fr_fr uk_ua zh_cn | mod |
| 55 | Enchantment Descriptions | `enchdesc, neoforge, minecraft, bookshelf, prickle` | `21.1.11` | bg_bg de_de en_ca en_us es_ar es_cl es_es es_mx fil_ph fr_fr it_it ja_jp ko_kr nl_be nl_nl pl_pl pt_br ru_ru sv_se ta_in tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 56 | Equivalent Legacy | `equivalent_legacy, neoforge, minecraft, regalia_slots_api, jei, wthit` | `0.0.0-beta.4` | cs_cz de_de en_au en_gb en_ud en_us es_es fr_fr it_it ja_jp ru_ru tr_tr uk_ua zh_cn | mod |
| 57 | Every Compat (Wood Good) | `everycomp, neoforge, minecraft, moonlight, create, mcwdoors, mcwtrpdoors, blockus, regions_unexplored` | `1.21-2.11.50` | de_de en_us es_cl es_mx ja_jp zh_cn | RP |
| 58 | Explorer's Compass | `explorerscompass, neoforge, minecraft` | `1.21.1-3.4.0-neoforge` | de_de en_us es_es fr_fr ja_jp pt_br ru_ru tr_tr uk_ua zh_cn zh_tw | mod |
| 59 | Farmer's Sandwiches (A Farmer's Delight Add-on) | `farmers_sandwiches, neoforge, minecraft` | `0.1.2` | en_us | RP |
| 60 | Farmer's Delight | `farmersdelight, neoforge, minecraft, crafttweaker` | `1.3.4` | be_by bg_bg ca_es da_dk de_de en_gb en_nz en_pt en_us es_ar es_cl es_ec es_es es_mx es_uy es_ve fi_fi fr_ca fr_fr hu_hu id_id it_it ja_jp kk_kz ko_kr lol_us lzh nl_be nl_nl no_no pl_pl pt_br pt_pt ru_ru sk_sk sr_sp sv_se tok tr_tr uk_ua vi_vn vp_vl zh_cn zh_hk zh_tw | mod |
| 61 | Farmers Delight: Pizza Lovers | `farmer_delight_pizza_lovers, neoforge, minecraft, jei` | `1.0.0` | en_us | RP |
| 62 | Fast Async World Save[Forge/Neo/Fabric] | `fastasyncworldsave, minecraft, cupboard` | `2.6` | (ninguno) | - |
| 63 | Fast IP Ping | `fastipping, minecraft` | `1.0.11` | (ninguno) | - |
| 64 | FerriteCore ((Neo)Forge) | `ferritecore, neoforge, minecraft` | `7.0.3` | (ninguno) | - |
| 65 | Fragmentum [NeoForge Edition] | `fragmentum, minecraft, neoforge` | `2.4.4` | (ninguno) | - |
| 66 | Fusion (Connected Textures) | `fusion, neoforge, minecraft` | `1.3.15` | en_us hu_hu tr_tr | RP |
| 67 | GeckoLib | `geckolib, neoforge, minecraft, geckoanimfix` | `4.9.2` | (ninguno) | - |
| 68 | GlitchCore | `glitchcore, neoforge` | `2.1.0.2` | (ninguno) | - |
| 69 | Golems Are Friends Not Fodder | `golemsarefriends, neoforge, minecraft` | `1.21.1-1.0.1` | (ninguno) | - |
| 70 | fix GPU memory leak | `gpumemleakfix, minecraft, cupboard` | `1.8` | (ninguno) | - |
| 71 | Guard Villagers | `guardvillagers, neoforge, minecraft` | `2.4.12` | cs_cz de_de en_us es_es es_mx fil_ph fr_fr it_it ja_jp ko_kr pl_pl pt_br ro_ro ru_ru tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 72 | Nether Trials & Chambers | `hellish_trials, neoforge, minecraft, architectury` | `1.0.5` | (ninguno) | - |
| 73 | Zombie Hordes | `horde_hoard, neoforge, minecraft` | `1.1.0` | en_us | RP |
| 74 | Integrated Dungeons and Structures | `idas, minecraft, create, supplementaries, quark, integrated_api` | `1.13.7+1.21.1-neoforge` | en_us zh_cn | RP |
| 75 | Illager Structures | `illagerstructures, neoforge, minecraft` | `0.1.2` | (ninguno) | - |
| 76 | ImmediatelyFast | `immediatelyfast, minecraft, neoforge` | `1.6.13+1.21.1` | (ninguno) | - |
| 77 | Info Tab | `info_tab, neoforge, minecraft` | `0.0.0-beta.1` | en_us | RP |
| 78 | Integrated API | `integrated_api, minecraft` | `1.8.0` | (ninguno) | - |
| 79 | Integrated Cataclysm | `integrated_cataclysm, minecraft, integrated_api, create, supplementaries, quark, cataclysm` | `1.0.6+1.21.1-neoforge` | en_us | RP |
| 80 | Integrated Stronghold | `integrated_stronghold, minecraft, create, quark, supplementaries` | `1.1.4+1.21.1-neoforge` | en_us | RP |
| 81 | Integrated Villages | `integrated_villages, minecraft, integrated_api, create, supplementaries` | `1.3.3+1.21.1-neoforge` | (ninguno) | RP |
| 82 | Inventory Essentials | `inventoryessentials, neoforge, minecraft, balm` | `21.1.18` | en_us zh_tw | RP |
| 83 | Iron's Lib | `irons_lib, neoforge, minecraft, geckolib, irons_patreon_lib` | `1.21.1-2.1.0` | en_us | RP |
| 84 | Iron's Spells 'n Spellbooks | `irons_spellbooks, neoforge, minecraft, geckolib, playeranimator, curios, irons_lib` | `1.21.1-3.16.3` | en_us es_es es_mx fr_fr it_it ja_jp ko_kr pl_pl pt_br ru_ru uk_ua vi_vn zh_cn zh_hk zh_tw | mod |
| 85 | Jade | `jade, neoforge` | `15.10.6+neoforge` | de_de en_us es_es it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru uk_ua zh_cn zh_tw | mod |
| 86 | Jauml | `jauml, neoforge, minecraft` | `2.1.1` | (ninguno) | - |
| 87 | Just Enough Items (JEI) | `jei, neoforge, minecraft` | `19.51.0.418` | ar_sa bg_bg cs_cz de_de el_gr en_us es_ar es_ec es_es fi_fi fil_ph fr_fr he_il hu_hu id_id it_it ja_jp kk_kz ko_kr lt_lt lzh no_no pl_pl pt_br pt_pt ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 88 | Jewelry (RPG Series) | `jewelry, neoforge, minecraft, spell_power, ranged_weapon_api, structure_pool_api, curios` | `2.4.0` | cs_cz de_de en_us es_ar es_es fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 89 | Just-In NETHER | `just_in_nether, neoforge, minecraft` | `1.0.0` | en_us zh_tw | RP |
| 90 | Just Enough Breeding (JEBr) | `justenoughbreeding, neoforge, minecraft` | `3.2.1` | de_de en_us es_ar fr_fr ja_jp pt_pt ru_ru uk_ua zh_cn zh_tw | RP |
| 91 | Just Enough Professions (JEP) | `justenoughprofessions, jei, neoforge, minecraft` | `4.0.5` | en_us es_ar ja_jp pt_br tr_tr zh_cn | RP |
| 92 | Just Enough Resources (JER) | `jeresources, jei` | `1.6.0.17` | de_de en_us es_ar es_es fr_fr it_it ja_jp ko_kr nl_nl pt_br pt_pt ru_ru zh_cn zh_tw | mod |
| 93 | L_Ender 's Cataclysm | `cataclysm, neoforge, minecraft, curios, lionfishapi` | `3.33` | en_us es_ar es_cl es_es es_mx fr_ca fr_fr hu_hu it_it ja_jp ko_kr pl_pl pt_br ru_ru tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 94 | Lionfish API | `lionfishapi, neoforge, minecraft` | `3.1` | en_us | RP |
| 95 | Lootr (Forge & NeoForge) | `lootr, minecraft, neoforge` | `1.21.1-1.11.38.124` | af_za ar_sa ca_es cs_cz da_dk de_de el_gr en_us es_es es_mx fi_fi fr_fr he_il hu_hu it_it ja_jp ko_kr lol_us nl_nl no_no pl_pl pt_br pt_pt ro_ro ru_ru sr_sp sv_se tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 96 | Macaw's Bridges | `mcwbridges` | `3.1.2` | de_de en_us es_cl es_es es_mx fr_fr it_it ja_jp ko_kr pt_br ru_ru sk_sk tr_tr uk_ua zh_cn | mod |
| 97 | Macaw's Stairs | `mcwstairs` | `1.0.2` | en_us es_cl es_es es_mx fr_fr ja_jp ko_kr pt_br ru_ru zh_cn | mod |
| 98 | Macaw's Windows | `mcwwindows` | `2.4.2` | de_de en_us es_cl es_es es_mx fr_fr it_it ja_jp ko_kr pt_br ru_ru tr_tr uk_ua zh_tw | mod |
| 99 | Macaw's Roofs | `mcwroofs` | `2.3.2` | de_de en_us es_cl es_mx fr_fr ja_jp ru_ru tr_tr uk_ua | RP |
| 100 | ModernFix | `modernfix, neoforge, minecraft, jei` | `5.27.24+mc1.21.1` | de_de en_us es_mx it_it ja_jp ru_ru vi_vn zh_cn zh_tw | RP |
| 101 | MES - Moog's End Structures | `moogs_structures` | `?` | en_us | RP |
| 102 | MNS - Moog's Nether Structures | `moogs_structures` | `?` | en_us | RP |
| 103 | Moog's Structure Lib (moogs_structures) | `moogs_structures, minecraft` | `3.1.2` | en_us | RP |
| 104 | Moonlight Lib | `moonlight, minecraft` | `1.21.1-3.6.0` | en_us es_ar es_es fr_fr ja_jp pt_br ru_ru uk_ua vi_vn zh_cn | mod |
| 105 | More Villagers | `morevillagers, neoforge, minecraft` | `6.0.0` | de_de en_us no_no pl_pl ru_ru zh_cn zh_tw | RP |
| 106 | Mouse Tweaks | `mousetweaks` | `2.26.1` | (ninguno) | - |
| 107 | Mowzie's Cataclysm | `mowzies_cataclysm, neoforge, minecraft, cataclysm, mowziesmobs` | `1.2.2` | en_us | RP |
| 108 | Mowzie's Mobs | `mowziesmobs, neoforge, minecraft, geckolib` | `1.8.2` | de_de en_us es_es es_mx fr_fr it_it ja_jp ko_kr pt_br ru_ru uk_ua zh_cn zh_tw | mod |
| 109 | Much More Dungeons | `muchmoredungeons, neoforge, minecraft` | `1.2.0` | (ninguno) | - |
| 110 | Mystical Agriculture | `mysticalagriculture, neoforge, minecraft, cucumber` | `8.0.28` | de_de en_us es_ar es_es es_mx fr_fr ja_jp ko_kr pl_pl pt_br ru_ru tr_tr uk_ua zh_cn zh_tw | mod |
| 111 | Mystical Automation | `mysticalautomation, neoforge, minecraft, cucumber, mysticalagriculture` | `1.0.7` | en_us ja_jp pt_br zh_cn | RP |
| 112 | Nature's Compass | `naturescompass, neoforge, minecraft` | `1.21.1-3.4.0-neoforge` | de_de en_us eo_uy es_ec es_es es_mx fr_fr hy_am it_ch it_it ja_jp kk_kz ko_kr pl_pl pt_br ru_ru sv_se tr_tr uk_ua zh_cn zh_tw | mod |
| 113 | Regrowth | `regrowth, neoforge, minecraft` | `21.34.7` | de_de en_us es_es fr_fr hi_in it_it ja_jp ko_kr no_no pt_br ru_ru uk_ua zh_cn | mod |
| 114 | NeOculus | `oculus, iris, neoforge, minecraft, embeddium` | `1.8.7` | cs_cz de_ch de_de en_pt en_ud en_us es_ar es_es et_ee fa_ir fi_fi fr_fr hu_hu it_it ja_jp ko_kr lol_us lzh nl_nl pl_pl pr_pt pt_br ru_ru sk_sk th_th tr_tr uk_ua zh_cn zh_tw | mod |
| 115 | Not Enough Crashes (Forge) | `notenoughcrashes, neoforge, minecraft` | `4.4.9+1.21.1` | de_de en_us et_ee fr_fr ja_jp ms_my pt_br ro_ro ru_ru uk_ua zh_cn zh_hk zh_tw zlm_arab | RP |
| 116 | Obscure Tooltips | `obscure_tooltips, minecraft, neoforge, fragmentum` | `4.2.4` | en_us es_es ja_jp pt_br pt_pt ru_ru tok zh_cn | mod |
| 117 | ShatterLib / OctoLib | `octolib, neoforge, minecraft, architectury` | `0.6.2` | (ninguno) | - |
| 118 | Paladins & Priests (RPG Series) | `paladins, neoforge, minecraft, armor_model_api, spell_engine, runes` | `3.1.1` | cs_cz de_de en_us es_ar es_es fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn | mod |
| 119 | Patchouli | `patchouli, neoforge, minecraft` | `1.21.1-93-NEOFORGE` | cs_cz de_de en_us es_es fr_fr it_it ko_kr pl_pl pt_br ru_ru uk_ua zh_cn | mod |
| 120 | Placebo | `placebo, minecraft, neoforge` | `9.9.2` | en_us fr_fr it_it ko_kr pt_br ru_ru tr_tr uk_ua zh_cn | RP |
| 121 | Player Activity View | `player_activity_view, neoforge, minecraft` | `0.0.0-beta.1` | en_us | RP |
| 122 | playerAnimator | `playeranimator, minecraft` | `2.0.4+1.21.1` | (ninguno) | - |
| 123 | Prickle | `prickle, neoforge, minecraft` | `21.1.11` | (ninguno) | - |
| 124 | Puzzles Lib | `puzzleslib, minecraft, neoforge` | `21.1.56` | (ninguno) | - |
| 125 | Quark | `quark, neoforge, zeta, biolith, lootr` | `4.1-482` | de_de en_gb en_nz en_pt en_us es_ar es_cl es_es es_mx fi_fi fr_fr hu_hu it_it ja_jp ko_kr pl_pl pt_br pt_pt ru_ru sv_se tok uk_ua zh_cn zh_tw | mod |
| 126 | Ranged Weapon API | `ranged_weapon_api, neoforge, minecraft` | `3.0.0+1.21.1` | cs_cz de_de en_us es_ar es_es fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn | mod |
| 127 | Regalia Slots API | `regalia_slots_api, neoforge, minecraft, curios, neoforge, minecraft` | `0.0.0-beta.12` | de_de en_us es_es fr_fr it_it ja_jp ko_kr lzh pl_pl pt_br ru_ru tok tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 128 | Relics | `relics, minecraft, neoforge, curios, octolib` | `0.10.7.8` | en_us es_es ja_jp ko_kr ru_ru zh_cn | mod |
| 129 | Reliquary Reincarnations | `reliquary, neoforge, minecraft` | `2.0.80` | en_us ja_jp ko_kr pt_br ru_ru uk_ua zh_cn | RP |
| 130 | Rogues & Warriors (RPG Series) | `rogues, neoforge, minecraft, armor_model_api, spell_engine, structure_pool_api` | `3.1.1` | cs_cz de_de en_us es_ar es_es fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn | mod |
| 131 | Embeddium (Rubidium) Extra | `embeddium_extra, neoforge, embeddium, minecraft` | `0.5.7e+mc1.21-build.132` | cs_cz de_at de_ch de_de el_gr en_us es_ar es_mx et_ee fi_fi fr_ca fr_fr hu_hu it_it ja_jp ko_kr ms_my pl_pl pt_br pt_pt ru_ru th_th tr_tr uk_ua vi_vn zh_cn zh_hk zh_tw | RP |
| 132 | Runes | `runes, neoforge, minecraft` | `1.3.2+1.21.1` | cs_cz de_de en_us es_ar es_es fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn | mod |
| 133 | Shield API | `shield_api, neoforge, minecraft` | `2.2.0` | (ninguno) | - |
| 134 | SKD Menu | `skd_menu, neoforge, minecraft` | `0.0.0-beta.4` | en_us | RP |
| 135 | Sophisticated Backpacks | `sophisticatedbackpacks, sophisticatedcore, neoforge, minecraft` | `3.25.78` | de_de en_us es_es es_mx fr_fr ja_jp ko_kr lzh pl_pl pt_br ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 136 | Sophisticated Core | `sophisticatedcore, jei, neoforge, minecraft` | `1.4.90` | de_de en_us es_es es_mx ja_jp ko_kr lzh pt_br ru_ru tr_tr uk_ua zh_cn | mod |
| 137 | Spell Engine | `spell_engine, neoforge, minecraft, cloth_config, playeranimator, spell_power, curios` | `1.10.5` | cs_cz de_de en_us es_ar es_es fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn | mod |
| 138 | Spell Power Attributes | `spell_power, neoforge, minecraft` | `1.6.0+1.21.1` | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn | RP |
| 139 | Storage Drawers | `storagedrawers, minecraft, neoforge` | `13.11.4` | de_de en_us es_es fr_fr ja_jp ko_kr nl_nl pt_br pt_pt ru_ru zh_cn zh_tw | mod |
| 140 | Structure Pool API | `structure_pool_api, neoforge, minecraft` | `1.2.1+1.21.1` | (ninguno) | - |
| 141 | Structure Essentials | `structureessentials, minecraft, cupboard` | `5.0` | (ninguno) | - |
| 142 | SuperMartijn642's Core Lib | `supermartijn642corelib, neoforge, minecraft` | `1.1.24` | en_us | RP |
| 143 | Supplementaries | `supplementaries, neoforge, minecraft, moonlight, create, amendments, farmersdelight, sodium` | `1.21.1-3.9.6` | ca_es cs_cz de_de en_gb en_pt en_us es_ar es_es es_mx fi_fi fr_ca fr_fr hu_hu it_it ja_jp kk_kz ko_kr ms_my pl_pl pt_br pt_pt ru_ru sr_sp tok tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 144 | Teleport Animation | `teleport_animation, neoforge, minecraft, waystones` | `1.1.0` | en_us ja_jp | RP |
| 145 | TerraBlender (NeoForge) | `terrablender, neoforge` | `4.1.0.8` | de_de en_gb en_us pt_br ru_ru sv_se tr_tr uk_ua | RP |
| 146 | Corail Tombstone | `tombstone, neoforge, minecraft, iris` | `9.5.5` | en_us es_es fr_fr nl_nl pt_br ru_ru zh_cn | mod |
| 147 | Tom's Simple Storage Mod | `toms_storage, neoforge, minecraft, sophisticatedstorage` | `2.4.2` | en_us fr_fr ja_jp ko_kr pt_br ru_ru zh_cn | RP |
| 148 | Towers of the Wild Modded | `totw_modded, neoforge, minecraft` | `1.0.9` | (ninguno) | - |
| 149 | Towers of the Wild Modded - Extra Towers | `(sin toml)` | `?` | (ninguno) | - |
| 150 | TT20 (TPS Fixer) | `tt20, minecraft` | `0.8.4` | (ninguno) | - |
| 151 | Utility Nexus Admin | `utility_nexus_admin, neoforge, minecraft` | `0.0.0-beta.13` | (ninguno) | - |
| 152 | Utility Nexus Fixes | `utility_nexus_fixes, neoforge, minecraft, iris, sodium` | `0.0.0-beta.3` | (ninguno) | RP |
| 153 | Vellumli | `vellumli, neoforge, minecraft` | `0.0.0-beta.1` | cs_cz de_de en_us es_es fr_fr it_it ko_kr pl_pl pt_br ru_ru uk_ua zh_cn | mod |
| 154 | Villager Guards (Fabric/Forge/NeoForge/Quilt) | `(sin toml)` | `?` | (ninguno) | - |
| 155 | VillagersPlus (Fabric/Neoforge) | `villagersplus, neoforge, minecraft, villagertradingplus` | `4.0.0+mc1.21.1` | de_de en_us es_es fr_fr it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru uk_ua zh_cn | mod |
| 156 | VillagersTradingPlus | `villagertradingplus, neoforge, minecraft` | `1.0.0+mc1.21.1` | de_de en_us es_es fr_fr it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru uk_ua zh_cn | mod |
| 157 | Visual Workbench | `visualworkbench, neoforge, minecraft, puzzleslib` | `21.1.2` | en_us | RP |
| 158 | Waystone Towers | `waystone_towers, neoforge, minecraft` | `1.0.9` | en_us | - |
| 159 | Waystones | `waystones, neoforge, minecraft, balm` | `21.1.42` | cs_cz de_de en_us es_ar es_cl es_es es_mx fr_fr hu_hu it_it ja_jp ko_kr no_no pl_pl pt_br pt_pt ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw | mod |
| 160 | Wishful Recipes | `wishfulrecipes, neoforge, minecraft, deimos` | `1` | en_us | RP |
| 161 | Wizards (RPG Series) | `wizards, neoforge, minecraft, armor_model_api, spell_engine, runes, structure_pool_api` | `3.1.2` | cs_cz de_de en_us es_ar es_es fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn | mod |
| 162 | Workhand Tool | `workhand_tools, neoforge, minecraft, vellumli` | `0.0.0-beta.3` | de_de en_us es_es fr_fr it_it ja_jp ko_kr pt_br ru_ru zh_cn | mod |
| 163 | WorldWeaver: New Dawn | `wover, neoforge, minecraft, wunderlib` | `21.0.25` | de_de en_us ru_ru | RP |
| 164 | WunderLib: New Dawn | `wunderlib, neoforge, minecraft` | `21.0.10` | (ninguno) | - |
| 165 | Xaero's Minimap | `xaerominimap, neoforge, minecraft, openpartiesandclaims, xaeroworldmap, xaerolib` | `26.4.2` | cs_cz da_dk de_de el_gr en_us es_ar es_es es_mx et_ee fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr lv_lv nl_nl pl_pl pt_br pt_pt ru_ru sr_sp th_th tr_tr uk_ua vi_vn zh_cn | mod |
| 166 | Xaero's World Map | `xaeroworldmap, neoforge, minecraft, openpartiesandclaims, xaerominimap, xaerobetterpvp, xaerolib` | `1.44.2` | de_de en_us | RP |
| 167 | YetAnotherConfigLib | `yet_another_config_lib_v3, neoforge, minecraft` | `3.8.2+1.21.1-neoforge` | be_by de_at de_ch de_de el_gr en_us es_ar es_es et_ee fr_fr it_it ja_jp ms_my nl_nl pl_pl pt_br pt_pt ru_ru sl_si tt_ru uk_ua zh_cn zh_tw zlm_arab | mod |
| 168 | YUNG's API (NeoForge) [1.20.4-1.21.1 ONLY] | `yungsapi, minecraft, neoforge` | `1.21.1-NeoForge-5.1.8` | (ninguno) | - |
| 169 | YUNG's Better End Island (NeoForge) [1.20.4 - 1.21.1 ONLY] | `betterendisland, minecraft, neoforge, yungsapi` | `1.21.1-NeoForge-3.1.2` | en_us ru_ru | RP |
| 170 | Zeta | `zeta, neoforge` | `1.1-40` | en_us ru_ru zh_cn | RP |

---

## 3. Mods que YA traen es_es (sin accion necesaria)

Total: 66

| Mod | modid | Version | Otros locales del mod |
|---|---|---|---|
| Apotheosis | `apotheosis, minecraft, neoforge, placebo, apothic_attributes, apothic_spawners, apothic_enchanting, curios, gateways` | `8.7.0` | en_us fr_fr ja_jp ko_kr lzh pl_pl pt_br ru_ru tr_tr uk_ua zh_cn |
| Apothic Attributes | `apothic_attributes, minecraft, neoforge, placebo` | `2.10.1` | en_us ja_jp ko_kr pl_pl pt_br ru_ru tr_tr uk_ua vi_vn zh_cn |
| AppleSkin | `appleskin, neoforge` | `3.0.9+mc1.21` | cs_cz de_de en_us es_ar es_cl es_ec es_mx es_uy es_ve fr_fr hy_am ja_jp ko_kr pl_pl pt_br ru_ru tr_tr uk_ua zh_cn zh_tw |
| Aquaculture 2 | `aquaculture, neoforge` | `2.7.21` | de_de en_pt en_us es_ar es_mx fr_fr he_il it_it ja_jp ko_kr pt_br ru_ru tr_tr uk_ua zh_cn zh_tw |
| Aquamirae [Neo/Forge Edition] | `aquamirae, minecraft, neoforge, fragmentum, geckolib` | `7.2.4` | de_de en_us fr_fr id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru th_th tr_tr uk_ua vi_vn zh_cn zh_tw |
| Armor Cosmetic | `armor_cosmetic, neoforge` | `1.0.0` | cs_cz de_de en_us fr_fr it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se tr_tr zh_cn |
| Armor of the Ages | `armoroftheages, neoforge, minecraft, yet_another_config_lib_v3` | `1.5.10` | af_za ar_sa ca_es cs_cz da_dk de_de el_gr en_us fi_fi fr_fr he_il hu_hu id_id it_it ja_jp jv_id ko_kr nl_nl no_no pl_pl pt_br pt_pt ro_ro ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw |
| Ars Elemental | `ars_elemental, minecraft, ars_nouveau, ars_creo` | `0.7.10.1` | de_de el_gr en_us fr_fr it_it ja_jp ko_kr pt_br pt_pt ru_ru tr_tr uk_ua zh_cn zh_tw |
| Ars Nouveau | `ars_nouveau, neoforge, curios, geckolib` | `5.13.1` | af_za ar_sa ca_es cs_cz da_dk de_de el_gr en_us fi_fi fr_fr he_il hu_hu it_it ja_jp ko_kr nl_nl no_no pl_pl pt_br pt_pt ro_ro ru_ru sr_sp sv_se tr_tr uk_ua vi_vn zh_cn zh_tw |
| Arsenal (RPG Series) | `arsenal, neoforge, minecraft, spell_engine, ranged_weapon_api` | `1.5.0` | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn |
| AzureLib | `azurelib, neoforge, minecraft` | `3.1.11` | en_us fr_fr ru_ru zh_cn |
| Better Combat [Fabric & Forge] | `bettercombat, neoforge, minecraft, playeranimator, cloth_config` | `2.4.0+1.21.1` | de_de en_us es_ar es_mx fr_fr it_it ja_jp ko_kr pt_br ru_ru uk_ua vi_vn zh_cn |
| Better Party | `better_party, neoforge, minecraft` | `1.1.5` | de_de en_us fr_fr pt_br ru_ru |
| BetterEnd: New Dawn | `betterend, neoforge, minecraft, bclib, wover, wunderlib` | `21.0.34` | de_de en_gb en_us ko_kr pt_br ru_ru thai_th tr_tr zh_cn |
| Biomes O' Plenty | `biomesoplenty, neoforge, glitchcore, terrablender` | `21.1.0.14` | cs_cz de_de en_us es_ar es_cl es_mx fr_fr it_it ja_jp kk_kz ko_kr nl_nl nn_no pl_pl pt_br ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw |
| Cloth Config API (Fabric/Forge/NeoForge) | `cloth_config, neoforge` | `15.0.140` | bg_bg de_de en_ud en_us es_mx et_ee fr_fr hu_hu it_it ja_jp kk_kz ko_kr lol_us lzh pt_br ru_ru sv_se tt_ru uk_ua zh_cn zh_hk zh_tw |
| Configured | `configured, neoforge, minecraft, framework, jei` | `2.6.3` | de_de en_us it_it ru_ru |
| Connected Glass | `connectedglass, neoforge, minecraft, supermartijn642corelib, fusion` | `1.1.14` | de_at de_ch de_de en_us es_ar es_cl es_mx es_uy es_ve fr_fr it_it ja_jp ko_kr nl_be nl_nl ru_ru tr_tr uk_ua vi_vn |
| Corail Tombstone | `tombstone, neoforge, minecraft, iris` | `9.5.5` | en_us fr_fr nl_nl pt_br ru_ru zh_cn |
| Create | `create, neoforge, minecraft, flywheel, ponder, sodium, lithium, journeymap, xaeroworldmap, radium, palladium` | `6.0.10` | af_za ar_sa be_by bel_tr bg_bg ca_es cs_cz cy_gb da_dk de_de el_gr en_gb en_pt en_ud en_us enws eo_uy es_cl es_mx et_ee eu_es fa_ir fi_fi fr_ca fr_fr he_il hr_hr hu_hu hy_am id_id is_is it_it ja_jp kk_kz ko_kr ksh lol_us lt_lt lt_lv lzh nl_nl no_no pl_pl pt_br pt_pt qep ro_ro rpr ru_ru sv_se th_th tok tr_tr uk_ua vi_vn vp_vl zh_cn zh_tw |
| Dawn Of Time | `dawnoftimebuilder, neoforge, minecraft, fusion` | `1.6.6` | af_za ar_sa ca_es cs_cz da_dk de_de el_gr en_us fi_fi fr_fr he_il hu_hu id_id it_it ja_jp jv_id ko_kr la_la lo_la nl_nl no_no pl_pl pt_br pt_pt ro_ro ru_ru sr_sp sv_se tr_tr uk_ua vi_vn zh_cn zh_tw |
| Deeper and Darker | `deeperdarker, minecraft, neoforge` | `1.4.1` | ca_es de_de en_au en_ca en_gb en_nz en_pt en_us fr_ca fr_fr he_il it_it ja_jp ko_kr la_la lol_us nl_be nl_nl pl_pl pt_br pt_pt ro_ro ru_ru sl_si sv_se tr_tr uk_ua vi_vn zh_cn zh_hk zh_tw |
| Embeddium | `embeddium, neoforge, sodium` | `1.0.15+mc1.21.1` | de_de en_us fr_fr uk_ua zh_cn |
| Enchantment Descriptions | `enchdesc, neoforge, minecraft, bookshelf, prickle` | `21.1.11` | bg_bg de_de en_ca en_us es_ar es_cl es_mx fil_ph fr_fr it_it ja_jp ko_kr nl_be nl_nl pl_pl pt_br ru_ru sv_se ta_in tr_tr uk_ua vi_vn zh_cn zh_tw |
| Equivalent Legacy | `equivalent_legacy, neoforge, minecraft, regalia_slots_api, jei, wthit` | `0.0.0-beta.4` | cs_cz de_de en_au en_gb en_ud en_us fr_fr it_it ja_jp ru_ru tr_tr uk_ua zh_cn |
| Explorer's Compass | `explorerscompass, neoforge, minecraft` | `1.21.1-3.4.0-neoforge` | de_de en_us fr_fr ja_jp pt_br ru_ru tr_tr uk_ua zh_cn zh_tw |
| Farmer's Delight | `farmersdelight, neoforge, minecraft, crafttweaker` | `1.3.4` | be_by bg_bg ca_es da_dk de_de en_gb en_nz en_pt en_us es_ar es_cl es_ec es_mx es_uy es_ve fi_fi fr_ca fr_fr hu_hu id_id it_it ja_jp kk_kz ko_kr lol_us lzh nl_be nl_nl no_no pl_pl pt_br pt_pt ru_ru sk_sk sr_sp sv_se tok tr_tr uk_ua vi_vn vp_vl zh_cn zh_hk zh_tw |
| Guard Villagers | `guardvillagers, neoforge, minecraft` | `2.4.12` | cs_cz de_de en_us es_mx fil_ph fr_fr it_it ja_jp ko_kr pl_pl pt_br ro_ro ru_ru tr_tr uk_ua vi_vn zh_cn zh_tw |
| Iron's Spells 'n Spellbooks | `irons_spellbooks, neoforge, minecraft, geckolib, playeranimator, curios, irons_lib` | `1.21.1-3.16.3` | en_us es_mx fr_fr it_it ja_jp ko_kr pl_pl pt_br ru_ru uk_ua vi_vn zh_cn zh_hk zh_tw |
| Jade | `jade, neoforge` | `15.10.6+neoforge` | de_de en_us it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru uk_ua zh_cn zh_tw |
| Jewelry (RPG Series) | `jewelry, neoforge, minecraft, spell_power, ranged_weapon_api, structure_pool_api, curios` | `2.4.0` | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn zh_tw |
| Just Enough Items (JEI) | `jei, neoforge, minecraft` | `19.51.0.418` | ar_sa bg_bg cs_cz de_de el_gr en_us es_ar es_ec fi_fi fil_ph fr_fr he_il hu_hu id_id it_it ja_jp kk_kz ko_kr lt_lt lzh no_no pl_pl pt_br pt_pt ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw |
| Just Enough Resources (JER) | `jeresources, jei` | `1.6.0.17` | de_de en_us es_ar fr_fr it_it ja_jp ko_kr nl_nl pt_br pt_pt ru_ru zh_cn zh_tw |
| L_Ender 's Cataclysm | `cataclysm, neoforge, minecraft, curios, lionfishapi` | `3.33` | en_us es_ar es_cl es_mx fr_ca fr_fr hu_hu it_it ja_jp ko_kr pl_pl pt_br ru_ru tr_tr uk_ua vi_vn zh_cn zh_tw |
| Lootr (Forge & NeoForge) | `lootr, minecraft, neoforge` | `1.21.1-1.11.38.124` | af_za ar_sa ca_es cs_cz da_dk de_de el_gr en_us es_mx fi_fi fr_fr he_il hu_hu it_it ja_jp ko_kr lol_us nl_nl no_no pl_pl pt_br pt_pt ro_ro ru_ru sr_sp sv_se tr_tr uk_ua vi_vn zh_cn zh_tw |
| Macaw's Bridges | `mcwbridges` | `3.1.2` | de_de en_us es_cl es_mx fr_fr it_it ja_jp ko_kr pt_br ru_ru sk_sk tr_tr uk_ua zh_cn |
| Macaw's Stairs | `mcwstairs` | `1.0.2` | en_us es_cl es_mx fr_fr ja_jp ko_kr pt_br ru_ru zh_cn |
| Macaw's Windows | `mcwwindows` | `2.4.2` | de_de en_us es_cl es_mx fr_fr it_it ja_jp ko_kr pt_br ru_ru tr_tr uk_ua zh_tw |
| Moonlight Lib | `moonlight, minecraft` | `1.21.1-3.6.0` | en_us es_ar fr_fr ja_jp pt_br ru_ru uk_ua vi_vn zh_cn |
| Mowzie's Mobs | `mowziesmobs, neoforge, minecraft, geckolib` | `1.8.2` | de_de en_us es_mx fr_fr it_it ja_jp ko_kr pt_br ru_ru uk_ua zh_cn zh_tw |
| Mystical Agriculture | `mysticalagriculture, neoforge, minecraft, cucumber` | `8.0.28` | de_de en_us es_ar es_mx fr_fr ja_jp ko_kr pl_pl pt_br ru_ru tr_tr uk_ua zh_cn zh_tw |
| Nature's Compass | `naturescompass, neoforge, minecraft` | `1.21.1-3.4.0-neoforge` | de_de en_us eo_uy es_ec es_mx fr_fr hy_am it_ch it_it ja_jp kk_kz ko_kr pl_pl pt_br ru_ru sv_se tr_tr uk_ua zh_cn zh_tw |
| NeOculus | `oculus, iris, neoforge, minecraft, embeddium` | `1.8.7` | cs_cz de_ch de_de en_pt en_ud en_us es_ar et_ee fa_ir fi_fi fr_fr hu_hu it_it ja_jp ko_kr lol_us lzh nl_nl pl_pl pr_pt pt_br ru_ru sk_sk th_th tr_tr uk_ua zh_cn zh_tw |
| Obscure Tooltips | `obscure_tooltips, minecraft, neoforge, fragmentum` | `4.2.4` | en_us ja_jp pt_br pt_pt ru_ru tok zh_cn |
| Paladins & Priests (RPG Series) | `paladins, neoforge, minecraft, armor_model_api, spell_engine, runes` | `3.1.1` | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn |
| Patchouli | `patchouli, neoforge, minecraft` | `1.21.1-93-NEOFORGE` | cs_cz de_de en_us fr_fr it_it ko_kr pl_pl pt_br ru_ru uk_ua zh_cn |
| Quark | `quark, neoforge, zeta, biolith, lootr` | `4.1-482` | de_de en_gb en_nz en_pt en_us es_ar es_cl es_mx fi_fi fr_fr hu_hu it_it ja_jp ko_kr pl_pl pt_br pt_pt ru_ru sv_se tok uk_ua zh_cn zh_tw |
| Ranged Weapon API | `ranged_weapon_api, neoforge, minecraft` | `3.0.0+1.21.1` | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn |
| Regalia Slots API | `regalia_slots_api, neoforge, minecraft, curios, neoforge, minecraft` | `0.0.0-beta.12` | de_de en_us fr_fr it_it ja_jp ko_kr lzh pl_pl pt_br ru_ru tok tr_tr uk_ua vi_vn zh_cn zh_tw |
| Regrowth | `regrowth, neoforge, minecraft` | `21.34.7` | de_de en_us fr_fr hi_in it_it ja_jp ko_kr no_no pt_br ru_ru uk_ua zh_cn |
| Relics | `relics, minecraft, neoforge, curios, octolib` | `0.10.7.8` | en_us ja_jp ko_kr ru_ru zh_cn |
| Rogues & Warriors (RPG Series) | `rogues, neoforge, minecraft, armor_model_api, spell_engine, structure_pool_api` | `3.1.1` | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn |
| Runes | `runes, neoforge, minecraft` | `1.3.2+1.21.1` | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn |
| Sophisticated Backpacks | `sophisticatedbackpacks, sophisticatedcore, neoforge, minecraft` | `3.25.78` | de_de en_us es_mx fr_fr ja_jp ko_kr lzh pl_pl pt_br ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw |
| Sophisticated Core | `sophisticatedcore, jei, neoforge, minecraft` | `1.4.90` | de_de en_us es_mx ja_jp ko_kr lzh pt_br ru_ru tr_tr uk_ua zh_cn |
| Spell Engine | `spell_engine, neoforge, minecraft, cloth_config, playeranimator, spell_power, curios` | `1.10.5` | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn |
| Storage Drawers | `storagedrawers, minecraft, neoforge` | `13.11.4` | de_de en_us fr_fr ja_jp ko_kr nl_nl pt_br pt_pt ru_ru zh_cn zh_tw |
| Supplementaries | `supplementaries, neoforge, minecraft, moonlight, create, amendments, farmersdelight, sodium` | `1.21.1-3.9.6` | ca_es cs_cz de_de en_gb en_pt en_us es_ar es_mx fi_fi fr_ca fr_fr hu_hu it_it ja_jp kk_kz ko_kr ms_my pl_pl pt_br pt_pt ru_ru sr_sp tok tr_tr uk_ua vi_vn zh_cn zh_tw |
| Vellumli | `vellumli, neoforge, minecraft` | `0.0.0-beta.1` | cs_cz de_de en_us fr_fr it_it ko_kr pl_pl pt_br ru_ru uk_ua zh_cn |
| VillagersPlus (Fabric/Neoforge) | `villagersplus, neoforge, minecraft, villagertradingplus` | `4.0.0+mc1.21.1` | de_de en_us fr_fr it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru uk_ua zh_cn |
| VillagersTradingPlus | `villagertradingplus, neoforge, minecraft` | `1.0.0+mc1.21.1` | de_de en_us fr_fr it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru uk_ua zh_cn |
| Waystones | `waystones, neoforge, minecraft, balm` | `21.1.42` | cs_cz de_de en_us es_ar es_cl es_mx fr_fr hu_hu it_it ja_jp ko_kr no_no pl_pl pt_br pt_pt ru_ru sv_se tr_tr uk_ua vi_vn zh_cn zh_tw |
| Wizards (RPG Series) | `wizards, neoforge, minecraft, armor_model_api, spell_engine, runes, structure_pool_api` | `3.1.2` | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn |
| Workhand Tool | `workhand_tools, neoforge, minecraft, vellumli` | `0.0.0-beta.3` | de_de en_us fr_fr it_it ja_jp ko_kr pt_br ru_ru zh_cn |
| Xaero's Minimap | `xaerominimap, neoforge, minecraft, openpartiesandclaims, xaeroworldmap, xaerolib` | `26.4.2` | cs_cz da_dk de_de el_gr en_us es_ar es_mx et_ee fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr lv_lv nl_nl pl_pl pt_br pt_pt ru_ru sr_sp th_th tr_tr uk_ua vi_vn zh_cn |
| YetAnotherConfigLib | `yet_another_config_lib_v3, neoforge, minecraft` | `3.8.2+1.21.1-neoforge` | be_by de_at de_ch de_de el_gr en_us es_ar et_ee fr_fr it_it ja_jp ms_my nl_nl pl_pl pt_br pt_pt ru_ru sl_si tt_ru uk_ua zh_cn zh_tw zlm_arab |

---

## 4. Mods sin es_es que NUESTRO resource pack cubre

Total: 62

Columna 'Alcance': 'propio' = el RP traduce el namespace principal del mod; 'solo dependencia' = el RP solo cubre namespaces compartidos que el mod empaqueta como compat (create, supplementaries, quark, jei...), por lo que las cadenas propias del mod pueden seguir sin traducir.

| Mod | modid principal | Version | Namespace(s) es_es en el RP | Alcance | Locales del mod |
|---|---|---|---|---|---|
| Ace's Spell Utils | `aces_spell_utils` | `1.2.7.2-1.21.1` | aces_spell_utils | propio | en_us |
| Apothic Enchanting | `apothic_enchanting` | `1.6.2` | apothic_enchanting, placebo | propio | en_us fr_fr ja_jp ko_kr pt_br ru_ru tr_tr vi_vn zh_cn |
| Apothic Spawners | `apothic_spawners` | `1.4.0` | apothic_spawners, placebo | propio | en_us pt_br ru_ru tr_tr uk_ua zh_cn |
| Aquaculture Delight (A Farmer's Delight Add-on) | `aquaculturedelight` | `1.1.0` | aquaculturedelight | propio | en_us ru_ru |
| Ars Additions | `ars_additions` | `1.21.1-21.3.0` | ars_additions, ars_nouveau | propio | en_us zh_cn |
| Ars Creo | `ars_creo` | `5.4.0` | ars_creo, ars_nouveau, create | propio | en_us pt_br zh_cn |
| AttributeFix | `attributefix` | `21.1.3` | bookshelf | solo dependencia | (ninguno) |
| Balm | `balm` | `21.0.65` | balm | propio | en_us es_ar es_mx it_it pt_br tr_tr |
| BCLib: New Dawn | `bclib` | `21.0.26` | bclib, wover | propio | de_de en_us ko_kr pt_br ru_ru tr_tr uk_ua zh_cn |
| Better Party X Xaero's World Map | `better_party_x_xaeros_world_map` | `1.0.0` | better_party_x_xaeros_world_map, xaeroworldmap | propio | de_de en_us |
| Better Villager Animations | `bettervillageranimations` | `1.0.0` | bettervillageranimations | propio | ar_sa en_us |
| Bookshelf | `bookshelf` | `21.1.81` | bookshelf | propio | en_us es_ar ja_jp pt_br zh_cn |
| Butchery | `butchery` | `5.2` | butchery, jei | propio | en_us |
| Carry Mechanics | `carry_mechanics` | `0.0.0-beta.2` | carry_mechanics | propio | en_us |
| Crafting Tweaks | `craftingtweaks` | `21.1.11` | balm, craftingtweaks | propio | en_us es_mx fr_fr pl_pl pt_br pt_pt ru_ru sv_se uk_ua zh_cn |
| Cucumber Library | `cucumber` | `8.0.16` | cucumber | propio | en_us fr_fr ja_jp ko_kr pt_br ru_ru uk_ua zh_cn |
| Dangerous - Just A Difficulty Mod | `dangerous` | `1.5.2` | dangerous | propio | en_us |
| Data Miner | `data_miner` | `0.0.0-beta.2` | data_miner | propio | en_us |
| Embeddium (Rubidium) Extra | `embeddium_extra` | `0.5.7e+mc1.21-build.132` | embeddium, sodium-extra | solo dependencia | cs_cz de_at de_ch de_de el_gr en_us es_ar es_mx et_ee fi_fi fr_ca fr_fr hu_hu it_it ja_jp ko_kr ms_my pl_pl pt_br pt_pt ru_ru th_th tr_tr uk_ua vi_vn zh_cn zh_hk zh_tw |
| Every Compat (Wood Good) | `everycomp` | `1.21-2.11.50` | create, everycomp, moonlight | propio | de_de en_us es_cl es_mx ja_jp zh_cn |
| Farmers Delight: Pizza Lovers | `farmer_delight_pizza_lovers` | `1.0.0` | farmer_delight_pizza_lovers, jei | propio | en_us |
| Farmer's Sandwiches (A Farmer's Delight Add-on) | `farmers_sandwiches` | `0.1.2` | farmers_sandwiches | propio | en_us |
| Fusion (Connected Textures) | `fusion` | `1.3.15` | fusion | propio | en_us hu_hu tr_tr |
| Info Tab | `info_tab` | `0.0.0-beta.1` | info_tab | propio | en_us |
| Integrated Cataclysm | `integrated_cataclysm` | `1.0.6+1.21.1-neoforge` | cataclysm, create, quark, supplementaries | solo dependencia | en_us |
| Integrated Dungeons and Structures | `idas` | `1.13.7+1.21.1-neoforge` | create, idas, quark, supplementaries | propio | en_us zh_cn |
| Integrated Stronghold | `integrated_stronghold` | `1.1.4+1.21.1-neoforge` | create, integrated_stronghold, quark, supplementaries | propio | en_us |
| Integrated Villages | `integrated_villages` | `1.3.3+1.21.1-neoforge` | create, supplementaries | solo dependencia | (ninguno) |
| Inventory Essentials | `inventoryessentials` | `21.1.18` | balm, inventoryessentials | propio | en_us zh_tw |
| Iron's Lib | `irons_lib` | `1.21.1-2.1.0` | irons_lib, irons_patreon_lib | propio | en_us |
| Just Enough Breeding (JEBr) | `justenoughbreeding` | `3.2.1` | justenoughbreeding | propio | de_de en_us es_ar fr_fr ja_jp pt_pt ru_ru uk_ua zh_cn zh_tw |
| Just Enough Professions (JEP) | `justenoughprofessions` | `4.0.5` | jei, justenoughprofessions | propio | en_us es_ar ja_jp pt_br tr_tr zh_cn |
| Just-In NETHER | `just_in_nether` | `1.0.0` | just_in_nether | propio | en_us zh_tw |
| Lionfish API | `lionfishapi` | `3.1` | lionfishapi | propio | en_us |
| Macaw's Roofs | `mcwroofs` | `2.3.2` | mcwroofs | propio | de_de en_us es_cl es_mx fr_fr ja_jp ru_ru tr_tr uk_ua |
| MES - Moog's End Structures | `moogs_structures` | `?` | mes, moogs_structures | propio | en_us |
| MNS - Moog's Nether Structures | `moogs_structures` | `?` | mns, moogs_structures | propio | en_us |
| ModernFix | `modernfix` | `5.27.24+mc1.21.1` | jei, modernfix | propio | de_de en_us es_mx it_it ja_jp ru_ru vi_vn zh_cn zh_tw |
| Moog's Structure Lib (moogs_structures) | `moogs_structures` | `3.1.2` | moogs_structures | propio | en_us |
| More Villagers | `morevillagers` | `6.0.0` | morevillagers | propio | de_de en_us no_no pl_pl ru_ru zh_cn zh_tw |
| Mowzie's Cataclysm | `mowzies_cataclysm` | `1.2.2` | cataclysm, mowzies_cataclysm, mowziesmobs | propio | en_us |
| Mystical Automation | `mysticalautomation` | `1.0.7` | cucumber, mysticalagriculture, mysticalautomation | propio | en_us ja_jp pt_br zh_cn |
| Not Enough Crashes (Forge) | `notenoughcrashes` | `4.4.9+1.21.1` | notenoughcrashes | propio | de_de en_us et_ee fr_fr ja_jp ms_my pt_br ro_ro ru_ru uk_ua zh_cn zh_hk zh_tw zlm_arab |
| Pillager Caravans | `caravans` | `3.0.0` | caravans | propio | en_us pt_br |
| Placebo | `placebo` | `9.9.2` | placebo | propio | en_us fr_fr it_it ko_kr pt_br ru_ru tr_tr uk_ua zh_cn |
| Player Activity View | `player_activity_view` | `0.0.0-beta.1` | player_activity_view | propio | en_us |
| Reliquary Reincarnations | `reliquary` | `2.0.80` | reliquary | propio | en_us ja_jp ko_kr pt_br ru_ru uk_ua zh_cn |
| SKD Menu | `skd_menu` | `0.0.0-beta.4` | skd_menu | propio | en_us |
| Sophisticated Backpacks: Ars Compat / Sophisticated Backpacks Ars-Nouveau Compatibility | `arssophisticatedcompat` | `0.3.0` | ars_nouveau, arssophisticatedcompat, sophisticatedbackpacks, sophisticatedcore | propio | en_us |
| Spell Power Attributes | `spell_power` | `1.6.0+1.21.1` | spell_power | propio | cs_cz de_de en_us es_ar fr_fr hr_hr hu_hu id_id it_it ja_jp ko_kr nl_nl pl_pl pt_br ru_ru sv_se th_th tr_tr uk_ua vi_vn zh_cn |
| SuperMartijn642's Core Lib | `supermartijn642corelib` | `1.1.24` | supermartijn642corelib | propio | en_us |
| Teleport Animation | `teleport_animation` | `1.1.0` | teleport_animation, waystones | propio | en_us ja_jp |
| TerraBlender (NeoForge) | `terrablender` | `4.1.0.8` | terrablender | propio | de_de en_gb en_us pt_br ru_ru sv_se tr_tr uk_ua |
| Tom's Simple Storage Mod | `toms_storage` | `2.4.2` | toms_storage | propio | en_us fr_fr ja_jp ko_kr pt_br ru_ru zh_cn |
| Utility Nexus Fixes | `utility_nexus_fixes` | `0.0.0-beta.3` | iris | solo dependencia | (ninguno) |
| Visual Workbench | `visualworkbench` | `21.1.2` | visualworkbench | propio | en_us |
| Wishful Recipes | `wishfulrecipes` | `1` | wishfulrecipes | propio | en_us |
| WorldWeaver: New Dawn | `wover` | `21.0.25` | wover, wover-generator, wover-ui | propio | de_de en_us ru_ru |
| Xaero's World Map | `xaeroworldmap` | `1.44.2` | xaerobetterpvp, xaerominimap, xaeroworldmap | propio | de_de en_us |
| YUNG's Better End Island (NeoForge) [1.20.4 - 1.21.1 ONLY] | `betterendisland` | `1.21.1-NeoForge-3.1.2` | betterendisland | propio | en_us ru_ru |
| Zeta | `zeta` | `1.1-40` | zeta | propio | en_us ru_ru zh_cn |
| Zombie Hordes | `horde_hoard` | `1.1.0` | horde_hoard | propio | en_us |

---

## 5. Mods sin es_es que NO cubrimos (huecos)

### 5a. Tienen texto (lang/ con al menos un locale) pero nada en espanol

Total: 1

| Mod | modid | Version | Locales que SI trae el mod |
|---|---|---|---|
| Waystone Towers | `waystone_towers, neoforge, minecraft` | `1.0.9` | en_us |

### 5b. Sin ningun archivo lang/ en el jar

Normalmente librerias, mods de rendimiento o mods con texto minimo/generado. No siempre requieren traduccion.

Total: 41

| Mod | modid | Version |
|---|---|---|
| Architectury API | `architectury, minecraft, neoforge` | `13.0.11` |
| Armor Model API | `armor_model_api, neoforge, minecraft` | `1.1.0+1.21.1` |
| AttributeFix-Sync | `attributefixsync, neoforge, minecraft, attributefix` | `0.0.2` |
| Better End Cities Better End | `` | `?` |
| Bundle API | `bundleapi, neoforge, minecraft` | `1.1.0` |
| Cataclysm & BetterCombat - Compatibility | `` | `?` |
| Cataclysmic Combat | `cataclysmiccombat, neoforge, minecraft` | `1.4.1` |
| Clean Swing Through Grass | `cleanswing, neoforge, minecraft` | `1.9` |
| Connectivity | `connectivity, neoforge, minecraft, cupboard` | `7.6` |
| Cupboard | `cupboard, minecraft` | `4.1` |
| CustomSkinLoader | `customskinloader-bootstrap` | `15.0.1` |
| Deimos Lib | `deimos, neoforge, minecraft` | `2.7` |
| Fast Async World Save[Forge/Neo/Fabric] | `fastasyncworldsave, minecraft, cupboard` | `2.6` |
| Fast IP Ping | `fastipping, minecraft` | `1.0.11` |
| FerriteCore ((Neo)Forge) | `ferritecore, neoforge, minecraft` | `7.0.3` |
| fix GPU memory leak | `gpumemleakfix, minecraft, cupboard` | `1.8` |
| Fragmentum [NeoForge Edition] | `fragmentum, minecraft, neoforge` | `2.4.4` |
| GeckoLib | `geckolib, neoforge, minecraft, geckoanimfix` | `4.9.2` |
| GlitchCore | `glitchcore, neoforge` | `2.1.0.2` |
| Golems Are Friends Not Fodder | `golemsarefriends, neoforge, minecraft` | `1.21.1-1.0.1` |
| Illager Structures | `illagerstructures, neoforge, minecraft` | `0.1.2` |
| ImmediatelyFast | `immediatelyfast, minecraft, neoforge` | `1.6.13+1.21.1` |
| Integrated API | `integrated_api, minecraft` | `1.8.0` |
| Jauml | `jauml, neoforge, minecraft` | `2.1.1` |
| Mouse Tweaks | `mousetweaks` | `2.26.1` |
| Much More Dungeons | `muchmoredungeons, neoforge, minecraft` | `1.2.0` |
| Nether Trials & Chambers | `hellish_trials, neoforge, minecraft, architectury` | `1.0.5` |
| playerAnimator | `playeranimator, minecraft` | `2.0.4+1.21.1` |
| Prickle | `prickle, neoforge, minecraft` | `21.1.11` |
| Puzzles Lib | `puzzleslib, minecraft, neoforge` | `21.1.56` |
| ShatterLib / OctoLib | `octolib, neoforge, minecraft, architectury` | `0.6.2` |
| Shield API | `shield_api, neoforge, minecraft` | `2.2.0` |
| Structure Essentials | `structureessentials, minecraft, cupboard` | `5.0` |
| Structure Pool API | `structure_pool_api, neoforge, minecraft` | `1.2.1+1.21.1` |
| Towers of the Wild Modded | `totw_modded, neoforge, minecraft` | `1.0.9` |
| Towers of the Wild Modded - Extra Towers | `` | `?` |
| TT20 (TPS Fixer) | `tt20, minecraft` | `0.8.4` |
| Utility Nexus Admin | `utility_nexus_admin, neoforge, minecraft` | `0.0.0-beta.13` |
| Villager Guards (Fabric/Forge/NeoForge/Quilt) | `` | `?` |
| WunderLib: New Dawn | `wunderlib, neoforge, minecraft` | `21.0.10` |
| YUNG's API (NeoForge) [1.20.4-1.21.1 ONLY] | `yungsapi, minecraft, neoforge` | `1.21.1-NeoForge-5.1.8` |

---

## 6. Namespaces del resource pack sin mod asociado en este modpack

Namespaces con lang/ en el RP que no casan con ningun modid ni carpeta assets/<ns>/lang de los jars de v5.134.4. Suelen ser sub-namespaces de compat, libros Patchouli, o restos de versiones anteriores del modpack.

Total: 2

| Namespace RP | Locales presentes en el RP |
|---|---|
| `ascendant_spawners` | es_es |
| `common_toolkit` | es_es |

---

## 7. Detalle: contenido lang/ del resource pack por namespace

| Namespace | Locales en el RP | es_es |
|---|---|---|
| `aces_spell_utils` | es_es | si |
| `apothic_enchanting` | es_es | si |
| `apothic_spawners` | es_es | si |
| `aquaculture` | es_es | si |
| `aquaculturedelight` | es_es | si |
| `aquamirae` | es_es | si |
| `armoroftheages` | es_es | si |
| `ars_additions` | es_es | si |
| `ars_creo` | es_es | si |
| `ars_elemental` | es_es | si |
| `ars_nouveau` | es_es | si |
| `arssophisticatedcompat` | es_es | si |
| `ascendant_spawners` | es_es | si |
| `balm` | es_es | si |
| `bclib` | es_es | si |
| `better_party_x_xaeros_world_map` | es_es | si |
| `bettercombat` | es_es | si |
| `betterend` | es_es | si |
| `betterendisland` | es_es | si |
| `bettervillageranimations` | es_es | si |
| `biomesoplenty` | es_es | si |
| `bookshelf` | es_es | si |
| `butchery` | es_es | si |
| `caravans` | es_es | si |
| `carry_mechanics` | es_es | si |
| `cataclysm` | es_es | si |
| `common_toolkit` | es_es | si |
| `configured` | es_es | si |
| `craftingtweaks` | es_es | si |
| `create` | es_es | si |
| `cucumber` | es_es | si |
| `dangerous` | es_es | si |
| `data_miner` | es_es | si |
| `dawnoftimebuilder` | es_es | si |
| `deeperdarker` | es_es | si |
| `embeddium` | es_es | si |
| `enchdesc` | es_es | si |
| `everycomp` | es_es | si |
| `farmer_delight_pizza_lovers` | es_es | si |
| `farmers_sandwiches` | es_es | si |
| `farmersdelight` | es_es | si |
| `fusion` | es_es | si |
| `guardvillagers` | es_es | si |
| `horde_hoard` | es_es | si |
| `idas` | es_es | si |
| `info_tab` | es_es | si |
| `integrated_stronghold` | es_es | si |
| `inventoryessentials` | es_es | si |
| `iris` | es_es | si |
| `irons_lib` | es_es | si |
| `irons_patreon_lib` | es_es | si |
| `irons_spellbooks` | es_es | si |
| `jade` | es_es | si |
| `jei` | es_es | si |
| `jeresources` | es_es | si |
| `just_in_nether` | es_es | si |
| `justenoughbreeding` | es_es | si |
| `justenoughprofessions` | es_es | si |
| `lionfishapi` | es_es | si |
| `mcwbridges` | es_es | si |
| `mcwroofs` | es_es | si |
| `mes` | es_es | si |
| `mns` | es_es | si |
| `modernfix` | es_es | si |
| `moogs_structures` | es_es | si |
| `moonlight` | es_es | si |
| `morevillagers` | es_es | si |
| `mowzies_cataclysm` | es_es | si |
| `mowziesmobs` | es_es | si |
| `mysticalagriculture` | es_es | si |
| `mysticalautomation` | es_es | si |
| `naturescompass` | es_es | si |
| `notenoughcrashes` | es_es | si |
| `obscure_tooltips` | es_es | si |
| `placebo` | es_es | si |
| `player_activity_view` | es_es | si |
| `quark` | es_es | si |
| `regalia_slots_api` | es_es | si |
| `relics` | es_es | si |
| `reliquary` | es_es | si |
| `skd_menu` | es_es | si |
| `sodium-extra` | es_es | si |
| `sophisticatedbackpacks` | es_es | si |
| `sophisticatedcore` | es_es | si |
| `spell_power` | es_es | si |
| `supermartijn642corelib` | es_es | si |
| `supplementaries` | es_es | si |
| `teleport_animation` | es_es | si |
| `terrablender` | es_es | si |
| `tombstone` | es_es | si |
| `toms_storage` | es_es | si |
| `vellumli` | es_es | si |
| `villagertradingplus` | es_es | si |
| `visualworkbench` | es_es | si |
| `waystones` | es_es | si |
| `wishfulrecipes` | es_es | si |
| `workhand_tools` | es_es | si |
| `wover` | es_es | si |
| `wover-generator` | es_es | si |
| `wover-ui` | es_es | si |
| `xaerobetterpvp` | es_es | si |
| `xaerominimap` | es_es | si |
| `xaeroworldmap` | es_es | si |
| `zeta` | es_es | si |
