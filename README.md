# Configuración de escritorio

Este repositorio vive en `~/.config` y versiona una selección de configuraciones personales; no es una copia completa de ese directorio.

## Contenido

- `alacritty/`: configuración y tema de la terminal.
- `niri/`: línea base de configuración instalada por CachyOS (`cachyos-niri-noctalia`), organizada en módulos KDL. `cfg/display.kdl` conserva la disposición específica de los monitores de esta máquina; los atajos, reglas y el inicio de sesión dependen en parte de Noctalia y de las aplicaciones configuradas.
- `noctalia/`: configuración, paletas y fondos de pantalla de Noctalia.
- `zed/`: ajustes seleccionados y tema personalizado de Zed basado en la paleta Rose Pine Classic de Noctalia.
- `AGENTS.md`: pautas para trabajar en este repositorio con OpenCode.

El `.gitignore` limita intencionalmente qué partes de `~/.config` se versionan. En Niri se versionan `config.kdl` y los módulos `cfg/*.kdl`; se excluyen el archivo vacío `config` y `config.kdl.bak`. La configuración de Niri se validó con `niri validate`. No hay un flujo general de instalación ni pruebas automatizadas definido en la raíz; valida cada cambio con la aplicación correspondiente.
