**Nivel 13 -> 14**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit14.html)

**Descripción**

Para este nivel no se necesita recuperar de algún archivo, si no que necesitamos conectarnos mediante la clave privada al usuario `bandit14`

**Solución**

La clave privada está disponible en el directorio de `bandit13` y si al intentamos usar nos va a dar un error. La razón es que tienen bloqueado la conexión a localhost, por lo que nos tendremos que buscar una manera de pasarnos la clave privada y conectarnos desde nuestra máquina física, para ello tendremos que investigar sobre `scp`. Es un herramienta muy útil pues nos permite la transferencia de datos de manera cifrada, y aunque cambia un poco lo que nos resultada útil será:
  - `-i` -> para indicar la clave que usaremos
  - `-P` -> indicar el puerto (sí, en mayúsculas, en ssh es en minúsculas)

Si al realizar la conexión utilizando la clave trata de leer el error que te pone, yo sólo te dire que está relacionado con `chmod`


*Comandos sugeridos*

`ssh` `scp` `umask` `chmod` `cat` `nc` `install`


*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
