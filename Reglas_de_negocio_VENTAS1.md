## Hechos 
* Cada producto tiene un código.
* Se tiene que registrar cada venta.
* El cliente debe ser atendido por un vendedor.

## Restricciones
* El sistema no permite finalizar una venta si no se emite un comprobante fiscal electronico que cumpla con las condiciones establecidas por ARCA:
<<<<<<< HEAD:Reglas_de_negocio_VENTAS.md
    - Ser electronico y válido ante ARCA.
    - Inluir la condicion frente al IVA del cliente(CF,RI,etc.)
    - Estar asociado a un punto de venta habilitado.
    - Cumplimiento de precios de los productos 
=======
    * Ser electronico y válido ante ARCA.
    * Incluir la condicion frente al IVA del cliente(CF,RI,etc.)
    * Estar asociado a un punto de venta habilitado.
    * Cumplimiento de precios de los productos 
>>>>>>> edae68344ca82d659e91b34cd34d11c956bbb91f:Reglas_de_negocio_VENTAS1.md
* No se puede operar el sistema sin iniciar sesión con un usuario válido.
* No se puede modificar el total de la venta manualmente

    

## Acciones disparadoras
* Si es el primer dia del mes, debe generar un informe de las ventas del mes anterior.
* Si el cliente es frecuente, se le otorgará determinados beneficios.

## Cálculo 
<<<<<<< HEAD:Reglas_de_negocio_VENTAS.md
* El precio total de la venta será igual al precio unitario del producto, más el impuesto sobre el mismo, menos el descuento (beneficios y/o promociones) por el volumen de la compra. 
* El margen de ganancia del negocio es el precio de venta al cliente menos el costo sobre precio de compra del producto menos costo de reabastecimiento del producto.
=======
* El precio total de la venta será igual al precio unitario del producto más el impuesto sobre el mismo, en caso de ser cliente frecuente, se aplica un descuento por el volumen de la compra. 
* El margen de ganancia del negocio es el precio de venta al cliente, menos el costo sobre precio de compra del producto, menos costo de reabastecimiento del producto.
>>>>>>> edae68344ca82d659e91b34cd34d11c956bbb91f:Reglas_de_negocio_VENTAS1.md
* El IVA del producto se calcula como el precio del producto por el porcentaje del iva correspondiente.


## Inferencia 
* Si el cliente ha comprado mas de 10 veces en el último mes, entonces es considerado cliente frecuente.


