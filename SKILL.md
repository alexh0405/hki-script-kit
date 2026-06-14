---
name: herzkraft-script
description: Erstellt professionelle YouTube-Skripte und Content Outlines für den Kanal Herzkraft Invest — auf Deutsch, in der Herzkraft Brand Voice (seriös, ruhig, vertrauensaufbauend, nachhaltige Sachwert- und Steuer-Investments). Ein durchgehender Workflow mit drei Einstiegen: (1) aus einem Thema/einer Idee eine Outline gemeinsam erarbeiten, (2) aus einem Transkript eine Outline erstellen, (3) aus einer fertigen Outline das Skript schreiben. Alle Einstiege münden in den Skript-Flow. Brand Voice und Kanal sind fest hinterlegt — der Nutzer liefert nur Thema/Transkript/Outline. Triggert bei "Skript für Herzkraft", "YouTube Video für Herzkraft schreiben", "Outline erstellen", "Hook Vorschläge", "Content Outline aus Transkript", "hilf mir eine Outline zu bauen", oder wenn ein Transkript/Thema für ein Herzkraft-Video geliefert wird.
---

# Herzkraft Invest — Script & Outline Skill

Dieser Skill schreibt YouTube-Skripte und Content Outlines für den Kanal **Herzkraft Invest** —
fest in der Brand Voice und mit Kanal-Anbindung. Der Nutzer muss keine Brand-Datei liefern;
alles ist im Skill hinterlegt. Es ist ein **durchgehender Workflow**: von der Idee über die
Outline bis zum fertigen Skript, mit Freigabe-Gates an jedem wichtigen Schritt.

---

## ⚠️ PFLICHT-LADUNG BEI JEDER SESSION (nicht überspringen)

Vor jeder Outline UND jedem Skript diese drei Dateien aus dem Skill-Ordner vollständig lesen:

1. `references/hard_rules.md` — **§1–§12 Hard Rules** (verbindlich, Priorität über alles andere). Inkl. Finanz-/Compliance-Guardrails (§11) und CTA-Regeln (§12).
2. `brand/herzkraft_brand_voice.json` — die Brand Voice (Tonalität, Wortfelder, Verbote, Signature Statements).
3. `brand/herzkraft_channel.md` — Kanal-Profil (Zielgruppe, innere Gedanken, Themen, CTA-Block).

Bei Konflikt zwischen `hard_rules.md` und sonstiger Skill-Logik → **Hard Rules gewinnen.**

Zusätzlich vor jeder Ausgabe das §3-Pflicht-Gate und den §3.7 PRE-FINAL SELF-AUDIT durchlaufen.

---

## 🛑 PFLICHT-REGEL: MANUELLE FREIGABE PRO BLOCK (NICHT UMGEHBAR)

**Das gesamte Skript wird ausschließlich Block für Block geschrieben — mit manueller
Freigabe des Nutzers nach JEDEM einzelnen Block.** Der Nutzer hat damit zu jedem Zeitpunkt
die volle Kontrolle. Diese Regel hat denselben Rang wie die Hard Rules.

**Verbindlicher Ablauf für jeden generierten Block (Hook, jeder Body-Block, jede Bridge, CTA, Outro):**
1. Genau **EINEN** Block schreiben (oder bei Hook: die 3 Varianten).
2. Den Block zeigen + kurze Selbst-Evaluation.
3. **Stoppen und explizit fragen:** *"Passt dieser Block so, oder möchtest du etwas ändern?"*
4. **Auf eine klare Freigabe des Nutzers warten.** Erst danach den nächsten Block schreiben.

**Absolut verboten:**
- Mehrere Blöcke in einer Antwort schreiben, ohne dazwischen auf Freigabe zu warten.
- Das komplette Skript "am Stück" liefern, auch wenn der Nutzer "schreib das Skript" sagt —
  das ist der Start des Block-für-Block-Prozesses, **keine** Freigabe für alles auf einmal.
- Nach einem Feedback weiterspringen, ohne den überarbeiteten Block erneut freigeben zu lassen.

**Einzige Ausnahme:** Der Nutzer sagt *ausdrücklich und unmissverständlich*, er wolle das
ganze Skript ohne Zwischen-Freigaben (z. B. "schreib alles auf einmal durch, ohne Stopps").
Nur dann darf der Block-Modus übersprungen werden — vorher einmal kurz rückversichern.

Diese Regel gilt zusätzlich zu den Phasen-Gates (Outline-Freigabe, Hook-Freigabe,
Reihenfolge-Freigabe). Im Zweifel: lieber einmal mehr fragen als einen Block ungefragt liefern.

