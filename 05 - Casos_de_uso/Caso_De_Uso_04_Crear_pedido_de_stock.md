# Caso de uso: Crear pedido de stock

* Actores primarios: Empleado, Encargado
* Actores secundarios: No tiene
* Precondiciones: El usuario debe tener permisos para crear pedidos
* Postcondiciones: No tiene

### Camino básico:

1. El usuario selecciona la opción “Crear pedido de stock”.
2. El sistema obtiene todos los productos registrados, filtra y muestra aquellos con faltante (productos con cantidad actual <= 10).
3. El usuario modifica manualmente las cantidades a reponer por producto y confirma el pedido.
4. El sistema muestra el detalle final del pedido con: producto, cantidad a reponer y proveedor.

### Caminos alternativos

2.a No existen productos con faltante.
2.a.1 El sistema muestra el mensaje: "No existen productos con faltante de stock. Puede ajustar manualmente si desea generar un pedido".
2.a.2 El caso de uso continúa en el paso 3.

### Escenario de éxito

* El usuario pudo generar el detalle del pedido de stock.

### Escenario de fracaso

* No tiene.
