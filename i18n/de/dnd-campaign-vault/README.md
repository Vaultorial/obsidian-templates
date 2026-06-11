# D&D-Kampagnen-Vault — Obsidian-Vorlage

Ein Kampagnen-Verwaltungs-Vault für Tischrollenspiele, die mit der fünften Edition kompatibel sind, gebaut um Dataview-Dashboards und eine Eine-Notiz-pro-Entität-Struktur. Er kommt geladen mit **Die Verschwörung der Salzstraße**, einer kompletten originalen Mini-Kampagne — drei erzählte Sitzungen, acht NSC, vier verlinkte Orte, drei Begegnungen mit originalen Werteblöcken, drei Spielercharaktere und stützender Hintergrund — sodass jede Abfrage, jeder Link und jeder Arbeitsablauf mit echten Spieldaten demonstriert ist. Graphenansicht öffnen: Ein Kampagnen-Vault sollte wie ein Netz aussehen, und dieser tut es.

Alle Inhalte sind original. Der Vault ist regelkompatibel mit 5e, enthält aber keinen Text aus einem veröffentlichten Regelwerk.

## Struktur

```
dnd-campaign-vault/
├── Hier starten.md        ← zuerst lesen
├── Spielleiterschirm.md   ← Dataview-Dashboard: NSC nach Ort, Sitzungen, Begegnungen, Gruppe
├── Sitzungen/             ← 3 Sitzungsnotizen (Rückblick, Hinweise, Vorbereitung)
├── NSC/                   ← 8 NSC mit role / location / status / faction im Frontmatter
├── Orte/                  ← 4 verlinkte Orte
├── Begegnungen/           ← 3 Begegnungen: 2 gespielt, 1 vorbereitet und bereit
├── SC/                    ← 3 Spielercharaktere mit Bindungen und Aufhängern
├── Hintergrund/           ← Fraktionen und Geschichte, von mehreren Notizen geteilt
└── Vorlagen/              ← Sitzung, NSC, Ort, Begegnung, SC
```

## Installation

1. Vorlage herunterladen und entpacken: **Entpacken → Obsidian → Ordner als Vault öffnen**.
2. Wenn Obsidian fragt, Community-Plugins für diesen Vault aktivieren.
3. Dataview installieren, dann `Spielleiterschirm.md` in der Leseansicht öffnen.

## Plugins

**Erforderlich**

- Dataview — https://obsidian.md/plugins?id=dataview

**Optional**

- Leaflet — https://obsidian.md/plugins?id=obsidian-leaflet-plugin (interaktive Karten, sobald Kartenbilder da sind)
- Initiative Tracker — https://obsidian.md/plugins?id=initiative-tracker (Zugreihenfolge in der Seitenleiste)

## Lizenz

MIT. Nutzen, verändern, weitergeben — Namensnennung willkommen, aber nicht verpflichtend.

Vorlage von Vaultorial — https://vaultorial.com/de/dnd-kampagnen-vault/
