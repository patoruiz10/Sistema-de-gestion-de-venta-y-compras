# Caso de uso: Actualizar cantidad de productos
* Actores primarios: Empleado, Encargado
* Actores secundarios: No tiene
* Precondición: El usuario debe tener permisos para actualizar productos.
* Postcondición: No tiene

### Camino básico:

1. El usuario ingresa el código del producto e ingresa la nueva cantidad.
2. El sistema valida que la nueva cantidad no sea negativa, y muestra una alerta indicando que se actualizó correctamente.

### Caminos alternativos:
2.a El usuario ingresó una cantidad negativa.
2.a.1 El sistema muestra: "La cantidad ingresada no es válida".
2.a.2 Vuelve al paso 1.

2.b El usuario ingresó un código inexistente.
2.b.1 El sistema muestra: “El código de producto ingresado no existe”.
2.b.2 Vuelve al paso 1.

### Escenario de éxito:
* El usuario pudo actualizar la cantidad del producto.

### Escenario de fracaso:
* El usuario no pudo actualizar un producto por cantidad negativa.
* El usuario no pudo actualizar un producto por código inexistente.

