# Proyecto Selvent
### Requerimientos 
*El sistema debe registrar cada venta con: productos, cantidades, precios unitarios, total, fecha/hora y método de pago.
*Cada venta debe quedar asociada al empleado que la realizó.
*Debe generar reportes diarios de ventas e ingresos totales.
*Debe permitir consultar el historial de ventas filtrando por fecha.
*Debe permitir agregar productos al carrito mediante el ingreso manual del código o búsqueda por nombre/categoría.
*Debe manejar el stock de la mercadería disponible.
*Cada producto debe estar registrado con código, cantidad existente, precio unitario, descripción y categoría.
*Los productos de las ventas concretadas se deben descontar automáticamente el stock.
*Debe permitir consultar el inventario completo mostrando código, descripción, cantidad disponible, precio unitario y proveedor.
*Debe permitir consultar la variación del stock en una fecha específica, mostrando existencias actuales, existencias en la fecha consultada y la diferencia entre las fechas.
*Debe permitir actualizar manualmente el stock de un producto.
*Debe permitir generar pedidos de stock para los productos cuyo nivel de existencias sea menor o igual al mínimo establecido.
*Debe identificar productos con stock por debajo del mínimo requerido y marcarlos como “con faltante”.

### Requerimientos No funcionales
* El sistema debe contar con una base de datos con todos los productos registrados.
* La base de datos debe ser segura, confiable y escalable.
* La interfaz debe ser intuitiva y fácil de usar para el personal del comercio.
* Las operaciones deben tener un tiempo de respuesta menor a 2 segundos.
* Debe realizar copias de seguridad automáticas diarias o semanales.
### Dominio
* Cada empleado debe contar con un usuario propio para acceder al sistema.
