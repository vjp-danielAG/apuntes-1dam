tags: #lenguaje #programacion
links: [presentación](https://docs.google.com/presentation/d/e/2PACX-1vTkpmUXkJd9HnyyKq6PnIQuohJGnz-ZIR-nXOseRJuAShtTMJoiZiDeAJhwLPWGQOKYiF0hbO0574ni/pub?start=false&loop=false&delayms=20000), [información sobre C++](https://www.zator.com/Cpp/E4_11_2d.htm)

### ¿Qué es [[C++]]?
[[C++]] es un lenguaje de programación multiparadigma creado en 1979. 
También es conocido como [[C++|Cpp]] o [[C++|Cxx]].

[[C++]] es un lenguaje híbrido que fue creado con la intención de extender el lenguaje [[C]] para agregar funcionalidad necesaria para crea y manipular [[OOP|Objetos]].

### Origen
El nombre de [[C++]] lo propuso Rick Mascitti en 1982, cuando se comenzó a comercializar el lenguaje. Al principio simplemente se le llamaba "[[C]] extendido", "[[C]] orientado a objetos" o "[[C]] con clases".

Como este lenguaje es una versión extendida de [[C]], se le llamó [[C++]].
Esto literalmente significa "el Incremento de [[C]]"; ya que ++ es el operador de incremento en la mayoría de lenguajes de programación.

### Ventajas de [[C++]]
- Sintaxis similar a la de [[C]]
- Soporta programación Orientada a Objetos
- Los programas escritos en [[C]]/[[C++]] suelen ser más rapidos y ocupar menos
- Ofrece un mayor control sobre la memoria del programa y del sistema 
- Al ser un lenguaje estandarizado, existen compiladores para la gran mayoría de [[Arquitectura|Arquitecturas]] y [[SO|Sistemas Operativos]]
- Permite programación modular haciendo uso del sistema de dependencias

### Desventajas de [[C++]]
- Hay que compilar el programa para cada [[SO|Sistema Operativo]], y para cada [[Arquitectura|Arquitectura de procesador]] individualmente
- No hay un Gestor de Memoria o [[Garbage Collector]], por lo que hay que liberar la memoria manualmente, lo que aumenta la complejidad de los programas escritos en [[C++]].


### ¿Para qué se usa [[C++]]?
Al ser un lenguaje multiparadigma, este tiene muchos usos, pero entre ellos destacan:
- Desarrollo de Sistemas Operativos
- Desarrollo de Videojuegos
- Desarrollo de Videojuegos en Unreal Engine
- Aplicaciones para [[SOC|Sistemas Embebidos]]
- Firmware y Drivers

### Software programado en [[C++]]
-   Chromium
-   Bitcoin
-   BitTorrent
-   Open Broadcaster Software (OBS)
-   Navegador Web Opera

### [[HelloWorld]] en [[C++]]
```cpp
#include <iostream>  // Entrada/Salida
using namespace std; // Libreria base de C

int main() { // Punto de entrada
	cout << "HelloWorld" << endl; 
	return 0; // Codigo de error
}
```

### Clases
```cpp
// Ejemplo de Clase
class Animal { // Declaración de la clase
public: // Modificador de acceso
	string nombre; // Variable
	// Constructor
	Animal(string nombre_animal) {
		this.nombre = nombre_animal;
	}
	void DecirNombre() { cout << this.nombre << endl; }
}
```

```cpp
// Ejemplo de Herencia
class Perro : public Animal { // Hereda de Animal
public:
	// Constructor alternativo | El Constructor no se hereda
	Perro(string nombre_animal):nombre(nombre_animal){}
	// Implementa un método nuevo
	void Ladrar() { cout << "Woof!" << endl; }
}
```

```cpp
int main() {
	// Creación
	Animal _animal = new Animal("Toby");	// Declaración estandar
	Perro* _perro = new Perro("Thor");		// Declaración persistente
	// Uso
	_animal.DecirNombre();	// => Toby
	_animal.nombre = "Leo"; // Ok
	_animal.Ladrar();		// Error: no está en Animal
	_perro->DecirNombre();	// => Thor
	_perro->nombre = "Leo"; // Ok
	_perro->Ladrar();		// => Woof!
	// Destrucción
	delete _perro; // "_perro" hay que destruirlo manualmente

	return 0;
	// "_animal" se destruye automaticamente en este punto
}	
```