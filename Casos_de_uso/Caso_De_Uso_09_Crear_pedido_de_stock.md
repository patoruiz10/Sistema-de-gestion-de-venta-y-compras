# Caso de uso: Crear pedido de stock
* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos para crear pedidos 
* Postcondición: No tiene

### Camino básico:

1. El usuario selecciona la opción de “Crear pedido de stock”.  
2. El sistema muestra las existencias de los productos actuales registrados, y las existencias que el usuario fijó como “cantidad mensual requerida” y calcula la diferencia entre ambas.  
3. El usuario modifica si desea alguna cantidad mayor o menor y guarda el pedido.  
4. El sistema muestra la información de que productos debe pedir, las cantidades de unidades, costos de los productos y a que proveedor debe hacerlo.

### Caminos alternativos:
4.a No hay productos para solicitar  
4.a.1 El sistema muestra una alerta visual de que ningún producto tiene faltante de stock comparado con la “cantidad mensual requerida” o la que el usuario ingresó.  
4.a.2 Vuelve al paso “3”.

### Escenario de éxito:

* El usuario pudo generar un pedido del stock a reabastecer.

### Escenario de fracaso:

* El usuario no pudo generar un pedido del stock.

