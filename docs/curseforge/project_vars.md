# CurseForge — Variables del proyecto

## Proyecto

| Variable | Valor |
|----------|-------|
| `curseforge_project_id` | `1679111` |
| `mod_id` | `mystical_realms_resource_pack` |
| `display_name` | `Mystical Realms Resource Pack` |
| `summary` | `A server-synced companion resource pack for the Mystical Realms modpack that ships lightweight fixes for broken model, texture and sound assets in bundled mods, without editing the mods themselves.` |
| Categoría (class Resource Packs) | `Data Packs` (no es un pack de resolución) |

## Tokens

El API token de CurseForge es **de cuenta**, el mismo que el resto de proyectos de Stalking Dragons
(ver `enchantventure-pack/docs/curseforge/project_vars.md`). No se versiona aquí.

- Autenticación Upload: cabecera `X-Api-Token`
- Autenticación Core (GET): cabecera `x-api-key`

## Versión actual

| Variable | Valor |
|----------|-------|
| `minecraft_version` | `1.21.1` |
| `pack_format` | `34` |
| `environment` | `Client` (se descarga y aplica en el cliente) |

## Rama

```
minecraft/1.21.1/resourcepack/production
```

## Tag

Formato: `<mc-version>-<version>`
Ejemplo: `1.21.1-0.0.0-beta.1`

## Parámetros del upload

| Campo | Valor | Notas |
|-------|-------|-------|
| `displayName` | `Mystical Realms Resource Pack (0.0.0-beta.1)` | `display_name (version)` |
| `changelog` | HTML (no Markdown) | `docs/curseforge/versions/<version>.md` |
| `changelogType` | `html` | Obligatorio |
| `releaseType` | `beta` | Según el tipo de versión |
| `gameVersions` | `[11779]` | `gameVersionId` de Minecraft 1.21.1 (no el pack format) |

> `gameVersions` usa el `gameVersionId` de Minecraft (de `GET /v1/minecraft/version`), **no** el pack
> format 34. `11779` = Minecraft 1.21.1, ya validado en `mystical_realms_data_pack` y demás repos 1.21.1
> de Stalking Dragons.

## Estructura del changelog (HTML)

```html
<h2>v0.0.0-beta.1 - Initial release</h2>

<h3>Added</h3>
<ul>
<li><strong>Butchery <code>ravager_carcass</code> fix</strong>: replaces an orphan model file with an
illegal <code>-90</code> element rotation by the mod's own corrected sibling model. Silences a startup
<code>ERROR</code> from MC's bulk model loader. No in-game visual change.</li>
</ul>

<hr>

<p><strong>ZIP</strong>: <code>MysticalRealms_ResourcePack-0.0.0-beta.1.zip</code></p>
```

## Variables parseables (para scripts)

El script `scripts/curseforge-upload.ps1` lee estas líneas (`key = value`). Rellenar tras crear el
proyecto:

```
project_id = 1679111
api_token = ee776b0a-ee95-4850-b554-06be02a8657f
game_versions = 11779
release_type = beta
```

## Flujo completo

1. `python build_pack.py`
2. Actualizar `docs/curseforge/versions/<version>.md` con HTML
3. Actualizar `CHANGELOG.md`
4. `git commit -m "chore: bump version to <version>"` + `git push`
5. `git tag -a 1.21.1-<version> -m "v<version>: descripción"` + `git push origin <tag>`
6. Subir ZIP a CurseForge con `scripts/curseforge-upload.ps1`
7. Actualizar la URL + SHA1 del server pack en `server.properties` del servidor
8. Verificar con GET que el changelog se vea bien
