conceptos de kotlin:
Seguridad Nula (Null Safety): Kotlin aborda el problema de las referencias nulas de manera integral, lo que significa que el sistema de tipos ayuda a prevenir los errores de referencia nula durante la compilación

Funciones de Extensión (Extension Functions): Kotlin permite agregar nuevas funciones a clases existentes sin heredar de ellas o modificar su código fuente original

Inmutabilidad: Kotlin promueve el uso de datos inmutables siempre que sea posible, lo que facilita la programación concurrente y reduce los errores

Funciones Lambda: Kotlin tiene soporte nativo para funciones lambda, lo que facilita la escritura de código conciso y expresivo

Interoperabilidad con Java: Kotlin está diseñado para ser completamente interoperable con Java, lo que permite a los desarrolladores migrar gradualmente sus proyectos Java existentes a Kotlin

Tipos de Datos Enumerados (Enums): Kotlin ofrece una sintaxis mejorada para definir tipos enumerados, lo que facilita la creación de estructuras de datos enumeradas más potentes y expresivas

Data Classes: Las data classes en Kotlin permiten definir clases que solo contienen datos, eliminando la necesidad de escribir código boilerplate para métodos como equals(), hashCode(), toString(), entre otros

Corrutinas (Coroutines): Kotlin ofrece soporte para la programación asíncrona mediante corrutinas, que permiten escribir código asíncrono de manera secuencial, evitando los problemas de callback anidados

Funciones de Orden Superior (Higher-Order Functions): Kotlin permite el uso de funciones como parámetros de otras funciones, lo que facilita la escritura de código más modular y reutilizable

Tipos de Datos Nativos: Kotlin proporciona tipos de datos integrados para trabajar con colecciones, como List, Set, Map, entre otros, con métodos útiles y sintaxis mejorada en comparación con Java


variables:
val (inmutable):
Utilizas val para declarar variables inmutables, es decir, variables cuyo valor no puede cambiar una vez asignado.
Utilizas var para declarar variables mutables, es decir, variables cuyo valor puede cambiar durante la ejecución del programa.
ariables Primitivas:
Kotlin proporciona tipos de datos primitivos similares a Java, pero con algunas mejoras, como la prevención de errores de referencia nula (null safety).
Variables de Objetos:
Kotlin permite declarar variables que almacenan referencias a objetos de clases personalizadas o predefinidas.
Variables de Colecciones:
Kotlin proporciona tipos de datos específicos para trabajar con colecciones, como listas, conjuntos y mapas.
En Kotlin, las funciones también pueden asignarse a variables usando funciones lambda y funciones de orden superior.

constantes
1. const:
La palabra clave const se utiliza para definir constantes en tiempo de compilación. Esto significa que el valor debe ser conocido en el momento de la compilación y debe ser un tipo de dato primitivo o una cadena de caracteres.

Las constantes const solo pueden declararse en el nivel superior del archivo, es decir, fuera de cualquier función, clase o bloque.

2. val para valores inmutables:
Aunque no es una constante en el sentido estricto, puedes usar val para declarar valores inmutables que no cambiarán durante la ejecución del programa.
Solo se puede utilizar const en propiedades de nivel superior (top-level properties) o en miembros de objetos de compañía (companion object).
Los valores de const deben ser tipos de datos primitivos (como Int, Long, Double, etc.) o cadenas de caracteres (String).
Las constantes const se utilizan para valores que se conocen en tiempo de compilación y deben ser constantes en el contexto del bytecode generado.
  
opciones
Seguridad Nula: Manejo seguro de referencias nulas para evitar errores durante la ejecución del programa.

Funciones de Extensión: Agregar funcionalidades a clases existentes sin modificar su código.

Corrutinas: Soporte para programación asíncrona que simplifica la escritura de código concurrente.

Clases de Datos: Simplificación de la creación de clases que solo almacenan datos, generando automáticamente métodos como equals(), hashCode(), etc.

Funciones Lambda y de Orden Superior: Facilitan la escritura de código modular y reutilizable al permitir pasar funciones como parámetros o devolverlas como resultados.

manejo de nulos

En Kotlin, todos los tipos de datos por defecto son non-nullable, lo que significa que no pueden contener valores nulos a menos que se especifique explícitamente. Para permitir la asignación de valores nulos, debes declarar el tipo de dato como nullable agregando un ? al final del tipo.

Non-nullable Types (Tipos no nulos)
Los tipos de datos no nulos no pueden contener valores nulos y Kotlin te obligará a manejar cualquier posible nulo antes de compilar
val nombre: String = "Juan" // No puede ser nulo
val edad: Int = 30 // No puede ser nulo
``

Nullable Types (Tipos de datos anulables)
