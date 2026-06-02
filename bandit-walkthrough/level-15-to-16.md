**Nivel 15 -> 16**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit16.html)

**Descripción**

La contraseña de este nivel se puede obtener entregándola a localhost por el puerto 30001 utilizando SSL/TLS.

**Solución**

Como ya hemos probado a utilizar e investigar sobre openssl en el nivel anterior, este debería de ser sencillo pues sabiendo que nos piden utilizar SSL/TLS tendremos que utilizar `openssl`. Realizamos una conexion a la direccion indicada en la descripción, introducimos la contraseña de bandit15 y ya deberíamos de obtener las credenciales del siguiente nivel.

*Comandos sugeridos*

`ssh`, `telnet`, `nc`, `ncat`, `socat`, `openssl`, `s_client`, `nmap`, `netstat`, `ss`

*Contenido sugerido*

`Secure Socket Layer/Transport Layer Security on Wikipedia`
`OpenSSL Cookbook - Testing with OpenSSL`


*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
