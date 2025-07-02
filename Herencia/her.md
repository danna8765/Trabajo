#  Mapa Conceptual de Herencia

```plaintext
                             +-------------------------------+
                             |       Herencia en POO         |
                             +-------------------------------+
                                          |
                                          v
             +---------------------------------------------------------+
             | Permite que una clase hija herede atributos y métodos   |
             | de una clase padre (reutilización de código)            |
             +---------------------------------------------------------+
                                          |
             +----------------------------+----------------------------+
             |                                                         |
             v                                                         v
+----------------------------+                         +-----------------------------+
|     Clase Padre            |                         |      Clase Hija             |
|     (Persona)              |                         |      (Estudiante)           |
+----------------------------+                         +-----------------------------+
| - Atributo: nombre         |                         | - Hereda nombre             |
| - Método: saludar()        |                         | - Método propio: estudiar() |
+----------------------------+                         +-----------------------------+
             |                                                         |
             +----------------------------+----------------------------+
                                          |
                                          v
                 Herencia: "Es un tipo de..." (Estudiante es una Persona)
                 - Reutiliza código existente
                 - La clase hija puede extender o sobrescribir comportamientos
```
## Diagrama UML 

```plaintext
+----------------+
|    Persona     |
+----------------+
| - nombre: str  |
+----------------+
| + __init__()   |
| + saludar()    |
+----------------+
         ▲
         |
+--------------------+
|    Estudiante      |
+--------------------+
| + estudiar()       |
+--------------------+
