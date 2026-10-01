# ZSA Voyager Keymap

Mein persönliches Keymap-Layout für das ZSA Voyager.

- Bearbeitet in [Oryx](https://configure.zsa.io) und als QMK-Quellcode exportiert nach `qmk/zsa_voyager_default-v2_source/`.
- Das Layout ist auf Windows ausgerichtet; für den Mac gibt es einen Zusatz-Layer (Layer 3).
- Geflasht wird über Oryx (Compile) und [Keymapp](https://www.zsa.io/flash).

## Bedienung
- **`Alt+Tab` (Windows):** Alt-Combo halten (`D`+`F` oder `J`+`K`) und mit dem linken Daumen Tab tippen.
- **`Cmd+Tab` (Mac, Layer 3):** Tab-Daumen halten (= `Cmd`) und links unten außen Tab tippen.
- **Großbuchstaben/Shift-Zeichen:** Taste länger halten (Auto Shift).

## Änderungen

### 2026-10-01: Ctrl auf dem Mac, Combos verlegt
- **Layer 3 (Mac):** rechts unten außen jetzt `Left Ctrl` (vorher fiel sie auf `Cmd` durch); die extra eingetragenen `W`/`E` sind wieder durchlässig.
- **Alt-Combo:** `M`+`,` → `J`+`K`.
- **Tab-Combo:** `W`+`E` → `X`+`C` (`we` kommt beim Tippen zu oft vor).

### 2026-10-01: Tap Dances raus, Mac-Tab umgezogen
- **Tap Dances auf `Z` und `/` entfernt:** wieder normale Tasten; großes `Z` und `?` kommen jetzt über Auto Shift (gleiches Timing wie alle anderen Buchstaben). `zz`/`//` per Doppeltipp und Right Alt fallen weg.
- **Layer 3 (Mac):** `Tab` von links außen in der Q-Reihe nach links unten außen verschoben (für `Cmd+Tab`). Damit ist Caps Word auf dem Mac wieder da.
- **Combo:** `W`+`E` gleichzeitig = `Tab`.

### 2026-10-01: Mac-Layer und Alt-Combos
- **Layer 3 (Mac):** neuer Layer, der nur wenige Tasten überschreibt: der Tab-Daumen ist gehalten `Cmd` (statt `Ctrl`), links außen in der Q-Reihe liegt `Tab` (statt Caps Word). Alles andere fällt auf Layer 0 durch.
- **Umschalten:** auf Layer 2 (Space halten) schaltet die `0`-Position fest auf Layer 3 (Mac), die Taste rechts oben außen zurück auf Layer 0 (Windows).
- **Layer 0:** links unten außen jetzt One-Shot-Alt (antippen = Alt für die nächste Taste, halten = normales Alt).
- **Combos:** `D`+`F` und `M`+`,` gleichzeitig gedrückt = `Left Alt` (Mac: Option).
- **LEDs:** auf Layer 0 leuchten nur zwei LEDs, alle anderen sind aus; auf Layer 3 läuft die normale RGB-Animation.

### 2026-09-29: Alt besser erreichbar machen
Unter Windows wird Alt oft gebraucht (`Alt+Tab`, `Alt+F4`, Menüs). Bisher gab es Alt nur über „zweimal tippen und halten“ auf `Z`/`/`.

- **Layer 0:** links unten außen jetzt `Left Alt` (vorher `Win`); rechts unten außen jetzt `Win` (vorher `Right Ctrl`). `Alt+Tab` geht so mit einer Hand (Alt + Tab-Daumen).
- **Layer 1:** `Left Alt` auf der Z-Position; links unten außen zusätzlich `` ` ``.
- **Tap Dance `Z`:** halten = großes `Z` (vorher: nichts).
- **Tap Dance `/`:** halten = `?` (vorher: nichts).
