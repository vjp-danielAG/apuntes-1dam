### Periféricos
Un periférico es un dispositivo axiliar e independiente que se conecta a la placa base.
___

##### Teclado
Sirve únicamente para entrada. Se compone de una matriz de cables, un codificador y una interfaz serial. Normalmente usan la distribución QWERTY. Hay varios tipos de teclados:
- Mecánicos
- Membrana
- Táctiles
___

##### Ratón
Sirve únicamente para entrada. Originalmente se usaba una bola para determinar el movimiento del ratón, pero actualmente se utiliza una fuente de luz y una matríz de sensores foto-eléctricos. Hay dos tipos de ratones.
- Direcciónal: Indica la dirección en la que debe moverse el cursor.
- Posicional: Indica la posición en la que debe estar el cursor.

##### TrackBall:
Sirve únicamente para entrada. Es como un ratón de bola, pero invertido, ya que lo que se mueve es la bola, en vez del ratón entero.
___

##### Impresoras: 
[Impresoras de impacto](https://es.wikipedia.org/wiki/Impresora_de_impacto) 
(normalmente las líneas eran de 80 o 132 caracteres)

[Impresora de líneas](https://es.wikipedia.org/wiki/Impresora_de_l%C3%ADnea)

[Impresora de matricial](https://es.wikipedia.org/wiki/Impresora_matricial)

Las había de 9, 18, 27, 36 agujas. Mucha resolución (72, 360 ppp)

Ventajas: 
- Puedes modificar el juego de caracteres
- Puedes hacer gráficos en blanco y negro
- Las cintas de tinta son muy baratas y algunas reutilizables
- El mecanismo es mucho más simple
- Son mucho más silenciosas
- Se puede usar papel autocopiante (las buenas hasta 4 copias)
- Se puede usar hojas sueltas, no hace falta papel continuo
- Son mucho más ligeras
- Mayor rango de formatos de papel

Desventajas: Casi ninguna comparativamente

[Impresora Térmica](https://es.wikipedia.org/wiki/Impresora_t%C3%A9rmica)

[Impresora de injección de tinta](https://es.wikipedia.org/wiki/Impresora_de_inyecci%C3%B3n)

Cada inyector se puede controlar independientemente. Tienen mucha mayor resolución, alrededor los 600 ppp. El cabezal no hace contacto con el papel y son más silenciosas. 

Los hay de varios tipos:
- Depósito removible: El cabezal es fijo y es parte de la impresora.
- Cartucho con cabezal: El cabezal está incluido en el propio cartucho. Tienen el problema de tener que alinear los diferentes cabezales de forma independiente y la limpieza de los cabezales. Si el cabezal se obtruye, se puede cambiar el cartucho. Son buenas para impresión a pequeña escala. 

Para impresoras fotográficas, se necesita usar papel especial, y mayor variedad de tintas.
Cyan, Magenta, Amarillo y Negro (CMYK) son los colores que se usan en impresoras normales.
- No se debe tocar una hoja recién impresa, porque la impresora tarda en secar. El tiempo de sacado depende de la cantidad de tinta.
- No hacen copia con papel autocopiante.
- Imprimir imágenes es un proceso lento, ya que precisa de muchos cálculos.

[Impresoras Láser](https://es.wikipedia.org/wiki/Impresora_l%C3%A1ser)
Una impresora láser se basa en un rodillo fotosensible que se carga electricamente según reciba, o no, luz. El principio de funcionamiento es sencillo, y se basa en cargas electroestáticas.
- Un rodillo cargado electroestaticamente se lleva las partículas del toner y las lleva a el papel. Luego el papel pasa por un fusor, que derrite las partículas en el papel.
- La función del láser/leds es descargar parte del rodillo, para que las partículas no se peguen al rodillo. [Xerografía](https://es.wikipedia.org/wiki/Xerograf%C3%ADa)
- También hay dos tipos de cartuchos: Con rodillo, o solo el toner.
___

##### [Impresoras 3D](https://es.wikipedia.org/wiki/Impresora_3D)
Las impresoras 3D están compuestos por: una plataforma de cristal que hace de suelo (que debe estar perfectamente nivelada) y un marco por el que se mueven tres motores (uno por eje), que desplazan una cabeza extrusora que se encarga de depositar material.

También hay otro tipo de impresoras que imprimen con resina, pero estas funcionan de forma diferente.
Normalmente usan filamentos de plástico, pero hay algunas que pueden usar metales blandos (aplicaciones industriales).

El producto final no tiene muy buen acabado, y suele hacer falta pulir y quitar material sobrante.
___

##### [Escaner](https://es.wikipedia.org/wiki/Esc%C3%A1ner_inform%C3%A1tico)
La barra del escaner no es mas que un sensor CCD (Charge Coupled Device) que se mueve de un lado a otro. 

Originalmente solo escaneaban en blanco y negro, luego se pasó a escala de grises, y luego ya se empezó a incrementar la gama de colores  ([[Codificación de Color|RGB]]) que los escáneres podían diferenciar. Las resoluciones más común es de 8000ppp.
___

##### Cámara
El funcionamiento es muy similar al de un escaner, pero esta vez con una matríz de sensores. Suelen tener un problemas para filtrar la luz infrarroja.
___

##### Tarjeta de Sonido
Suelen tener un bus de entrada, un DSP (Digital Signal Processor) y buses que conectan a su propia memoria.

El DSP se encarga de hacer el postprocesado, es decir; eco, reberv, etc.

La salida de las tarjetas de sonido van a un DAC (Digital to Analog Converter) y un ADC (Analog to Digital Converter) se encarga de la entrada.

El sonido son ondas puras, pero el ordenador lo que hace es convertir esto a muestras discretas, es decir a números entre 0 y MAX (que determina la resolución).

[Teorema de Nyquist](https://es.wikipedia.org/wiki/Teorema_de_muestreo_de_Nyquist-Shannon):
Para poder muestrear una frecuencia, por lo menos hay que poder escuchar el doble.

No hay problema con tener una resolución de 0-4000Hz en un microfono (la voz humana llega a los 3800Hz), pero el oido humano escucha hasta los 20-20.000Hz, así que para grabar en estereo hacen falta 80.000Hz (40.000 por lado).

La tarjeta de sonido no solo sirve para capturar y reproducir sonidos, si no que también sirve para generar sonido. Hay dos formas de hacer esto:
- Tabla de ondas: Una tabla donde se guardan grabaciones de instrumentos reales. No se graban todas las notas, si no que se hace de forma salteada, y el resto se interpolan de las que tenemos grabadas. La tabla de ondas más usada es la Tabla MIDI. Está muy bien definida; hay 256 instrumentos y de ellos los 128 primeros intrumentos son canónicos. Además, los últimos 64 instrumentos no están definidos.
- Síntesis FM: Para generar un sonido se añaden ondas para emular los sonidos. De esta forma se intenta emular instrumentos reales. Hoy en día se usa mayoritariamente para la síntesis de voz. La modulación de frecuencia es un proceso que usa bastante CPU.

Conectores internos:
- Entrada: CD/BlueRay/S-PDIF
- Salida interna: S-PDIF para conectarse a otra tarjeta, o para sonido digital HDMI.

Conectores externos: Todos suelen ser estereo.
- IN: Entrada de audio de alta fidelidad (20 a 22000Hz).
- OUT: Salida de audio de alta fidelidad (20 a 22000Hz).
- MIC: Entrada de audio de un microfono (0 a 4000Hz).
- EAR: Salida de audio para auriculares. Suelen recortar bajos y altos.

Además, algunas incluyen más puertos, para sistemas de audio 5.1:
- OUT-F: Salida frontal
- OUT-R: Salida lateral (rear)

Otros conectores que pueden tener:
- S/PDIF: Sonido digital.
- Óptico o RCA: Sonido digital directo a altavoces.
- [[MIDI]]: Comandos para instrumentos.
___
##### Tarjeta Gráfica
La GPU no deja de ser un procesador especializado. Está conectado al bus principal del sistema, por lo que tiene acceso a la memoria principal del sistema (RAM).

Las GPU tienen su propia memoria interna/local con la que trabajan, y no hacen uso de la CPU, salvo para realizar operaciones que no tienen conocimiento de como realizar.

Varias tarjetas gráficas pueden trabajar como una sola mediante el uso de Crossfire/SLI (ATI/Nvidia).

La memoria de una GPU se divide en una parte reservada para la pantalla (screen buffer), y la memoria de computo.

Suelen soportar varios tipos de salida:
- VGA y DVI, que usan las señales `R G B`, `SyncHorizontal`, `SyncVertical`.
- HDMI.
___

##### Pantalla
Las primeras pantallas no usaban un modo gráfico, por lo que en vez de mostrar una matriz de píxeles, trabajaban matrizes de [[Codificación de Caracteres|caracteres]] y un color simple con atributos.

Luego ya se pasó al modo gráfico, en el que cada pixel se podía controlar independientemente.

Los primeros modelos se usaba CGA y permitia hasta una resolución de 640x200p, luego se pasó a EGA con [[Codificación de Color|RGB]] (con 4 bits), que permitió hasta 640x480p y con codificación [[Codificación de Color|RGB]] (con 8 bits).

Más tarde llegó VGA y el TrueColor ([[Codificación de Color|RGB]] con 16 bits `554`), y hoy en día se utiliza XGA, que usa la codificación [[Codificación de Color|RGB]] (con 24 bit `888`), que alcanza 1360x1024p.

Hoy en día está FullHD, que llega a los 1920x1080p, que soporta TrueColor (de 24 y 32 bits).
___

##### JoyStick
El joystick se inventó antes que el ratón. Se enchufaban por puerto serial, y los primeros no podían mandar direcciones en diagonal.

Luego esto evolucionó, y se usaba un potenciometro por eje.
La señal analógica de los potenciometros se pasaba por un ADC, y con eso se alcanzaba muchas más direcciones. Estos ya usaban el GamePort para conectarse.

Hoy en día los controles de consola suenen llevar dos controles direccionales. Es decir, dos joysticks, o un joystick y un DPad (Cruzeta).