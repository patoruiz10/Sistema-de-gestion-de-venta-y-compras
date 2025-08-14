# Caso de Uso: Proceso de Venta
* Actores Primarios: Encargado, empleado
* Actores Secundarios: No tiene
* Precondiciones: El usuario debe estar logueado y la caja debe estar abierta
* Postcondiciones: No tiene

### Camino Básico
1. El usuario inicia el proceso de venta y carga el código de todos los productos a vender.
2. El sistema muestra el monto total a pagar.
3. El usuario selecciona el método de pago que prefiera el cliente.
4. El sistema verifica el método de pago elegido y concreta la venta, guardando el comprobante emitido, registrando la venta y reduciendo del stock el producto.

### Caminos Alternativos
1.a El código de producto ingresado no está registrado en el sistema.  
1.a.1 El sistema muestra una alerta: "Código inexistente", vuelve al paso "1". 
3.a El método de pago no está disponible.  
3.a.1 El sistema muestra una alerta: "Método de pago no disponible", vuelve al paso "3".  
4.a El monto elegido no se puede concretar por fondos insuficientes.  
4.a.1 El sistema muestra un mensaje: "No es posible efectuar el pago", vuelve al paso "3".  
4.b El monto elegido no se puede concretar por tener que sustituir el método de pago elegido.  
4.b.1 El sistema muestra un mensaje: "Proceso de pago cancelado", vuelve al paso "3".

### Escenario de Éxito
El usuario realizó la venta y el registro.

### Escenario de Fracaso
El usuario no pudo efectuar la venta por un código de producto no existente.
El usuario no pudo efectuar la venta por un método de pago no disponible. 
El usuario no pudo efectuar la venta por monto insuficiente. 

