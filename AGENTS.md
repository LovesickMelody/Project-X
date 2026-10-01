# AGENTS.md – Hauptanweisungen für KI-Agenten

Diese Datei legt fest, wie KI-Agenten (z. B. Claude Code) in diesem Projekt arbeiten.
Sie gilt für jede Sitzung und jede Aufgabe.

## Projekt in einem Satz

**Project-X** ist eine Lernplattform für **KI-Manager**: Fach- und Führungskräfte, die KI-Projekte
in Unternehmen verantworten, strategisch planen, einführen und steuern.

## Pflichtablauf in jeder Sitzung

1. **Zuerst `STATUS.md` lesen.** Sie enthält den aktuellen Projektstand, offene Aufgaben und
   getroffene Entscheidungen. Nichts tun, bevor der Stand bekannt ist.
2. **Aufgabe mit dem Stand abgleichen.** Passt die Anfrage zu einer offenen Aufgabe? Widerspricht
   sie einer getroffenen Entscheidung? Dann kurz nachfragen statt raten.
3. **Aufgabe erledigen.** Klein, nachvollziehbar, in sich abgeschlossen.
4. **`STATUS.md` aktualisieren, sobald eine Aufgabe erfolgreich erledigt ist:**
   - Aufgabe von „Offen“/„In Arbeit“ nach „Erledigt“ verschieben (mit Datum).
   - Neue Erkenntnisse, Entscheidungen oder Folgeaufgaben eintragen.
   - Abschnitt „Aktueller Stand“ und „Zuletzt aktualisiert“ anpassen.
5. **Committen und pushen** – Code-Änderungen und das Update von `STATUS.md` gemeinsam.

## Arbeitsprinzipien

- **Sprache:** Kommunikation mit der Projektinhaberin und Dokumentation auf **Deutsch**.
  Code, Variablen-, Datei- und Funktionsnamen auf **Englisch**.
- **Zielgruppe im Blick behalten:** Inhalte und UI richten sich an Manager, nicht an Entwickler.
  Klar, praxisnah, ohne unnötigen Fachjargon; Fachbegriffe beim ersten Auftreten erklären.
- **Kleine Schritte:** Lieber mehrere kleine, funktionierende Zwischenstände als ein großer Wurf.
- **Keine stillen Annahmen bei wichtigen Entscheidungen:** Technologie-Stack, Bezahlmodell,
  Datenschutz, Hosting und Design werden mit der Projektinhaberin abgestimmt und dann in
  `STATUS.md` unter „Entscheidungen“ festgehalten.
- **Ehrlich berichten:** Wenn etwas nicht funktioniert, Tests fehlschlagen oder ein Schritt
  übersprungen wurde, wird das klar gesagt – und in `STATUS.md` vermerkt.
- **Datenschutz & Recht:** Die Plattform richtet sich (voraussichtlich) an den DACH-Raum.
  DSGVO-Konformität und der EU AI Act sind von Anfang an mitzudenken.
- **Barrierefreiheit:** Oberflächen sollen gut lesbar, tastaturbedienbar und mobil nutzbar sein.

## Struktur der Dokumentation

| Datei        | Zweck                                                                 |
|--------------|-----------------------------------------------------------------------|
| `AGENTS.md`  | Dauerhafte Regeln und Arbeitsweise (ändert sich selten)               |
| `STATUS.md`  | Aktueller Projektstand, To-dos, Entscheidungen (ändert sich ständig)  |
| `CLAUDE.md`  | Verweist auf `AGENTS.md`, damit Claude Code die Regeln automatisch lädt |

Diese Datei (`AGENTS.md`) wird nur angepasst, wenn sich grundlegende Regeln ändern – und nur in
Absprache mit der Projektinhaberin.

## Git-Konventionen

- Aussagekräftige Commit-Nachrichten (kurze Zusammenfassung, bei Bedarf Details darunter).
- Keine Zugangsdaten, API-Schlüssel oder persönlichen Daten ins Repository committen.
- Pull Requests nur nach ausdrücklicher Aufforderung erstellen.
