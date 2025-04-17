# Proyecto Minimarket
## Control de Ventas
### Enunciado de idea general

Se socilita un sistema que tenga como fin principal administrar el registro de ventas de un minimarket. En el cual se busca que sea capaz de registrar cada producto vendido en una caja registradora, comprobar si hay una existencia de stock, llevar un registro de los ingresos y egreso de dinero en el día a día y las ganancias por categoría de productos para asi poder llegar a un balance.

### Carateristicas generales
El cajero a través de una lectura de código de barra, registra el código del producto a vender en el carrito de compra y lo agrega en un ticket DIGITAL que al momento de imprimirlo lo convierte en un comprobante del ticket y factura. Tambien genera una copia del mismo almacenada en una base de datos.
Se busca la automatización de la carga impositiva de los productos (I.V.A).  


# Ticket / Factura
Se integrará en el ticket los siguientes datos de venta: 
* Datos del local y empresa.
* Fecha y hora de la venta.
* QR del ticket.
* Código del producto.
* Descripción.
* Precio.
* Cantidad de productos.
* Subtotal.
* Total.
* Cambio.

# Tipos de Factura
* Consumidor Final 
* Responsable Inscripto 
* Monotributista
* Tipo C

# Ingresos y Egresos de Dinero.
Se busca llevar un registro de los Ingresos y la salida de dinero en el día a día, las ganancias por categoría de productos, si se cumplen las ventas esperadas del dia.

### (Opcional) Proyeccion de ganancias: establecida por el usuario
Ejemplo de prueba: 
Ganancias mensuales deseadas $250.000 
Se divide por dias del mes (30) $8.333,33

Al momento de cerrar la caja se consulta el estado de las ganancias diarias y se da un informe de estado "Ganaste $$ más de lo proyectado// Ganaste $$ menos de lo proyectado"

### Registro de productos 
Tipos de registro:
* Lectura de código de barra.
* Ingreso manual del código.
* Búsqueda manual indexado. 
