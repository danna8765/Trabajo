# Mapa Conceptual de Composición
                           +----------------------------------+
                           |      Composición en POO         |
                           +----------------------------------+
                                         |
                                         v
            +-------------------------------------------------------+
            | Relación "parte-de" más fuerte entre dos clases       |
            | Una clase contiene completamente a otra               |
            +-------------------------------------------------------+
                                         |
         +-------------------------------+-------------------------------+
         |                                                               |
         v                                                               v
+---------------------------+                             +---------------------------+
|   Clase Contenedora       |                             |   Clase Compuesta         |
|       (Coche)             |                             |       (Motor)             |
+---------------------------+                             +---------------------------+
| - Crea y posee Motor      |                             | - No puede existir solo   |
| - Controla su ciclo de    |                             | - Se crea dentro del Coche|
|   vida                   |                             |                           |
+---------------------------+                             +---------------------------+
         |                                                               |
         +-------------------------------> Si Coche se destruye         |
                                         entonces Motor también. <------+

                    Composición: Relación de "propiedad total"
                   - El objeto contenido depende del contenedor
                   - No puede existir por separado ni compartirse
# Diagrama UML de Composición
+----------------+          +----------------+
|     Coche      |<>------- |     Motor      |
+----------------+          +----------------+
| - motor: Motor |          | - tipo: str    |
+----------------+          +----------------+
| + __init__()   |          | + __init__()   |
| + encender()    |          | + arrancar()   |
+----------------+          +----------------+