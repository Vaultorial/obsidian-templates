# Statisches Gantt-Beispiel

Ein von Hand geschriebenes Gantt-Diagramm, ganz ohne Plugin. Obsidian zeichnet Mermaid-Diagramme selbst, deshalb funktioniert dieser Block in jedem Vault. Nimm ihn für einen einmaligen Plan und den [[Zeitplan]], wenn die Termine in deinen Aufgabennotizen stehen.

```mermaid
gantt
    title Produktlaunch
    dateFormat YYYY-MM-DD
    axisFormat %d.%m.
    excludes weekends
    section Recherche
    Marktforschung :done, r1, 2026-11-02, 8d
    Wettbewerbsanalyse :active, r2, after r1, 5d
    section Entwicklung
    Prototyp :crit, b1, after r2, 10d
    Betatest :b2, after b1, 6d
    section Launch
    Launch-Tag :milestone, m1, after b2, 0d
```

## So funktioniert die Syntax

- `dateFormat` legt fest, wie die Daten in den Aufgabenzeilen geschrieben werden, `axisFormat`, wie sie auf der Achse erscheinen.
- Jede Zeile lautet `Name :Tags, ID, Start, Ende-oder-Dauer`. Tags sind optional: `done`, `active`, `crit` und `milestone`.
- `after id` lässt eine Aufgabe beginnen, wenn eine andere endet. Verschiebst du die erste, folgen die übrigen.
- `excludes weekends` sorgt dafür, dass Dauern wie `5d` nur Werktage zählen.