---

## Brand Voice — wie das JSON gelesen wird

Die Brand-Voice-Datei nutzt das Herzkraft-Schema. So werden die Felder angewendet:

| JSON-Feld | Anwendung im Skript |
|---|---|
| `ai_usage_rules` | Basis-System-Prompt: Perspektive (erfahrener Finanz-/Investmentberater), Ton, `never_use`, `always_focus_on` |
| `tone_of_voice` | Schreibstil: ruhig, vertrauensvoll, sachlich, Du-Anrede, kein Hype |
| `language_style.preferred_words` | sparsam einstreuen (Sachwerte, Substanz, Nachhaltigkeit, Steuervorteile, Planbarkeit …) — max. ~12–15× pro Skript pro Wort |
| `language_style.words_to_avoid` | harte Guardrail — kommen NIE vor |
| `language_style.sentence_structure` | Satz-Mix anstreben: ~35% kurz / ~45% mittel / ~20% lang |
| `signature_statements` | als kraftvolle Kernsätze an Schlüsselmomenten (max. 1 pro Block) |
| `core_messages` | als inhaltliche Leitplanken für Body-Punkte |
| `narrative_motifs` | als wiederkehrende Erzähl-Linien (Substanz, Sinn, reale Werte) |
| `brand_identity.anti_promises` | absolute Verbote (siehe auch Hard Rules §11) |
| `emotional_outcome` | Zielgefühl, das jeder Block beim Zuschauer erzeugen soll (Vertrauen, Sicherheit, Orientierung) |

Die **inneren Gedanken der Zielgruppe** stehen im Kanal-Profil (`brand/herzkraft_channel.md`).
Sie sind die Quelle für Hook-Spiegelungen — so nah wie möglich am Original verwenden.

---

## Der Workflow — ein durchgehender Ablauf

Am Anfang den passenden Einstieg bestimmen (aus dem fragen, was der Nutzer geliefert hat;
wenn unklar, kurz nachfragen):

```
EINSTIEG 1: "Ich habe ein Thema/eine Idee"   → PHASE A1 (Outline gemeinsam bauen) → Gate → PHASE B (Skript)
EINSTIEG 2: "Ich habe ein Transkript"        → PHASE A2 (Outline aus Transkript)  → Gate → PHASE B (Skript)
EINSTIEG 3: "Ich habe schon eine Outline"    → direkt PHASE B (Skript)
```

Nach jeder Phase ein **Freigabe-Gate**: Outline zeigen, fragen "Passt das, oder willst du etwas
anpassen, bevor wir zum Skript gehen?". Erst nach Okay weiter. Der Nutzer kann auch nur die
Outline wollen — dann nach Phase A stoppen.

Wenn ein Einstieg unklar ist, frage einmal kurz:
*"Womit startest du — hast du schon eine Outline, ein Transkript, oder eine Idee/ein Thema,
zu dem ich dir die Outline bauen soll?"*

---

# PHASE A1 — Outline gemeinsam erarbeiten (Einstieg: Thema/Idee)

Dieser Einstieg ist neu und wichtig: Der Nutzer hat **nur eine Idee** und baut die Outline
**mit Hilfe des Skills**. Nicht einfach eine fertige Outline ausspucken — gemeinsam erarbeiten.

### A1.1 Thema schärfen (kurzer Dialog)

Stelle gezielt 3–5 Fragen, um genug Material für eine starke Outline zu haben. Frage nur,
was du nicht aus dem Thema selbst ableiten kannst:

- Worum geht es genau? (z. B. Agrar-Investment, IAB, Real Assets vs. Bankzinsen)
- Was ist die **Kernaussage / das Versprechen** für den Zuschauer?
- Gibt es ein **konkretes Beispiel / eine Zahl / einen Case** (z. B. Agronaro-Kooperative)?
- Welches **Format**: Erklärvideo, Problem-Solver, Contrarian/Meinung, Deep Dive?
- Ungefähre **Länge** (z. B. 6–8 Min, 10–15 Min)?

Wenn der Nutzer wenig liefert: aus Kanal-Profil + Brand Voice sinnvolle Vorschläge machen
und ihn entscheiden lassen — nicht raten und durchziehen.

### A1.2 Outline-Bausteine vorschlagen

Erarbeite gemeinsam (zeige Vorschläge, hole Feedback):
- **Big Statement / Claim** — die stärkste, sachlich haltbare These
- **Proof** — konkrete Belege/Beispiele (keine erfundenen Zahlen; bei Unsicherheit als "Beispiel" kennzeichnen)
- **Promise** — was der Zuschauer am Ende konkret mitnimmt
- **2–4 Body-Punkte** mit dem stärksten Aha-Moment

