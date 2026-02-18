# Caso de uso: Crear nuevo empleado

* Actores primarios: Encargado , Empleado
* Actores secundarios: No tiene
* Precondición: El usuario debe tener permisos.
* Postcondición: El usuario se agrega a la lista de usuarios del sistema.

### Camino básico:

1. El usuario ingresa los datos: nombre, teléfono, DNI, usuario, contraseña y rol.
2. El sistema agrega el nuevo empleado al listado de empleados.

### Caminos alternativos
2.a Existen campos obligatorios sin completar.  
2.a.1 El sistema muestra: "Faltan completar campos obligatorios".  
2.a.2 Vuelve al paso 1.

### Escenario de éxito
* El usuario pudo crear un nuevo empleado.

### Escenario de fracaso
* El usuario no pudo crear el nuevo empleado porque dejó campos obligatorios sin completar.
