# Configuración de escritorio

Este repositorio vive en `~/.config` y versiona una selección de configuraciones personales; no es una copia completa de ese directorio.

## Contenido

- `alacritty/`: configuración y tema de la terminal.
- `niri/`: configuración KDL derivada de la plantilla de CachyOS (`cachyos-niri-noctalia`), con personalizaciones locales. `cfg/display.kdl` conserva la disposición específica de los monitores; las reglas incluyen el backdrop difuminado de Noctalia.
- `noctalia/`: configuración, paletas y fondos de pantalla de Noctalia. La paleta activa es Rose Pine Classic; su color de superficie tiñe el backdrop de Niri.
- `zed/`: ajustes seleccionados y tema personalizado de Zed basado en la paleta Rose Pine Classic de Noctalia.
- `AGENTS.md`: pautas para trabajar en este repositorio con OpenCode.

## Entorno de referencia

Versiones observadas en CachyOS rolling el 2026-10-12; son una referencia del entorno donde se mantiene esta configuración, no requisitos ni versiones fijadas por el repositorio:

- `cachyos-niri-noctalia`: `1.4.0-1` (plantilla de configuración de CachyOS).
- `niri`: `26.04-1.1`.
- `noctalia`: `5.2.1-1.1`.

El `.gitignore` limita intencionalmente qué partes de `~/.config` se versionan. En Niri se versionan `config.kdl` y los módulos `cfg/*.kdl`; se excluyen el archivo vacío `config` y `config.kdl.bak`. Para validar cambios, ejecuta `niri validate` y `noctalia config validate`. Estas comprobaciones validan la configuración, no garantizan por sí solas el comportamiento visual o la integración en una sesión activa. No hay un flujo general de instalación ni pruebas automatizadas definido en la raíz.
