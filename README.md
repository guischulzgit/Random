# Zufallsauswahl – mündliche Beteiligung

Ein einzelnes `index.html`-Programm für den Unterricht: Schülerinnen und Schüler werden
aus einer Namensliste per Zufall für die mündliche Beteiligung aufgerufen.
Läuft direkt vom USB-Stick im Browser (Edge/Chrome) – ohne Installation.

## So wird es benutzt

1. `index.html` von diesem Repository herunterladen und auf den USB-Stick legen.
2. Ebenfalls auf den Stick legen:
   - `logo.png` (oder `logo.jpg`, `logo.jpeg`, `logo.webp`, `logo.gif`, `logo.svg`) –
     dein Logo. Es erscheint oben rechts und liefert auch die Farben des Designs.
     Solange kein Logo vorhanden ist, wird ein neutraler Dunkelblau-Ton benutzt.
   - eine oder mehrere **Namenslisten als `.txt`** (z. B. `Klasse 7a.txt`),
     jeweils ein Name pro Zeile (maximal 35 Namen)
3. `index.html` per Doppelklick öffnen.
4. Auf der Startseite den Stick-Ordner wählen (Schaltfläche **„Ordner öffnen“**) –
   alle gefundenen Listen werden ohne Dateiendung angezeigt. Ab 8 Einträgen wird
   gescrollt, wie im Dateimanager.
5. Liste anklicken (oder mit **↑/↓** auswählen und **Enter** drücken).

## Steuerung

| Taste | Wirkung |
| --- | --- |
| `Leertaste` | Neuer zufälliger Name |
| `Esc` | Zurück zur Listenauswahl |
| `Esc` (auf der Startseite) | Programm beenden* |
| `↑` / `↓` + `Enter` | Liste per Tastatur auswählen |

\* Manche Browser erlauben das automatische Schließen nicht – dann erscheint ein
Hinweis und der Tab muss von Hand geschlossen werden.

## Einzelheiten

- Ausgewählte Namen werden nicht erneut vorgeschlagen, bis jeder Name einmal dran war;
  danach wird die Liste **unbemerkt neu gemischt**.
- `.txt`-Dateien werden als UTF-8 **oder** Windows-ANSI (windows-1252) gelesen –
  beides funktioniert, ganz ohne Einstellung.
- Umlaute (ä, ö, ü, ß) werden korrekt angezeigt.
- Unten links steht das Kürzel **UH**, unten in der Mitte die Steuerungshinweise.
- Farbschema folgt dem Logo (wird automatisch aus `logo.png` ausgewertet).

## Projektstruktur

```
index.html    Das komplette Programm (eine Datei)
README.md     Diese Anleitung
```

Auf dem Stick einfach `logo.png` und die `*.txt`-Listen danebenlegen – fertig.
