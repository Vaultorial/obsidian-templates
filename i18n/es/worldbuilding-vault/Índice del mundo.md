---
type: índice
---

# Índice del mundo — Las Cortes de la Marea

El Mar Somero se vacía y vuelve dos veces al día, y dos veces al año las mareas regias redibujan la costa misma. Alrededor de su bahía se alzan las Cortes de la Marea: ciudades-estado cuya ley no trata de la tierra sino de *cuándo* existe la tierra. La ley de mareas decide quién puede construir, cultivar y cosechar en suelo que se inunda — y la ley de mareas vale lo que valgan las cartas en que se apoya. Las cartas están derivando. Este índice es la puerta de entrada a todo.

## La situación presente, en tres frases

La Corte del Reflujo, en [[Ostreve]], sostiene las cartas viejas, que programan [[El Anegamiento de Bajamarca]] para este pleno verano. Los Juramentados de la Creciente, de [[Bajamarca]], quieren impedirlo, por petición o rompiendo los diques. Y la Orden de la Campana Ahogada, cuyas mediciones hacen posible la ley, ha descubierto en silencio que las mediciones ya no concuerdan con el mar — ver [[La Plaga de la Marisma del Espejo]].

## Lugares

- [[Ostreve]] — ciudad acantilado, sede de la Corte del Reflujo, guardiana de cartas y peajes.
- [[Bajamarca]] — el puerto de abajo: zancos, humo de pescado y el barrio programado para anegarse.
- [[La Calzada de las Campanas]] — el único camino entre las dos, transitable en bajamar.
- [[La Marisma del Espejo]] — llanos mareales y bancos de musgo perla; una riqueza que hay que cosechar corriendo más que el mar.
- [[Altabreña]] — pueblo de mercado de las tierras altas, fuera de la ley de mareas; el terreno neutral de todos.
- [[La Abadía Anegada]] — archivo medio hundido de la Orden, alcanzable a pie solo en marea muerta.

## Facciones

- [[La Corte del Reflujo]] — la ley. Sede: Ostreve. La dirige la Maestra de Mareas [[Elowen Hark]].
- [[Los Juramentados de la Creciente]] — la protesta. Sede: Bajamarca. Los dirige [[Bren Callow]].
- [[Orden de la Campana Ahogada]] — los medidores. Sede: la Abadía Anegada. La dirige [[Maud Pell]].

## Personas

```dataview
TABLE role AS "Rol", home AS "Hogar", faction AS "Facción"
FROM "Personajes"
SORT file.name ASC
```

### Por facción

```dataview
TABLE rows.file.link AS "Miembros", rows.role AS "Rol"
FROM "Personajes"
GROUP BY faction
```

## Cronología

La versión narrada completa vive en [[Cronología]].

```dataview
TABLE year AS "Año", location AS "Lugar", status AS "Estado"
FROM "Eventos"
SORT year ASC
```

## Hilos de los que tirar

- ¿Aguantará el acuerdo secreto de [[Verity Ostreve]] con [[Bren Callow]] cuando llegue la votación de las compuertas?
- ¿Qué le pasa a la ley de mareas cuando [[Maud Pell]] publique que las cartas están mal?
- [[Wick el Barquero]] ha llevado todos los secretos de este índice al menos una vez. ¿A quién se lo cuenta al final?
