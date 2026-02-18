# Caso de uso: Consultar variación del stock
* Actores primarios: Empleado, Encargado
* Actores secundarios: No tiene
* Precondición: El usuario debe tener permisos para consultar la variación del stock.
* Postcondición: No tiene

### Camino básico

1. El usuario ingresa la fecha para consultar.
2. El sistema muestra la lista de variaciones del stock.

### Caminos alternativos
2.a La fecha ingresada es futura.
2.a.1 El sistema muestra: "La fecha ingresada es futura".
2.a.2 Vuelve al paso 1.

### Escenario de éxito
* El usuario pudo ver la variación del stock de los productos para la fecha consultada.

### Escenario de fracaso
* El usuario no pudo obtener la variación del stock porque ingresó una fecha futura.
