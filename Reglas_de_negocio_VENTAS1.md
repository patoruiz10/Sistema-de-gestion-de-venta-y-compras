## Hechos 
* Cada producto tiene un código.
* Se tiene que registrar cada venta.
* El cliente debe ser atendido por un vendedor.

## Restricciones
* El sistema no permite finalizar una venta si no se emite un comprobante fiscal electronico que cumpla con las condiciones establecidas por ARCA:
    * Ser electronico y válido ante AFIP.
    * Inluir la condicion frente al IVA del cliente(CF,RI,etc.)
    * Estar asociado a un punto de venta habilitado.
    * Cumplimiento de precios de los productos 
* No se puede operar el sistema sin iniciar sesión con un usuario válido.
* No se puede modificar el total de la venta manualmente

    

## Acciones disparadoras
* Si es el primer dia del mes, debe generar un informe de las ventas del mes anterior.
* Si el cliente es frecuente, se le otorgará determinados beneficios.

## Cálculo 
* El precio total de la venta será igual al precio unitario del producto más el impuesto sobre el mismo menos el descuento por el volumen de la compra. 
* El margen de ganancia es el precio de venta menos el costo sobre precio de venta.
* El IVA del producto se calcula como el precio del producto por el porcentaje del iva correspondiente.


## Inferencia 
* Si el cliente ha comprado mas de 10 veces en el último mes, entonces es considerado cliente frecuente.


