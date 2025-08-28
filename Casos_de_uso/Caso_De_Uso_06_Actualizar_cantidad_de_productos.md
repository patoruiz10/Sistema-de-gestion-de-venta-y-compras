# Caso de uso: Actualizar cantidad de productos
* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos para actualizar productos
* Postcondición: No tiene

### Camino básico:

1. El usuario selecciona la opción de “Actualizar cantidad de productos” dentro del sistema.  
2. El sistema muestra todos los productos registrados.  
3. El usuario modifica los precios del producto que desea cambiar, y termina el proceso guardando los datos seleccionando en la opción “Guardar”.  
4. El sistema muestra mediante una alerta visual que el producto se actualizó correctamente.

### Caminos alternativos:
4.a El usuario ingresó un precio negativo.  
4.a.1 El sistema muestra una alerta visual con un mensaje que informa que el precio ingresado no es válido.  
4.a.2 Vuelve al paso “3”.

### Escenario de éxito:

* El usuario pudo actualizar un producto.

### Escenario de fracaso:

* El usuario no pudo actualizar un producto.

