**Nivel 16 -> 17**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit17.html)

**Descripción**

La contraseña de este nivel se puede obtener entregándola a localhost utilizando SSL/TLS. Pero esta vez nos dan un rango de 31000 to 32000.

**Solución**

Para solucionar este nivel tendremos que utilizar una combinación de lo aprendido en los dos niveles anteriores, `nmap` y `openssl`.

Primero deberemos escanear los puertos de la máquina en ese rango. 

Una vez sepamos que puertos estan siendo utilizados, realizamos la conexión. Podremos comprobar como al final se queda esperando en un `R BLOCK`, es decir, está esperando por nuestro input, deberemos introducir la contraseña de bandit16. Si la respuesta es **KEYUPDATE** deberas leer en el manual, en particular esta parte, pues hay un parámetro que nos ayudara a conseguir la clave privada:

```
If a connection is established with an SSL server then any data received from the server is displayed and  any
key  presses  will  be  sent to the server. If end of file is reached then the connection will be closed down.
When used interactively (which means neither -quiet nor -ign_eof have been given), then certain  commands  are
also  recognized  which perform special operations. These commands are a letter which must appear at the start
of a line. They are listed below.
```

Una vez tengamos la clave, la enviaremos a nuestro ordenador. 

*Comandos sugeridos*

`ssh`, `telnet`, `nc`, `ncat`, `socat`, `openssl`, `s_client`, `nmap`, `netstat`, `ss`

*Contenido sugerido*

`Port scanner on Wikipedia`



*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
