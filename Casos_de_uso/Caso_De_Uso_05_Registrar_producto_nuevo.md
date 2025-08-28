# Caso de uso: Registrar producto nuevo
* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos  
* Postcondición: No tiene

### Camino básico:

1. El usuario selecciona la opción de “añadir nuevo producto” dentro del sistema.  
2. El sistema muestra un formulario con los datos requeridos a completar sobre el producto que se desea ingresar (ID, nombre, descripción, proveedor).   
3. El usuario ingresa los datos solicitados del nuevo producto y termina el proceso guardando los datos seleccionando en la opción “Guardar”.  
4. El sistema muestra mediante una alerta visual que el producto se registró correctamente.

### Caminos alternativos:
4.a El usuario no ingresó un ID.  
4.a.1 El sistema muestra una alerta con un mensaje que informa que faltan completar la casilla de ID del producto.  
4.a.2 Vuelve al paso “3”.  
4.b El usuario ingresó un codigo de producto repetido.  
4.b.1 El sistema muestra una alerta con un mensaje que informa que el ID del producto ingresado ya existe.  
4.b.2 Vuelve al paso “3”.

### Escenario de éxito:

* El usuario pudo registrar un producto.

### Escenario de fracaso:

* El usuario no pudo registrar un producto.