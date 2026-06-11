# MOC-Starterkit

Ein Obsidian-Starter-Vault zum Organisieren von Notizen mit Maps of Content (MOCs). Er kommt voll ausgearbeitet: ein Home-MOC, drei Themen-MOCs (Produktivität, Lernen, Schreiben) und fünfzehn verlinkte Notizen darunter — die Graphansicht öffnen, und der dreistufige Baum ist schon da.

## Ordnerstruktur

```
moc-template/
├── Hier starten.md     ← zuerst lesen
├── Home MOC.md         ← Ebene 1: der einzige Einstiegspunkt
├── MOCs/               ← Ebene 2: eine Landkarte pro Thema (3 Beispiele)
├── Notizen/            ← Ebene 3: eine Idee pro Notiz, flach (15 Beispiele)
└── Vorlagen/           ← MOC-Vorlage mit den Verlinkungskonventionen
```

## Durchgängig genutzte Konventionen

- **Home MOC → MOC → Notiz**: Die Startseite verlinkt nur auf MOCs; MOCs verlinken auf Notizen mit je einer Zeile Kontext; Notizen verlinken `Up:` auf ihr MOC und seitwärts auf verwandte Notizen.
- Notizen liegen flach in `Notizen/` — die Landkarten tragen die Struktur, nicht der Ordnerbaum.

## Installation

1. Den Download entpacken.
2. Obsidian öffnen → **Ordner als Vault öffnen** → den entpackten Ordner wählen.
3. Fragt Obsidian nach dem eingeschränkten Modus, anlassen — dieser Vault nutzt keine Community-Plugins.
4. Das Core-Plugin **Templates** aktivieren (Einstellungen → Core-Plugins), um die MOC-Vorlage zu nutzen.

## Plugins

- **Erforderlich:** keine. Funktioniert ganz mit Core-Plugins.
- **Optional:** keine.

## Lizenz

MIT. Nutzen, ändern, darauf aufbauen — privat oder kommerziell. Keine Namensnennung erforderlich.

Vorlage von Vaultorial — https://vaultorial.com/de/moc-vorlage/
