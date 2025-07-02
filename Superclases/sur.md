#  Mapa Conceptual de Superclases

```plaintext
                           +----------------------------------+
                           |         Superclase en POO        |
                           +----------------------------------+
                                         |
                                         v
              +----------------------------------------------------+
              | Clase base de la cual otras clases heredan         |
              | atributos y métodos                                 |
              +----------------------------------------------------+
                                         |
              +---------------------------+------------------------+
              |                                                    |
              v                                                    v
+---------------------------+                        +--------------------------+
|    Clase Superclase       |                        |     Clase Subclase       |
|       (Vehiculo)          |                        |        (Coche)           |
+---------------------------+                        +--------------------------+
| - Atributo: marca         |                        | - Hereda marca           |
| - Método: arrancar()      |                        | - Hereda método arrancar()|
+---------------------------+                        +--------------------------+
                                         |
                       Relación "es-un tipo de"
                      - Subclase reutiliza código de superclase
                      - Subclase puede extender o modificar comportamiento

```
## Diagrama UML 
```plaintext

+---------------------+
|     Vehiculo        |  <<superclase/base class>>
+---------------------+
| - marca: str        |
+---------------------+
| + __init__(marca)   |
| + arrancar()        |
+---------------------+
          ▲
          |
+---------------------+
|       Coche         |  <<subclase/derived class>>
+---------------------+
|  (hereda todo)      |
+---------------------+
