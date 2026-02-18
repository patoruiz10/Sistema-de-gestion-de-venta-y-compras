# Caso de uso: Proceso de Venta

* Actores primarios: Empleado, Encargado
* Actores secundarios: No tiene
* Precondiciones: El usuario debe estar logueado y la caja debe estar abierta.
* Postcondiciones: La venta queda registrada, se genera ticket/comprobante, se actualiza stock y se actualiza el balance de caja.

### Camino básico

1. El usuario inicia una nueva venta.
2. El sistema crea e inicia la venta.
3. El usuario ingresa los datos del cliente: nombre, teléfono, DNI, y condición IVA.
4. El sistema asocia el cliente a la venta.
5. El usuario ingresa los código de los producto.
6. El sistema obtiene los productos.
7. El usuario ingresa las cantidades de los producto.
8. El sistema agrega los productos a la venta y muestra el total.
9. El usuario selecciona el método de pago.
10. El sistema registra el pago y guarda el comprobante.

### Caminos alternativos
4.a Algún campo obligatorio del cliente está vacío.  
4.a.1 El sistema muestra: "Faltan completar campos obligatorios".  
4.a.2 Vuelve al paso 3.

6.a Código inexistente. 
6.a.1 El sistema muestra: "Código inexistente, vuelva a ingresar".  
6.a.2 Vuelve al paso 5.

10.a Método de pago no disponible.
10.a.1 El sistema muestra: "Método de pago no disponible".  
10.a.2 Vuelve al paso 9.

10.b Fondos insuficientes.  
10.b.1 El sistema muestra: "No es posible efectuar el pago".  
10.b.2 Vuelve al paso 9.

10.c Proceso de pago cancelado.  
10.c.1 El sistema muestra: "Proceso de pago cancelado".  
10.c.2 Fin del caso de uso.

### Escenario de éxito
* La venta se registra y se guarda comprobante/ticket.

### Escenario de fracaso
* La venta no se concreta por campos de cliente incompletos
* La venta no se concreta por código inexistente.
* La venta no se concreta por método de pago no disponible.
* La venta no se concreta por fondos insuficientes.
