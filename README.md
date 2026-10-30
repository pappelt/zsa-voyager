# ZSA Voyager Keymap

Mein persönliches Keymap-Layout für das ZSA Voyager.

- Bearbeitet in [Oryx](https://configure.zsa.io) und als QMK-Quellcode exportiert nach `qmk/zsa_voyager_default-v2_source/`.
- Das Layout ist auf Windows ausgerichtet. Am Mac sind in den macOS-Einstellungen (Tastatur → Sondertasten, nur für das Voyager) `Ctrl` und `Cmd` vertauscht, damit dieselben Shortcuts funktionieren.
- Geflasht wird über Oryx (Compile) und [Keymapp](https://www.zsa.io/flash).

## Bedienung
- **Shortcut-Layer (Layer 3):** Combo `J`+`K` oder `D`+`F`. Antippen = Layer nur für die nächste Taste, halten = Layer solange gehalten.
- **Modifier auf Layer 3 (Grundreihe):** `S` = Shift, `F`/`J` = Alt, `G`/`H` = Ctrl, `K` = Win (Mac: Ctrl). Je nach Combo hat die freie Hand Alt unter dem Zeigefinger.
- **Befehlspalette:** Layer 3, `P` = `Ctrl+Shift+P` (Mac: `Cmd+Shift+P`), am besten mit `D`+`F`.
- **`Alt+Tab` (Windows):** `J`+`K` halten, `F` (= Alt) halten und mit dem linken Daumen Tab tippen; mit `S` dazu rückwärts. Mit `D`+`F` liegt Alt auf `J`.
- **`Cmd+Tab` (Mac):** `J`+`K` halten, `G` (Ctrl → durch macOS-Tausch `Cmd`) halten, Daumen-Tab tippen. Alternativ Daumen halten und Combo `C`+`V` (= Tab).
- **Tab-Daumen:** tippen = Tab, halten = Ctrl.
- **Tab ohne Daumen:** Combo `C`+`V`.
- **Großbuchstaben/Shift-Zeichen:** Taste länger halten (Auto Shift, Timeout 185 ms).
- **Trackpad (Navigator):** Sobald das Trackpad bewegt wird, schaltet sich Layer 4 (Auto-Mouse) für 450 ms ein: `R`/`V` = Linksklick, `E`/`C` = Mittelklick, `W`/`X` = Rechtsklick, Backspace-Daumen = Linksklick, Tab-Daumen = Ctrl. Der Space-Daumen ist dort ohne Funktion.
- **Markieren mit Pfeiltasten:** Space halten (Layer 2), Tab-Daumen halten (= Shift), Pfeile auf `H J K L`.
- **Browser-Tabs:** auf Layer 2 `M` = `Ctrl+Bild↑`, `.` = `Ctrl+Bild↓`.

## Änderungen

### 2026-10-30: Layer 2 aufgeräumt, Medien-Layer ausgelagert, Trackpad-Daumen
- **Layer 2:** nur noch Navigation. Neu: Shift auf dem Tab-Daumen; Tab-Wechsel mit `Ctrl+Bild↑`/`Ctrl+Bild↓` auf `M` und `.` (am Mac wird daraus durch den Ctrl/Cmd-Tausch `Cmd+Bild↑`/`Cmd+Bild↓`).
- **Layer 5 (neu):** Medien, Lautstärke, RGB und die alten Tab-Shortcuts sind von Layer 2 hierher gezogen. Noch keine Taste führt auf diesen Layer.
- **Layer 1:** rechts auf der Grundreihe `:` statt `+` und `P` statt `*`.
- **Layer 4:** Tab-Daumen = Ctrl, Backspace-Daumen = Linksklick, Space-Daumen ohne Funktion.
- **Auto-Mouse:** Timeout 450 ms.
- **LEDs:** eigene Farben für Layer 2.

### 2026-10-22: Tap Dance auf dem Tab-Daumen wieder raus
- **Tab-Daumen:** zurück auf `MT(Ctrl, Tab)`. Der Tap Dance hat bei schnellem `Ctrl+C` & Co. als Tab gefeuert und jedes Tab verzögert.
- **Layer 3:** `Ctrl+Shift+P` (Befehlspalette) jetzt auf `P`; `Win` neu auf `K`.

### 2026-10-22: Modifier auf der Grundreihe von Layer 3, Tap Dance auf dem Tab-Daumen
- **Layer 3:** `Alt` von `G`/`H` nach `F`/`J`, `Ctrl` neu auf `G`/`H`, `Shift` neu auf `S`.
- **Layer 3:** links oben außen `Meh` jetzt normal gehalten statt One-Shot.
- **Tab-Daumen:** `MT(Ctrl, Tab)` → Tap Dance: tippen = Tab, halten = Ctrl, zweimal tippen = 2× Tab, zweimal tippen und halten = `Ctrl+Shift+P`.
- **LEDs:** Farben für die neuen Modifier auf Layer 3.

### 2026-10-22: Navigator Trackpad, Shortcut-Layer erweitert
- **Navigator Trackpad** eingebunden (Oryx-Module `zsa/navigator_trackpad` und `zsa/automouse`).
- **Layer 4 = Auto-Mouse-Layer:** Maustasten auf `W`/`E`/`R` und `X`/`C`/`V`, Rest durchlässig. Wird ab 5 Bewegungseinheiten automatisch aktiv.
- **Layer 3 (Shortcuts) erweitert:**
  - `Alt` von `F` auf `G` und `H` verlegt (je nach Combo erreichbar)
  - `Ctrl+W` auf `W`, `Win+Tab` (Task-Ansicht) auf `B`
  - links unten außen `Win+Shift+S` (Screenshot)
  - links außen Q-Reihe `Ctrl+Alt+Shift+1`, links oben außen One-Shot-`Meh` (`Ctrl+Alt+Shift`)
- **Auto Shift:** Timeout explizit auf 185 ms.
- **LEDs:** eigene Farben für Layer 0, 1, 3 und 4.

### 2026-10-05: Shortcut-Layer statt Mac-Layer
- **Mac-Layer entfernt:** Ctrl/Cmd werden jetzt in macOS getauscht statt in der Firmware. Die Umschalttasten `TO(3)`/`TO(0)` auf Layer 2 sind weg.
- **Layer 3 = Shortcut-Layer** (linke Hand):
  - Z-Reihe: `Ctrl+Z`, `Ctrl+X`, `Ctrl+C`, `Ctrl+V`
  - A-Reihe: `Ctrl+A` auf `A`, `Alt` auf `F`
  - Zahlenreihe: Zoom `Ctrl+-` auf `3`, `Ctrl+=` auf `4`, `Ctrl+0` auf `5`
- **Combos:** `J`+`K` und `D`+`F` öffnen jetzt Layer 3 als One-Shot-Layer (vorher `Alt`); Tab-Combo `X`+`C` → `C`+`V`.
- **LEDs:** eigene LED-Belegung für Layer 0 entfernt, überall läuft die normale RGB-Animation.

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
