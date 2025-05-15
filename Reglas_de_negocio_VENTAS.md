## Hechos 
* Cada producto tiene un código.
* Se tiene que registrar cada venta.
* El cliente debe ser atendido por un vendedor.
* No vender productos vencidos.

## Restricciones
* La aplicación debe cumplir con las regulaciones ARCA.
* No vender a un cliente con crédito excedido.
* No vender bebidas alcohólicas a menores de 18 años.
* No se puede realizar una venta sin haber seleccionado un método de pago válido.

## Acciones disparadoras
* Si es el primer dia del mes, debe generar un informe de las ventas del mes anterior.
* Cuando se escanea un producto se reducirá del stock.
* Se recalculara el totál de la venta al quitar un producto del carrito.
* Al registrar un producto se actualizara el precio de la venta.
* Si el método de pago es tarjeta y la transacción es rechazada, entonces se solícita un nuevo método de pago.

## Cálculo 
* El precio total de un pedido se calcula como la suma del precio de los artículos. pedidos, más el impuesto sobre las ventas, menos el descuento por volúmen. 

## Inferencia 
* Si el cliente ha comprado mas de 20 veces en el último mes, entonces es considerado cliente frecuente.
* Si el pago no se recibe luego de la fecha de vencimiento, el cliente es moroso. 