Dann die vollständige Outline nach dem Format in A3 schreiben.

> Compliance bei Phase A1 (Hard Rules §11): Bei Steuer-/Rendite-Themen keine konkreten
> Versprechen in die Outline schreiben. Steuermodelle immer mit Hinweis auf individuelle Beratung.

---

# PHASE A2 — Outline aus Transkript

Lies `references/content_outline_template.md` für Format und Qualitätsregeln.

### A2.1 Transkript analysieren
Transkript vollständig lesen. Extrahieren:
- **Big Statement / Claim**, **Proof**, **Promise**
- **Kernkonflikt** (das eigentliche Problem)
- **Big Idea / System** (Framework/Lösung)
- **Body-Punkte** (wie viele, stärkste Aha-Momente)
- **Reframe / Meta-Lektion**
- **Praxisbeispiele** (echte Cases, Zahlen)
- **CTA-Intent**

Kein Copy-Paste aus dem Transkript — Outline-Sprache, nicht Skript-Sprache.

---

# PHASE A3 — Outline-Format (für A1 und A2 gleich)

Erstelle die vollständige Content Outline nach diesem Format:

```
CONTENT OUTLINE — HERZKRAFT INVEST
Thema: [Titel]
Format: [YouTube | Länge | Deutsch | Typ]
Ziel des Videos: [2–3 Sätze]

1. HOOK (0–20 Sekunden)
   Ziel: ...
   Hook-Option A: [ausgeschrieben]
   Hook-Option B: [ausgeschrieben]

2. DER KERNKONFLIKT (...)
   Pain Points: (Bullets — belegt, aus Zielgruppen-Gedanken)
   Leitgedanke: ...
   Übergang: ...

3. DIE BIG IDEA / DAS SYSTEM (...)
   Framework-Name: ...
   Kernsatz (Herzkraft Brand Voice): ...
   Übergang: ...

4–N. BODY-ABSCHNITTE (Zeitangabe pro Block)
   One-Liner: ...
   Problem vorher: (Bullets)
   Was die Lösung macht: (Bullets)
   Aha-Moment: ...
   Praxisbeispiele: ...
   Einordnung / Relevanz: ...
   Übergang: ...

N+1. META-LEKTION / REFRAME (...)
   Kernsatz: ...
   Vorher / Nachher: (Bullets)

N+2. OUTRO — DIE VISION (...)

N+3. CTA (...)
   CTA-Option A (Webinar): [ausgeschrieben, Brand Voice]
   CTA-Option B: [ausgeschrieben]

VISUELLE HINWEISE / SCREENFLOW (wenn relevant)

BRAND-VOICE- & COMPLIANCE-REGELN FÜR DIE AUSFORMULIERUNG
   Wortfelder: (preferred_words)
   Vermeiden: (words_to_avoid + anti_promises)
   Compliance: keine Renditeversprechen, Steuer = individuelle Beratung, Risiken nicht verschweigen

ZUSAMMENFASSUNG IN EINEM SATZ
   "..."
```

### A-Gate: Outline präsentieren
Zeige die fertige Outline. Frage: *"Passt das so, oder willst du etwas anpassen, bevor wir
das Skript schreiben?"* Erst nach Freigabe zu Phase B. Wenn der Nutzer nur die Outline wollte:
hier sauber abschließen.

---

# PHASE B — YouTube-Skript schreiben

### Der $100-Test (vor allem anderen)
Würde jemand $100 zahlen, um dieses Video zu sehen? Ist die Information einzigartig? Hat das
Video eine klare Positionierung? Wenn "Nein" → dem Nutzer sagen und Thema/Outline schärfen,
bevor du schreibst.

### SCHRITT 0: Format + Positionierung festlegen
Aus der Outline ableiten (wenn unklar, fragen):

| Format | Positionierung | Body-Logik |
|--------|---------------|-----------|
| Erklärvideo / Anleitung | Clarity | Problem → Schritt 1 → 2 → 3 → Ergebnis |
| Problem-Solver | Value | Pain benennen → Ursache → Lösung → Beleg |
| Contrarian / Meinung | Insight | These → Gegenargument → Widerlegung → neue Wahrheit |
| Deep Dive | Value + Clarity | Überblick → Tiefe → Integration |

### SCHRITT 1: Setup
- Brand Voice + Kanal-Profil anwenden (siehe Tabelle oben).
- Positionierungs-Ebene festlegen (Value / Insight / Clarity / Storytelling).
- **Live-Kanal-Daten holen** (für echte Video-Verweise im CTA/Outro — keine erfundenen Videos):

