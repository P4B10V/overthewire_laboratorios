**Nivel 0**

[Enunciado original](https://overthewire.org/wargames/natas/natas0.html)

**Descipción**

Natas te enseña lo básico sobre la seguridad web del lado del servidor.

Cada nivel consiste en su propia web localizada en http://natasX.natas.labs.overthewire.org, donde X es el numero del nivel. No hay login por SSH. Para acceder al nivel, introduce el usuario de ese nivel y su contraseña.

**Solución**

La única información que nos dan es la página web, un usuario y una contraseña. Lo primero que probé fue a realizar una petición con `curl` a la página web. Como sólo me interesaba saber el tipo de respuesta, usé el parámetro `-I` para recibir los headers. 

La respuesta fue un `HTTP/1.1 401 Unauthorized` indicándonos `Authentication required` por lo que está claro a partir de aquí, realizaremos la misma petición `curl` pero esta vez proporcionando las credenciales de `natas0` 


Como mi primer pensamiento fue acceder a esta web mediante linea de comandos, ahora voy a probar a acceder por web, al visitar la página nos salta un pop-up pidiendonos usuario y contraseña, al introducirla nos lleva a una página que solo nos dice:

<img width="598" height="120" alt="image" src="https://github.com/user-attachments/assets/f8dca511-a033-4cca-933e-213f95d91be4" />


La pista es `en esta página`, es decir, la contraseña está en esa página pero no esta visible para una petición utilizando un navegador web. 




**Herramientas utiles**

`A webbrowser`, `curl`, `ZAP proxy`


*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
