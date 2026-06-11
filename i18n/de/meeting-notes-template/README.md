# Meeting-Notizen-Paket — Obsidian-Vorlage

Drei einsatzbereite Besprechungsnotiz-Vorlagen für Obsidian — Teammeeting, 1-on-1 und Kundengespräch — mit strukturiertem Frontmatter, einem einheitlichen Layout aus Agenda/Notizen/Entscheidungen/Aktionspunkten und einem Dataview-Dashboard, das jede Besprechung und jeden offenen Aktionspunkt sichtbar macht. Enthält vier ausgefüllte Beispielbesprechungen aus einem einzigen Projekt, damit das Dashboard beim ersten Öffnen funktioniert.

Aktionspunkte verwenden die Datumssyntax des Tasks-Plugins (`- [ ] Verantwortlich — Aktion 📅 2026-06-15`), sodass sie sich direkt in einen GTD-Vault mit dem Tasks-Plugin übernehmen lassen.

## Struktur

```
meeting-notes-template/
├── Hier starten.md             ← lies das zuerst
├── Besprechungs-Dashboard.md   ← Dataview: nach Typ, nach Projekt, offene Aktionspunkte
├── Vorlagen/
│   ├── Teammeeting.md
│   ├── 1-on-1.md
│   └── Kundengespräch.md
└── Besprechungen/              ← vier ausgefüllte Beispiele, ein zusammenhängendes Projekt
    ├── 2026-05-04 Kickoff Kundenportal.md
    ├── 2026-05-11 1-on-1 Sarah und Priya.md
    ├── 2026-05-14 Kundengespräch Brightleaf.md
    └── 2026-06-01 Sprint-Review Kundenportal.md
```

## Installation

1. Lade die Vorlage herunter und entpacke sie: **Entpacken → Obsidian → Ordner als Vault öffnen**.
2. Wenn Obsidian fragt, aktiviere die Community-Plugins für diesen Vault.
3. Installiere Dataview und öffne `Besprechungs-Dashboard.md` in der Leseansicht.

## Plugins

**Erforderlich**

- Dataview — https://obsidian.md/plugins?id=dataview

**Optional**

- Templater — https://obsidian.md/plugins?id=templater-obsidian (tausch die Core-Templates-Variablen gegen dynamische, wenn du es bereits nutzt)

## Lizenz

MIT. Nutzen, verändern, weitergeben — Namensnennung willkommen, aber nicht erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/meeting-notizen-vorlage/
