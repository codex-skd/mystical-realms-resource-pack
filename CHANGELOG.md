# Changelog

Todos los cambios notables de Mystical Realms Resource Pack se documentan en este archivo.

El formato sigue [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)
y el proyecto adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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
