# Mapa Conceptual de Asociación
                         +--------------------------------+
                         |       Asociación en POO        |
                         +--------------------------------+
                                        |
                                        v
             +-----------------------------------------------------+
             | Relación entre dos clases que se comunican          |
             | pero pueden existir independientemente              |
             +-----------------------------------------------------+
                                        |
             +--------------------------+--------------------------+
             |                                                     |
             v                                                     v
+-------------------------+                         +----------------------------+
|      Clase Profesor     |                         |        Clase Curso         |
+-------------------------+                         +----------------------------+
| - nombre: str           |                         | - nombre: str              |
| + ensenar(curso)        |                         |                            |
+-------------------------+                         +----------------------------+
             |                                                     |
             +--------------------------+--------------------------+
                                        |
                                        v
                       Asociación: comunicación sin dependencia
                - Profesor "usa" un Curso para enseñar  
                - Curso no necesita conocer al Profesor

# Diagrama UML de Asociación 
+----------------+          +----------------+
|    Profesor     |          |     Curso      |
+----------------+          +----------------+
| - nombre: str   |<>------- | - nombre: str  |
+----------------+          +----------------+
| + __init__()    |          | + __init__()   |
| + ensenar()     |          +----------------+
+----------------+