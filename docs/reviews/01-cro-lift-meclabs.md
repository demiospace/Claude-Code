# Review 1: Conversion-Optimierung (LIFT-Modell + MECLABS)

> **Framework:** LIFT-Modell (WiderFunnel: Value Proposition, Clarity, Relevance, Urgency,
> Anxiety, Distraction) und MECLABS Conversion Sequence Heuristic (C = 4m + 3v + 2(i−f) − 2a)
> **Prüfgegenstand:** Design-Entwurf v2 der manibase-Startseite
> **Datum:** 07.07.2026 · unabhängiger Prüf-Agent
> **Alle Befunde wurden in Entwurf v3 umgesetzt** – siehe [design-kompendium.md](../design-kompendium.md)

---

## Priorisierte Befunde

**1. [HOCH] · Gesamte Seite · Value Proposition / MECLABS „v" + „a" (Credibility)**
Es gibt auf der kompletten Seite null Belege: keine Kundenstimme, kein Fallbeispiel, keine Zahl („X Stunden/Woche gespart"), kein Kundenlogo, kein „bereits N Betriebe". Die Formel gewichtet „v" mit Faktor 3 — hier steht nur Behauptung gegen Behauptung, und für eine skeptische Handwerker-Zielgruppe kollabiert damit die gesamte Argumentation. Vorschlag: Mindestens ein konkretes Mini-Fallbeispiel mit Zahl direkt nach den Pains oder Helfern („Tischlerei Muster: Angebote in 20 statt 90 Minuten") — der Annex plant das für die Branchenseiten, die Startseite braucht es zuerst.

