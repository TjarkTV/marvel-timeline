# Marvel-Wegweiser

Eine interaktive Übersicht über alle Marvel-Filme und -Serien: in welcher Reihenfolge sie erschienen sind, wo sie in der Handlung liegen und wie sie zusammenhängen.

Die Seite ist eine einzelne HTML-Datei ohne Build-Schritt und ohne Server.

## Was die Seite kann

- **Zeitachse als Liniennetzplan.** Jede Reihe (Iron Man, Thor, Guardians …) ist eine farbige Linie, jeder Film eine Station. Wo Geschichten zusammenlaufen, biegen die Linien in den gemeinsamen Film ein.
- **Zwei Reihenfolgen.** Umschaltbar zwischen Erscheinungsreihenfolge und Chronologie der Handlung.
- **Abhaken.** Gesehene Titel werden markiert. Daraus ergeben sich der Fortschritt und der Vorschlag, was als Nächstes dran ist.
- **Spoilerschutz.** Was in einem Titel passiert, überraschende Auftritte und die Übergänge zwischen den Filmwelten erscheinen erst, wenn der jeweilige Titel abgehakt ist.
- **Steckbriefe.** Rund 45 Figuren mit Fähigkeiten, Hintergrund, Comic-Herkunft und Darstellern.
- **Mehr als das MCU.** Enthalten sind auch die Netflix-Serien, die ABC-Serien, die X-Men- und Fantastic-Four-Filme von Fox, Sonys Spider-Man-Filme und Blade.

## Benutzen

`index.html` im Browser öffnen, oder das Repository über GitHub Pages veröffentlichen (Settings → Pages → Branch `main`, Ordner `/`).

Die Häkchen werden nur lokal im Browser gespeichert (`localStorage`). Es werden keine Daten übertragen.

## Daten anpassen

Alle Inhalte stehen als Daten am Anfang des Skripts in `index.html`:

- `TITLES`: Filme und Serien mit Datum, Handlungszeit, Voraussetzungen (`before`) und Folgetiteln (`leadsTo`)
- `CHARS`: Figuren mit Auftritten und Entwicklungen je Titel
- `DOCKS` und `UNIINFO`: Übergänge und Erklärungen zu den Filmwelten

Ein Auftritt mit vorangestelltem `!` gilt als Überraschung und bleibt verborgen, bis der Titel abgehakt ist.

## Hinweise

- Datumsangaben sind US-Starttermine. Stand der Daten: November 2026.
- Die Einordnung in die Handlungschronologie ist bei vielen neueren Titeln nur ungefähr, weil es keine offiziellen Jahresangaben gibt.
- Inoffizielles Fanprojekt, nicht mit Marvel oder Disney verbunden. Alle Namen und Titel gehören ihren jeweiligen Inhabern.
