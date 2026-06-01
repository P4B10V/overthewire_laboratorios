**Nivel 1 -> 2**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit2.html)

**Descripción**

Para este nivel, nos piden obtener el contenido de un fichero llamado `-` en la carpeta personal del usuario `bandit1`

**Solución**

Antes de nada, realizar la conexión con el usuario mediante `ssh`. Como lo mas normal es estar ubicados ya en el directorio personal al realizar la conexión podríamos hacer un `ls` para listar en contenido de la carpeta, pero podriamos hacer `pwd` para comprobarlo.

Aunque sencillo leer un archivo, el problema está en que - es un caracter especial y además entran en juego dos puntos que son importantes en el entorno UNIX, las rutas absolutas y relativas. Con esto último que acabo de decir, ya di una pista bastante clara de porque hacer `cat -` no va a funcionar, sólo añadire que si tienes conocimiento de bash scripting, ¿has intentado ejecutar un archivo .sh sabiendo que está ahí, y el ordenador te contesta, el archivo no existe?

Pues el tema va por ahí, por último, decir que todas las carpetas en Linux tienen dos subcarpetas, . y .. 

*Comandos utilizados*

`ssh`, `cat`, `ls`

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*



