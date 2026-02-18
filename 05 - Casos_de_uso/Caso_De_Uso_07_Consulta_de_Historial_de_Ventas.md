# Caso de uso: Consulta de historial de ventas
* Actores primarios: Encargado, Empleado.
* Actores secundarios: No tiene
* Precondición: El usuario debe tener permisos.  
* Postcondición: No tiene

### Camino básico
1. El usuario ingresa una fecha a consultar.
2. El sistema muestra la lista de todas las ventas correspondientes a la fecha ingresada.

### Caminos alternativos
2.a La fecha ingresada es futura respecto al día actual.  
2.a.1 El sistema muestra: "La fecha ingresada es futura".  
2.a.2 Vuelve al paso 1.

2.b No se encontraron ventas registradas en la fecha consultada.  
2.b.1 El sistema muestra: "No se encontraron ventas registradas en la fecha consultada".  
2.b.2 Vuelve al paso 1.

### Escenario de éxito
* El usuario pudo ver las ventas de la fecha consultada.

### Escenario de fracaso
* El usuario no pudo obtener ventas porque ingresó una fecha futura.
