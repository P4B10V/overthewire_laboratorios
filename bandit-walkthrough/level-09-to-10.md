Bandit Level 9 → Level 10
Level Goal
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

encontrada información en: https://geekland.eu/uso-del-comando-tr-en-linux-y-unix-con-ejemplos/ 


cat data.txt | tr -cd "[:print:]\n" | grep "===="

**Nivel 9 -> 10**

[Enunciado original](https://overthewire.org/wargames/bandit/bandit10.html)

**Descripción**

La contraseña esta almacenada en el fichero `data.txt` y lo que nos dicen que es la única linea que se repite una vez.

**Solución**

Como comandos sugeridos están y que me llaman la atención son: `sort`, `uniq`, `strings` y `tr` por lo que examinaremos el manual de cada uno y ver que nos ofrece.

  - `tr` -> herramienta para reemplazar caracteres 
  - `strings` -> busca texto legible dentro de archivos que normalmente no son texto
  - `sort` -> ordena lineas de texto
  - `uniq` -> avisa o omite lineas repetidas 

Tras ver por encima que hace cada comando, creo que los que pueden sernos de utilidad son `sort` y `uniq`. Como recordatorio, queremos encontrar la única linea que se repite, por lo que leeremos otra vez el manual de `uniq` detenidamente a ver que encontramos.

En está parte me atasqué un poco, hasta que me di cuenta de un detalle en el manual: Filter **adjacent matching lines** from INPUT (or standard input), writing to OUTPUT (or standard output). 

Una vez me di cuenta de esto, supe que para obtener la solución habría que realizar una combinación de comandos. 

Como pista final, será necesario utilizar algo que ya vimos en los niveles anteriores: `|`


*Comandos utilizados*

`ssh`, `cat`, `find`, `grep`

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
