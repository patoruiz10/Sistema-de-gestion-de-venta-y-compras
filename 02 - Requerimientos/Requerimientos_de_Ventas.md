# Proyecto Minimarket
## Requerimientos de Ventas
### Requerimientos Funcionales:
* Debe registrar cada venta, incluyendo producto(s), cantidad, precio unitario, total de la venta, fecha y hora.
* Debe generar reportes financieros diarios, semanales y mensuales, con ingresos por ventas, egresos por compras o devoluciones, y ganancias netas.
* Debe permitir agregar productos al carrito mediante escaneo de código de barras, ingreso manual del código, o búsqueda por nombre o categoría.
* Cada venta debe registrar: nombre del producto, cantidad vendida, precio unitario, total, stock restante, fecha/hora y método de pago.
* Debe permitir la anulación o edición de ventas recientes por errores humanos, con el debido registro de auditoría.
* Debe permitir aplicar descuentos por producto o por venta total
* Debe manejar el stock de la mercadería faltante
* Debe manejar stock de la mercadería disponible
* La mercadería debe estar declarada por código de barra, cantidad existente, descripción, tipo de producto, nombre y nombre de marca  
* Las ventas realizadas deben impactar en el stock  
* Cuando se realiza reabastecimiento debe impactar en el stock


### Requerimientos No funcionales
* El sistema debe tener una base de datos con todos los productos registrados
* El sistema debe utilizar una base de datos segura, confiable y escalable para almacenar información de productos, ventas, usuarios y reportes.
* El sistema debe permitir múltiples métodos de pago por transacción (efectivo, tarjeta, billeteras virtuales, combinaciones).
* El sistema debe tener una interfaz gráfica intuitiva y responsiva para facilitar su uso por parte del personal del minimarket.
* El sistema debe garantizar tiempos de respuesta menores a 2 segundos por operación común.
* El sistema debe realizar copias de seguridad automáticas diariamente/semanalmente.
* Debe tener dia, mes, año y hora, usuario del empleado, nombre del negocio: usabilidad  
* El reabastecimiento de los productos debe tener un tiempo de respuesta menor a 3 seg: eficiencia


### Dominio
* Generar facturas que cumplan con las condiciones ARCA 
* El ticket debe contener los datos fiscales exigidos por la ley, incluyendo un código QR, tipo de factura y razón social del comercio.
* Cada empleado debe contar con un usuario 


