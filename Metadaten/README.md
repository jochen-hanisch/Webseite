---
author: Jochen Hanisch-Johannsen
title: README
Repository: https://github.com/jochen-hanisch/webseite
created: 2025-10-27
updated: 2025-10-27
publish: false
tags:
published: 2025-10-27
---

# Webseite – Open Research and Knowledge Hub

## Überblick

Dieses Repository bündelt die Markdown-Inhalte meiner beruflichen Webseite. Der Open Research and Knowledge Hub (ORKH) dokumentiert Forschungsarbeiten, Beratungsangebote sowie reflektierte Praxis an der Schnittstelle von Bildungswissenschaft, Systemik und Gesundheitsberufen. Die Texte entstehen in Obsidian, werden kontinuierlich in Git versioniert und unter der GNU AGPL v3 veröffentlicht. Ziel ist ein nachvollziehbarer, dialogorientierter Veröffentlichungsprozess: Versionierung macht Denkschritte sichtbar, Veröffentlichung markiert bewusst gesetzte Referenzen.

## Struktur der Inhalte

- [`Herzlich Willkommen.md`](Herzlich%20Willkommen.md) – Einstieg in den ORKH, leitende Haltung und Forschungsfelder.
- [`Hinweise.md`](Allgemein%20beruflich/Webseite/Metadaten/Hinweise.md) – Dokumentation der epistemischen und versionsbezogenen Arbeitsweise einschließlich Commit-Typen und Git-Logik.
- [`Curriculum Vitae.md`](Curriculum%20Vitae.md) – Verweis auf den gepflegten Europass-Lebenslauf und Einbettung in die Versionierungspraxis.
- Fach- und Angebotsseiten wie [`Wissenschaftler.md`](Wissenschaftler.md), [`Systemischer Berater.md`](Systemischer%20Berater.md), [`Soziotherapeut.md`](Soziotherapeut.md), [`Therapiebegleithund.md`](Allgemein%20beruflich/Webseite/Human-Services/Therapiebegleithund.md) oder [`Lehrender.md`](Lehrender.md) erläutern Rollen, Projekte und Haltung.
- Rechtliche Grundlagen (`Impressum.md`, `Datenschutz.md`, `Disclaimer.md`, `Allgemeine Geschäftsbedingungen.md`) sichern Transparenz und erfüllen die Anforderungen für den professionellen Auftritt.
- [`public.md`](public.md) bündelt Links zu interaktiven Visualisierungen und datengestützten Analysen, die über `echo.jochen-hanisch.de` bereitgestellt werden.

## Front Matter & Veröffentlichung

Jede Datei nutzt konsistente YAML-Metadaten, damit Obsidian, Build-Prozess und Git-Historie dieselben Informationen interpretieren können.

| Feld | Bedeutung |
| --- | --- |
| `title`, `author` | Lesbare Seitentitel und Zuordnung. |
| `created`, `updated` | Zeitliche Verortung innerhalb des Forschungs- und Publikationsprozesses. |
| `publish` | `true` markiert Seiten, die auf der Webseite erscheinen; `false` hält Entwürfe intern. |
| `published` | Datum der formalen Freigabe (z. B. nach DOI- oder PDF-Veröffentlichung). |
| `Repository` | Referenz auf dieses GitHub-Repository für Transparenz und Zitierbarkeit. |
| `tags` | Obsidian-Schlagworte für interne Navigation. |

Die eigentliche Ausspielung der Seite erfolgt in einem separaten Static-Site-Build. Dieses Repository fokussiert ausschließlich die inhaltliche Ebene; Deployment-Skripte und Infrastruktur liegen bewusst außerhalb.

## Arbeitsweise & Versionierung

- Git dient als epistemisches Protokoll. `git add` markiert den Moment, in dem Gedanken den privaten Raum verlassen; `git commit` stabilisiert die Fassung; `git push` macht sie öffentlich nachvollziehbar.
- Semantische Commit-Präfixe wie `[Reflexion]`, `[Reentry]` oder `[Setup]` kennzeichnen den Charakter einer Änderung (siehe `Hinweise.md`).
- Erkenntnisrelevante Wendepunkte werden, wenn notwendig, per leerem Commit dokumentiert, um die Denklinie auch ohne inhaltliche Textänderung sichtbar zu halten.
- Veröffentlichungsreife Inhalte werden zusätzlich als PDF mit DOI (z. B. via Zenodo) archiviert; die dynamische Weiterentwicklung bleibt über Git transparent.

## Lokal arbeiten

1. Repository klonen: `git clone git@github.com:jochen-hanisch/webseite.git`
2. Vault in Obsidian öffnen oder einen Editor mit YAML-Unterstützung nutzen.
3. Neue Seiten mit obigem Front Matter anlegen und konsequent in Markdown schreiben.
4. Vor der öffentlichen Sichtbarkeit `publish` auf `true` setzen und Inhalte testlesen.
5. Commits mit sprechenden Nachrichten versehen, Änderungen in Issues oder Commit-Beschreibungen verorten und anschließend `git push`.

Für eine statische Vorschau kann ein beliebiger Generator (z. B. Quartz, Eleventy, Astro) eingesetzt werden. Entscheidend ist, dass der Build-Prozess YAML-Felder ausliest und die interne Linksyntax `[[Zielseite]]` in funktionsfähige Verweise überführt.

## Lizenz & Zitierpraxis

Alle Inhalte stehen unter der **GNU Affero General Public License v3**. Die Lizenz erlaubt Nutzung, Veränderung und Weitergabe, solange dieselben Freiheitsgrade gewahrt bleiben. Bei Zitaten bitte Commit-Hash, Datei und (falls gesetzt) DOI angeben, damit der Forschungs- und Entstehungskontext eindeutig nachvollziehbar bleibt.

## Feedback & Kontakt

Rückmeldungen, Korrekturen oder inhaltliche Diskussionen sind willkommen. Offene Fragen bitte über [GitHub Discussions](https://github.com/jochen-hanisch/webseite/discussions) einbringen; thematisch fokussierte Hinweise oder Fehler lassen sich gezielt über Issues oder Pull Requests nachverfolgen. Für Anliegen, die nicht öffentlich dokumentiert werden sollen, stehen die in `Kontakt.md` genannten Kanäle bereit.
