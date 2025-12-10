# Proyecto Selvent
### Requerimientos Funcionales:
* Cada venta debe registrar: nombre del producto, cantidad vendida, precio unitario, total, stock restante, fecha/hora y método de pago.
* Cada venta debe quedar asociada al empleado que la realizó.
* Debe permitir múltiples métodos de pago por transacción (efectivo, tarjeta, billeteras virtuales, combinaciones).
* Debe generar reportes financieros diarios, con ingresos por ventas, egresos por compras, y ganancias netas.
* Debe permitir consultar el historial de ventas filtrando por fecha.
* Debe permitir agregar productos al carrito mediante escaneo de código de barras, ingreso manual del código, o búsqueda por nombre o categoría.
* Debe permitir la anulación o edición de ventas recientes por errores humanos, con el debido registro de auditoría.
* Debe manejar stock de la mercadería disponible.
* La mercadería debe estar declarada por código de barra, cantidad existente, descripción, tipo de producto, nombre y nombre de marca
* Las ventas realizadas deben impactar en el stock
* Cuando se realiza reabastecimiento debe impactar en el stock
* Debe permitir consultar el inventario completo de productos, mostrando código, descripción, cantidad en stock, precio y proveedor.
* Debe permitir consultar la variación del stock de los productos para una fecha determinada, mostrando existencias actuales, existencias en la fecha consultada y la diferencia.
* Debe permitir actualizar manualmente la cantidad en stock de un producto específico.
* Debe permitir generar pedidos de reabastecimiento en base a la diferencia entre la cantidad actual y la cantidad mensual requerida, indicando productos, cantidades a pedir y proveedor asociado.
* Debe identificar productos con stock por debajo de un mínimo o de la cantidad mensual requerida y marcarlos como ‘con faltante’ para reabastecimiento.




### Requerimientos No funcionales

* El sistema debe tener una base de datos con todos los productos registrados
* El sistema debe utilizar una base de datos segura, confiable y escalable para almacenar información de productos, ventas, usuarios y reportes.
* El sistema debe tener una interfaz gráfica intuitiva y responsiva para facilitar su uso por parte del personal del minimarket.
* El sistema debe garantizar tiempos de respuesta menores a 2 segundos por operación común.
* El sistema debe realizar copias de seguridad automáticas diariamente/semanalmente.
* El reabastecimiento de los productos debe tener un tiempo de respuesta menor a 3 seg: eficiencia



### Dominio
* Cada empleado debe contar con un usuario
