El Sistema Informático es una caja negra. Que se sabe lo que hace, pero no como lo hace.

A mismas entradas, mismas salidas.
Aunque no lo parezca ya que pueden haber diversas entradas ocultas y/o aleatorias.

## Entrada/Salida


## CPU
![Arquitectura CPU|500](http://ignasibarri.com/blog/assets/vn.png)

Esta arquitectura se llama Vonn Newman, pero las usadas hoy en día son más complejas

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