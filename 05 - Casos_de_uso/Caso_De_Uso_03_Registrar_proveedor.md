# Caso de uso: Registrar proveedor nuevo
* Actores primarios: Empleado, Encargado
* Actores secundarios: No tiene
* Precondición: El usuario debe tener permisos para registrar proveedores.
* Postcondición: No tiene

### Camino básico

1. El usuario ingresa los datos del proveedor (nombre, teléfono, CUIT, mail, dirección)
2. El sistema valida que todos los campos obligatorios estén completos y muestra mediante una alerta que el proveedor se registró.

### Caminos alternativos
2.a Algún campo obligatorio está vacío.  
2.a.1 El sistema muestra: "Faltan completar campos obligatorios".  
2.a.2 Vuelve al paso 1.

2.b El CUIT ingresado ya corresponde a un proveedor existente.
2.b.1 El sistema muestra: "El CUIT ingresado ya corresponde a un proveedor existente".  
2.b.2 Vuelve al paso 1.

### Escenario de éxito
* El usuario registró un proveedor correctamente.

### Escenario de fracaso
* El usuario no pudo registrar el proveedor por datos incompletos o por CUIT repetido.
