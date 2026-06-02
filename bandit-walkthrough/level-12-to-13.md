[Enunciado original](https://overthewire.org/wargames/bandit/bandit13.html)

**Descripción**

La contraseña de este nivel esta almacenada en el fichero `data.txt` que es un `hexdump` de un fichero que ha sido comprimido repetidamente. 

**Solución**

Este nivel me tomó un poco mas de tiempo por el hecho de que nunca me había parado a entender `hexdump` y su finalidad. 

Según lo entendí: un hexdump es una herramienta que permite mostrar la representación en bytes de un fichero en formato hexadecimal. Mi duda era: ¿pero para qué sirve esto?  
La respuesta era más lógica de lo que pensaba.

Hay archivos que pueden ser binarios, desconocidos o incluso maliciosos, y no quieres ejecutarlos directamente. Necesitas una forma de inspeccionarlos sin correr riesgos, y ahí entra en juego el hexdump. Al convertir un archivo a su representación en texto hexadecimal, puedes analizar patrones, cabeceras, estructuras y contenido sin ejecutar nada.

Una vez entendido hexdump, pasamos al ejercicio. Lo primero de todo será hacer lo que nos aconsejan, hacer `mktemp -d` para crear un directorio temporal y copiar en él `data.txt` para asi trabajar cómodamente. 

En resumen, nuestro objetivo es revertir el hexdump de data.txt, analizar que tipo de archivo es y descomprimirlo, teniendo en cuenta que tiene que tener la extensión adecuada.


*Comandos sugeridos*

`grep`, `sort`, `uniq`, `strings`, `base64`, `tr`, `tar`, `gzip`, `bzip2`, `xxd`, `mkdir`, `cp`, `mv`, `file`

*Contenido sugerido* 

`Hex dump on Wikipedia`

*Las credenciales y soluciones no serán escritas, aunque esto sea un juego está centrado en los pasos y errores que hice durante su solución.*
