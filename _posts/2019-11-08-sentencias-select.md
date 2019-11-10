---
layout: post
title: Sentencias select parte 1
---

¡Bienvenidos a la parte de las sentencias select!

En este apartado vamos a ver como realizar consultas directamente de las tablas,
para ello utilizaremos las partes fijas  (SELECT, FROM, WHERE).

SELECT parte obligatoria que indica los campos que queremos seleccionar.

FROM parte obligatoria que indica la tabla que queremos seleccionar.

WHERE parte opcional en la cual vamos a indicar las condiciones a poner.

``` sql
SELECT * FROM tabla1;
SELECT campo1,campo2 FROM tabla1;
SELECT campo1,campo2 FROM tabla1 WHERE campo1 = 0;
```
