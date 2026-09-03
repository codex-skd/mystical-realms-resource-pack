<h1>Mystical Realms Translation &amp; Fixes</h1>

<p>Companion resource pack for the <strong>Mystical Realms</strong> modpack (Minecraft 1.21.1, NeoForge).
It bundles <strong>Spanish (es_es) translations</strong> and <strong>small asset fixes</strong> for the
included mods <strong>without editing the mods themselves</strong>, so everything survives mod updates
and can be served straight from the game server.</p>

<h2>Spanish translations</h2>

<p>Adds <code>es_es</code> language files for <strong>101 mod namespaces</strong> (~12,500 keys) that
either shipped no Spanish locale at all or an incomplete one. Item, block and entity names, tooltips
and GUI text that used to show up in English (or as raw <code>translation.keys</code>) now appear in
Spanish.</p>

<p>Minecraft merges language files across resource packs, so for mods that already had a partial
Spanish translation this pack only fills in the missing keys &mdash; it never overwrites work the mod
authors or their translators already did. Source text is each mod's own <code>en_us.json</code>.</p>

<p>Covered mods include Every Compat, Butchery, Reliquary, Supplementaries, Ars Nouveau,
Iron's Spells 'n Spellbooks, BetterEnd, Quark, Create, Farmer's Delight, JEI, Waystones, Xaero's
Minimap / World Map, Macaw's Roofs, Biomes O' Plenty, Deeper and Darker, L_Ender's Cataclysm,
Sophisticated Backpacks, Tom's Simple Storage, Corail Tombstone and dozens more &mdash; see the
changelog for the full list.</p>

<h2>Asset fixes</h2>

<ul>
<li><strong>Butchery</strong> &mdash; replaces an orphan <code>ravager_carcass</code> model file that has
an illegal element rotation, which otherwise makes Minecraft's model loader print an <code>ERROR</code>
on every startup. Purely a log-noise fix; no visual change in-game.</li>
</ul>

<h2>Install</h2>

<p>Bundled with the Mystical Realms modpack. It is also served by the official server via
<code>server.properties</code> (<code>resource-pack</code> + <code>resource-pack-sha1</code>), so it
downloads automatically when you join.</p>

<p>Standalone: drop <code>MysticalRealms_TranslationFixes-&lt;version&gt;.zip</code> into
<code>resourcepacks/</code> and enable it in <em>Options &rarr; Resource Packs</em>. Set your game
language to <em>Español (España)</em> to see the translations.</p>

<h2>Requirements</h2>

<ul>
<li>Minecraft <strong>1.21.1</strong> (resource pack format 34)</li>
</ul>

<h2>Credits</h2>

<p>Maintained by <strong>Stalking Dragons</strong>. Translations are derived from each mod's own English
locale. Ravager carcass geometry is the mod author's own corrected model, redistributed here under the
fix.</p>
