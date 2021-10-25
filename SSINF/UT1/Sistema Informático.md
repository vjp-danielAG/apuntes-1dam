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
- etc...

### Periféricos
Un periférico es un dispositivo axiliar e independiente que se conecta a la placa base.

Entrada:
- Teclado: Sirve únicamente para entrada. Se compone de una matriz de cables, un codificador y una interfaz serial. Normalmente usan la distribución QWERTY. Hay varios tipos de teclados:
	- Mecánicos
	- Membrana
	- Táctiles


- Ratón: Sirve únicamente para entrada. Originalmente se usaba una bola para determinar el movimiento del ratón, pero actualmente se utiliza una fuente de luz y una matríz de sensores foto-eléctricos. Hay dos tipos de ratones.
	- Direcciónal: Indica la dirección en la que debe moverse el cursor.
	- Posicional: Indica la posición en la que debe estar el cursor.

- TrackBall: Sirve únicamente para entrada. Es como un ratón invertido.

Salida:
- Impresoras: 
	- [Impresoras de impacto](https://es.wikipedia.org/wiki/Impresora_de_impacto) (normalmente las líneas eran de 80 o 132 caracteres)
	- [Impresora de líneas](https://es.wikipedia.org/wiki/Impresora_de_l%C3%ADnea)
	- [Impresora de matricial](https://es.wikipedia.org/wiki/Impresora_matricial)
		- Las había de 9, 18, 27, 36 agujas. Mucha resolución (72, 360 ppp)
		- Ventajas: 
			- Puedes modificar el juego de caracteres
			- Puedes hacer gráficos en blanco y negro
			- Las cintas de tinta son muy baratas y algunas reutilizables
			- El mecanismo es mucho más simple
			- Son mucho más silenciosas
			- Se puede usar papel autocopiante (las buenas hasta 4 copias)
			- Se puede usar hojas sueltas, no hace falta papel continuo
			- Son mucho más ligeras
			- Mayor rango de formatos de papel
		- Desventajas: Casi ninguna comparativamente
	- [Impresora Térmica](https://es.wikipedia.org/wiki/Impresora_t%C3%A9rmica)
	- [Impresora de injección de tinta](https://es.wikipedia.org/wiki/Impresora_de_inyecci%C3%B3n)
		- Cyan, Magenta, Amarillo y Negro (CMYK) son los colores que se usan.
		- Cada inyector se puede controlar independientemente. Tienen mucha mayor resolución, alrededor los 600 ppp. El cabezal no hace contacto con el papel y son más silenciosa.
		- De depósito removible: El cabezal es fijo y es parte de la impresora.
		- Cartucho con cabezal: El cabezal está incluido en el propio cartucho. Tienen el problema de tener que alinear los diferentes cabezales de forma independiente y la limpieza de los cabezales. Si el cabezal se obtruye, se puede cambiar el cartucho. Son buenas para impresión a pequeña escala. 
		- Para impresoras fotográficas, se necesita usar papel especial, y mayor variedad de tintas.
		- No se debe tocar una hoja recién impresa, porque la impresora tarda en secar. El tiempo de sacado depende de la cantidad de tinta.
		- No hacen copia con papel autocopiante.
		- Imprimir imágenes es un proceso lento, ya que precisa de muchos cálculos.
	- [Impresoras Láser](https://es.wikipedia.org/wiki/Impresora_l%C3%A1ser)
		- Una impresora láser se basa en un rodillo fotosensible que se carga electricamentesegún reciba, o no, luz. El principio de funcionamiento es sencillo, y se basa en cargas electroestáticas.
		- Un rodillo cargado electroestaticamente se lleva las partículas del toner y las lleva a el papel. Luego el papel pasa por un fusor, que derrite las partículas en el papel.
		- La función del láser/leds es descargar parte del rodillo, para que las partículas no se peguen al rodillo. [Xerografía](https://es.wikipedia.org/wiki/Xerograf%C3%ADa)
		- También hay dos tipos de cartuchos: Con rodillo, o solo el toner.
	- [Impresoras 3D](https://es.wikipedia.org/wiki/Impresora_3D)
		- Las impresoras 3D están compuestos por: una plataforma de cristal que hace de suelo (que debe estar perfectamente nivelada) y un marco por el que se mueven tres motores (uno por eje), que desplazan una cabeza extrusora que se encarga de depositar material.
		- También hay otro tipo de impresoras que imprimen con resina, pero estas funcionan de forma diferente.
		- Normalmente usan filamentos de plástico, pero hay algunas que pueden usar metales blandos (aplicaciones industriales).
		- El producto final no tiene muy buen acabado, y suele hacer falta pulir y quitar material sobrante.
	- [Escaner](https://es.wikipedia.org/wiki/Esc%C3%A1ner_inform%C3%A1tico)
		- La barra del escaner no es mas que un sensor CCD (Charge Coupled Device) que se mueve de un lado a otro. 
		- Originalmente solo escaneaban en blanco y negro, luego se pasó a escala de grises, y luego ya se empezó a incrementar la gama de colores  (RGB) que los escáneres podían diferenciar. Las resoluciones más común es de 8000ppp.
	- [Cámara]()
		- El funcionamiento es muy similar al de un escaner, pero esta vez con una matríz de sensores. Suelen tener un problemas para filtrar la luz infrarroja.