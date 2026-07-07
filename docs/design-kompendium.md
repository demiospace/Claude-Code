# Design-Kompendium: manibase-Startseite v1 → v3

**Was wurde geändert, warum und wie.** Dieses Dokument bündelt die Ergebnisse des
Redesign-Prozesses inklusive der drei Framework-Reviews. Stand: 07.07.2026, Entwurf v3.

---

## 1. Ausgangslage

### Die Live-Seite (v1)

https://manibase.aicoreinfra.de/ ist ein gut gemachter One-Pager für **ein** Angebot:
KI-Helfer für kleine Betriebe, mit dem KI-Klartag (1.800 € Festpreis) als Unterseite und
einem Blog. Analyse der Seite ergab ein durchdachtes, eigenständiges Design-System
(aus `styles/tokens.css` extrahiert):

| Element | Wert |
|---|---|
| Primärfarbe | Indigo-Cobalt `#2F3FDB` |
| Akzent | Gelb `#F2D414` („Golden Yellow Rule": gelbe Fläche, dunkler Text) |
| Grund | Warme Papiertöne (`#FCFAF4` / `#F8F4EC`), Ink `#14224F` |
| Typografie | Sora (Display) + Hanken Grotesk (Body), selbst gehostet (DSGVO) |
| Marken-Motive | „Bauplan-Raster" (32px-Zellen), Maßlinien-Eyebrows, handgezogener gelber Marker |
| Figuren | Vier Helfer-Illustrationen (Dachs, Biene, Eichhörnchen, Eule) mit eigenen Farben: Anton (teal), Emma (violett), Doreen (pink), Wiktor (blau) |
| Tonalität | Persönlich, handwerksnah, „Sie"-Ansprache, kein Tech-Jargon |

### Das Geschäftsziel

manibase wächst zur **Dachmarke mit vier Bereichen**:

1. **KI-Klartag** – die Diagnose (existiert)
2. **KI-Helfer** – das Kernangebot (existiert)
3. **manibase Academy** – Schulungen (neu, in Vorbereitung)
4. **Community** – externer Austausch (neu, extern)

Dazu **Branchen-Landingpages auf eigenen Domains** für: Handwerk & Bau ·
Architektur & Planung (Architekten, Bauingenieure, Planungsbüros) · Physio & Fitness
(inkl. Kältetherapie) · Zahnlabore.

### Abgestimmte Grundsatzentscheidungen

- **Marke weiterentwickeln**, kein neuer Look – Bestandskunden sollen die Seite wiedererkennen
- **Erst Mockup, dann Code** – der Entwurf wird als self-contained HTML abgestimmt,
  die echte Seite folgt nach Freigabe
- **Statisches HTML/CSS** wie die Live-Seite (kein Framework, kein Build-Tool)

---

## 2. Entwurf v2: der Dachmarken-Hub

Kernidee: Die Startseite wird vom Ein-Produkt-One-Pager zum **Hub**, der alle vier
Geschäftsbereiche als eine Geschichte erzählt.

**Neue Elemente in v2:**
- Sektion „Ihr Weg mit manibase" (4 Stationen: Diagnose → Umsetzung → Befähigung → Austausch)
- Hero mit „Plan-Karte" statt Stock-Foto (Bauplan-Motiv der Marke)
- Branchen-Sektion mit 4 Kacheln für die künftigen Domains
- Academy-Teaser als einzige gelbe Flächensektion (Sub-Identität)
- Erweiterte Navigation und Footer-Sitemap
- Design-Rationale-Anhang direkt im Mockup

**Technische Fixes während v2:**
- Scroll-Reveal-Animation entfernt (Sektionen blieben bei schnellem Scrollen unsichtbar –
  IntersectionObserver-Falle)
- Grid-Bug in der Ablauf-Liste behoben (Inhalt rutschte in die 44px-Nummernspalte)
- `<meta charset="utf-8">` ergänzt (Umlaute waren beim Direkt-Rendern der Datei kaputt;
  im Artifact hatte der Wrapper das kaschiert)

---

## 3. Die drei Framework-Reviews

Drei unabhängige Prüf-Agenten haben v2 parallel gegen je ein bewährtes Framework geprüft.
Volltexte: [`reviews/01-cro-lift-meclabs.md`](reviews/01-cro-lift-meclabs.md) ·
[`reviews/02-storybrand-sb7.md`](reviews/02-storybrand-sb7.md) ·
[`reviews/03-trust-stanford.md`](reviews/03-trust-stanford.md)

| Review | Framework | Blickwinkel |
|---|---|---|
| 1 | LIFT-Modell + MECLABS Conversion Sequence Heuristic | Conversion: Klarheit, Reibung, Ablenkung, Dringlichkeit, Angst |
| 2 | StoryBrand SB7 (Donald Miller) | Botschaft: Kunde als Held, ein Plan, ein CTA, Erfolg/Misserfolg |
| 3 | Stanford Web Credibility (BJ Fogg) + deutsche B2B-Konventionen | Vertrauen: Belege, echte Organisation, Preistransparenz, DSGVO |

### Der Kernbefund (von allen drei unabhängig bestätigt)

> **Die Seite behauptet Vertrauen, statt es zu belegen.**

Design und Tonalität bestanden die Prüfung durchweg; die Schwächen lagen im Inhalt
(fehlende Belege) und in der Conversion-Führung (CTA-Chaos, zwei konkurrierende Pläne,
Traffic-Export).

### Was alle drei ausdrücklich lobten (unverändert beibehalten)

- Pain-Points in echter Kundensprache („Angebote um 22 Uhr")
- Kostenloses 15-Minuten-Gespräch mit ehrlicher Absage-Option als niedrigschwelliger Einstieg
- Ampel-Logik inkl. „Rot: lassen Sie es" – Empfehlung gegen das eigene Umsatzinteresse
  als stärkstes Glaubwürdigkeitssignal
- „Sie prüfen, ergänzen, senden" – der Mensch behält die Kontrolle
- Ehrliches „in Vorbereitung"-Label der Academy

---

## 4. Änderungen v2 → v3 (Was · Warum · Wie)

| # | Was | Warum (Befund · Framework · Schwere) | Wie umgesetzt |
|---|---|---|---|
| 1 | **Ein CTA-Wortlaut** | 3 verschiedene Labels für dieselbe Handlung; Newsletter-Button kannibalisierte den Haupt-CTA; keine CTAs in der Seitenmitte (CRO 3/6/8, SB 3/9 · HOCH) | „Kostenloses 15-Min-Gespräch" 11× identisch (Nav, Hero, Seitenmitte, 4 Branchen-Kacheln, Termin) + Microcopy „kostenlos · unverbindlich · ohne Folien"; Newsletter-Button als Outline abgestuft; neuer Zwischen-CTA nach der Helfer-Sektion |
| 2 | **Ein Plan statt zwei** | 4-Stationen-„Weg" und 5-Schritte-„Ablauf" konkurrierten; der sichtbare erste Schritt trug ein 1.800-€-Preisschild (SB 2 · HOCH) | Überall derselbe 3-Schritte-Plan: kostenloses Gespräch → Klartag → Umsetzung & Schulung. Die vier Bereiche sind jetzt Angebotsübersicht („Was manibase für Sie tut"), keine Wegnummerierung mehr |
| 3 | **Hero: Nutzen statt Kategorie** | „Ihre persönliche KI-Assistenz für [Rotator]" benannte die Kategorie, nicht den Nutzen; Rotator zwang zum Warten (CRO 5, SB 5 · MITTEL) | H1: „Ihr Bürokram ist *vorbereitet*, bevor Sie im Büro sind." – bewusst „vorbereitet" statt „fertig" (ehrlich: Mensch prüft). Rotator + JS entfernt |
| 4 | **Social-Proof-Sektion** | Null Belege auf der ganzen Seite – für eine 1.800-€-Entscheidung der größte Einzelfehler (alle 3 · HOCH) | Neue Sektion „Was Betriebe sagen": 2 Testimonial-Slots + Kennzahlen-Zeile, als PLATZHALTER markiert (echte Stimmen oder ehrlich „N Pilotbetriebe") |
| 5 | **Branchen: konvertieren statt exportieren** | 4 große „eigene Seite ↗"-Kacheln schickten Besucher im Moment höchster Relevanz von der Seite (CRO 2 · HOCH) | Kacheln sind keine Links mehr: Branchen-Pain + zuständige Helfer + Gespräch-CTA; externe Branchen-Seite nur noch als Fußnote „folgt ↗" |
| 6 | **„Daten & Technik"-Block** | „DSGVO-konform" 4× behauptet, 0× belegt; Newsletter selbst ohne Einwilligung (Trust 2, CRO 10 · HOCH) | Neuer Block mit 4 konkreten Punkten (Hoster, Modell-Standort als PLATZHALTER; kein Training mit Kundendaten; AV-Vertrag inklusive); Hero-Trustline verlinkt darauf; Newsletter mit Einwilligungs-Checkbox + Datenschutz-Link |
| 7 | **Überversprechen geerdet** | „bis alles von allein läuft", „nichts bleibt liegen", „bevor jemand suchen muss" = Verkäufersprache, kollidiert mit „kein Buzzword-Bingo" (Trust 6 · MITTEL) | Alle Absolutaussagen ersetzt: „bis Ihr Team selbstständig damit arbeitet", „Gesendet wird erst, wenn Sie freigeben", „aus Ihren eigenen Unterlagen" |
| 8 | **Preis mit Wertanker** | 1.800 € stand ohne Nutzenkontext; „voll anrechenbar" undefiniert; Helfer ohne Preisrahmen (CRO 7, Trust 7 · MITTEL) | Preis überall mit Deliverable gekoppelt („Ergebnis: Maßnahmenplan mit Ampel"); Anrechenbarkeits-Präzisierung + Helfer-Preislogik als PLATZHALTER in der Termin-Sektion |
| 9 | **Ehrliche Urgency** | Kein Grund, *jetzt* zu handeln (MECLABS i=0, CRO 4 · HOCH) | Kapazitätszeile am Termin-CTA („max. [3] Betriebe/Monat, nächste freie Klartage: [KW]") – als PLATZHALTER, nur mit echten Zahlen verwenden |
| 10 | **Erfolg & Einsatz benannt** | Weder das Leben *nach* manibase noch die Kosten des Nichthandelns wurden gemalt (SB 6/7/8 · MITTEL) | Erfolgsbild „Montagabend, 18:30 Uhr…" nach den Helfern; Einsatz-Satz + inneres Problem („nicht, um abends Verwaltungsassistent zu sein") als Pains-Abbinder |
| 11 | **„Unsere Helden" gestrichen** | Produkt statt Kunde als Held – klassischster StoryBrand-Fehler; kippte mit Cartoon-Tieren ins Alberne (SB 1 · HOCH, Trust 9) | Eyebrow „Ihre neuen Mitarbeiter fürs Büro", H2 „Die vier KI-Helfer", Funktion vor Name |
| 12 | **Team greifbar** | „Nikolaus" ohne Nachname wirkt halb-anonym; Bios ohne prüfbare Station (alle 3 · MITTEL) | PLATZHALTER-Slots: Nachname, je 2 belegbare Stationen, LinkedIn |
| 13 | **Firma greifbar** | Keine Rechtsform/Anschrift/Telefon; kontakt@demiospace.ai = fremde Domain (Trust 3 · HOCH) | Mail auf kontakt@manibase.de umgestellt; Telefon- und Rechtsform/Anschrift-Zeilen als PLATZHALTER im Footer |
| 14 | **Community konkretisiert** | Extern, namenlos, aber „Baustein 04 des Wegs" – wirkt wie eine Behauptung (Trust 8 · MITTEL) | Als „Austausch · extern" gerahmt (kein Weg-Baustein mehr), Plattform + Größe als PLATZHALTER |
| 15 | **Jargon entfernt** | „Go-live", „Hands-on", „On-Demand" (SB 10 · NIEDRIG) | „Nach dem Start", „Praxisarbeit", „Wann Sie Zeit haben"; Academy-Kurse als „Geplante Kurse" mit Start-PLATZHALTER; Academy-Button führt jetzt wirklich zum Newsletter |
| 16 | **Platzhalter-System** | Erfundene Fakten wären selbst ein Trust-Bruch | CSS-Klasse `.ph`: gelb gestrichelte Umrandung + „PLATZHALTER"-Badge, unübersehbar im Mockup; komplette Liste im Annex des Entwurfs |

---

## 5. Offene Punkte (Launch-Checkliste)

Diese Fakten kann nur der Auftraggeber liefern – im Mockup als `PLATZHALTER` markiert:

1. 2 echte Kundenstimmen + Kennzahlen — oder ehrlich: „Aktuell begleiten wir [N] Pilotbetriebe"
2. Daten & Technik: Hosting-Partner und KI-Modell-Anbieter mit Standort
3. Kapazitätszeile nur mit echten, gepflegten Zahlen — sonst streichen
4. Nikolaus: Nachname + je Gründer 2 belegbare Stationen + LinkedIn
5. Firmenangaben: Rechtsform, Anschrift, Telefon; kontakt@manibase.de einrichten
6. Klartag-Anrechenbarkeit präzisieren (Zeitraum, Bedingungen)
7. Helfer-Preislogik („ab X €/Monat" oder Projektpreis-Rahmen)
8. Community: Plattform + Größe; Academy: Startzeitraum
9. Alle toten Links ersetzen: Impressum, Datenschutz, Blog, Klartag-Seite, Community
10. Terminbuchung: DSGVO-freundliche Alternative zu Calendly prüfen (passend zum eigenen Versprechen)

---

## 6. Nächste Schritte

1. **Startseite als statische Webseite umsetzen** (HTML/CSS/JS wie die Live-Seite,
   selbst gehostete Fonts) — auf Basis des freigegebenen v3-Entwurfs
2. **Klartag- und Academy-Unterseiten** im neuen System
3. **Branchen-Landingpage-Template** (ein Baukasten, vier Domains): Hero mit Branchen-Pain,
   3 Pain-Karten in Branchensprache, passender Helfer im Fokus, Mini-Fallbeispiel mit Zahl,
   identischer Klartag-CTA, Rückverweis auf die Hauptseite

## Artefakte

- Aktueller Entwurf: [`../entwurf/manibase-redesign.html`](../entwurf/manibase-redesign.html)
  (self-contained, mit eingebetteten Original-Fonts und -Illustrationen)
- Abstimmungs-Link (privat, Login nötig): https://claude.ai/code/artifact/f5cd8ba1-eb81-47f0-b207-9912c0b7c482
