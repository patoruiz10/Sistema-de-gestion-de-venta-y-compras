# Caso de uso: Registrar proveedor nuevo
* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos para registrar proveedor nuevo
* Postcondición: No tiene

### Camino básico:

1. El usuario selecciona la opción de “Registrar proveedor nuevo”.
2. El sistema muestra los datos requeridos a completar sobre el proveedor que se desea ingresar (CUIT, compañía, nombre del contacto, número de contacto, detalles).   
3. El usuario ingresa los datos solicitados del nuevo proveedor y termina el proceso guardando los datos.  
4. El sistema muestra mediante una alerta visual que el proveedor se registró.

### Caminos alternativos:
4.a El usuario no ingresó el CUIT de proveedor.  
4.a.1 El sistema muestra una alerta visual con un mensaje que informa que faltan completar la casilla de CUIT del proveedor.
4.a.2 Vuelve al paso “3”.  
4.b El usuario ingresó el CUIT repetido del proveedor.  
4.b.1 El sistema muestra una alerta visual con un mensaje que informa que el CUIT del proveedor ingresado ya existe.  
4.b.2 Vuelve al paso “3”.

### Escenario de éxito:

* El usuario pudo registrar un proveedor.

### Escenario de fracaso:

* El usuario no pudo registrar un proveedor debido a errores en la información ingresada.

