# ZSA Voyager Keymap

Mein persönliches Keymap-Layout für das ZSA Voyager.

- Bearbeitet in [Oryx](https://configure.zsa.io) und als QMK-Quellcode exportiert nach `qmk/zsa_voyager_default-v2_source/`.
- Das Layout ist auf Windows ausgerichtet.
- Geflasht wird über Oryx (Compile) und [Keymapp](https://www.zsa.io/flash).

## Änderungen

### 2026-09-29: Alt besser erreichbar machen
Unter Windows wird Alt oft gebraucht (`Alt+Tab`, `Alt+F4`, Menüs). Bisher gab es Alt nur über „zweimal tippen und halten“ auf `Z`/`/`.

- **Layer 0:** links unten außen jetzt `Left Alt` (vorher `Win`); rechts unten außen jetzt `Win` (vorher `Right Ctrl`). `Alt+Tab` geht so mit einer Hand (Alt + Tab-Daumen).
- **Layer 1:** `Left Alt` auf der Z-Position; links unten außen zusätzlich `` ` ``.
- **Tap Dance `Z`:** halten = großes `Z` (vorher: nichts).
- **Tap Dance `/`:** halten = `?` (vorher: nichts).
