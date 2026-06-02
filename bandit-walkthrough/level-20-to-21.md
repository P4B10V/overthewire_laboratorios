**Nivel 20 -> 21**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit21.html)

**Descripción**

En el directorio personal hay un binario que hace lo siguiente: realiza una conexión a localhost al puerto que se especificó, lee la linea de texto de la conexion, y la compara con la del nivel anterior. Si es correcta, te devolverá la contraseña del siguiente nivel.

**Solución**

Para resolver este nivel, tendremos que aprender una función de `ssh` y es que nos permite ejecutar comandos remotamente en la máquina en la que realizamos la conexión. Es decir, que si al conectarnos tratamos de leer el contenido del fichero, aunque nos eche podremos obtenerlo igualmente.

Como tendremos que realizar dos acciones en la misma sesión `ssh`, se decidió utilizar `tmux` para abrir dos terminales y de paso aprender algo nuevo:
```
  - control + b -> " nueva terminal horizontal
  - control + b -> % nueva terminal vertical 
  - control -b -> flechas de dirección para moverse entre paneles
```

Para la resolución, deberemos de dejar un servicio, por ejemplo con `netcat` escuchando en un puerto, y luego ejecutar el binario pasándole ese puerto en otra terminal, si todo va bien recibiras la contraseña del siguiente nivel. 

*Comandos sugeridos*
`ssh`, `nc`, `cat`, `bash`, `screen`, `tmux`, `Unix ‘job control’ (bg, fg, jobs, &, CTRL-Z, …)`



*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
