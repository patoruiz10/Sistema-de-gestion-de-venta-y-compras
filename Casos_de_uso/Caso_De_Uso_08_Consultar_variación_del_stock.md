# Caso de uso: Consultar variación del stock
* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos  
* Postcondición: No tiene

### Camino básico:

1. El usuario selecciona la opción de “Consultar variación del stock” dentro del sistema con el mouse.  
2. El sistema muestra un formulario con las existencias de los productos actuales registrados, las existencias del mes anterior al día de la fecha actual, y las existencias que el usuario fijó como “cantidad mensual requerida”.  
3. El usuario ingresa una fecha específica para consultar.  
4. El sistema muestra el mismo formulario con la información actualizada.

### Caminos alternativos:
4.a La fecha ingresada corresponde a una fecha futura.  
4.a.1 El sistema muestra una alerta de que la fecha es futura.  
4.a.2 Vuelve al paso “3”.

### Escenario de éxito:

* El usuario pudo ver la variación de los productos del stock.

### Escenario de fracaso:

* El usuario no pudo consultar la fecha deseada de la variación del stock.


