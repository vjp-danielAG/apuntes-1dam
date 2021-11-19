```c
TRATAMIENTO(_DNI_, _CodTratamiento_, nombre, importe)
```

```md
Dependencias Funcionales de TRATAMIENTO:
- DNI, CodTratamiento -> importe
- DNI -> nombre
```
___
Está en 1FN?
- Sí. Todos los atributos toman valores atómicos.

Está en 2FN?
- Sí está en 1FN.
- No. El atributo `nombre` no tiene dependencia `completa` de ambas  `PK`.

```c
'TRATAMIENTO(_DNI->CLIENTE_, _CodTratamiento_, importe)
CLIENTE(_DNI_, nombre)
```

Está en 3FN?
- Sí está en 2FN.
- Si. No hay dependencias transitivas.