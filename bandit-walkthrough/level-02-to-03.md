**Nivel 2 -> 3**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit3.html)

**Descripción**

Para este nivel, nos piden obtener el contenido de un fichero llamado `--spaces in this filename--` en la carpeta personal del usuario `bandit2`

**Solución**

Como el ejercicio anterior, no hay más que añadir sobre esos puntos. Lo nuevo que nos encontramos ahora son los espacios, y para comprender su funcionamiento utilizaremos una de las funcionalidades de `touch`

Ejecutaremos estos dos comandos y comprobar la diferencia: `touch hola que tal` y `touch "hola que tal"`, ya con esto y el conocimiento del nivel anterior, tendría que ser suficiente para resolver este nivel. Otra manera de resolverlo sería investigar sobre el carácter de escape `\`

*Comandos utilizados*

`ssh`, `cat`, `ls`

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*



