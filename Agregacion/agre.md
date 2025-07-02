 
 # Mapa Conoceptual de Agregación
 
                             +-----------------------------+
                             |     Agregación en POO       |
                             +-----------------------------+
                                          |
                                          v
                   +---------------------------------------------+
                   | Relación "tiene un" entre objetos (Has-A)  |
                   +---------------------------------------------+
                                          |
              +---------------------------+---------------------------+
              |                                                       |
              v                                                       v
+---------------------------+                          +------------------------------+
|  Objeto Contenedor (Libro)|                          | Objeto Contenido (Autor)     |
+---------------------------+                          +------------------------------+
| - Tiene referencia a Autor|                          | - Existe independientemente  |
| - Puede tener múltiples   |                          | - Puede estar en múltiples   |
|   instancias de Autor     |                          |   libros                    |
+---------------------------+                          +------------------------------+
              |                                                       |
              +-----------------------> Pueden vivir                  |
                                          por separado <--------------+

                 Si se destruye el objeto contenedor,
                     el contenido puede seguir existiendo.


# Diagrama UML de Agregación

```plaintext
+----------------+          +----------------+
|     Autor      |          |      Libro     |
+----------------+          +----------------+
| - nombre: str  |<>------- | - titulo: str  |
+----------------+          | - autor: Autor |
| + __init__()   |          +----------------+
+----------------+          | + __init__()   |
                            +----------------+







