**Nivel 5 -> 6**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit6.html)

**Descripción**

La contraseña esta almacenada en un fichero en algún sitio en el directorio `inhere`. Nos dicen que es `human-readable`, `1033 bytes` y `not executable`

**Solución**

Parecido al ejercicio anterior, sólo que esta vez nos dan mas información del fichero aunque hay mas cantidad de carpetas, por lo que quizas tendremos que ser mas especificos a la hora de ejecutar nuestros comandos.

Este ejercicio me costó bastante porque traté de hacer un comando que buscará todo, hay una manera de hacer este ejercicio utilizando sólo un parámetro, pero me parecía insuficiente, tras lograrlo me sentí satisfecho.

Recomiendo **LEER** tranquilamente el manual de `find`, especialmente dos elementos:
  - `!` → operador de negación
  - `-exec` → ejecutar un comando sobre cada archivo encontrado


*Comandos utilizados*

`ssh`, `cat`, `ls`, `find`

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
