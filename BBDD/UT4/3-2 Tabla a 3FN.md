```c
PRESTAMO(_CodigoLibro->LIBRO_, _NumSocio_, nombreSocio, fecha)
LIBRO(_CodigoLibro_, titulo, CodigoAutor, nombreAutor)
```

```md
Dependencias Funcionales PRESTAMO:
- CodigoLibro, NumSocio -> fecha
- NumSocio -> nombreSocio

Dependencias Funcionales LIBRO:
- CodigoLibro -> titulo, CodigoAutor
- CodigoAutor -> nombreAutor
```
___
Está en 1FN?:
- Sí. Todos los atributos toman valores atómicos.

Está en 2FN?:
- Sí está en 1FN.
- No. Hay atributos que no dependen de forma `completa` de las `PK`.

```c
'PRESTAMO(_CodigoLibro->LIBRO_, _NumSocio->SOCIO_, fecha)
LIBRO(_CodigoLibro_, titulo, CodigoAutor, nombreAutor)
SOCIO(_NumSocio_, nombreSocio)
```

Está en 3FN?:
- Sí está en 2FN.
- No. El atributo `nombreAutor` es dependiente de `CodigoAutor` transitivamente.

```c
'PRESTAMO(_CodigoLibro->LIBRO_, _NumSocio->SOCIO_, fecha)
'LIBRO(_CodigoLibro_, titulo, CodigoAutor->AUTOR)
SOCIO(_NumSocio_, nombreSocio)
AUTOR(_codigoAutor_, nombreAutor)
```