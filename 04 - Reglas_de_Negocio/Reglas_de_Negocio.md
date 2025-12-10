## Hechos 
* El usuario debe controlar la mercaderia disponible
* Debe estar conectado a la parte de ventas
* La mercadería debe estar declarada por código de barra, una cantidad existente, descripción, tipo de producto, nombre del producto y nombre de marca
* Cada producto tiene un código.
* Se tiene que registrar cada venta.
* El cliente debe ser atendido por un vendedor.

## Restricciones
* El sistema no permite finalizar una venta si no incluye la condicion frente al IVA del cliente(CF,RI,etc.)
* Si se quiere agregar un producto, se debe completar con toda la informacion del mismo por la clasificacion que tiene.

## Acciones disparadoras
* Si es el primer dia del mes, debe generar un informe de las ventas del mes anterior.
* Si el cliente es frecuente, se le otorgará determinados beneficios.
* Cuando el stock de un producto sea menor a tres unidades o llegue a cero, debe notificar mediante una alerta la cantidad existente o restante.

## Cálculo 
* El precio total de la venta será igual al precio unitario del producto, más el impuesto sobre el mismo, menos el descuento (beneficios y/o promociones) por el volumen de la compra. 
* El calculo de las ganancia del negocio es el precio de venta al cliente menos el costo sobre precio de compra del producto.
* El IVA del producto se calcula como el precio del producto por el porcentaje del iva correspondiente.
* Cada producto que este dentro de la venta, debe descontarse la cantidad especificada en el stock.

## Inferencia 
* Si el cliente ha comprado mas de 10 veces en el último mes, entonces es considerado cliente frecuente.


