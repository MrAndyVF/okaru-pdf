# Changelog

Each version has an English and a Spanish section. / Cada versión tiene una sección en inglés y otra en español.

## [1.0.2] - 2026-11-25

### English

#### Changes
- Dialog cards get a 2 px accent border, like OKARU panels.
- Released with OKARU 1.4.0, which brings square controls and 2 px borders to every app.
- CI: an optional `.okaru-core-ref` file builds the app against an unpublished okaru-core (branch, tag or commit).

### Español

#### Cambios
- Las tarjetas de diálogo llevan un borde de acento de 2 px, como los paneles de OKARU.
- Sale con OKARU 1.4.0, que trae controles cuadrados y bordes de 2 px a todas las apps.
- CI: un archivo `.okaru-core-ref` opcional compila la app contra un okaru-core sin publicar (rama, etiqueta o
  commit).

## [1.0.1] - 2026-11-22

### English

#### Changes
- Packaging: the package is **tied to the system libraries it was built against**. When a system update would
  rename one of them, pacman refuses it and names this package, instead of leaving the app unable to start; it goes
  through once OKARU publishes it rebuilt. Released with OKARU 1.3.8.

### Español

#### Cambios
- Empaquetado: el paquete queda **atado a las bibliotecas del sistema con las que se compiló**. Si una actualización
  del sistema le cambiaría el nombre a alguna, pacman se niega y nombra este paquete, en vez de dejar la app sin
  abrir; pasa en cuanto OKARU lo publica recompilado. Sale con OKARU 1.3.8.

## [1.0.0] - 2026-11-14

### English

#### Changes
- First release as its own package and repository. The document viewer used to ship inside `okaru` (up to 1.2.4); it now
  builds against the shared core (`okaru-core`) and carries its own translations.

### Español

#### Cambios
- Primera versión como paquete y repositorio propios. El visor de documentos venía dentro de `okaru` (hasta la 1.2.4); ahora
  se compila contra el núcleo compartido (`okaru-core`) y trae sus propias traducciones.
