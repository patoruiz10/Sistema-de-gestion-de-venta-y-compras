# Caso de uso: Apertura de Caja
* Actores primarios: Empleado, Encargado
* Actores secundarios: No tiene
* Precondición: El usuario debe estar logueado.
* Postcondición: No tiene

### Camino Básico
1. El usuario selecciona la opción “Apertura de Caja”.
2. El sistema abre la caja y muestra un mensaje indicando que la caja fue abierta correctamente (fecha y hora).


### Caminos alternativos:
2.a La caja ya se encuentra abierta.
2.a.1 El sistema muestra un mensaje: "La caja ya está abierta".
2.a.2 Fin de caso de uso.

### Escenario de éxito: 
* El usuario pudo realizar la apertura de caja.

### Escenario de fracaso: 
* El usuario no pudo realizar la apertura de caja por que la caja ya estaba abierta.