# okaru-pdf

**English** · [Español](#español)

The document viewer of [OKARU](https://github.com/MrAndyVF/okaru) (郁): read, search, fill in forms, highlight and print PDF documents, with the shell's look and theme.

## Install

It ships in OKARU's pacman repository `[okaru]` (set up by OKARU's installer):

```sh
sudo pacman -S okaru-pdf
```

## Build

It builds against OKARU's shared core, provided by the `okaru-core` package:

```sh
meson setup build && meson compile -C build
# Run it with the translations from this repository:
OKARU_APPS_DIR=$PWD/apps ./build/okaru-pdf
```

Translations live in `apps/pdf/translations/` (English and Spanish).

## License

MIT.

---

## Español

El visor de documentos de [OKARU](https://github.com/MrAndyVF/okaru) (郁): leer, buscar, rellenar formularios, resaltar e imprimir documentos PDF, con el aspecto y el tema de la shell.

### Instalar

Viene en el repositorio pacman de OKARU, `[okaru]` (lo configura el instalador de OKARU):

```sh
sudo pacman -S okaru-pdf
```

### Compilar

Se compila contra el núcleo compartido de OKARU, que trae el paquete `okaru-core`:

```sh
meson setup build && meson compile -C build
# Ejecutarla con las traducciones de este repositorio:
OKARU_APPS_DIR=$PWD/apps ./build/okaru-pdf
```

Las traducciones están en `apps/pdf/translations/` (inglés y español).

### Licencia

MIT.
