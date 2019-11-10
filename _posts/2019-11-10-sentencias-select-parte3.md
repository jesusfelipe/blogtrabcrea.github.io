---
layout: post
Title: Sentencias select parte3
---

¡Bienvenidos a la tercera parte de las consultas select !

En está parte vamos a incluir los agrupados, para ello vamos a introducir
(GROUP BY, SUM, COUNT, MIN, MAX), no se permite en este tipo de sentencias
utilizar el * para indicar todos los campos.

GROUP BY - nos permite indicar que campos son los que van a agruparse, tienen que ser
los campos que están en el SELECT que no se utilizen para calcular agrupado.

SUM - sobre un campo indica cual es el que vamos a sumar, tiene que ser un
un campo númerico.

COUNT - sobre un campo indica cual es el que vamos a contar, está permitido
hacerlos sobre cualquier campo

MIN - sobre un campo indica cual es el que vamos a conseguir su mínimo.

MAX - sobre un campo indica cual es el que vamos a conseguir el máximo.

```sql

SELECT campo1,campo2,SUM(campo3) as suma_campo3
FROM tabla1
GROUP BY campo1,campo2;

SELECT campo1,campo2,COUNT(campo1) as num_regs,MIN(campo3) as min_campo3,MAX(campo3) as max_campo3
FROM tabla1
GROUP BY campo1,campo2;

```
