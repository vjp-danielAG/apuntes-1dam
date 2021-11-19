# Linux
#### Redirección de salida
La salida de los comandos se puede redireccionar a otros comandos o ficheros.

- `>`: Rellena con la salida un fichero. Si no existe lo crea. Si existe lo sobreescribe.
- `>>`: Rellena con la salida un fichero. Si no existe lo crea. Si existe concatena.
- `|`: Manda la salida de un comando a otro comando.
- `&`:  Manda el proceso al fondo.
- `&>`: Redirección de errores.
#### Filtros:
- `head -n <X>`: te devuelve las `X` primeras lineas.
- `tail -n <X>`: te devuelve las `X` últimas lineas.
- `cut -f <campo> -d <delimiter>`
- `grep <PERL regex>`: te devuelde las lineas que coincidan con el `regex`. 
___
###### ls -lah
Comando que te devuelve la información sobre directorios y ficheros en el siguiente formato:

`permisos` `inodo` `propietario` `grupo` `tamaño` `fecha y hora modificación`

La primera letra de los [[Sistema Operativo#Permisos en Linux|permisos]] nos da información sobre el tipo de elemento que es:
- `d` => directorio
- `l` => enlace
- `c` => periférico
- `b` => dispositivo de bloques 

###### cd &lt;ruta&gt;
Comando que permite cambiar de directorio al directorio designado por `ruta`.

###### touch &lt;archivo&gt;
Comando que permite crear un archivo de nombre `archivo` en el directorio actual.

###### rm &lt;archivo&gt;
Comando que permite borrar definitivamente un archivo de nombre `archivo`.

###### cp &lt;archivo_1&gt; &lt;archivo_2&gt;
Comando que permite copiar un archivo `archivo_1` a otro de nombre `archivo_2`.

###### mv &lt;archivo/directorio&gt; &lt;nueva_ubicación&gt;
Comando que permite mover el `archivo/directorio` a `nueva_ubicación`.
Se puede usar para renombrar archivos o directorios, pero no comprueba si `nueva_ubicación` existe y lo reemplaza.

###### cat &lt;archivo&gt;
Comando que permite ver el contenido de un fichero.

