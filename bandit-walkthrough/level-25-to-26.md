**Nivel 25 -> 26**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit26.html)

**Descripción**

La shell de bandit26 no es /bin/bash. Averigua cual es, como trabaja y como salir de ella.

**Solución**

Lo primero de todo será averiguar que shell utiliza bandit26, para ello usaremos `/etc/passwd` y trataremos de investigar que es lo que se esta ejecutando. 

Podriamos usar `file` y `strings` para obtener el siguiente script:

```
#!/bin/sh
export TERM=linux
exec more ~/text.txt
exit 0
```

Esto es lo que se está ejecutando cada vez que nos conectamos por ssh utilizando la clave privada que nos proporcionan, en esta parte no se me ocurrió nada por lo que tuve que buscar información.

*Supuestamente, la clave era redimensionar la terminar y hacerla pequeña para que se ejecutara el comando more, la verdad es que no se me iba a ocurrir jamas hacer esto creo yo*

Cuando lo consigamos, es posible poder ver la ayuda de more, en ella nos enseñan que podemos ejecutar el editor de texto `vi` y a partir de ahi, pivotar hacia una shell.

**Comandos sugeridos**

`ssh`, `cat`, `more`, `vi`, `ls`, `id`, `pwd`

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*

