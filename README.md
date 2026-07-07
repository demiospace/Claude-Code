# manibase – Redesign der KI-Agentur-Webseite

Dieses Repository dokumentiert das Redesign der manibase-Startseite
(https://manibase.aicoreinfra.de/) hin zu einem Dachmarken-Hub für vier Geschäftsbereiche:

1. **KI-Klartag** – die Diagnose (1 Tag, Festpreis)
2. **KI-Helfer** – das Kernangebot (Anton, Emma, Doreen, Wiktor)
3. **manibase Academy** – Schulungen (in Vorbereitung)
4. **Community** – externer Austausch

## Inhalt

| Pfad | Inhalt |
|---|---|
| [`docs/design-kompendium.md`](docs/design-kompendium.md) | **Das Kompendium**: Was wurde geändert, warum (Review-Befunde) und wie (konkrete Umsetzung) |
| [`docs/reviews/`](docs/reviews/) | Die drei vollständigen Framework-Reviews (LIFT/MECLABS, StoryBrand SB7, Stanford Web Credibility) |
| [`docs/landingpages/`](docs/landingpages/) | **Landingpage-Blaupausen**: Funnel-Architektur (Value Ladder, Subdomains) + Skelette für 5 LPs (3 Branchen, Community, Newsletter-Kurs) |
| [`entwurf/manibase-redesign.html`](entwurf/manibase-redesign.html) | Der aktuelle Design-Entwurf v3 als self-contained HTML-Mockup |

## Status

**Entwurf v3** – alle Review-Befunde eingearbeitet. Offene Punkte sind im Mockup als gelb
gestrichelte `PLATZHALTER` markiert und in der Launch-Checkliste des Kompendiums gelistet.

Die Landingpages laufen künftig auf **Subdomains** (ein Ordner = eine Subdomain,
Ziel-Layout siehe [`docs/landingpages/00-funnel-architektur.md`](docs/landingpages/00-funnel-architektur.md));
die ursprüngliche Website-Struktur bleibt unter `site/` unangetastet erhalten.

Nächste Schritte: HTML-Skelett-Mockups der Landingpages im v3-Design-System, Umsetzung
der Startseite als statische Webseite, danach Klartag- und Academy-Unterseiten.
