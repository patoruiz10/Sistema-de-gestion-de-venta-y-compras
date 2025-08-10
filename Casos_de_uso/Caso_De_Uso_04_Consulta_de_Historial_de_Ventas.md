# Caso de uso: Consulta de historial de ventas

* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos  
* Postcondición: No tiene

### Camino básico: 
1. El usuario selecciona la opción de “Consulta de historial de ventas” dentro del sistema con el mouse. 
2. El sistema muestra un formulario con opciones para consultar todas las ventas correspondientes de un día en particular, semana o mes.  
3. El usuario elige la opción deseada y realiza la consulta.  
4. El sistema muestra un formulario con todas las ventas realizadas en la fecha consultada.

             
### Caminos alternativos:  
4.a No se encontraron ventas registradas en la fecha consultada.  
4.a.1 El sistema muestra una alerta con un mensaje que indica que en la fecha consultada no se encontraron ventas registradas.  
4.a.2 Vuelve al paso “3”.  
4.b La fecha ingresada corresponde a una fecha futura. 4.b.1 El sistema muestra una alerta de que la fecha es futura.  
4.b.2 Vuelve al paso “3”.  
4.c Consulta no realizada por falta de datos (fecha).
4.c.1 El sistema muestra una alerta con un mensaje que informa que falta completar la fecha.  
4.c.2 Vuelve al paso “3”.


### Escenario de éxito:
* El usuario pudo realizar la consulta de ventas efectivamente.

### Escenario de fracaso:
* El usuario no pudo realizar la consulta de ventas efectivamente.