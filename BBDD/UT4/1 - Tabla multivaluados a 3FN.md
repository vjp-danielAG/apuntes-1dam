```c
PERSONA(_DNI_, nombre, apellidos, direcciónes, cp, población, provincia)
```

```md
Dependencias Funcionales PERSONA:
- DNI -> Nombre, Apellidos, Direcciónes, CP
- CP -> Población, Provincia
```
___
Está en 1FN?
- No. El atributo Dirección es multivaluado. 

```c
PERSONA(_DNI_, nombre, apellidos)
DIRECCION(_cp_, _dirección_, población, provincia, DNI->PERSONA)
```

Está en 2FN?
- Sí está en 1FN.
- Si. Todos los atributos dependen de forma `completa` de las `PK`.

Está en 3FN?
- Sí está en 2FN.
- No. Hay dependencias transitivas (CP).

```c
PERSONA(_DNI_, nombre, apellidos)
DIRECCION(_cp->LOCALIZACION_, _dirección_, DNI->PERSONA)
LOCALIZACION(_cp_, población, provincia)
```