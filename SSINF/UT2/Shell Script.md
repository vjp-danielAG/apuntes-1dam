### Shell Scripts
Lo primero que deben incluir todos los shell scripts es el `shebang`:

```bash
#!/bin/bash
```

El `shebang` es un comentarío especial con el que se especifica el intérprete de comandos que se debe usar para ejecutar el script.
___
#### Argumentos
Los argumentos de todos los scripts/comandos en linux son tratados como variables de solo lectura.

Estas variables son `$N`, siendo `N` la posición del argumento empezando en `1`.

Hay otras variables especiales:
- `$0`: El nombre del comando/script.
- `$#`: Número total de argumentos.
- `$?`: Resultado de ejecución de la orden anterior.
___

#### Control de Flujo
```bash
if [ condicion ]; then
	...
else
	...
fi
```

En shell script no existe la sentencia `else if`, y la sentencia `else` es opcional.
___

#### Condiciones
Si lo que se compara son `strings`, tenemos los siguientes operadores:
- `==`, `!=`: igual que, diferente de.
- `>`, `>=`: mayor que, mayor o igual que. (ordena alfabeticamente)
- `<`, `<=`: menor que, menor o igual que. (ordena alfabeticamente)
- `-z`:  está vacía.

Si lo que se compara son `numeros`, tenemos los siguientes operadores:
- `eq`, `ne`: igual que, diferente de.
- `gt`, `ge`: mayor que, mayor o igual que.
- `lt`, `le`: menor que, menor o igual que.

Si lo que se compara son `rutas/ficheros`, tenemos los siguientes operadores:
- `-f`: es un fichero y existe.
- `-d`: es un directorio y existe.