<h1>Mystical Realms Resource Pack</h1>

<p>Companion resource pack for the <strong>Mystical Realms</strong> modpack (Minecraft 1.21.1, NeoForge).
It bundles small asset fixes for included mods <strong>without editing the mods themselves</strong>, so
they survive mod updates and can be served straight from the game server.</p>

<h2>What it fixes</h2>

<ul>
<li><strong>Butchery</strong> &mdash; replaces an orphan <code>ravager_carcass</code> model file that has
an illegal element rotation, which otherwise makes Minecraft's model loader print an <code>ERROR</code>
on every startup. Purely a log-noise fix; no visual change in-game.</li>
</ul>

<h2>Install</h2>

<p>Bundled with the Mystical Realms modpack. It is also served by the official server via
<code>server.properties</code> (<code>resource-pack</code> + <code>resource-pack-sha1</code>), so it
downloads automatically when you join.</p>

<p>Standalone: drop <code>MysticalRealms_ResourcePack-&lt;version&gt;.zip</code> into
<code>resourcepacks/</code> and enable it in <em>Options &rarr; Resource Packs</em>.</p>

<h2>Requirements</h2>

<ul>
<li>Minecraft <strong>1.21.1</strong> (resource pack format 34)</li>
</ul>

<h2>Credits</h2>

<p>Maintained by <strong>Stalking Dragons</strong>. Ravager carcass geometry is the mod author's own
corrected model, redistributed here under the fix.</p>
