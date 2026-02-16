# Caso de uso: Actualizar cantidad de productos
* Actores primarios: Empleado, Encargado
* Actores secundarios: No tiene
* Precondición: El usuario debe tener permisos para actualizar productos.
* Postcondición:  No tiene

### Camino básico:

1. El usuario selecciona la opción “Actualizar cantidad de productos”.
2. El sistema solicita el código del producto a actualizar.
3. El usuario ingresa el código del producto e ingresa la nueva cantidad.
4. El sistema busca el producto por código, actualiza la cantidad en stock reemplazando la anterior y muestra una alerta indicando que se actualizó correctamente.

### Caminos alternativos:
4.a El usuario ingresó una cantidad negativa.
4.a.1 El sistema muestra una alerta indicando que la cantidad ingresada no es válida.
4.a.2 Vuelve al paso “3”.
4.b El usuario ingresó un código inexistente.
4.b.1 El sistema muestra una alerta: “El código del producto ingresado no existe”.
4.b.2 Vuelve al paso “3”.

### Escenario de éxito:
* El usuario pudo actualizar la cantidad del producto.

### Escenario de fracaso:
* El usuario no pudo actualizar un producto por código inexistente.
* El usuario no pudo actualizar un producto por cantidad negativa.
