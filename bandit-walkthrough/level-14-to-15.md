**Nivel 14 -> 15**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit15.html)

**Descripción**

La contraseña de este nivel se puede obtener entregándola a localhost por el puerto 30000.

**Solución**

Este nivel ya se pone interesante porque nos sugieren bastantes herramientas relacionadas con las redes. 

Lo primero que deberíamos tener claro es, ¿qué significa `localhost`?. Pues bien, significa *la propia máquina* también conocido como *127.0.0.1* o *loopback*, eso quiere decir que si mandas un mensaje a localhost es mandarte un mensaje a tí mismo directamente por lo que si nos piden entregar la contraseña a localhost 30000 deberemos entender que en la máquina existe un servicio escuchando en el puerto 30000.

Utilizando los comandos sugeridos, podríamos utilizar la herramienta `nmap` para escanear los puertos que tenemos abiertos. Este paso no es necesario pero es bueno ir practicando con esta herramienta pues es extremadamente útil.

Como yo ya lo conocía, probare con `nc (netcat)` pues es una herramienta vieja aunque versatil:
```man nc
It can open TCP connections, send UDP packets, listen on arbitrary TCP and UDP ports, do port  scan‐
       ning,  and  deal  with  both IPv4 and IPv6.  Unlike telnet(1), nc scripts nicely, and separates error messages
       onto standard error instead of sending them to standard output, as telnet(1) does with some.
```

Con esta herramienta podremos obtener la contraseña del siguiente nivel. 

Probé con `openssl` pero no funcionó. Tiene sentido porque requiere un intercambio de protocolos SSL/TLS y como el servicio escuchando en 30000 no lo implementa, pues no funciona.

*Comandos sugeridos*

`ssh`, `telnet`, `nc`, `openssl`, `s_client`, `nmap`


*Contenido sugerido*

`How the Internet works in 5 minutes (YouTube) (Not completely accurate, but good enough for beginners)`
`IP Addresses`
`IP Address on Wikipedia`
`Localhost on Wikipedia`
`Ports`
`Port (computer networking) on Wikipedia`


*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
