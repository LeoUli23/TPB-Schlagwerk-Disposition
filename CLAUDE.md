# CLAUDE.md – TPB-Schlagwerk-Disposition (öffentlich, GitHub Pages)

Instrumentenübersicht / Schlagwerk-Planer unter https://leouli23.github.io/TPB-Schlagwerk-Disposition/ (früher „Untertitel-Studio“), eine Seite (`index.html`), in der TPB-App als Werkzeug eingebettet. Speichert nur im Gerät (localStorage `tpb_instrumente_v1`), kein Login, keine Datenbank. Sicherheitsregeln: `SICHERHEIT.md` – vor jeder Änderung lesen.

## Prüfung

Bei jedem Pull Request läuft „Release Prüfung“ mit Gitleaks (`.gitleaks.toml`). Von Hand: Handy-Breite 320 bis 390 px ohne seitliches Scrollen (F-013).

## Regeln

- Änderungen nur nach Leos Go als Pull Request auf eigenem Branch; Leo mergt, Claude mergt nie.
- Keine Geheimwerte, keine personenbezogenen Daten in diesem öffentlichen Repository.
- Schriften (Inter, Space Grotesk) aus `schrift/`, jsPDF aus `bibliothek/`, jeweils mit Lizenzdatei; nie von Google Fonts oder CDNs laden (wie F-032). Die Prüfung schlägt fehl, wenn index.html eine fremde Adresse lädt.
- Gedächtnis-Dokumente schreibt nur der App-Chat (siehe CLAUDE.md der TPB-App).