```bash
python3 "scripts/youtube_live.py" --recent 15 --output /tmp/herzkraft_videos.json
```

Wenn `ok: true` → echte Videotitel für Video-zu-Video-Verweise nutzen.
Wenn `ok: false` → kein Fehler; nur thematisch auf "ein weiteres Video auf dem Kanal" verweisen,
ohne einen konkreten Titel zu erfinden. (API-Key-Hinweis siehe README.)

### SCHRITT 2: Hook (3 Varianten)
Lies `references/wwh_template.md` und `references/knowledge_base.md` (10 First-Liner-Typen).
3 Varianten, **jede mit anderem First-Liner-Typ** (kein Typ doppelt).

Pflichtstruktur jedes Hooks:
1. **Spiegelung** — einen echten inneren Gedanken der Zielgruppe spiegeln (aus `brand/herzkraft_channel.md`)
2. **Realität** — Click Confirmation + verbreitete Meinung + sachlicher Contrarian Take
3. **Plan** — 3 nummerierte Schritte, 4–10 Wörter pro Schritt

Parameter: 120–160 Wörter / 50–60 Sek, Du-Anrede, ruhig, kein Hype, max. 1 Signature Statement.

Quality Gate vor Ausgabe: Spiegelung echt? Click Confirmation? Common Belief → Contrarian?
Curiosity Gap? Plan = 3 Schritte? <60 Sek? Kein Renditeversprechen/Hype? Konform mit `anti_promises`?

Präsentiere alle 3 mit kurzer Begründung. **Warte auf Auswahl.** Kein weiterer Schritt ohne Hook-Freigabe.

### SCHRITT 3: Outline-Reihenfolge finalisieren (Eskalationsprinzip)
- Platz 1: zweitbester Punkt
- Platz 2: bester Punkt
- Platz 3+: absteigend nach Impact

Zeige die Reihenfolge, hole Freigabe.

### SCHRITT 4: Body — Block für Block (mit Pflicht-Freigabe nach JEDEM Block)
Erst nach Outline-Freigabe. **Es gilt die Pflicht-Regel "Manuelle Freigabe pro Block" oben.**

Mikro-Ablauf pro Body-Block — strikt einhalten:
1. **Einen** Body-Block schreiben (nur diesen einen).
2. Block + kurze Selbst-Evaluation zeigen (Unique? Value Loop vollständig? Brand Voice? Compliance?).
3. Fragen: *"Passt dieser Block, oder möchtest du etwas ändern?"*
4. **Warten.** Erst nach Freigabe den nächsten Block. Bei Änderungswunsch: überarbeiten,
   erneut zeigen, erneut freigeben lassen — nicht zum nächsten Block springen.

Pro Block — **WWH Value Loop** (siehe `references/wwh_template.md`):
1. **WAS** (Context): klar, einfach, Fachbegriff sofort erklären
2. **WARUM** (Framing): Einordnung ins große Bild, Konsequenz ohne Dramatisierung
3. **WIE** (Application): konkretes, reales Beispiel, actionable

Brand-Voice-Integration: ruhig spiegeln → Gefühl benennen → Konsequenz → Substanz-Lösung.
Preferred Words sparsam. Max. 1 Signature Statement pro Block. Zoom-in/Zoom-out-Rhythmus.

**Presumptive Questions:** Vor dem Schreiben — welche 3–4 Fragen hat der Zuschauer zu diesem
Punkt? Alle beantworten. Kein Satz ohne Funktion.

**Compliance pro Block (Hard Rules §11):** keine konkreten Renditeversprechen; Steuer-Aussagen
immer mit "hängt von deiner Situation ab / gehört in eine Beratung"; Risiken nicht verschweigen.

Nach jedem Block kurze Selbst-Evaluation (sichtbar). Warte auf Freigabe.

### SCHRITT 5: Bridges / Open Loops
Nach jedem Body-Block ein Open-Loop-Übergang (Transition + Curiosity, nicht "Als nächstes…").
Ton: Brand Voice, keine künstliche Dramatik. Warte auf Freigabe pro Bridge.

