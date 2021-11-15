#### Sistema Operativo
El [[Sistema Operativo]] (SO o OS) es un programa o conjunto de programas que dotan de funcionalidad al ordenador, y proveen servicios a otros programas (aplicaciones).

Los [[Sistema Operativo|SO]] están programados por capas (como una cebolla):
- Kernel: Es núcleo que provee servicios al resto del SO y es la parte más cercana al procesador. Suele estar programado en ensamblador. El usuario no hace llamadas al Kernel de forma directa.
- Modulos: Son los procesos que llaman al Kernel. Los modulos no pueden llamarse entre ellos directamente, para ello tienen que pasar por el Kernel. 
	- Gestior de Procesos: Es el programa encargado de cargar y ejecutar procesos. Llama al kernel para que cambie el proceso en ejecución.
	- Gestion de Memoria: La memoria se solía dividir en segmentos de 64KB, pero ahora se está dividiendo en 256KB. Cuando la memoria principal (RAM) se llena, los segmentos de memoria que no estén en uso, se copian a disco, y se carga otro segmento.
	- Gestión de Disco: Los discos al igual que la memoria se divide en bloques, y son susceptibles a la fragmentación. Esto es el por qué Windows se realentiza con el tiempo. Normalmente los bloques son de 32-64KB para sistemas multimedia o con gráficos, y para sistemas ofimáticos 8-16KB.
		- Lo primero que se hace con un disco es particionarlo. Es decir, dividir el espacio físico en "cachos" virtuales. En MBR se pueden tener 4 particiones principales, y si necesitamos más, en la 4 se montará 
		- Sobre las particiones se montan los sistemas de ficheros. 
			- Windows es compatible con __NTFS__, FAT, y además puede leer ISO9660. FAT tiene un problema, que es que no tiene seguridad, al contrario que NTFS. 
			- Linux por el contrario usa __ext4__ por defecto, y es compatible con ext2-3-4, UFS, NFS, ReiserFS (usado por Suse), etc...
			- Linux además tiene un tipo de partición especial, llamada swap. Esta se usa para intercambio de datos entre el disco y la memoria principal.
	- Entrada/Salida: Este modulo se encarga de interactuar con los periféricos.
	- Red: No deja de ser Entrada/Salida, pero se considera una parte diferente.
	- Usuarios: Modulo que gestiona los usuarios del sistema.
	- BOOT: Arranque.
- Drivers: Son programas proporcionados por el fabricante delos periféricos.

##### ¿Cómo arranca un ordenador?
- POST: Testea el hardware para comprobar la configuración de hardware y que sea válida. Si hay algún error, lo hará saber mediante una serie de pitidos (el significado depende del fabricante). Esto lo hace la BIOS.
- Carga el MBR: Junto a esto se carga el bootstrap.
- Carga el Boot Loader: Programa que te deja elegir los Sistemas Operativos/Kernels a cargar.
- Carga el Kernel: Luego de que el Kernel se ha cargado, se termina de cargar el propio sistema operativo.
- Carga el Sistema Operativo.

##### Distribución de directorios
Linux:
- `/`: Directorio raiz
- `/bin`: Donde se encuentran los ejecutables del sistema.
- `/sbin`: Son los ejecutables del superusuario.
- `/boot`: Cómo se arranca el sistema, el bootloader y los kernels instalados.
- `/cdrom`: Directorio virtual donde tradicionalmente se montaban los CDs.
- `/mnt`: Directorio virtual donde tradicionalmente se montaba el resto de unidades.
- `/media`: Directorio virtual donde se montan actualmente los dispositivos.
- `/dev`: Directorio donde se encuentran los dispositivos del sistema 
- `/dev/loop*` => dispositivo de red locales (localhost)
- `/dev/zero` => dispositivo especial que devuelve ceros
- `/dev/null` => dispositivo especial que recibe entradas y la borra

##### Permisos en Linux
Nota: El prompt nos notifica de los permisos: `$` es usuario normal. `#` es un superusuario.

Al ejecutar el comando: `ls -lh` (ls largo, modo humanos), te devuelve la información sobre directorios y ficheros en el siguiente formato:

`permisos` `inodo` `propietario` `grupo` `tamaño` `fecha y hora modificación`

La primera letra de los permisos nos da información sobre el tipo de elemento que es:
- `d` => directorio
- `l` => enlace
- `c` => periférico
- `b` => dispositivo de bloques 

El resto de permisos usa la notación `UGO` (`user`,`group`,`other`) y hay tres posibles permisos para cada parte, `rwx` (`read`,`write`,`execute`).
Algunos puntos a tener en cuenta:
- En directorios, el permiso de ejecución (`x`) significa que lo podemos abrir.
- Los permisos 1 y 2 (en octal, `--x` y `-w-` en ugo), no tienen sentido ya que sin permiso de lectura (`r`) no podemos hacer nada.