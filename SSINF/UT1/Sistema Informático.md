El Sistema Informático es una caja negra. Que se sabe lo que hace, pero no como lo hace.

A mismas entradas, mismas salidas.
Aunque no lo parezca ya que pueden haber diversas entradas ocultas y/o aleatorias.

## Entrada/Salida


## CPU
![Arquitectura CPU|500](http://ignasibarri.com/blog/assets/vn.png)

Esta arquitectura se llama Vonn Newman, pero las usadas hoy en día son más complejas.

### Buses de la CPU
- (Address Bus) Direcciones = Salida (El ancho es la longitud de la memoria)
- (Control Bus) Control = Entrada/Salida
- (Data Bus) Datos = Entrada/Salida (El ancho es tamaño de los datos)

### Registros de la CPU
- (MDR/RIM) Registro de Intercambio de Memoria
- (MAR/RDM) Registro de Dirección de Memoria

### Componentes Internos
- (SR) Registro de Estado: Contiene las Flags
- (UC) Unidad de Control: Mayoría de la lógica de la CPU
- (IR) Registro de Instrucción: Contiene
- (TMPS) Accumulador: Registro temporal
- (PC) Contador de Programa: Dirección de memoria de por donde se está la ejecución
- (ALU) Unidad Aritmetico-Lógicas: Realiza las operaciones de la CPU
	- Suma, Resta, Multiplicación, División, Mayor qué, Menor qué, ...
- (Rn) Registros Internos


## Memoria
La memoria principal es la que se encarga de mantener cargados los datos necesarios para ejecutar los programas.

### Buses y Lineas de la Memoria
- (Address Bus) Direcciones = Entrada
- (Data Bus) Datos = Entrada/Salida
- (R/W) Linea de Lectura/Escritura
- (ChipSelect) Linea para deshabilitar un módulo
- (RAS y CAS) Subdivisiones del bus AB dentro de la distribución real de memoria
- (Refresh) Linea de refresco de la memoria

### Registros de la Memoria
- (MDR/RIM) Registro de Intercambio de Memoria
- (MAR/RDM) Registro de Dirección de Memoria

### Evolución de la memoria
- Memoria con tubos de vacío
- Memoria de transistores y condensadores
-  ![Memoria de ferrita|100](https://images.fineartamerica.com/images-medium-large-5/magnetic-core-memory-of-univac-computer-pasieka.jpg) ![Memoria de ferrita de cerca|150](https://upload.wikimedia.org/wikipedia/commons/0/04/KL_Kernspeicher_Makro_1.jpg)Memoria de ferrita
- Memoria de DiscPack


### Evolución de los procesadores
- Intel 4004 - 4 bits : se usó en calcuradoras con BCD para los decimales
- Intel 8080 - 8 bits : trabajaba directamente con binario
- AMD 2900 - 4 bits : se podían juntar, escalable hasta los 32 bits
- Motorola 6800 - 8 bits : equivalente al Intel 8080
- Zilog Z80 - 8 bits : basado en el Intel 8080 => ZX Spectrum
- Motorola 6800 => sale el Apple 1 y 2 (64KB de memoria) => Comodore
- Intel 8086 - 16 bits (max 640KB de memoria) => IBM PC
- Desaparece Zilog
- Motorola 68000 - 16 bits => Apple Mac 1 (MAC OS gráfico) => Comodore Amiga => Atari
- Aparece Windows (copia de MS DOS de IBM)
- Intel 80286 => IBM PC/AT
- Intel 80386 (i368): 32 bits => usa memoria vitrual
- Motorola se rindió con el mercado de ordenadores
- Intel 80486 (i486) => Intel Pentium
- Vuelve a aparecer AMD => copia el i486 => AMD 486DX => AMD K6 (primer 1 GHz 64b)
- Salen los Intel i3-5

La velocidad de los ordenadores se dobla cada 18 meses como media.


### Placa Base
Es simplemente un circuito impreso. 
- Sockets
- Puertos de Expansión
- Puertos [[IDE]] / Paralel ATA
- Puertos [[SATA]]
- ![Puerto Interno SCSI|200](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fimages-na.ssl-images-amazon.com%2Fimages%2FI%2F41eLK6A5QeL.__AC_SX300_QL70_ML2_.jpg&f=1&nofb=1) SCSI

- Bus trasero (Backend Bus) => Conecta GPU, Puente Norte, CPU y Memoria
- Bus frontal (FS Bus) => Conecta CPU y Puente Sur => USB, SATA...

### Discos duros:
Suelen tener una base plástica recubierta de material ferromagnetico, sobre la que pasa una cabeza lecto-escritora.

Se divide en pistas (concéntricas) y sectores. Todas las pistas tienen la misma capacidad y todos los sectores tienen la misma capacidad.

Por lo tanto la parte interior del disco tiene mayor capacidad que la exterior. Las pistas van numeradas de fuera hacia dentro, pero los sectores no son contiguos.

Tiene 3 tiempos: 
- Acceso/Posicionamiento: Lo que tarda la cebaza en situarse en la pista.
- Latencia: Lo que tarda el sector en situarse bajo la cabeza.
- Transferencia: Lo que se tarda en pasar la información a memoria.

Los cabezales de un disco duro se mueven de manera conjunta.
Los sectores no están situados de manera contigua, si no de manera Salteada ([Interleaving](https://en.wikipedia.org/wiki/Interleaving_(disk_storage)))

La capacidad de un disco: `nPlatos x nPistas x sectores/pista x bytes/sector`
### Conectores de la Placa Base [^1](https://drive.google.com/file/d/1lu5eo2LPzbF4qecVMAe9WEcAP6GhlE1J/view) 
### Conectores externos de la Placa Base
- Pantalla: DB-15 o [[VGA]], [[DVI]], [[HDMI]], [[DisplayPort]]
- Periféricos: [[PS2]] (morado|verde, teclado|ratón)
- Audio: [[Jack 3.5]] => MIC, EAR, Audio-IN
- Datos: Firewire, [[USB|USB-A]], USB-C, USB-B, MicroB
- Red: [[RJ-45]]
- Serial (DB-9) y Puerto Paralelo (DB-25)

### Conectores internos de la Placa Base
- ATX1 2v 24p - Alimentación de la placa
- EATX 12v - 4/8p - Alimentación del procesador
- SPDIFF - Audio de alta fidelidad
- 