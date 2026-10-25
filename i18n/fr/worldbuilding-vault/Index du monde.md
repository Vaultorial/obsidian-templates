---
type: index
---

# Index du monde — Les Cours des Marées

La Mer des Hauts-Fonds se vide et revient deux fois par jour, et deux fois l'an les marées royales redessinent la côte elle-même. Autour de sa baie se dressent les Cours des Marées : des cités-États dont la loi ne porte pas sur la terre mais sur le moment *où* la terre existe. La loi des marées décide qui peut bâtir, cultiver et récolter sur un sol qui s'inonde — et la loi des marées ne vaut que ce que valent les cartes qui la portent. Les cartes dérivent. Cet index est la porte d'entrée vers tout.

## La situation présente, en trois phrases

La Cour du Jusant, à [[Ostreve]], maintient les vieilles cartes, qui programment [[La Noyade de Basmarche]] pour cette mi-été. Les Jurés du Flot, de [[Basmarche]], entendent l'empêcher, par pétition ou en brisant les digues. Et l'Ordre de la Cloche Engloutie, dont les mesures rendent la loi possible, a découvert en silence que les mesures ne s'accordent plus avec la mer — voir [[Le Fléau du Marais-Miroir]].

## Lieux

- [[Ostreve]] — ville-falaise, siège de la Cour du Jusant, gardienne des cartes et des péages.
- [[Basmarche]] — le port d'en bas : pilotis, fumée de poisson, et le quartier programmé pour la noyade.
- [[La Chaussée des Cloches]] — la seule route entre les deux, praticable à marée basse.
- [[Le Marais-Miroir]] — estran et bancs de mousse perlière ; une richesse qu'il faut récolter en courant plus vite que la mer.
- [[Hautelande]] — bourg marchand des hautes terres, hors de la loi des marées ; le terrain neutre de tous.
- [[L'Abbaye Engloutie]] — archive à demi engloutie de l'Ordre, accessible à pied seulement en morte-eau.

## Factions

- [[La Cour du Jusant]] — la loi. Siège : Ostreve. Menée par la Maîtresse des Marées [[Elowen Hark]].
- [[Les Jurés du Flot]] — la protestation. Siège : Basmarche. Menés par [[Bren Callow]].
- [[Ordre de la Cloche Engloutie]] — les mesureurs. Siège : l'Abbaye Engloutie. Mené par [[Maud Pell]].

## Personnes

```dataview
TABLE role AS "Rôle", home AS "Foyer", faction AS "Faction"
FROM "Personnages"
SORT file.name ASC
```

### Par faction

```dataview
TABLE rows.file.link AS "Membres", rows.role AS "Rôle"
FROM "Personnages"
GROUP BY faction
```

## Cultures, croyances et objets

- [[Le Peuple des pilotis de Basmarche]] — les familles de la baie, qui vivent au rythme de la planchette des marées.
- [[La Veille des Cloches]] — la promesse tenue sur la chaussée : on doit un son aux noyés.
- [[Les Cartes maîtresses]] — douze feuilles dans une presse fermée qui décident quand la terre existe.

```dataview
TABLE held-by AS "Détenu par", location AS "Gardé à", status AS "Statut"
FROM "Objets"
SORT file.name ASC
```

## Chronologie

La version racontée complète vit dans [[Chronologie]].

```dataview
TABLE year AS "Année", location AS "Lieu", status AS "État"
FROM "Événements"
SORT year ASC
```

## Fils à tirer

- L'accord secret de [[Verity Ostreve]] avec [[Bren Callow]] tiendra-t-il quand viendra le vote des vannes ?
- Qu'arrive-t-il à la loi des marées quand [[Maud Pell]] publiera que les cartes sont fausses ?
- [[Wick le Passeur]] a transporté chaque secret de cet index au moins une fois. À qui finit-il par le dire ?
