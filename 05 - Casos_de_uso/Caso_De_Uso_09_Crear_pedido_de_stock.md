# Caso de uso: Crear pedido de stock
* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos para crear pedidos 
* Postcondición: No tiene

### Camino básico:

1. El usuario selecciona la opción de “Crear pedido de stock”.  
2. El sistema muestra las existencias de los productos actuales registrados, y las existencias que el usuario fijó como “cantidad mensual requerida” y calcula la diferencia entre ambas.  
3. El usuario modifica si desea alguna cantidad mayor o menor y guarda el pedido.  
4. El sistema muestra la información de que productos debe pedir, las cantidades de unidades y a que proveedor debe hacerlo.

### Caminos alternativos:
2.a No hay productos para solicitar  
2.a.1 El sistema informa que no hay productos para reabastecer, pero permite al encargado ajustar manualmente cantidades si desea igualmente generar un pedido.

### Escenario de éxito:

* El usuario pudo generar un pedido del stock a reabastecer.

### Escenario de fracaso:

* El usuario no pudo generar un pedido del stock.

