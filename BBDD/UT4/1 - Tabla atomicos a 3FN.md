```c
PERSONA(DNI_, nombre, apellidos, dirección, cp, población, provincia)
```

```
Dependencias Funcionales PERSONA:
- DNI -> Nombre, Apellidos, Dirección, CP
- CP -> Población, Provincia
```
___
Está en 1FN?
- Sí. Todos los atributos toman valores atómicos.

Está en 2FN? 
- Sí está en 1FN.
- Sí. Todos los aributos que no forman parte de la `PrimaryKey` dependen de ella de forma `completa`.

Está em 3FN?
- Sí está en 2FN.
- No. Hay dependencias funcionales transitivas.

```c
PERSONA(_DNI_, nombre, apellidos, dirección, cp->LOCALIZACION)
LOCALIZACION(_CP_, población, provincia)
```