# Caso de uso: Registrar proveedor nuevo
* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos  
* Postcondición: No tiene

### Camino básico:

1. El usuario selecciona la opción de “Registrar proveedor nuevo” dentro del sistema.  
2. El sistema muestra un formulario con los datos requeridos a completar sobre el proveedor que se desea ingresar (ID, compañía, nombre del contacto, número de contacto, detalles).   
3. El usuario ingresa los datos solicitados del nuevo proveedor y termina el proceso guardando los datos seleccionando en la opción “Guardar”.  
4. El sistema muestra mediante una alerta que el proveedor se registró correctamente.

### Caminos alternativos:
4.a El usuario no ingresó un ID.  
4.a.1 El sistema muestra una alerta con un mensaje que informa que faltan completar la casilla de ID del proveedor.  
4.a.2 Vuelve al paso “3”.  
4.b El usuario ingresó un ID repetido.  
4.b.1 El sistema muestra una alerta con un mensaje que informa que el ID del proveedor ingresado ya existe.  
4.b.2 Vuelve al paso “3”.

### Escenario de éxito:

* El usuario pudo registrar un proveedor correctamente.

### Escenario de fracaso:

* El usuario no pudo registrar un proveedor.


