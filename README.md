# mikesokol.ch

Persönliche Webseite von Mike Sokol, veröffentlicht über GitHub Pages (Jekyll wird von GitHub automatisch gebaut).

## Wo was steht

| Was | Datei |
|---|---|
| Texte, Bilder, Reihenfolge der Abschnitte pro Reiter | `_seiten/*.md` (nur der Teil zwischen den `---`) |
| Name, LinkedIn-Link, Fusszeile | `_data/einstellungen.yml` |
| Bilder | `img/` |
| Aussehen (Farben, Schrift, Abstände) | `style.css` |
| Aufbau der Seite | `_layouts/default.html`, `_includes/abschnitt.html` |

## Bausteine eines Abschnitts

Jeder Eintrag unter `abschnitte:` ist ein Block. Alles ist freiwillig – was leer bleibt, wird nicht angezeigt.

- `titel`, `text` (Absätze mit Leerzeile trennen, Aufzählung mit `- `)
- `hintergrund: grau`
- `bild`, `bild_text`, `bild_2`, `bild_2_text`, `bild_seite: links`
- `stationen` (Zeitstrahl mit `zeit` und `text` – Daten immer in Anführungszeichen, z. B. `"07.2024"`)
- `karten` (Kästchen mit `titel`, `zeit`, `text`, `knopf_text`, `knopf_link`)
- `stichworte` (runde Etiketten)
- `knopf_text`, `knopf_link`
- `sichtbar: false` blendet einen Abschnitt oder eine Karte aus, ohne ihn zu löschen

Neuer Reiter: Datei in `_seiten/` kopieren, `titel` und `menue_position` anpassen.

## Lokal ansehen

```bash
jekyll serve
```
