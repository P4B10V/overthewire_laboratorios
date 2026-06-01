**Nivel 6 -> 7**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit7.html)

**Descripción**

La contraseña esta almacenada en algún lugar del servidor y tiene las siguientes propiedades: `owned by user bandit7`, `owned by group bandit6` y `33 bytes in size`

**Solución**

Otra vez, deberemos utilizar el comando `find` pero en este punto ya sabremos utilizarlo mejor además de haber leído su manual. 

Aquí tuve que utilizar dos conceptos:
  - Utilizar `/dev/null` para reedirigir errores.
  - La raíz del sistema es `/` y que significa buscar usándolo.

Sabemos que tenemos que utilizar `find` y sus propiedades. Para filtrarlas por dueño y grupo, se encuentran en su manual (al igual que su tamaño como hicimos anteriormente). Una vez llegamos a este punto la salida será un tanto fea pues nos encontraremos con demasiada información, por eso tras realizar intentos con `grep` decidí probar con `/dev/null`

*Comandos utilizados*

`ssh`, `cat`, `ls`, `find`

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
