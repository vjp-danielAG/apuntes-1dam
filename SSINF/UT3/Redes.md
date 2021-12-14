# Redes
###### Historia
Por la década de los 70, se vio que los ordenadores necesitaban comunicarse entre si.

Al principio se usaban cables coaxiales para las conexiones. Lo que permitía conexiones de largas distancias, pero a cambio de ser una conexión muy lenta.

Luego salió el par trenzado junto con las conexiones telefonicas. Lo cual permitía una mayores velocidades, pero sigue siendo muy limitado.

Para redes más pequeñas se usa el RJ45 (UTP y STP), que son 4 pares trenzados, que permite gran capacidad de transmisión (100M), pero solo llega hasta los 100 metros.

Luego ya apareció la fibra óptica, que revolucionó las telecomunicaciones, permitiendo la comunicación de alta velocidad a largas distancias (50 kilometros).

Otra forma de comunicaciones son las inalámbricas. Entre ellas WiFi (cortas distancias) y WiMAX (largas distancias).
___

##### Componentes de una red
Estos son el Emisor, el Receptor y el Canal por el que pasa la información.

Además hay otro componente llamado `ruido`.

##### Mediciones
En REDES, todo se mide en `bits/s`.

##### Tipos de conexiones
- Punto a Punto o "Peer to Peer". Conexión directa 
- En bus o "Token Bus". Tiene el problema de la falta de redundancia.
- En anillo o "Token Ring". 
- Red en arbol. Las más comunes en redes internas.
- Red mallada o en estrella. 


##### Software de red
El software de red se suele basar en dos modelos (estandard): OSI y TCP/IP

El modelo OSI se divide en siete capas:
- Aplicación
- Presentación
- Sesión
- Transporte (trabaja con buzones/[[puertos]])
- Red (direcciones globales : trabaja con [[IP Address|IPs]])
- Enlace (dirección dispositivos de red : trabaja con [[MAC Address|MACs]])
- Fisica (cables)

El modelo OSI era demasiado complicado, así que se paso al modelo TCP/IP:
- Aplicación - `Aplicación/Presentación/Sesión`
- Transporte - `Transporte`
- Red - `Red`
- Enlace - `Enlace/Física`

Las MACs las tienen los Switchs, los Hubs y los NICs (tarjeta de red).

___
Los Routers trabajan en la capa de Red.

Pasarelas/Bridges trabajan en la capa de Transporte.

Dos tipos de puertos: TCP y UDP

Los routers sirven para unir redes.
Los switches y hubs para conectar dispositivos.

IPv4 => `255.255.255.255` o `ff.ff.ff.ff`

IPv6 => `ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff`

