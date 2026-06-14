# Herzkraft Invest — YouTube Script & Outline Skill

Ein Claude-Code-Skill, der **YouTube-Skripte und Content Outlines** für den Kanal
**Herzkraft Invest** schreibt — auf Deutsch, in der hinterlegten Brand Voice, mit
Anbindung an den echten Kanal.

Du musst keine Brand-Voice-Datei mehr liefern: Tonalität, Zielgruppe, Kanal-Themen und
die Qualitätsregeln sind fest im Skill eingebaut. Du gibst nur **dein Thema, dein
Transkript oder deine Outline** — der Skill macht den Rest, Schritt für Schritt.

---

## ⚡ Installation in 10 Sekunden (der einfachste Weg)

Öffne **Claude Code**, füge diese Zeile ein und schick sie ab:

```
Installier mir diesen Skill: https://github.com/alexh0405/hki-script-kit
```

Claude liest die `INSTALL.md` aus diesem Repo und installiert den Skill automatisch nach
`~/.claude/skills/`. Danach Claude Code einmal neu starten — fertig.

> Falls Claude nachfragt: einfach bestätigen. Der Skill ist schreibgeschützt und sicher.

---

## Was der Skill kann

Ein durchgehender Workflow mit drei Einstiegen:

1. **Nur eine Idee?** → Der Skill baut die Content Outline **gemeinsam mit dir** auf (stellt
   gezielte Fragen, schlägt Bausteine vor) und schreibt danach das Skript.
2. **Ein Transkript?** → Der Skill erstellt die Outline aus dem Transkript und dann das Skript.
3. **Schon eine Outline?** → Der Skill schreibt direkt das Skript.

Nach jedem Schritt ein Freigabe-Gate — du behältst die Kontrolle. Du kannst auch nur die
Outline erstellen lassen und später das Skript.

---

## Alternative: manuelle Installation

Falls du es lieber selbst per Terminal machst:

```bash
mkdir -p ~/.claude/skills && \
git clone --depth 1 https://github.com/alexh0405/hki-script-kit ~/.claude/skills/herzkraft-script
```

Danach Claude Code neu starten und tippen:
```
/herzkraft-script
```
oder einfach: *"Schreib mir ein YouTube-Skript für Herzkraft Invest über IAB-fähige Investments."*

**Voraussetzung:** [Claude Code](https://claude.com/claude-code) installiert, Python 3 vorhanden
(für die Live-Kanal-Daten; auf macOS meist schon da).

---

## Optional: YouTube-API-Key (für echte Video-Verweise)

Der Skill kann am Ende auf **echte Videos deines Kanals** verweisen (statt Titel zu erfinden).
Dafür gibt es zwei Wege:

**Weg 1 — API-Key (empfohlen, zuverlässig):**
1. Key erstellen: [Google Cloud Console](https://console.cloud.google.com/) → neues Projekt →
   "YouTube Data API v3" aktivieren → unter "Anmeldedaten" einen API-Schlüssel erzeugen.
2. Key setzen (einmalig, dauerhaft):
   ```bash
   echo 'export YOUTUBE_API_KEY="DEIN_KEY"' >> ~/.zshrc
   source ~/.zshrc
   ```
   (Bei bash: `~/.bashrc` statt `~/.zshrc`.)

**Weg 2 — ohne Key (Fallback):**
Installiere `yt-dlp` — dann braucht der Skill keinen Key:
```bash
pip install yt-dlp
```

**Ganz ohne beides** funktioniert der Skill ebenfalls — er verweist dann nur allgemein auf
"ein weiteres Video auf dem Kanal", ohne einen Titel zu erfinden.

Test:
```bash
python3 ~/.claude/skills/herzkraft-script/scripts/youtube_live.py --recent 5
```

---

## Ordnerstruktur

```
herzkraft-script/
├── SKILL.md                       # Der Workflow (von Claude gelesen)
├── README.md                      # Diese Anleitung
├── brand/
│   ├── herzkraft_brand_voice.json # Brand Voice (fest hinterlegt)
│   └── herzkraft_channel.md       # Kanal-Profil, Zielgruppe, CTA-Block
├── references/
│   ├── hard_rules.md              # Verbindliche Qualitäts- & Compliance-Regeln
│   ├── knowledge_base.md          # Hook-Typen, Frameworks, Techniken
│   ├── wwh_template.md            # Skript-Struktur (Was/Warum/Wie)
│   └── content_outline_template.md
└── scripts/
    └── youtube_live.py            # Live-Kanal-Daten (API-Key oder yt-dlp)
```

---

## So nutzt du ihn

Beispiele, die den Skill auslösen:
- *"Hilf mir eine Outline für ein Video über Agrar-Investments zu bauen."*
- *"Hier ist ein Transkript — mach mir die Content Outline daraus."*
- *"Ich habe eine Outline, schreib mir das Skript dazu."*
- *"Gib mir 3 Hook-Varianten für ein Video über Real Assets vs. Bankzinsen."*

Der Skill arbeitet kollaborativ: Er zeigt dir jeden Schritt (Hook, Outline-Reihenfolge,
jeden Body-Block) und wartet auf deine Freigabe, bevor er weitermacht.

---

## Hinweise zur Qualität

Der Skill enthält feste **Finanz-/Compliance-Guardrails**: keine konkreten Renditeversprechen,
keine Steuerberatung im rechtlichen Sinn (immer Hinweis auf individuelle Beratung), Risiken
werden nicht verschwiegen. Das schützt die Brand. Diese Regeln lassen sich im Dialog nicht
abschalten — das ist Absicht.
