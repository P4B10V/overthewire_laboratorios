**Nivel 7 -> 8**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit8.html)

**Descripción**

La contraseña esta almacenada en el fichero `data.txt` al lado de la palabra `millionth`

**Solución**

Lo primero que hice fue utilizar `cat` sobre el archivo, pensando que no iba a tener mucho contenido, pobre de mi. 

En este ejercicio hay que tener claro:
  - El uso de `|` llamadas pipes, que sirven para enviar la salida de un comando a la entrada de otro.
  - La herramienta `grep` para *agarrar* patrones

Con estos conceptos, deberías completar el ejercicio sin problema.

*Comandos utilizados*

`ssh`, `cat`, `find`, `grep`

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
