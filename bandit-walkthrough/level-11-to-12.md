**Nivel 11 -> 12**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit12.html)

**Descripción**

La contraseña para este nivel está almacenada en el fichero `data.txt`, en el que todas las minúsculas y mayúsculas han sido desplazadas 13 posiciones. 


**Solución**

Lo primero de todo será pensar, si son desplazadas 13 posiciones entonces la a será una n, la b será una o... y así sucesivamente. 

```
a b c d e f g h i j k l m 
n o p q r s t u v w x y z
```

Como ya vimos en niveles anteriores hay un comando que nos permite trasladar carácteres, `tr` por lo que tendremos que mirar su manual. Después de leerlo, seguía igual, sin idea, pues las ayudas que aparecian ahí eran demasiado generales, por lo que probe a buscarlo en wikipedia pues era una sugerencia. Después de leer el articulo ya supe la solución. 

Como consejo, trata de pensar un poco y deja wikipedia hasta el final, porque una vez que vayas a wikipedia lo tendrás resuelto.

*Material sugerido*

`Rot13 on Wikipedia`

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*



