# Mapa Conceptual de Herencia 

                            +-------------------------------------+
                            |       Polimorfismo en POO           |
                            +-------------------------------------+
                                            |
                                            v
           +---------------------------------------------------------------+
           | Mismo método (misma interfaz), pero comportamientos distintos |
           | según la clase que lo implemente                              |
           +---------------------------------------------------------------+
                                            |
               +----------------------------+----------------------------+
               |                                                         |
               v                                                         v
+--------------------------+                              +--------------------------+
|     Clase Perro          |                              |     Clase Gato           |
+--------------------------+                              +--------------------------+
| + Método hablar():       |                              | + Método hablar():       |
|   imprime "Guau!"        |                              |   imprime "Miau!"        |
+--------------------------+                              +--------------------------+
               \                                                         /
                \                                                       /
                 \_________________    _______________________________/
                                   |  |
                                   v  v
                        +------------------------------+
                        |  Función: hacer_hablar()     |
                        |  - Recibe un objeto cualquiera|
                        |  - Llama a su método hablar() |
                        +------------------------------+

        Polimorfismo: Permite usar el mismo método en diferentes tipos
        - Código más flexible y extensible
        - No importa el tipo de objeto, solo que tenga el método esperado

# Diagrama UML de Herencia 

            <<interface>>
            Animal
               |
       +-------+--------+
       |                |
+--------------+  +--------------+
|    Perro     |  |    Gato      |
+--------------+  +--------------+
| + hablar()   |  | + hablar()   |
+--------------+  +--------------+

       (Ambas clases implementan el mismo método: hablar())

+------------------------------+
|      hacer_hablar(animal)    |
+------------------------------+
| - Recibe objeto con .hablar()|
| - Llama: animal.hablar()     |
+------------------------------+
