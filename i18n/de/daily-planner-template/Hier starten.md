# Hier starten

Willkommen. Dieser Vault ist ein Time-Blocking-Tagesplaner: Jeder Tag bekommt drei Prioritäten (die **Top 3**), eine Timeline aus Blöcken im Day-Planner-Format und einen zweiminütigen **Tagesabschluss**. Drei ausgefüllte Tage und eine Wochenübersicht sind enthalten — eine echte, unperfekte Woche, inklusive Blöcken, die verschoben werden mussten.

## Wie der Vault aufgebaut ist

- `Planer/` — eine Notiz pro Tag (`YYYY-MM-DD`) plus eine schlichte Wochenübersicht (`Woche vom 2026-06-08`). Die Beispiele decken Montag bis Mittwoch, 8.–10. Juni 2026 ab; der Mittwoch steht absichtlich mitten am Tag, der Nachmittag ist noch nicht abgehakt.
- `Vorlagen/` — `Tagesplaner` (wird neuen Tagesnotizen automatisch zugewiesen) und `Wochenübersicht`.

Das Core-Plugin **Daily notes** ist so eingerichtet, dass Planer-Notizen in `Planer/` aus der Vorlage entstehen.

## Die Methode, in vier Regeln

1. **Top 3 zuerst.** Wenn nur diese drei Dinge passieren, war der Tag gut. Sie auswählen, bevor der Kalender aufgeht.
2. **Die Timeline blocken.** Zeilen wie `- [ ] 09:00 - 10:30 Deep Work: Sache` unter *Tagesplan* nutzen. Blöcke sind Wetten, keine Versprechen — verschieben, wenn die Realität dazwischenfunkt, statt die Liste aufzugeben.
3. **Ein Deep-Work-Block vor dem Mittagessen.** Schützen wie einen Kundentermin.
4. **Tagesabschluss, immer.** Abhaken, was passiert ist, notieren, was auf morgen wandert, Laptop zuklappen. Der Abschluss ist der Grund, warum die Planung morgen fünf Minuten dauert statt dreißig.

## Erste Schritte

1. Die drei Beispieltage der Reihe nach lesen — der Montag lief nach Plan, der Dienstag nicht, der Mittwoch läuft noch. Genau dieser Kontrast ist der Punkt.
2. Die heutige Tagesnotiz öffnen (Kalender-Symbol oder `Tagesnotiz für heute öffnen`). Die Vorlage lädt sich selbst.
3. Die Top 3 aufschreiben, den Vormittag blocken, anfangen.

## Plugins

- **Day Planner** (optional, aber empfohlen) — macht aus den Timeline-Zeilen einen visuellen Zeitplan mit „Jetzt"-Marker in der Seitenleiste und zeigt den Tag als Zeitstrahl. Installieren, die Standardeinstellungen behalten, und das Plugin liest die `- [ ] HH:mm - HH:mm`-Aufgaben aus den Tagesnotizen automatisch aus.

Alles andere sind Core-Plugins, bereits konfiguriert.

> [!tip] In Hälften schätzen
> Wer neu im Time-Blocking ist, macht jeden Block halb so ehrgeizig, wie es sich richtig anfühlt. Zwei ehrliche 90-Minuten-Blöcke schlagen jeden Fantasie-Zeitplan, der um 10:15 zusammenbricht.
