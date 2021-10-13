## Almacenamiento de Información
### Discos duros:
Suelen tener una base plástica recubierta de material ferromagnetico, sobre la que pasa una cabeza lecto-escritora.

Se divide en pistas (concéntricas) y sectores. Todas las pistas tienen la misma capacidad y todos los sectores tienen la misma capacidad.

Por lo tanto la parte interior del disco tiene mayor capacidad que la exterior. Las pistas van numeradas de fuera hacia dentro, pero los sectores no son contiguos.

Tiene 3 tiempos: 
- Acceso/Posicionamiento: Lo que tarda la cebaza en situarse en la pista.
- Latencia: Lo que tarda el sector en situarse bajo la cabeza.
- Transferencia: Lo que se tarda en pasar la información a memoria.

Los sectores no están situados de manera contigua, si no de manera Salteada ([Interleaving](https://en.wikipedia.org/wiki/Interleaving_(disk_storage)))

La capacidad de un disco es determinada por: Bytes/Cilindro x NºPistas