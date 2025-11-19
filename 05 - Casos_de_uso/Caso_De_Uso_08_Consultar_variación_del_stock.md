# Caso de uso: Consultar variación del stock
* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos para consultar la variación del stock
* Postcondición: No tiene

### Camino básico:

1. El usuario selecciona la opción de “Consultar variación del stock”.
2. El sistema muestra las existencias de los productos actuales registrados, las existencias del mes anterior al día de la fecha actual, y la cantidad mensual requerida previamente fijada por el usuario (es decir, la demanda estimada necesaria para cubrir un mes de ventas).  
3. El usuario ingresa una fecha específica para consultar.  
4. El sistema muestra la información actualizada.

### Caminos alternativos:
4.a La fecha ingresada corresponde a una fecha futura del día consultado.  
4.a.1 El sistema muestra una alerta visual de que la fecha es futura  a la del día consultado.  
4.a.2 Vuelve al paso “3”.

### Escenario de éxito:

* El usuario pudo ver la variación de los productos del stock.

### Escenario de fracaso:

* El usuario no pudo consultar la fecha deseada de la variación del stock.

