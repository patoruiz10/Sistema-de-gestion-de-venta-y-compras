# Caso de uso: Registrar producto nuevo

* Actores primarios: Empleado, Encargado
* Actores secundarios: No tiene
* Precondición: El usuario debe tener permisos.
* Postcondición: El producto queda asociado a su proveedor y categoría correspondientes.

### Camino básico

1. El usuario  ingresa los datos: código, descripción, cantidad, precio unitario, CUIT del proveedor y nombre de categoría.
2. El sistema agrega el producto al listado de productos.

### Caminos alternativos

2.a Algún campo obligatorio está vacío.  
2.a.1 El sistema muestra: "Faltan completar campos obligatorios".  
2.a.2 Vuelve al paso 1.

2.b El código del producto ya existe.
2.b.1 El sistema muestra: "El código del producto ingresado ya existe".  
2.b.2 Vuelve al paso 1.

2.c El proveedor no existe.  
2.c.1 El sistema muestra: "El proveedor ingresado no existe".  
2.c.2 Vuelve al paso 1.

2.d La categoría no existe.  
2.d.1 El sistema muestra: "La categoría ingresada no existe".  
2.d.2 Vuelve al paso 1.

### Escenario de éxito

* El usuario registró el producto correctamente.

### Escenario de fracaso

* El usuario no pudo registrar el producto por campos incompletos.
* El usuario no pudo registrar el producto por código repetido.
* El usuario no pudo registrar el producto por proveedor inexistente.
* El usuario no pudo registrar el producto por categoría inexistente.
