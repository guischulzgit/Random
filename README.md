# Zufallsauswahl – mündliche Beteiligung

Ein einzelnes `index.html`-Programm für den Unterricht: Schülerinnen und Schüler werden
aus einer Namensliste per Zufall für die mündliche Beteiligung aufgerufen.
Läuft direkt vom USB-Stick im Browser – ohne Installation.

> **Empfehlung: Edge oder Chrome.** Diese Browser merken sich den gewählten Ordner
> (nach einem einzigen Klick beim ersten Start erscheinen die Klassen danach bei
> jedem Start automatisch). Firefox erlaubt das Merken aus Sicherheitsgründen nicht –
> dort muss der Ordner bei jedem Start neu gewählt werden.

## So wird es benutzt

1. `index.html` von diesem Repository herunterladen und auf den USB-Stick legen.
2. Ebenfalls auf den Stick legen:
   - `logo.png` (oder `logo.jpg`, `logo.jpeg`, `logo.webp`, `logo.gif`, `logo.svg`) –
     dein Logo. Es erscheint oben rechts und liefert auch die Farben des Designs.
     Solange kein Logo vorhanden ist, wird ein neutraler Dunkelblau-Ton benutzt.
   - eine oder mehrere **Namenslisten als `.txt`** (z. B. `Klasse-A.txt`),
     jeweils ein Name pro Zeile (maximal 35 Namen)
3. `index.html` per Doppelklick öffnen.
4. Beim **ersten Start** den Stick-Ordner wählen (Schaltfläche **„Ordner öffnen“**) –
   alle Dateien des Ordners werden ohne Dateiendung angezeigt (das Programm selbst
   und das Logo nicht). Ab 8 Einträgen wird gescrollt, wie im Dateimanager.
   Der gewählte Ordner wird **gemerkt**: Bei jedem weiteren Start erscheinen die
   Klassen sofort. Über **„📂 Anderen Ordner wählen“** kann jederzeit ein
   anderer Ordner (z. B. eine andere Klasse auf einem anderen Stick) gewählt werden.

   Tipps, wenn eine Liste scheinbar fehlt:
   - Windows blendet Dateiendungen oft aus. Eine Datei, die in Word erstellt wurde,
     heißt vielleicht in Wahrheit `Datei.TXT.docx` – im Programm erscheint sie als
     „Datei.TXT“ und meldet beim Anklicken, dass sie keine `.txt`-Datei ist.
   - Die Liste muss **im selben Ordner** liegen wie `index.html` (bzw. in dem Ordner,
     den man auf der Startseite auswählt).
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
- Es werden nur echte `.txt`-Dateien geöffnet (Groß-/Kleinschreibung egal: `.txt`,
  `.TXT`); andere Dateien bleiben sichtbar, zeigen beim Anklicken aber den echten
  Dateinamen als Hinweis.
- `.txt`-Dateien werden als UTF-8 **oder** Windows-ANSI (windows-1252) gelesen –
  beides funktioniert, ganz ohne Einstellung.
- Umlaute (ä, ö, ü, ß) werden korrekt angezeigt.
- Unten links steht das Kürzel **UH**, unten in der Mitte die Steuerungshinweise.
- Farbschema folgt dem Logo (wird automatisch aus `logo.png` ausgewertet).

## Projektstruktur

```
index.html      Das komplette Programm (eine Datei)
Klasse-A.txt    Beispielliste (30 Namen, zum Testen/Ausprobieren)
Klasse-B.txt    Beispielliste (30 Namen, zum Testen/Ausprobieren)
README.md       Diese Anleitung
```

Die beiden Beispieldateien können durch echte Klassenlisten ersetzt bzw. gelöscht
werden. Auf dem Stick einfach `logo.png` und die `*.txt`-Listen danebenlegen – fertig.