**2. [HOCH] · Branchen-Sektion · Distraction**
Vier große Kacheln mit „eigene Seite ↗" leiten Besucher mitten auf der Seite auf externe Domains — bevor sie je den Termin-CTA gesehen haben. Das ist ein aktiver Traffic-Export an der Stelle mit der höchsten Relevanz-Resonanz („meine Branche!"). Vorschlag: Kacheln nicht als Exit, sondern als Relevanz-Beleg gestalten (Branchen-Pain + passender Helfer, CTA „Orientierungsgespräch für Ihr Gewerk"); der externe Link maximal als kleiner Sekundärlink.

**3. [HOCH] · Termin-Sektion · Distraction / Friction**
Im entscheidenden Moment konkurrieren drei gleichrangige Handlungen: „Termin auswählen" (gelber Button), „E-Mail schreiben" und die Newsletter-Box mit einem identisch gestylten gelben „Anmelden"-Button daneben. Der sekundäre Conversion-Pfad kannibalisiert visuell den primären. Vorschlag: Newsletter aus der Termin-Sektion herauslösen (eigener schmaler Streifen darunter oder Footer) bzw. den Anmelden-Button deutlich abstufen (Ghost-Stil).

**4. [HOCH] · Gesamte Seite · Urgency + Incentive (MECLABS: i = 0, LIFT: Urgency fehlt)**
Es existiert kein einziger Grund, *jetzt* zu buchen — keine Verknappung, kein Anreiz, kein zeitlicher Bezug. Für eine „später kümmere ich mich drum"-Zielgruppe ist das der klassische Absprung ohne Handlung. Vorschlag: Ehrliche Kapazitäts-Urgency („Wir begleiten max. 3 neue Betriebe pro Monat — nächste freie Klartage: KW 38") und/oder ein kleines Incentive im Gespräch (z. B. „Sie gehen mit 3 konkreten Ansatzpunkten für Ihren Betrieb raus").

**5. [MITTEL] · Hero · Clarity / MECLABS „v"**
„Ihre persönliche KI-Assistenz für [Rotator]" ist nach 5 Sekunden nicht selbsterklärend: Der Rotator zwingt zum Warten (und „die Planung" sieht man erst nach ~10 s), das Nutzenversprechen bleibt unquantifiziert, und die rechte Hero-Hälfte erklärt das *eigene* Vier-Bausteine-Modell statt den Kundennutzen — Firmenarchitektur ist keine Value Proposition. Vorschlag: Headline mit Ergebnis statt Kategorie („Der Bürokram ist fertig, bevor Sie im Büro sind"), Plan-Karte durch ein Ergebnis-Artefakt ersetzen (z. B. Ausschnitt eines Ampel-Maßnahmenplans oder Vorher/Nachher-Zahl).

**6. [MITTEL] · Hero + Nav + Termin · Clarity / Friction (CTA-Inkonsistenz)**
Drei verschiedene Labels für dieselbe Handlung („Gespräch buchen", „Orientierungsgespräch buchen", „Termin auswählen") und das entscheidende risikoarme Framing „kostenlos · 15 Minuten" steht erst ganz unten — im Hero fehlt es am Button komplett. Vorschlag: Ein einheitliches Label überall („Kostenloses 15-Min-Gespräch buchen") plus Microcopy unter dem Hero-Button („kostenlos · unverbindlich · Calendly").

**7. [MITTEL] · Station 01 / Warum · Anxiety (Preis ohne Wertkontext)**
„1.800 € Festpreis" steht zweimal auf der Seite, aber nirgends, was der Tag konkret einbringt oder erspart — der Preis ist das erste und einzige harte Faktum der Seite und wirkt ohne Nutzenanker teuer. „Voll anrechenbar" ist gut, reicht aber nicht. Vorschlag: Preis immer mit Deliverable + Wertanker koppeln („1.800 € — Sie erhalten einen priorisierten Maßnahmenplan; typische Betriebe identifizieren dabei 5–10 Std. Bürozeit/Woche") und idealerweise eine Risikoumkehr ergänzen.

**8. [MITTEL] · Seitenarchitektur · Friction (CTA-Wüste in der Seitenmitte)**
Zwischen Hero und Termin-Sektion (~7 Sektionen, auf mobil sehr lang) gibt es keinen einzigen primären CTA — nur Ghost-Links, davon zwei ins Leere („Mehr zum KI-Klartag" → `#`) und einer nach extern (Community ↗ in der Weg-Sektion). Wer nach Pains oder Helfern überzeugt ist, findet keinen Abschluss. Vorschlag: Einen primären CTA-Button nach der Helfer-Sektion einschieben; tote und externe Links aus der Kern-Kaufstrecke entfernen.

**9. [MITTEL] · Academy + Team · Anxiety / Clarity**
Zwei Vertrauensbrüche: Der Academy-Button „Bei Start informiert werden" führt auf `#termin` (Terminbuchung statt der erwarteten Newsletter-Anmeldung — Erwartungsbruch = Friction), und der zweite Gründer heißt nur „Nikolaus" ohne Nachnamen mit generischer Rollen-Bio — bei einer Zielgruppe, die Menschen kauft, wirkt das unfertig. Vorschlag: Academy-Button gezielt auf das Newsletter-Feld ankern (mit vorausgewähltem Interesse), Team-Sektion nur mit echten Namen, Bios und idealerweise regionalem Bezug launchen.

**10. [NIEDRIG] · Hero-Trust / Footer · Anxiety (DSGVO nur behauptet)**
„DSGVO-konform · Server in Deutschland" wird dreimal wiederholt, aber nie belegt — kein Hosting-Partner, kein AVV-Hinweis, keine Detailseite. Für eine explizit DSGVO-sensible Zielgruppe ist die nackte Behauptung schwächer als ein Beleg. Vorschlag: Trust-Zeile verlinken („So schützen wir Ihre Daten →") mit konkretem Anbieter/Standort; das Wort „konform" nur mit nachprüfbarer Substanz verwenden. Kleinigkeit ebenfalls hier: „Unsere Helden" vs. „KI-Helfer" — eine Bezeichnung durchziehen.

## Was der Entwurf richtig macht

1. **Pains in echter Kundensprache** („Angebote um 22 Uhr", „das weiß nur der Kollege im Urlaub") — starke Motivation-Anknüpfung (MECLABS 4m), kein Tech-Jargon.
2. **Friction-armer primärer Conversion-Schritt**: 15 Minuten, kostenlos, „ohne Folien", mit ehrlichem „wir sagen auch, ob KI bei Ihnen keinen Sinn ergibt" — gutes Anxiety-Management am Abschlusspunkt, plus E-Mail als Ausweichkanal.
3. **Ehrlichkeit als Stilmittel**: Academy klar als „in Vorbereitung" markiert, Ampel-Logik inkl. „Rot: lassen Sie es", Festpreis statt Tagessatz-Nebel — das zahlt konsistent auf Vertrauensaufbau bei einer beratermüden Zielgruppe ein.
