# Review 3: Vertrauenswürdigkeit (Stanford Web Credibility + deutsche B2B-Konventionen)

> **Framework:** Stanford Web Credibility Guidelines (BJ Fogg, 10 Guidelines) + deutsche
> B2B-Trust-Konventionen (Impressum/Datenschutz, DSGVO-Belege, Referenzen, Preistransparenz,
> erreichbare Ansprechpartner)
> **Prüfgegenstand:** Design-Entwurf v2 der manibase-Startseite
> **Datum:** 07.07.2026 · unabhängiger Prüf-Agent
> **Alle Befunde wurden in Entwurf v3 umgesetzt** – siehe [design-kompendium.md](../design-kompendium.md)

---

## Priorisierte Befunde

**1. [HOCH] · Gesamte Seite · Fogg #1 (Verifizierbarkeit) & #3 (Expertise/Referenzen)**
Es gibt auf der kompletten Seite **null Social Proof**: keine Kundenstimme, keine Referenz, keine Fallstudie, keine Zahl („X Betriebe begleitet"), kein Logo, kein Siegel. Für eine 1.800-€-Entscheidung eines skeptischen Inhabers fehlt damit der wichtigste Beleg überhaupt — jede Aussage der Seite bleibt Selbstauskunft.
→ Mindestens 2–3 Testimonials mit vollem Namen, Betrieb, Ort und Foto einbauen (ideal direkt nach „Der Weg" und vor dem Termin-CTA), plus eine Mini-Fallstudie mit konkreter Zahl („Angebot in 20 statt 90 Minuten — Elektro Müller, Erfurt"). Wenn es noch keine Kunden gibt: ehrlich mit Pilotbetrieben arbeiten („Aktuell begleiten wir 5 Pilotbetriebe") — das ist glaubwürdiger als Schweigen.

**2. [HOCH] · Hero-Trustline, Helfer, „Warum", Footer · Fogg #1 (Verifizierbarkeit)**
„DSGVO-konform" und „Server in Deutschland" werden **viermal behauptet und nullmal belegt** — kein Hoster, kein Modell-/Anbietername, kein AV-Vertrag, keine verlinkte Detailseite. Die Formulierung „Ohne Ausnahme, ohne Kleingedrucktes" verschärft das: Genau die Zielgruppe mit Datenangst wird nachfragen, *wie* das technisch geht — und findet nichts. Pikant: Das Newsletter-Formular hat selbst keinen Datenschutzhinweis/Einwilligungstext — die Seite widerspricht ihrem eigenen Kernversprechen.
→ Eigene Seite „Datenschutz & Technik" anlegen und von jeder Trust-Zeile verlinken: Hosting-Partner nennen (z. B. Hetzner/IONOS), welche KI-Modelle wo laufen, „keine Nutzung Ihrer Daten zum Training", AVV-Muster zum Download. Newsletter-Formular mit Einwilligungs-Checkbox + Datenschutz-Link versehen.

**3. [HOCH] · Footer/Kontakt · Fogg #2 (echte Organisation) & #5 (Kontakt leicht machen)**
Die Firma ist nicht greifbar: keine Rechtsform, kein Ort, keine Anschrift, **keine Telefonnummer** — und die Kontakt-E-Mail lautet `kontakt@demiospace.ai`, eine fremde Domain mit .ai-Endung, die weder zur Marke passt noch erklärt wird. Für einen Handwerksmeister wirkt das wie eine Briefkastenfirma; Telefon ist in dieser Zielgruppe der Standard-Kanal.
→ `kontakt@manibase.de` einrichten, Footer-Brand-Spalte um „manibase · [Rechtsträger GmbH] · Musterstraße 1, 99084 Erfurt · Tel. 0361 …" ergänzen. Falls der Rechtsträger anders heißt, transparent machen: „manibase ist ein Angebot der … GmbH."

**4. [MITTEL] · Footer & alle CTAs · Deutsche Pflichtangaben (Impressum/Datenschutz), Fogg #10 (keine Fehler)**
Impressum und Datenschutz sind zwar korrekt platziert (Footer, von jeder Seite erreichbar), aber wie fast alle Links `href="#"` — inklusive des **primären CTA „Termin auswählen"**, „Mehr zum KI-Klartag", Blog und aller Branchen-Kacheln. Im Entwurf okay, beim Launch sind tote Pflichtlinks abmahnfähig und ein toter Haupt-CTA der teuerste Fehler der Seite.
→ Vor Freigabe eine Link-Checkliste ins Rationale-Annex aufnehmen; Impressum/Datenschutz/Terminbuchung (z. B. Calendly-Alternative mit DE-Hosting, passend zum Versprechen) als Launch-Blocker markieren.

**5. [MITTEL] · Team-Sektion · Fogg #4 (echte Menschen) & #3 (Expertise)**
Ein Gründer heißt nur „**Nikolaus**" — ohne Nachnamen wirkt eine Person halb-anonym und damit weniger real als gar kein Foto. Die Bios sind laut Annex Platzhalter und nennen keine einzige prüfbare Station (Ausbildung, frühere Betriebe, Jahre Erfahrung, Projekte).
→ Vollen Namen ergänzen, pro Gründer 1–2 verifizierbare Fakten („15 Jahre Software für den Mittelstand", „gelernter …") plus LinkedIn-Link. Gerade der „kennt die Abläufe aus der Praxis"-Claim braucht einen Beleg: *welche* Praxis?

**6. [MITTEL] · Hero, Helfer, Branchen · Fogg #1 & Zurückhaltung („zu gut um wahr zu sein")**
Mehrere Formulierungen überversprechen ohne Beleg: „bis alles **von allein** läuft", „beantwortet Fragen, **bevor jemand suchen muss**", „fertig vorbereitet, bevor Sie im Büro sind", „sorgt dafür, dass **nichts** Wichtiges liegen bleibt". Skeptiker, die KI-Hype gewohnt sind, lesen das als Verkäufersprache — und es kollidiert mit dem eigenen „kein Buzzword-Bingo"-Anspruch.
→ Auf die Mechanik erden, die die Seite an anderer Stelle vorbildlich zeigt („Sie prüfen, ergänzen, senden"): „entwirft Antworten — Sie entscheiden", „läuft nach der Einführung weitgehend ohne uns". Absolute Aussagen („nichts", „von allein") streichen oder belegen.

**7. [MITTEL] · Weg/Klartag, „Warum" · Deutsche Konvention Preistransparenz**
1.800 € Festpreis ist stark — aber die Preistransparenz endet dort abrupt: Die Helfer (das eigentliche Kernangebot) und die Academy haben **keinerlei Preisrahmen**, und „voll anrechenbar" bleibt undefiniert (worauf? wie lange gültig? auch anteilig?). Risikoaverse Inhaber fürchten genau das „Fass ohne Boden", das die Seite verneint.
→ Anrechenbarkeit präzisieren („wird bei jedem Folgeprojekt innerhalb von 12 Monaten voll verrechnet") und für die Helfer mindestens eine Preislogik nennen („Helfer ab X €/Monat, typisches Einführungsprojekt X–Y €" oder ein „Was kostet das?"-FAQ-Punkt).

**8. [MITTEL] · Nav, Weg-Station 04, Footer · Fogg #2 & Weiterleitungs-Risiko**
Die Community ist Baustein 04 des offiziellen „Wegs", aber die Plattform wird **nie benannt** — der Nutzer soll per ↗ ins Unbekannte springen. Das ↗-Kennzeichen ist gut (siehe Positives), reicht aber nicht: „Extern + namenlos + leer" wirkt wie eine Behauptung, dass es diese Community überhaupt gibt.
→ Plattform und Charakter konkret machen: „Kostenlos auf [Skool/Discord/…] · 80 Betriebe · moderiert von uns". Solange die Community klein/neu ist, eher als Bonus („dazwischen: unsere Community") führen statt als gleichwertigen vierten Baustein des Wegs.

**9. [NIEDRIG] · Helfer, Weg-Station 02 · Fogg #6 (professionelles Design) — Verniedlichungs-Grenze**
Die Tierfiguren mit klaren Funktionsrollen (Angebotsmanager, E-Mail-Assistenz …) funktionieren als Merkhilfe und senken die Schwellenangst — die Grenze überschreitet erst die Sprache: Eyebrow „**Unsere Helden**" und „Unsere Helden kennenlernen" rahmen Cartoon-Tiere als Superhelden, was ein skeptischer Meister als albern lesen kann; zudem stehen die Vornamen im Hero-Plan (Schritt 02) vor jedem Kompetenzbeleg.
→ „Unsere Helden" → „Die vier KI-Helfer"; überall Funktion vor Name („Der Angebotsmanager — wir nennen ihn Anton"). Figuren als Illustration behalten, aber nie als Argument.

**10. [NIEDRIG] · Academy · Fogg #7 (Nützlichkeit) & Konsistenz**
Das „in Vorbereitung"-Label ist ehrlich und richtig — aber der Button „**Bei Start informiert werden**" verlinkt auf `#termin` (die Terminbuchung!) statt auf das Newsletter-Feld, und die drei ausformulierten Kurskarten wirken wie buchbares Angebot. Wer klickt und in einer Verkaufssituation landet, fühlt sich geködert.
→ CTA auf das Newsletter-Formular (oder ein eigenes „Academy-Warteliste"-Feld) zeigen lassen; Kursliste mit „Geplante Kurse" überschreiben, ideal mit Zeithorizont („Start Herbst 2026").

## Was der Entwurf aus Trust-Sicht richtig macht

1. **Preis- und Ergebnisehrlichkeit beim Einstieg:** 1.800 € Festpreis offen auf der Startseite, kostenloses 15-Min-Gespräch als niedrige Schwelle, und die Ampel mit explizitem „Rot: lassen Sie es" — eine Empfehlung gegen das eigene Umsatzinteresse ist das stärkste Glaubwürdigkeitssignal der Seite.
2. **Mensch behält die Kontrolle:** Formulierungen wie „Sie prüfen, ergänzen, senden" und „entwirft Antworten" adressieren die Kernangst (KI macht unkontrolliert Dinge mit Kundendaten) genau richtig — dieses Muster verdient Ausbau (siehe Befund 6).
3. **Saubere Kennzeichnung und Zurückhaltung:** Externe Ziele konsequent mit ↗ markiert, Academy ehrlich als „in Vorbereitung" gelabelt, keine Werbung/Popups/Countdown-Tricks, ruhiges konsistentes Design mit echten Gründerfotos — professioneller Gesamteindruck (Fogg #6, #9).

**Kernaussage:** Design und Tonalität sind trust-tauglich; was fehlt, sind Belege. Die drei HOCH-Befunde (kein Social Proof, unbelegte DSGVO-Claims, nicht greifbare Firma inkl. Fremd-Mail-Domain) betreffen alle dieselbe Schwäche — die Seite *behauptet* Vertrauenswürdigkeit, statt sie *nachzuweisen*. Für die Zielgruppe „risikoaverser Skeptiker" entscheidet genau das über die 1.800-€-Frage.
