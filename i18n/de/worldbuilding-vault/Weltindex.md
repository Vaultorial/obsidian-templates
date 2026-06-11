---
type: index
---

# Weltindex — Die Gezeitenhöfe

Die Seichte See läuft zweimal am Tag leer und kehrt zurück, und zweimal im Jahr zeichnen die Königsfluten die Küste selbst neu. Um ihre Bucht stehen die Gezeitenhöfe: Stadtstaaten, deren Recht nicht vom Land handelt, sondern davon, *wann* Land existiert. Das Gezeitenrecht entscheidet, wer auf Grund bauen, wirtschaften und ernten darf, der überflutet wird — und das Gezeitenrecht ist nur so gut wie die Karten, auf denen es steht. Die Karten driften. Dieser Index ist die Eingangstür zu allem.

## Die gegenwärtige Lage, in drei Sätzen

Der Hof der Ebbe in [[Ostreve]] hält an den alten Karten fest, die [[Die Flutung von Niedermark]] für diesen Hochsommer ansetzen. Die Flutgeschworenen von [[Niedermark]] wollen sie verhindern — per Petition oder durch das Brechen der Deiche. Und der Orden der Versunkenen Glocke, dessen Messungen das Recht erst möglich machen, hat im Stillen entdeckt, dass die Messungen nicht mehr mit der See übereinstimmen — siehe [[Die Spiegelmoor-Fäule]].

## Orte

- [[Ostreve]] — Klippenstadt, Sitz des Hofs der Ebbe, Hüterin der Karten und Zölle.
- [[Niedermark]] — der Hafen darunter: Stelzen, Fischrauch und das Viertel, das ertrinken soll.
- [[Der Glockendamm]] — der einzige Weg zwischen beiden, passierbar bei Niedrigwasser.
- [[Das Spiegelmoor]] — Wattflächen und Perlmoosbänke; Reichtum, den man schneller ernten muss, als die See zurückkehrt.
- [[Heidwiek]] — Marktstädtchen im Oberland, jenseits des Gezeitenrechts; der neutrale Boden aller.
- [[Die Versunkene Abtei]] — halb versunkenes Archiv des Ordens, zu Fuß nur bei Nipptide erreichbar.

## Fraktionen

- [[Der Hof der Ebbe]] — das Recht. Sitz: Ostreve. Geführt von Gezeitenmeisterin [[Elowen Hark]].
- [[Die Flutgeschworenen]] — der Protest. Sitz: Niedermark. Geführt von [[Bren Callow]].
- [[Orden der Versunkenen Glocke]] — die Messer. Sitz: die Versunkene Abtei. Geführt von [[Maud Pell]].

## Menschen

```dataview
TABLE role AS "Rolle", home AS "Zuhause", faction AS "Fraktion"
FROM "Charaktere"
SORT file.name ASC
```

### Nach Fraktion

```dataview
TABLE rows.file.link AS "Mitglieder", rows.role AS "Rolle"
FROM "Charaktere"
GROUP BY faction
```

## Chronologie

Die vollständig erzählte Fassung lebt in der [[Zeitleiste]].

```dataview
TABLE year AS "Jahr", location AS "Ort", status AS "Status"
FROM "Ereignisse"
SORT year ASC
```

## Fäden zum Ziehen

- Hält das geheime Abkommen von [[Verity Ostreve]] mit [[Bren Callow]], wenn das Sielvotum kommt?
- Was geschieht mit dem Gezeitenrecht, wenn [[Maud Pell]] veröffentlicht, dass die Karten falsch sind?
- [[Wick der Fährmann]] hat jedes Geheimnis dieses Index mindestens einmal befördert. Wem erzählt er es am Ende?
