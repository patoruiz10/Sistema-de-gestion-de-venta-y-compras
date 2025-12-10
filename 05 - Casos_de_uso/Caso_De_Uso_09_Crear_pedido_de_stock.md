# Caso de uso: Crear pedido de stock
* Actores primarios: Empleado, encargado  
* Actores secundarios: No tiene  
* Precondición: El usuario debe tener permisos para crear pedidos 
* Postcondición: No tiene

### Camino básico:

1. El usuario selecciona la opción de “Crear pedido de stock”.  
2. El sistema calcula, para cada producto, la diferencia entre la cantidad actual y la cantidad mensual requerida, y muestra los productos que necesitan reabastecimiento y las cantidades sugeridas a pedir.  
3. El usuario modifica manualmente las unidades a pedir por producto y confirma la generación del pedido.  
4. El sistema genera el pedido de stock con el detalle de productos, cantidades y proveedor asociado.

### Caminos alternativos:
2.a No hay productos con faltante de stock.
2.a.1 El sistema muestra un mensaje indicando que no existen productos con faltante, pero que el usuario puede ajustar manualmente las cantidades si desea generar un pedido.
2.a.2 Continúa al paso 3.

### Escenario de éxito:

* El usuario pudo generar un pedido del stock a reabastecer.

### Escenario de fracaso:

* El usuario no pudo generar un pedido de stock porque no había productos con faltante y decidió no ajustar cantidades manualmente.

