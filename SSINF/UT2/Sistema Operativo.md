#### Sistema Operativo
El [[Sistema Operativo]] (SO o OS) es un programa o conjunto de programas que dotan de funcionalidad al ordenador, y proveen servicios a otros programas (aplicaciones).

Los [[Sistema Operativo|SO]] están programados por capas (como una cebolla):
- Kernel: Es núcleo que provee servicios al resto del SO y es la parte más cercana al procesador. Suele estar programado en ensamblador. El usuario no hace llamadas al Kernel de forma directa.
- Modulos: Son los procesos que llaman al Kernel.
	- Gestior de Procesos: Es el programa encargado de cargar y ejecutar procesos. Llama al kernel para que cambie el proceso en ejecución.