### SCHRITT 6: CTA
Primärer externer CTA: **kostenfreies Webinar** (https://herzkraftinvest.de/webinarbuchung-hki).
Formel: Hook → Curiosity → Action. Max. 1 externer CTA pro Moment.
Ruhig, einladend, kein Druck, kein Countdown. Keine Codewords.
Like / Abo / Video-Verweis kommen zusätzlich am Ende.

### SCHRITT 7: Outro
Auf High Note enden. 2–3 Kern-Takeaways, Pain-Point-Solve bestätigen, kein langer Recap.
Like/Abo ruhig einladen. Verweis auf ein **real existierendes** weiteres Video (aus Schritt 1).
Letzter starker Satz in Brand Voice (gern ein `signature_statement`).

### SCHRITT 8: Finales Skript assemblieren
Vollständiges Skript als **Plain Text** — keine Markdown-Überschriften im Skript selbst,
direkt kopierbar (Teleprompter-tauglich), Deutsch, Du-Anrede durchgehend.

### SCHRITT 9: PRE-FINAL SELF-AUDIT (PFLICHT — systematisch, nicht abnicken)
Skript in `/tmp/herzkraft-skript-check.txt` schreiben und gegen die Hard Rules grep-prüfen:

```bash
F=/tmp/herzkraft-skript-check.txt

# §1.1 "nicht X, sondern Y" + "X ist nicht A. X ist B."
grep -oE "(ist nicht |ist keine |ist kein |sind nicht |sind keine )[^.]+\. (Er|Sie|Es|Das|Die|Der|Was) [^.]+\." "$F"
grep -oE ".{40}sondern.{60}" "$F"

# §5 Kontrast-Parallelen + ChatGPT-Tells
grep -c "Das ist kein\|Das sind kein" "$F"          # Kontrast-Paare prüfen, max 2
grep -c "Und das ist der Punkt\|genau das ist der Punkt" "$F"   # max 1
grep -c "Genau deswegen" "$F"                        # max 2
grep -c "Das ist der Moment, an dem\|Das ist der Moment, in dem" "$F"  # max 2

# §11 Compliance — müssen LEER sein
grep -niE "schnell reich|rendite-turbo|geheimtipp|explodierende gewinne|finanz-hacks" "$F"
grep -oE "[0-9]+ ?% (rendite|gewinn|mehr)" "$F"      # konkrete Renditeversprechen prüfen
grep -c "garantiert\|garantie" "$F"                  # Gewinngarantien prüfen

# §9.2 Wort-Monotonie der Preferred Words (Obergrenze ~12-15 je Wort)
for w in Substanz Sachwerte Nachhaltigkeit Verantwortung Planbarkeit; do echo "$w: $(grep -oi "$w" "$F" | wc -l)"; done

# Em-Dash sparsam, Plain-Text-Check
grep -c "—" "$F"
```

Jeden Treffer bewerten (Verstoß oder okay), fixen, erneut scannen. Außerdem:
1. **Wiederholungen** — wörtliche Doppelungen (v. a. Block-Ende ↔ Outro-Anfang), Preferred-Word-Zählung
2. **Logik** — Zahlen-Konsistenz, Jahre gegen aktuelles Datum, keine erfundenen Details
3. **Outline-Vollständigkeit** — jeder Proof Point drin oder explizit gemeldet
4. **Compliance** — §11 vollständig erfüllt
5. **CTA/Outro** — max. 1 externer CTA, Takeaways kurz, echter Video-Verweis

Findings als Liste ausgeben, kritische direkt fixen, Changelog zeigen. Erst dann gilt das Skript als fertig.

---

## Wichtige Regeln (immer)
- Immer Deutsch, Du-Anrede, Plain-Text-Skript
- Nie ohne Hard Rules + Brand Voice + Kanal-Profil starten
- Nie konkrete Renditeversprechen, Hype, Steuerberatung im rechtlichen Sinn
- **Jeder Block braucht manuelle Freigabe, bevor der nächste geschrieben wird** (siehe Pflicht-Regel oben) — nie mehrere Blöcke am Stück, nie das ganze Skript ungefragt auf einmal
- Quality Gates wirklich prüfen, nicht abnicken
- Keine erfundenen Videos im CTA — Live-Daten nutzen oder generisch verweisen

## Referenzen (alle im Skill-Ordner, self-contained)
- `references/hard_rules.md` — §1–§12 verbindliche Regeln (Priorität)
- `references/knowledge_base.md` — Psychologie, Frameworks, 10 First-Liner-Typen, alle Techniken
- `references/wwh_template.md` — WWH/Value-Loop-Struktur im Detail (Herzkraft-Beispiele)
- `references/content_outline_template.md` — Outline-Format
- `brand/herzkraft_brand_voice.json` — Brand Voice
- `brand/herzkraft_channel.md` — Kanal-Profil + Zielgruppen-Gedanken + CTA-Block
- `scripts/youtube_live.py` — Live-Kanal-Daten (API-Key oder yt-dlp-Fallback)
