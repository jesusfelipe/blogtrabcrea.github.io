---
layout: post
Title: Sentencias select parte2
---

¡Bienvenidos a la segunda parte de las consultas select!

En esta parte vamos a añadir la union de varias tablas, para ello 
vamos a utilizar (INNER JOIN, LEFT JOIN, RIGHT JOIN).

INNER JOIN - En este caso vamos a querer los registros que cumplan el 
criterio de union de las dos tablas.

LEFT JOIN - En este caso vamos a querer todos los registros de la primera
tabla, y rellenos los campos de aquellos registros que cumplan el criterio 
de union de la segunda tabla.

RIGHT JOIN - En este caso vamos a querer todos los registros de la segunda
tabla, y rellenos los campos de aquellos registros que cumplan el criterio
de union de la primera tabla.

ON - nos va a servir para poner los campos de union que vamos a necesitar.

``` sql

SELECT a.campo1,a.campo2,a.campo4,b.campo1,b.campo2,b.campo3 
FROM tabla1 a INNER JOIN tabla2 b
ON a.campo1 = b.campo1;

SELECT a.campo1,a.campo2,b.campo1,b.campo3
FROM tabla1 a LEFT JOIN tabla2 b
ON (a.campo1 = b.campo1) AND (a.campo2 = b.campo2);

SELECT a.campo1,a.campo2,b.campo1,b.campo3
FROM tabla1 a RIGTH JOIN tabla2 b
ON (a.campo1 = b.campo1) AND (a.campo2 = b.campo2);

```
