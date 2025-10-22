Enunciado del Problema:



En una cafetería pequeña, los pedidos se gestionan de forma manual y desorganizada, lo que genera pérdida de información, retrasos en la atención y dificultad para recuperar pedidos anteriores. El sistema actual no permite priorizar pedidos según su tipo (delivery, para llevar, en mesa), ni mantener un historial controlado.



Requerimientos Funcionales:

* 
* RF-01
* El sistema debe permitir registrar un nuevo pedido con descripción y tipo (mesa, llevar, delivery).
* RF-02
* Los pedidos deben almacenarse en una lista doblemente enlazada (DobleLinkedlist).
* RF-03
* El sistema debe atender el próximo pedido según prioridad:
* delivery > llevar > mesa
* RF-04
* Al atender un pedido, este debe marcarse como completado y moverse al historial.
* RF-05
* El historial debe implementarse con una lista simplemente enlazada (SimpleLinkedList) y limitarse a los últimos 10 pedidos.
* RF-06
* El sistema debe permitir buscar pedidos por descripción usando búsqueda lineal.
* RF-07
* El sistema debe permitir buscar pedidos por tipo (mesa, llevar, delivery) usando búsqueda lineal.
* RF-08
* El sistema debe mostrar todos los pedidos activos en orden de inserción.
* RF-09
* El sistema debe permitir deshacer la última acción realizada (registro o atención de pedido) mediante una pila (undoStack).
* RF-10
* El sistema debe permitir rehacer una acción deshecha mediante una pila auxiliar (redoStack).



Requerimientos No Funcionales:



* RNF-01
* Usabilidad: Interfaz de consola en español, clara y fácil de usar para usuarios sin experiencia técnica.
* RNF-02
* Rendimiento: Las operaciones básicas (agregar, atender, buscar) deben ejecutarse en tiempo constante o lineal, sin retrasos perceptibles.
* RNF-03
* Mantenibilidad: Código modular, con clases bien definidas, comentarios y nombres descriptivos.
* RNF-04
* Portabilidad: El sistema debe ejecutarse en cualquier máquina con Java 8 o superior, sin dependencias externas.
* RNF-05
* Confiabilidad: El sistema debe manejar entradas inválidas sin fallar (por ejemplo, tipos de pedido incorrectos).
* RNF-06
* Seguridad: No se requiere autenticación, pero el sistema no debe permitir acceso directo a estructuras internas desde fuera.



