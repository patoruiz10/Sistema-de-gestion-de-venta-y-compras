## Hechos 
* El usuario debe controlar la mercaderia disponible
* Debe estar conectado a la parte de ventas
* La mercadería debe estar declarada por un código, una cantidad existente, descripción, categoría y proveedor.
* Cada producto tiene un código único que lo identifica en el sistema.
* Cada producto está asociado a un proveedor registrado en el sistema.
* Cada producto pertenece a una categoría registrada.
* Se tiene que registrar cada venta.
* Cada venta queda asociada al vendedor que la llevo a cabo.
* Cada apertura de caja queda asociada a un empleado

## Restricciones
* Si se quiere agregar un producto nuevo, se debe completar toda la información obligatoria del mismo según su clasificación (código, descripción, cantidad, precio, proveedor y categoría).
* El sistema no permite finalizar una venta si la cantidad vendida de algún producto supera el stock disponible.
* El sistema no permite registrar ventas si la caja correspondiente se encuentra cerrada.
* El sistema no permite finalizar una venta si no se registra al menos un método de pago válido y aceptado.

## Acciones disparadoras
* Si es el primer dia del mes, debe generar un informe de las ventas del mes anterior.
* Cuando el stock de un producto sea igual al límite establecido por el usuario, debe notificar mediante una alerta la cantidad existente o restante.
* Al confirmar una venta, el sistema debe descontar del stock la cantidad vendida de cada producto, actualizar el saldo de la caja, generar y guardar el comprobante asociado a esa venta.
* Cuando se registra una entrega de proveedor (reabastecimiento), el sistema debe actualizar el stock de los productos recibidos.

## Cálculo 
* El precio total de la venta será igual al precio unitario del producto, más el impuesto sobre el mismo, por el volumen de la compra. 
* El calculo de las ganancia del negocio es el precio de venta al cliente menos el costo sobre precio de compra del producto.
* El IVA del producto se calcula como el precio del producto por el porcentaje del iva correspondiente.
* Cada producto que este dentro de la venta, debe descontarse la cantidad especificada en el stock.
* Para consultas de variación de stock entre dos fechas se calcula como; variación = existencias en la fecha actual − existencias en la fecha consultada.

## Inferencia 
* Si el cliente ha comprado mas de 10 veces en el último mes, entonces es considerado cliente frecuente.
* Si el stock actual de un producto es menor que la cantidad mensual requerida definida para ese producto, entonces el producto se considera con faltante y debe incluirse en el próximo pedido de reabastecimiento.

