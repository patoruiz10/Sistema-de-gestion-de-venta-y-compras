# Reglas de negocio
### Hechos
* El usuario debe controlar la mercaderia disponible
* Debe estar conectado a la parte de ventas
* La mercadería debe estar declarada por código de barra, cant existente, descripción, tipo de producto, nombre del producto y nombre de marca

### Restricciones
* Si se quiere agregar un producto, se debe completar con toda la informacion del mismo por la clasificacion que tiene.

### Acciones disparadoras
* Cuando el stock de un producto llegue a cero o la cantidad de producto sea menor a tres unidades, debe notificar mediante una alerta la cantidad existente o restante.

### Calculos
* Cada producto que este dentro de la venta, debe descontarse la cantidad especificada en el stock.

### Inferencias
* No hay inferencias.