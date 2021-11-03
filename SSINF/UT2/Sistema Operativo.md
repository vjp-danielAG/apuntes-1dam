#### Sistema Operativo
El [[Sistema Operativo]] (SO o OS) es un programa o conjunto de programas que dotan de funcionalidad al ordenador, y proveen servicios a otros programas (aplicaciones).

Los [[Sistema Operativo|SO]] están programados por capas (como una cebolla):
- Kernel: Es núcleo que provee servicios al resto del SO y es la parte más cercana al procesador. Suele estar programado en ensamblador. El usuario no hace llamadas al Kernel de forma directa.
- Modulos: Son los procesos que llaman al Kernel.
	- Gestior de Procesos: Es el programa encargado de cargar y ejecutar procesos. Llama al kernel para que cambie el proceso en ejecución.
	- Gestion de Memoria: La memoria se solía dividir en segmentos de 64KB, pero ahora se está dividiendo en 256KB. Cuando la memoria principal (RAM) se llena, los segmentos de memoria que no estén en uso, se copian a disco, y se carga otro segmento.
	- Gestión de Disco: Los discos al igual que la memoria se divide en bloques, pero pueden sufrir de problemas de fragmentación. Esto es el por qué Windows se realentiza con el tiempo. Normalmente los bloques son de 32-64KB para sistemas multimedia o con gráficos, y para sistemas ofimáticos 8-16KB. 
 
